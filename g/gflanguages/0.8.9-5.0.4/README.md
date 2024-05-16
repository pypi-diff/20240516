# Comparing `tmp/gflanguages-0.8.9.tar.gz` & `tmp/gflanguages-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gflanguages-0.8.9.tar", last modified: Thu Jun  8 11:34:19 2023, max compression
+gzip compressed data, was "gflanguages-5.0.4.tar", last modified: Fri Jul 28 13:47:19 2023, max compression
```

## Comparing `gflanguages-0.8.9.tar` & `gflanguages-5.0.4.tar`

### file list

```diff
@@ -1,2054 +1,2044 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:19.307593 gflanguages-0.8.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:18.891587 gflanguages-0.8.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:18.891587 gflanguages-0.8.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-08 11:33:59.000000 gflanguages-0.8.9/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-08 11:33:59.000000 gflanguages-0.8.9/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 11:33:59.000000 gflanguages-0.8.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-08 11:33:59.000000 gflanguages-0.8.9/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-08 11:33:59.000000 gflanguages-0.8.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-08 11:33:59.000000 gflanguages-0.8.9/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-06-08 11:33:59.000000 gflanguages-0.8.9/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:18.891587 gflanguages-0.8.9/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:18.895587 gflanguages-0.8.9/Lib/gflanguages/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 11:34:18.000000 gflanguages-0.8.9/Lib/gflanguages/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:18.891587 gflanguages-0.8.9/Lib/gflanguages/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:19.215591 gflanguages-0.8.9/Lib/gflanguages/data/languages/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ab_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/abi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/abq_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/abr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/acd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ace_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/acf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ach_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/acu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ada_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ade_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/adj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/adl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ady_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ae_Avst.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aeb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aeb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/af_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/agc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/agq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/agr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aha_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ahl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aho_Ahom.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ahs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Armi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Chrs.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Egyp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Elym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Hatr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Mani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Narb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Nbat.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Palm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Phli.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Phlp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Phnx.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Prti.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Samr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Sarb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Sogd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Sogo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Ugar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ain_Kana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ain_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ajg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/akk_Xsux.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/akp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/akz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ala_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ale_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aln_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/alt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/am_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/amc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ame_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ami_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/amo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/amr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/an_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/anc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ang_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ank_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ann_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/anp_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/anv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/any_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aoz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/apd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ar_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ar_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arc_Armi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arc_Nbat.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arc_Palm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/aro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arq_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ars_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/art_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ary_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/arz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/as_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/asa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/asg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ast_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/atg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/atj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/auc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/av_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/avk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/avn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/avu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/awa_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/awo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ayb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/az_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/az_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/az_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/azb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/azj_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ba_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bal_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bal_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ban_Bali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ban_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bap_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bar_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bas_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bax_Bamu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bax_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bbc_Batk.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bbc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bbj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bbp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bci_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bcn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bcq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bcw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bcy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bdh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/be_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/be_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/beh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bej_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bej_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bem_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ber_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ber_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ber_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bet_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bew_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bex_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bez_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bfa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bfd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bfq_Taml.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bft_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bft_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bfy_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bg_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bgc_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bgn_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bgx_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bhb_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bhi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bhk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bho_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bho_Kthi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bhy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bib_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bik_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bim_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bin_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/biv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bjj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bjn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bjt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bjv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bkc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bkm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bku_Buhd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bku_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bkv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bla_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/blo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/blt_Tavt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bm_Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bmq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bn_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bn_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bng_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bnm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bo_Marc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bo_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bo_Zanb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/boa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bom_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bov_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/box_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/boz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bpy_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bqc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bqi_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bqj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bqp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bqv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/br_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bra_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/brh_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/brh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/brx_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/brx_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/brx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bs_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bsc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bsj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bsp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bsq_Bass.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bsq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bss_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bto_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/btt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/btv_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bua_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/buc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bud_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bug_Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bum_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/buu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bvb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bvi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bwr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bwy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/byh_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/byn_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/byn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bys_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/byv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bza_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bze_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bzw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/bzx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ca_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cab_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/car_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cbi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cbj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cbk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cbr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cbs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cbt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cbu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cch_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ccp_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ccp_Cakm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cdr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ce_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ceb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cfa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cfm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cgg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ch_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chm_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chn_Dupl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cho_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chp_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chr_Cher.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chx_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/chy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cic_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cja_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cja_Cham.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cjk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cjm_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cjm_Cham.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cjs_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cjy_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ckb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ckl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cko_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ckt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cky_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cla_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cme_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cmg_Soyo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cnh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cni_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/co_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cof_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/con_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cop_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cop_Copt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cop_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cot_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cpf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cps_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cpu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cr_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crh_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cri_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crj_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crk_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crl_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crm_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/crs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/csa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/csb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/csk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/csw_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ctd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ctd_Pauc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cu_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cu_Glag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cwe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/cyo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/da_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/daa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dar_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dbd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dbq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dcc_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ddn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/de_Dupl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/de_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/de_Runr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/del_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/den_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/den_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dga_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dgh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dgi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dgr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dhi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dhw_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/did_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/din_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dip_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dje_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dmf_Medf.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dng_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dnj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/doi_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/doi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/doi_Dogr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/doi_Takr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dop_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dow_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dri_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dsb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dtm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dtp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dts_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dty_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dua_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dum_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/duu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dv_Thaa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dwr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dyi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dyo_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dyo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dyu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dyu_Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dz_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/dzg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ebu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ee_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/efi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/egl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/egy_Egyp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/eka_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ekm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/eky_Kali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/el_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ema_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/emk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/en_Brai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/en_Dsrt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/en_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/en_Shaw.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/enm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/enn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/eo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/es_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ese_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/esg_Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/esu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/et_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ett_Ital.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ett_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/etu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/etx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/eu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/eve_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/evn_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/evn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ewo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ext_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/eza_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fa_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fan_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fbl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ff_Adlm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ff_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ffm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fia_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fil_Tglg.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fit_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fkv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/flr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fmp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fod_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fon_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fr_Dupl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/frc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/frm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/frp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/frr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/frs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fub_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fuc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fud_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fue_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fuf_Adlm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fuf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fuh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fuq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fur_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fuv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fvr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/fy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ga_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gaa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gag_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gan_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gbm_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gby_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gbz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gcf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gcr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gde_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gej_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gel_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gem_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gez_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ggn_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ggn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/giw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gjk_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gjn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gju_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gju_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gkn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gkp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gld_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/glk_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gmh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gmm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gmv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gmy_Linb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gnd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gng_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/god_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gof_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/goh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gom_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gon_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gon_Gong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gon_Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gon_Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gor_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gos_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/got_Goth.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/got_Runr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gqr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/grb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/grc_Cprt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/grc_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/grc_Linb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/grt_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gsw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gu_Gujr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gub_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/guc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gud_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/guk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gur_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/guu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/guw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gux_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/guz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gvr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gwi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gyi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/gyr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ha_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ha_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hai_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hak_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hak_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/haw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/haz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/he_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hea_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hi_Mahj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hi_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hia_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hif_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hif_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hig_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hit_Xsux.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hlt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hlu_Hluw.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hmd_Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hmd_Plrd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hmn_Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hmn_Hmnp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hmn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hms_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hna_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hnd_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hne_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hni_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hnj_Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hnj_Laoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hnj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hnn_Hano.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hnn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hno_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hns_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ho_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hoc_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hoc_Wara.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hoj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hop_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hsb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hsn_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ht_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hup_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/huu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hy_Armn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hyw_Armn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/hz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ia_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/iba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ibb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/iby_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ica_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ich_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/id_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/id_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/idd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/idu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ie_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ife_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ig_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/igb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ige_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ii_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ii_Yiii.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ijj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ijs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ik_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ikk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ikt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ikw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ikx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ilo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/inh_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/inh_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/inh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/io_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/iqw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/iri_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/is_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/it_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/iu_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/iu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/izh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/izr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/izz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ja_Hira.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ja_Jpan.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ja_Kana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jab_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jbo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jbu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jen_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jgk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jgo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jib_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jiv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jmc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jml_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jpr_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jra_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jrb_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jut_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jv_Java.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/jv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ka_Geok.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ka_Geor.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kaa_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kab_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kab_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kac_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kai_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kaj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kao_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kbd_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kbp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kby_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kca_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kcg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kck_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kdc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kde_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kdh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kdl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kdt_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kea_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kek_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ken_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kez_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kfo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kfr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kfy_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kge_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kgj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kgp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kha_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kha_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/khb_Talu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/khn_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/khq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/khr_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/khr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/khr_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kht_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/khw_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/khw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ki_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kiu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kjg_Laoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kjg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kjh_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kk_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kkh_Lana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kkj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kln_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/km_Khmr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kmb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kmy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kn_Knda.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/knc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/knf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/knp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ko_Kore.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/koi_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/koi_Perm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kok_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/koo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kos_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kpe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kpo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kpy_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kqn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kqp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kqs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kr_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/krc_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kri_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/krj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/krl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/krs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kru_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ks_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ks_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ksb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ksf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ksh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ksp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ksw_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ktj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ktu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ku_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ku_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ku_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ku_Yezi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kub_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kuj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kum_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kun_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kut_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kv_Perm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kvf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kvr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kvx_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kwi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kxm_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kxp_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ky_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ky_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ky_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kye_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kyf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kyq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kyu_Kali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kyw_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kyw_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/kzr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/la_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lab_Lina.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lad_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lah_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/laj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/las_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lbe_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lbw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lcp_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ldb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/led_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lee_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lem_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lep_Lepc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/les_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lez_Aghb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lez_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lfn_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lfn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lgg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lhm_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/li_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lia_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lif_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lif_Limb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lig_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lij_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lip_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lis_Lisu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/liv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ljp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lki_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lkt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lld_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lln_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lmn_Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lmo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lmp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ln_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lns_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lnu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lo_Laoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lob_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/log_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lok_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lol_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/loq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lor_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lot_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/loz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lrc_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ltg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lua_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lue_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lui_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lun_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/luo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lus_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lut_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/luy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/luz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lwl_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lwo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lzh_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lzh_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lzh_Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lzz_Geor.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/lzz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/maf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mag_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mai_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mai_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mai_Tirh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mak_Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mak_Maka.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/man_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/man_Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mas_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/maw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/maz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mbo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mbu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mcd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mcf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mcp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mcu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mda_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mdf_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mdh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mdj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mdr_Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mdr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mdt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/men_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/men_Mend.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/meq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mer_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mey_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mfa_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mfe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mfi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mfn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mfo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mfq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mfv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mgc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mgh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mgo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mgp_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mgy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mhi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mic_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/min_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/min_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/miq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mis_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mis_Hatr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mis_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mis_Nshu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mkl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ml_Mlym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mls_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mlt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mmu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mn_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mn_Mong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mn_Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mn_Zanb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mnc_Mong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mnf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mni_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mni_Mtei.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mns_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mnw_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/moa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/moe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/moh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mor_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mos_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mqb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mql_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mr_Modi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mrd_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mrj_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mro_Mroo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mrw_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mrw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ms_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ms_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/msc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mto_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mtr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mua_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/muh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mui_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mur_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/muy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mvy_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mwk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mwl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mwr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mwv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mww_Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mxc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mxi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mxv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/my_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/myk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mym_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/myv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/myx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/myz_Mand.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mzi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mzk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mzm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mzn_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/mzw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/na_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nan_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nan_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nan_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/naq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nat_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/naw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nch_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ncu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ndc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ndj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nds_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ndz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ne_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ne_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/neb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/new_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/new_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nfr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ng_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nga_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ngb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ngl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ngp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nhb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nhe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nhn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nhu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nhw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nia_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nij_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nin_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nio_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/niu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/niy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/njo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nko_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nku_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nmg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nmz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nnh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nnp_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nnp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nnp_Wcho.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nnq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nnw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/no_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nod_Lana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/noe_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nog_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/non_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/non_Runr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/not_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nov_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nqo_Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nrb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nrf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nsk_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nsk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nso_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nst_Tnsa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ntm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ntr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nui_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nup_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nuv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nwb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nxq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ny_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nym_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nyn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nyo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/nzi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/oaa_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/oc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ogc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ohu_Hung.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/oj_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/oj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ojb_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/oki_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/okr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/om_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/om_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/omn_Lina.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/or_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/orh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/orv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/os_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/osa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/osa_Osge.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/osc_Ital.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/osc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ota_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ote_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/otk_Orkh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/otn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/owl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ozm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pa_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pa_Guru.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pal_Phli.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pal_Phlp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pau_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pbb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pbi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pcd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pck_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pcm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pdc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pdt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/peo_Xpeo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pfl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/phn_Phnx.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pi_Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pi_Sinh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pi_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pip_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pis_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/piu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pka_Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pko_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pms_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/png_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pnt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pnt_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pnt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pon_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pov_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/poy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ppl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pra_Khar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/prd_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/prg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/prq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/prs_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ps_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/puu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pwo_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/pym_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/quc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qud_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/quh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/quy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/quz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qva_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qvc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qvh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qvm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qvn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qwh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qxn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/qxu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rab_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/raj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rar_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ray_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rcf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rej_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rej_Rjng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rel_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/res_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rgn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rhg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rhg_Rohg.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ria_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rif_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rif_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rjs_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rkt_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rmf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rmn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rmo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rmt_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rmu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rng_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ro_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rob_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rof_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rom_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rom_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rtm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ru_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rub_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rue_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ruf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rup_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/rwk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ryu_Jpan.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ryu_Kana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Ahom.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Avst.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Bali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Batk.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Bhks.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Buhd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Cham.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    36822 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Dogr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Gran.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Hano.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Khar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Khoj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Kthi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Lepc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Limb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mahj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Marc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Modi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mroo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mtei.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mult.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Nand.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Olck.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Ranj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Rjng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Saur.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Shrd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sidd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sind.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sinh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sora.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Soyo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sund.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sylo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Tagb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Takr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Tirh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Wara.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Wcho.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Xpeo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Zanb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/saf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sah_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sam_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sam_Samr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/saq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sas_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sat_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sat_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sat_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sat_Olck.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sat_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/saz_Saur.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sbp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sck_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/scn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sco_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/scs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sd_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sd_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sd_Khoj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sd_Sind.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sdc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sdh_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/se_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/se_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/see_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sef_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/seh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sei_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sel_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ses_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sey_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sga_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sga_Ogam.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sgs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/she_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/shi_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/shi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/shi_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/shk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/shn_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/shp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/shu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/si_Sinh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sid_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sig_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sja_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/skr_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/skr_Mult.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sla_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sld_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sli_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/slr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sly_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sma_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/smj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/smn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/smp_Samr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sms_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/snf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/snk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/snn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/snw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/so_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/so_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/so_Osma.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sog_Sogd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sog_Sogo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sok_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sou_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/soy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/spp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sq_Elba.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sr_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/srb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/srb_Sora.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/srn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/srr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/srx_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ss_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ssy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/st_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/stq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/str_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/su_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/su_Sund.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/suk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/suq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sur_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sus_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/swb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/swb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/swc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/swg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/swv_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sxb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sxn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/sxw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/syc_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/syi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/syl_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/syl_Sylo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/syr_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/szl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ta_Taml.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tab_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/taj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/taj_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tal_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tan_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/taq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/taq_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tbw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tbw_Tagb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tbz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tca_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tcy_Knda.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tdd_Tale.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tdg_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tdg_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tdh_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tdt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/te_Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ted_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tem_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/teo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ter_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tet_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tfi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tg_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tg_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/th_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/thf_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/thl_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/thq_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/thr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ths_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ti_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tig_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tik_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tiv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tiw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tjs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tk_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tke_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tkl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tkr_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tkr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tkt_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tlh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tli_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tlj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tly_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tly_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tly_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tmh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tnr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/to_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tob_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tod_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tog_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/toi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/toj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/top_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/toq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tpi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tpm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tr_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/trp_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tru_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tru_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/trv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/trw_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ts_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tsd_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tsf_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tsg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tsi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tsj_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tsw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tsz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tt_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ttj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ttr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tts_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ttt_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ttt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ttt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tul_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tum_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tuq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tvd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tvl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tvu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/twq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/txg_Tang.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/txo_Toto.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ty_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tyv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tzh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tzm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tzm_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/tzo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ude_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/udm_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/udm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/udu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ug_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ug_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/uga_Ugar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/uk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/uli_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/umb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/unr_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/unr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/unr_Nagm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/unr_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/unx_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/unx_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ur_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ura_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/uth_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/utr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/uz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/uz_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/uz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vai_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vai_Vaii.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ve_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vec_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vep_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vi_Hani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vic_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vid_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vls_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vmf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vmw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vot_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vun_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/vut_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wae_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wal_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wal_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wan_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/war_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/was_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wbp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wbq_Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wbr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wci_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wib_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wja_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wji_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wls_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wmw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wni_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wo_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wob_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wsg_Gong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wsg_Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wtm_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wuu_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/wwa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xal_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xcr_Cari.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xed_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xlc_Lyci.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xld_Lydi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xly_Elym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xmf_Geor.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xmn_Mani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xmr_Merc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xmr_Mero.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xna_Narb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xnr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xog_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xon_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xpr_Prti.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xrb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xsa_Sarb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xsm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xsr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xum_Ital.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xum_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xuo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/xwe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yal_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yao_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yas_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yat_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yaz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ybb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ybh_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yer_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yi_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ykg_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yko_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yre_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yrk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yrl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yua_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yue_Hani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yue_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/yue_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/za_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/za_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/za_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zdj_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zdj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zea_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zen_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zgh_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zh_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zh_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zh_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zh_Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ziw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zlm_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zlm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zmi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zne_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/ztu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zul_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zun_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/languages/zza_Latn.textproto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:19.271592 gflanguages-0.8.9/Lib/gflanguages/data/regions/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AX.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/AZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BB.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/BZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CX.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/CZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/DE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/DG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/DJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/DK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/DM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/DO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/DZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/EA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/EC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/EE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/EG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/EH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ER.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ES.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ET.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/FI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/FJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/FK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/FM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/FO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/FR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GB.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/GY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/HK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/HM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/HN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/HR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/HT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/HU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ID.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/IT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/JE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/JM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/JO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/JP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/KZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LB.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/LY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ME.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ML.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MX.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/MZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/NZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/OM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/PY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/QA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/RE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/RO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/RS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/RU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/RW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SB.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ST.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SX.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/SZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/TZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/UA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/UG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/UM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/US.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/UY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/UZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/VA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/VC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/VE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/VG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/VI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/VN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/VU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/WF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/WS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/XK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/YE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/YT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ZA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ZM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/regions/ZW.textproto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:19.303593 gflanguages-0.8.9/Lib/gflanguages/data/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Adlm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Aghb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Ahom.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Aran.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Armi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Armn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Avst.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Bali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Bamu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Bass.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Batk.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Bhks.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Brai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Buhd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Cakm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Cari.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Cham.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Cher.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Chrs.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Copt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Cprt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Dogr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Dsrt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Dupl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Egyp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Elba.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Elym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Geok.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Geor.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Glag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Gong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Goth.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Gran.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Gujr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Guru.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hano.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hatr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hira.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hluw.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hmnp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Hung.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Ital.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Java.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Jpan.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Kali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Kana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Khar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Khmr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Khoj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Knda.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Kore.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Kthi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Lana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Laoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Lepc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Limb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Lina.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Linb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Lisu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Lyci.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Lydi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mahj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Maka.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mand.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Marc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Medf.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mend.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Merc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mero.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mlym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Modi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mroo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mtei.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mult.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Nagm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Nand.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Narb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Nbat.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Nshu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Ogam.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Olck.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Orkh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Osge.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Osma.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Palm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Pauc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Perm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Phli.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Phlp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Phnx.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Plrd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Prti.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Ranj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Rjng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Rohg.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Runr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Samr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sarb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Saur.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Shaw.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Shrd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sidd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sind.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sinh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sogd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sogo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sora.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Soyo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sund.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Sylo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tagb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Takr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tale.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Talu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Taml.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tang.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tavt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tglg.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Thaa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tirh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Tnsa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Toto.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Ugar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Vaii.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Wara.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Wcho.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Xpeo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Xsux.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Yezi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Yiii.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/data/scripts/Zanb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/languages_public.proto
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-06-08 11:33:59.000000 gflanguages-0.8.9/Lib/gflanguages/languages_public_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:18.895587 gflanguages-0.8.9/Lib/gflanguages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-08 11:34:18.000000 gflanguages-0.8.9/Lib/gflanguages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    97838 2023-06-08 11:34:18.000000 gflanguages-0.8.9/Lib/gflanguages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:34:18.000000 gflanguages-0.8.9/Lib/gflanguages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:34:18.000000 gflanguages-0.8.9/Lib/gflanguages.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 11:34:18.000000 gflanguages-0.8.9/Lib/gflanguages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 11:34:18.000000 gflanguages-0.8.9/Lib/gflanguages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-08 11:34:19.307593 gflanguages-0.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-08 11:33:59.000000 gflanguages-0.8.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:18.891587 gflanguages-0.8.9/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:18.891587 gflanguages-0.8.9/data/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:19.303593 gflanguages-0.8.9/data/test/nunito/
--rw-r--r--   0 runner    (1001) docker     (123)   113832 2023-06-08 11:33:59.000000 gflanguages-0.8.9/data/test/nunito/Nunito-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-08 11:33:59.000000 gflanguages-0.8.9/data/test/nunito/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:33:59.000000 gflanguages-0.8.9/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 11:33:59.000000 gflanguages-0.8.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:34:19.307593 gflanguages-0.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-08 11:33:59.000000 gflanguages-0.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:19.303593 gflanguages-0.8.9/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-08 11:33:59.000000 gflanguages-0.8.9/snippets/fix-exemplars-duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-08 11:33:59.000000 gflanguages-0.8.9/snippets/supported_languages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:34:19.307593 gflanguages-0.8.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-06-08 11:33:59.000000 gflanguages-0.8.9/tests/test_data_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-08 11:33:59.000000 gflanguages-0.8.9/tests/test_dottedcircle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-08 11:33:59.000000 gflanguages-0.8.9/tests/test_gflanguages_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 11:33:59.000000 gflanguages-0.8.9/tests/test_parsable.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 11:33:59.000000 gflanguages-0.8.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:19.068445 gflanguages-5.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:18.780429 gflanguages-5.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:18.788430 gflanguages-5.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-28 13:47:03.000000 gflanguages-5.0.4/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-28 13:47:03.000000 gflanguages-5.0.4/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:03.000000 gflanguages-5.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-28 13:47:03.000000 gflanguages-5.0.4/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-28 13:47:03.000000 gflanguages-5.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-28 13:47:03.000000 gflanguages-5.0.4/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-07-28 13:47:03.000000 gflanguages-5.0.4/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:18.780429 gflanguages-5.0.4/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:18.788430 gflanguages-5.0.4/Lib/gflanguages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 13:47:18.000000 gflanguages-5.0.4/Lib/gflanguages/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:18.780429 gflanguages-5.0.4/Lib/gflanguages/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:19.008442 gflanguages-5.0.4/Lib/gflanguages/data/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ab_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/abi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/abq_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/abr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/acd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ace_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/acf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ach_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/acu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ada_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ade_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/adj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/adl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ady_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ae_Avst.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aeb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aeb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/af_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/agc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/agq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/agr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aha_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ahl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aho_Ahom.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ahs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Armi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Chrs.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Egyp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Elym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Hatr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Mani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Narb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Nbat.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Palm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Phli.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Phlp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Phnx.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Prti.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Samr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Sarb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Sogd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Sogo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Ugar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ain_Kana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ain_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ajg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/akk_Xsux.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/akp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/akz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ala_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ale_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aln_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/alt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/am_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/amc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ame_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ami_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/amo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/amr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/an_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/anc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ang_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ank_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ann_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/anp_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/anv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/any_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aoz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/apd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ar_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ar_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arc_Armi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arc_Nbat.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arc_Palm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/aro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arq_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ars_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/art_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ary_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/arz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/as_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/asa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/asg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ast_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/atg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/atj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/auc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/av_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/avk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/avn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/avu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/awa_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/awo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ayb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/az_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/az_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/az_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/azb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/azj_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ba_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bal_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bal_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ban_Bali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ban_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bap_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bar_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bas_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bax_Bamu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bax_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bbc_Batk.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bbc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bbj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bbp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bci_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bcn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bcq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bcw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bcy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bdh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/be_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/be_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/beh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bej_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bej_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bem_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ber_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ber_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ber_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bet_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bew_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bex_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bez_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bfa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bfd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bfq_Taml.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bft_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bft_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bfy_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bg_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bgc_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bgn_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bgx_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bhb_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bhi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bhk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bho_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bho_Kthi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bhy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bib_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bik_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bim_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bin_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/biv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bjj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bjn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bjt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bjv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bkc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bkm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bku_Buhd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bku_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bkv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bla_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/blo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/blt_Tavt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bm_Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bmq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bn_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bn_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bng_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bnm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bo_Marc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bo_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bo_Zanb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/boa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bom_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bov_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/box_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/boz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bpy_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bqc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bqi_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bqj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bqp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bqv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/br_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bra_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/brh_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/brh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/brx_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/brx_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/brx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bs_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bsc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bsj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bsp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bsq_Bass.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bsq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bss_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bto_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/btt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/btv_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bua_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/buc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bud_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bug_Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bum_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/buu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bvb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bvi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bwr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bwy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/byh_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/byn_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/byn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bys_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/byv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bza_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bze_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bzw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/bzx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ca_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cab_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/car_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cbi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cbj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cbk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cbr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cbs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cbt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cbu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cch_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ccp_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ccp_Cakm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cdr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ce_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ceb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cfa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cfm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cgg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ch_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chm_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chn_Dupl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cho_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chp_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chr_Cher.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chx_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/chy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cic_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cja_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cja_Cham.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cjk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cjm_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cjm_Cham.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cjs_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cjy_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ckb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ckl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cko_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ckt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cky_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cla_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cme_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cmg_Soyo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cnh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cni_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/co_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cof_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/con_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cop_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cop_Copt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cop_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cot_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cpf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cps_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cpu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cr_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crh_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cri_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crj_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crk_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crl_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crm_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/crs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/csa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/csb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/csk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/csw_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ctd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ctd_Pauc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cu_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cu_Glag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cwe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/cyo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/da_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/daa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dar_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dbd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dbq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dcc_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ddn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/de_Dupl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/de_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/de_Runr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/del_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/den_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/den_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dga_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dgh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dgi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dgr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dhi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dhw_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/did_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/din_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dip_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dje_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dmf_Medf.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dng_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dnj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/doi_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/doi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/doi_Dogr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/doi_Takr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dop_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dow_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dri_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dsb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dtm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dtp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dts_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dty_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dua_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dum_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/duu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dv_Thaa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dwr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dyi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dyo_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dyo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dyu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dyu_Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dz_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/dzg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ebu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ee_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/efi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/egl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/egy_Egyp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/eka_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ekm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/eky_Kali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/el_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ema_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/emk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/en_Brai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/en_Dsrt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/en_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/en_Shaw.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/enm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/enn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/eo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/es_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ese_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/esg_Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/esu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/et_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ett_Ital.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ett_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/etu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/etx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/eu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/eve_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/evn_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/evn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ewo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ext_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/eza_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fa_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fan_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fbl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ff_Adlm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ff_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ffm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fia_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fil_Tglg.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fit_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fkv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/flr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fmp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fod_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fon_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fr_Dupl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/frc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/frm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/frp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/frr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/frs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fub_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fuc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fud_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fue_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fuf_Adlm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fuf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fuh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fuq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fur_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fuv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fvr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/fy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ga_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gaa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gag_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gan_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gbm_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gby_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gbz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gcf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gcr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gde_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gej_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gel_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gem_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gez_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ggn_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ggn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/giw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gjk_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gjn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gju_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gju_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gkn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gkp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gld_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/glk_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gmh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gmm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gmv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gmy_Linb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gnd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gng_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/god_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gof_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/goh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gom_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gon_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gon_Gong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gon_Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gon_Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gor_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gos_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/got_Goth.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/got_Runr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gqr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/grb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/grc_Cprt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/grc_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/grc_Linb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/grt_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gsw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gu_Gujr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gub_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/guc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gud_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/guk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gur_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/guu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/guw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gux_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/guz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gvr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gwi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gyi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/gyr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ha_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ha_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hai_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hak_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hak_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/haw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/haz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/he_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hea_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hi_Mahj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hi_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hia_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hif_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hif_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hig_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hit_Xsux.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hlt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hlu_Hluw.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hmd_Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hmd_Plrd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hmn_Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hmn_Hmnp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hmn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hms_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hna_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hnd_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hne_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hni_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hnj_Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hnj_Laoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hnj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hnn_Hano.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hnn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hno_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hns_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ho_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hoc_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hoc_Wara.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hoj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hop_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hsb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hsn_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ht_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hup_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/huu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hy_Armn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hyw_Armn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/hz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ia_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/iba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ibb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/iby_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ica_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ich_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/id_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/id_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/idd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/idu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ie_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ife_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ig_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/igb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ige_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ii_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ii_Yiii.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ijj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ijs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ik_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ikk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ikt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ikw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ikx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ilo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/inh_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/inh_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/inh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/io_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/iqw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/iri_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/is_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/it_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/iu_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/iu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/izh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/izr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/izz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ja_Hira.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ja_Jpan.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ja_Kana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jab_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jbo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jbu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jen_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jgk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jgo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jib_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jiv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jmc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jml_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jpr_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jra_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jrb_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jut_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jv_Java.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/jv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ka_Geok.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ka_Geor.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kaa_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kab_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kab_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kac_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kai_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kaj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kao_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kbd_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kbp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kby_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kca_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kcg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kck_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kdc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kde_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kdh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kdl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kdt_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kea_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kek_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ken_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kez_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kfo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kfr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kfy_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kge_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kgj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kgp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kha_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kha_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/khb_Talu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/khn_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/khq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/khr_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/khr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/khr_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kht_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/khw_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/khw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ki_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kiu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kjg_Laoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kjg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kjh_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kk_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kkh_Lana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kkj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kln_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/km_Khmr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kmb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kmy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kn_Knda.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/knc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/knf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/knp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ko_Kore.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/koi_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/koi_Perm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kok_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/koo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kos_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kpe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kpo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kpy_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kqn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kqp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kqs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kr_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/krc_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kri_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/krj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/krl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/krs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kru_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ks_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ks_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ksb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ksf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ksh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ksp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ksw_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ktj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ktu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ku_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ku_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ku_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ku_Yezi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kub_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kuj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kum_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kun_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kut_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kv_Perm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kvf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kvr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kvx_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kwi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kxm_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kxp_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ky_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ky_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ky_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kye_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kyf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kyq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kyu_Kali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kyw_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kyw_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/kzr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/la_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lab_Lina.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lad_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lah_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/laj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/las_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lbe_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lbw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lcp_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ldb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/led_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lee_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lem_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lep_Lepc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/les_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lez_Aghb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lez_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lfn_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lfn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lgg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lhm_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/li_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lia_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lif_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lif_Limb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lig_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lij_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lip_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-28 13:47:03.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lis_Lisu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/liv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ljp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lki_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lkt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lld_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lln_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lmn_Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lmo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lmp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ln_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lns_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lnu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lo_Laoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lob_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/log_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lok_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lol_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/loq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lor_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lot_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/loz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lrc_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ltg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lua_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lue_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lui_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lun_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/luo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lus_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lut_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/luy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/luz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lwl_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lwo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lzh_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lzh_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lzh_Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lzz_Geor.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/lzz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/maf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mag_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mai_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mai_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mai_Tirh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mak_Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mak_Maka.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/man_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/man_Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mas_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/maw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/maz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mbo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mbu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mcd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mcf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mcp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mcu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mda_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mdf_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mdh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mdj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mdr_Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mdr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mdt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/men_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/men_Mend.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/meq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mer_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mey_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mfa_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mfe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mfi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mfn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mfo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mfq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mfv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mgc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mgh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mgo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mgp_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mgy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mhi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mic_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/min_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/min_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/miq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mis_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mis_Hatr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mis_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mis_Nshu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mkl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ml_Mlym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mls_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mlt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mmu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mn_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mn_Mong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mn_Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mn_Zanb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mnc_Mong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mnf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mni_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mni_Mtei.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mns_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mnw_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/moa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/moe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/moh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mor_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mos_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mqb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mql_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mr_Modi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mrd_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mrj_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mro_Mroo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mrw_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mrw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ms_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ms_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/msc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mto_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mtr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mua_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/muh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mui_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mur_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/muy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mvy_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mwk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mwl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mwr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mwv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mww_Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mxc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mxi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mxv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/my_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/myk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mym_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/myv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/myx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/myz_Mand.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mzi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mzk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mzm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mzn_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/mzw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/na_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nan_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nan_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nan_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/naq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nat_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/naw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nch_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ncu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ndc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ndj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nds_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ndz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ne_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ne_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/neb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/new_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/new_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nfr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ng_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nga_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ngb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ngl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ngp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nhb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nhe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nhn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nhu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nhw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nia_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nij_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nin_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nio_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/niu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/niy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/njo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nko_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nku_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nmg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nmz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nnh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nnp_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nnp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nnp_Wcho.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nnq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nnw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/no_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nod_Lana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/noe_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nog_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/non_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/non_Runr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/not_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nov_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nqo_Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nrb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nrf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nsk_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nsk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nso_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nst_Tnsa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ntm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ntr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nui_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nup_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nuv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nwb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nxq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ny_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nym_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nyn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nyo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/nzi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/oaa_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/oc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ogc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ohu_Hung.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/oj_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/oj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ojb_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/oki_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/okr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/om_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/om_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/omn_Lina.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/or_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/orh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/orv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/os_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/osa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/osa_Osge.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/osc_Ital.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/osc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ota_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ote_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/otk_Orkh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/otn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/owl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ozm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pa_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pa_Guru.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pal_Phli.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pal_Phlp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pau_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pbb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pbi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pcd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pck_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pcm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pdc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pdt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/peo_Xpeo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pfl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/phn_Phnx.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pi_Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pi_Sinh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pi_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pip_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pis_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/piu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pka_Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pko_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pms_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/png_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pnt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pnt_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pnt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pon_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pov_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/poy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ppl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pra_Khar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/prd_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/prg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/prq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/prs_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ps_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/puu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pwo_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/pym_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/quc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qud_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/quh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/quy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/quz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qva_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qvc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qvh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qvm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qvn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qwh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qxn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/qxu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rab_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/raj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rar_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ray_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rcf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rej_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rej_Rjng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rel_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/res_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rgn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rhg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rhg_Rohg.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ria_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rif_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rif_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rjs_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rkt_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rmf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rmn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rmo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rmt_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rmu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rng_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ro_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rob_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rof_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rom_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rom_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rtm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ru_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rub_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rue_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ruf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rup_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/rwk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ryu_Jpan.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ryu_Kana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Ahom.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Bali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Bhks.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Cham.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Gran.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Khar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Limb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Marc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Modi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Mong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Mroo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Mtei.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Mult.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Nand.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Ranj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Rjng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Shrd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sidd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sind.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sinh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sora.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Soyo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sund.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sylo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Tagb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Tirh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Wara.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Wcho.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Xpeo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Zanb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/saf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sah_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sam_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sam_Samr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/saq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sas_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sat_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sat_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sat_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sat_Olck.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sat_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/saz_Saur.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sbp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sck_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/scn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sco_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/scs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sd_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sd_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sd_Khoj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sd_Khud.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sdc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sdh_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/se_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/se_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/see_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sef_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/seh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sei_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sel_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ses_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sey_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sga_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sga_Ogam.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sgs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/she_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/shi_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/shi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/shi_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/shk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/shn_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/shp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/shu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/si_Sinh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sid_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sig_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sja_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/skr_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/skr_Mult.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sla_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sld_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sli_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/slr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sly_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sma_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/smj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/smn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/smp_Samr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sms_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/snf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/snk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/snn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/snw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/so_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/so_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/so_Osma.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sog_Sogd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sog_Sogo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sok_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sou_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/soy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/spp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sq_Elba.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sq_Vith.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sr_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/srb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/srb_Sora.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/srn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/srr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/srx_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ss_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ssy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/st_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/stq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/str_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/su_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/su_Sund.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/suk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/suq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sur_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sus_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/swb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/swb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/swc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/swg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/swv_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sxb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sxn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/sxw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/syc_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/syi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/syl_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/syl_Sylo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/syr_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/szl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ta_Taml.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tab_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/taj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/taj_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tal_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tan_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/taq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/taq_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tbw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tbw_Tagb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tbz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tca_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tcy_Knda.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tdd_Tale.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tdg_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tdg_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tdh_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tdt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/te_Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ted_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tem_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/teo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ter_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tet_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tfi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tg_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tg_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/th_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/thf_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/thl_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/thq_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/thr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ths_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ti_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tig_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tik_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tiv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tiw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tjs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tk_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tke_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tkl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tkr_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tkr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tkt_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tlh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tli_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tlj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tly_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tly_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tly_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tmh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tnr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/to_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tob_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tod_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tog_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/toi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/toj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/top_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/toq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tpi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tpm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tr_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/trp_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tru_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tru_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/trv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/trw_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ts_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tsd_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tsf_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tsg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tsi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tsj_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tsw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tsz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tt_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ttj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ttr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tts_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ttt_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ttt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ttt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tul_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tum_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tuq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tvd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tvl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tvu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/twq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/txg_Tang.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/txo_Toto.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ty_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tyv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tzh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tzm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tzm_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/tzo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ude_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/udm_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/udm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/udu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ug_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ug_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/uga_Ugar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/uk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/uli_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/umb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/unr_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/unr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/unr_Nagm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/unr_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/unx_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/unx_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ur_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ura_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/uth_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/utr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/uz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/uz_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/uz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vai_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vai_Vaii.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ve_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vec_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vep_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vi_Hani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vic_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vid_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vls_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vmf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vmw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vot_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vun_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/vut_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wae_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wal_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wal_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wan_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/war_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/was_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wbp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wbq_Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wbr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wci_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wib_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wja_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wji_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wls_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wmw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wni_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wo_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wob_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wsg_Gong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wsg_Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wtm_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wuu_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/wwa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xal_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xcr_Cari.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xed_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xlc_Lyci.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xld_Lydi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xly_Elym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xmf_Geor.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xmn_Mani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xmr_Merc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xmr_Mero.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xna_Narb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xnr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xog_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xon_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xpr_Prti.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xrb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xsa_Sarb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xsm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xsr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xum_Ital.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xum_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xuo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/xwe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yal_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yao_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yas_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yat_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yaz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ybb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ybh_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yer_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yi_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ykg_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yko_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yre_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yrk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yrl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yua_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yue_Hani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yue_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    15072 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/yue_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/za_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/za_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/za_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zdj_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zdj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zea_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zen_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zgh_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zh_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zh_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zh_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zh_Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ziw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zlm_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zlm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zmi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zne_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/ztu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zul_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zun_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/languages/zza_Latn.textproto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:19.044443 gflanguages-5.0.4/Lib/gflanguages/data/regions/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AX.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/AZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BB.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/BZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CX.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/CZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/DE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/DG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/DJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/DK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/DM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/DO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/DZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/EA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/EC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/EE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/EG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/EH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ER.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ES.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ET.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/FI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/FJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/FK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/FM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/FO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/FR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GB.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/GY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/HK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/HM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/HN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/HR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/HT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/HU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ID.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/IT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/JE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/JM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/JO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/JP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/KZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LB.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/LY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ME.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ML.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MX.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/MZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/NZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/OM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/PY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/QA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/RE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/RO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/RS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/RU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/RW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SB.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ST.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SX.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/SZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/TZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/UA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/UG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/UM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/US.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/UY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/UZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/VA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/VC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/VE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/VG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/VI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/VN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/VU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/WF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/WS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/XK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/YE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/YT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ZA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ZM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/regions/ZW.textproto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:19.064445 gflanguages-5.0.4/Lib/gflanguages/data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Adlm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Aghb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Ahom.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Aran.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Armi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Armn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Avst.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Bali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Bamu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Bass.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Batk.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Bhks.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Brai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Buhd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Cakm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Cari.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Cham.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Cher.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Chrs.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Copt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Cprt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Dogr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Dsrt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Dupl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Egyp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Elba.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Elym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Geok.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Geor.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Glag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Gong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Goth.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Gran.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Gujr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Guru.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hano.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hatr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hira.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hluw.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hmnp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Hung.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Ital.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Java.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Jpan.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Kali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Kana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Khar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Khmr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Khoj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Knda.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Kore.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Kthi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Lana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Laoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Lepc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Limb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Lina.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Linb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Lisu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Lyci.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Lydi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mahj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Maka.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mand.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Marc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Medf.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mend.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Merc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mero.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mlym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Modi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mroo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mtei.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mult.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Nagm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Nand.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Narb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Nbat.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Nshu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Ogam.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Olck.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Orkh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Osge.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Osma.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Palm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Pauc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Perm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Phli.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Phlp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Phnx.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Plrd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Prti.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Ranj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Rjng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Rohg.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Runr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Samr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sarb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Saur.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Shaw.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Shrd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sidd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sind.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sinh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sogd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sogo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sora.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Soyo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sund.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Sylo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tagb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Takr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tale.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Talu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Taml.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tang.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tavt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tglg.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Thaa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tirh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Tnsa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Toto.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Ugar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Vaii.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Vith.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Wara.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Wcho.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Xpeo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Xsux.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Yezi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Yiii.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/data/scripts/Zanb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/languages_public.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-07-28 13:47:04.000000 gflanguages-5.0.4/Lib/gflanguages/languages_public_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:18.792430 gflanguages-5.0.4/Lib/gflanguages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-28 13:47:18.000000 gflanguages-5.0.4/Lib/gflanguages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    97343 2023-07-28 13:47:18.000000 gflanguages-5.0.4/Lib/gflanguages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:47:18.000000 gflanguages-5.0.4/Lib/gflanguages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:47:18.000000 gflanguages-5.0.4/Lib/gflanguages.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 13:47:18.000000 gflanguages-5.0.4/Lib/gflanguages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 13:47:18.000000 gflanguages-5.0.4/Lib/gflanguages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-28 13:47:19.068445 gflanguages-5.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-28 13:47:04.000000 gflanguages-5.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:18.780429 gflanguages-5.0.4/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:18.780429 gflanguages-5.0.4/data/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:19.064445 gflanguages-5.0.4/data/test/nunito/
+-rw-r--r--   0 runner    (1001) docker     (123)   113832 2023-07-28 13:47:04.000000 gflanguages-5.0.4/data/test/nunito/Nunito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-28 13:47:04.000000 gflanguages-5.0.4/data/test/nunito/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:47:04.000000 gflanguages-5.0.4/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 13:47:04.000000 gflanguages-5.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:47:19.068445 gflanguages-5.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-28 13:47:04.000000 gflanguages-5.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:19.064445 gflanguages-5.0.4/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-28 13:47:04.000000 gflanguages-5.0.4/snippets/fix-exemplars-duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-28 13:47:04.000000 gflanguages-5.0.4/snippets/supported_languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:47:19.068445 gflanguages-5.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-28 13:47:04.000000 gflanguages-5.0.4/tests/test_data_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-28 13:47:04.000000 gflanguages-5.0.4/tests/test_dottedcircle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-28 13:47:04.000000 gflanguages-5.0.4/tests/test_gflanguages_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-28 13:47:04.000000 gflanguages-5.0.4/tests/test_parsable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 13:47:04.000000 gflanguages-5.0.4/tox.ini
```

### Comparing `gflanguages-0.8.9/.github/workflows/publish-release.yml` & `gflanguages-5.0.4/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/.github/workflows/tox.yml` & `gflanguages-5.0.4/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/CHANGELOG.md` & `gflanguages-5.0.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-Below are the most important changes from each release.
+### Check the [releases notes](https://github.com/googlefonts/lang/releases), they are up to date and complete. 
 
-## Next release
+## 0.5.0 (2023-Jun-22)
+Add Vithkuqi script/language by @simoncozens in #88
+
+## 0.4.9 (2023-Jun-08)
+Replace Sanskrit Gunjala Gondi transliteration with new sample by @simoncozens in https://github.com/googlefonts/lang/pull/85
 
 ## 0.4.8 (2023-Jun-02)
 * Test languages exemplars canonical duplicates by @moyogo in https://github.com/googlefonts/lang/pull/41
 * fixup test_canonical_duplicates by @moyogo in https://github.com/googlefonts/lang/pull/75
 * Remove U+030D U+030E from Thai marks by @simoncozens in https://github.com/googlefonts/lang/pull/76
 * grc_Cprt: add source for samples by @moyogo in https://github.com/googlefonts/lang/pull/79
 * Add Makassarese in Old Makasar script by @simoncozens in https://github.com/googlefonts/lang/pull/74
```

### Comparing `gflanguages-0.8.9/CONTRIBUTORS.txt` & `gflanguages-5.0.4/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/LICENSE.txt` & `gflanguages-5.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/__init__.py` & `gflanguages-5.0.4/Lib/gflanguages/__init__.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aa_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ab_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ab_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ace_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ace_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/acf_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/acf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/acu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/acu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ada_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ada_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/adl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/adl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ady_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ady_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/af_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/af_Latn.textproto`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 region: "BW"
 region: "NA"
 region: "ZA"
 exemplar_chars {
   base: "a A á Á â Â b B c C d D e E é É è È ê Ê ë Ë f F g G h H i I î Î ï Ï j J k K l L m M n N o O ô Ô ö Ö p P q Q r R s S t T u U û Û v V w W x X y Y z Z"
   auxiliary: "à À å Å ä Ä ã Ã æ Æ ç Ç í Í ì Ì ó Ó ò Ò ú Ú ù Ù ü Ü ý Ý"
   marks: "◌̀ ◌̂ ◌̈"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Ee"
   styles: "AANGESIEN erkenning vir die inherente waardigheid"
   tester: "AANGESIEN minagting vir menseregte barbaarse dade wat die gewete"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/agq_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nmg_Latn.textproto`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-id: "agq_Latn"
-language: "agq"
+id: "nmg_Latn"
+language: "nmg"
 script: "Latn"
-name: "Aghem"
-autonym: "Wum"
-population: 38843
+name: "Kwasio"
+autonym: "Kwasio"
+population: 8878
 region: "CM"
 exemplar_chars {
-  base: "a A à À â Â ǎ Ǎ ā Ā b B c C d D e E è È ê Ê ě Ě ē Ē ɛ Ɛ {ɛ̀} {Ɛ̀} {ɛ̂} {Ɛ̂} {ɛ̌} {Ɛ̌} {ɛ̄} {Ɛ̄} f F g G h H i I ì Ì î Î ǐ Ǐ ī Ī ɨ Ɨ {ɨ̀} {Ɨ̀} {ɨ̂} {Ɨ̂} {ɨ̌} {Ɨ̌} {ɨ̄} {Ɨ̄} k K l L m M n N ŋ Ŋ o O ò Ò ô Ô ǒ Ǒ ō Ō ɔ Ɔ {ɔ̀} {Ɔ̀} {ɔ̂} {Ɔ̂} {ɔ̌} {Ɔ̌} {ɔ̄} {Ɔ̄} p P s S t T u U ù Ù û Û ǔ Ǔ ū Ū ʉ Ʉ {ʉ̀} {Ʉ̀} {ʉ̂} {Ʉ̂} {ʉ̌} {Ʉ̌} {ʉ̄} {Ʉ̄} v V w W y Y z Z ʔ"
-  auxiliary: "q Q r R x X"
-  marks: "◌̀ ◌̂ ◌̄ ◌̌"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  index: "A B C D E Ɛ F G H I Ɨ K L M N Ŋ O Ɔ P S T U Ʉ V W Y Z ʔ"
+  base: "a A á Á â Â ǎ Ǎ ä Ä ā Ā b B ɓ Ɓ c C d D e E é É ê Ê ě Ě ē Ē ǝ Ǝ {ǝ́} {Ǝ́} {ǝ̂} {Ǝ̂} {ǝ̌} {Ǝ̌} {ǝ̄} {Ǝ̄} ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̂} {Ɛ̂} {ɛ̌} {Ɛ̌} {ɛ̄} {Ɛ̄} f F g G h H i I í Í î Î ǐ Ǐ ï Ï ī Ī j J k K l L m M n N ń Ń ŋ Ŋ o O ó Ó ô Ô ǒ Ǒ ö Ö ō Ō ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̂} {Ɔ̂} {ɔ̌} {Ɔ̌} {ɔ̄} {Ɔ̄} p P r R ŕ Ŕ s S t T u U ú Ú û Û ǔ Ǔ ū Ū v V w W y Y"
+  auxiliary: "q Q x X z Z"
+  marks: "◌́ ◌̂ ◌̄ ◌̈ ◌̌"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  index: "A B Ɓ C D E Ǝ Ɛ F G H I J K L M N Ŋ O Ɔ P R S T U V W Y"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/agr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/agr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Armi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Armi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Brah.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Brah.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Chrs.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Chrs.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Egyp.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Egyp.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Elym.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Elym.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Hatr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Hatr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Mani.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Mani.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Narb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Narb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Nbat.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Nbat.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Palm.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Palm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Phli.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Phli.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Phlp.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Phlp.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Phnx.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Phnx.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Prti.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Prti.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Samr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Samr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Sarb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Sarb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Sogd.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Sogd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Sogo.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Sogo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Syrc.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Syrc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aii_Ugar.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aii_Ugar.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ajg_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ajg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ak_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ak_Latn.textproto`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Akan"
 autonym: "Fante"
 population: 11442678
 region: "GH"
 exemplar_chars {
   base: "a A b B d D e E ɛ Ɛ f F g G h H i I k K l L m M n N o O ɔ Ɔ p P r R s S t T u U w W y Y"
   auxiliary: "c C j J q Q v V z Z"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E Ɛ F G H I J K L M N O Ɔ P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "WwƆɔ"
   masthead_partial: "Oo"
   styles: "Ɔnam dɛ adasa hɔn enyimnyam yɛ pɛr na ndzinoa"
   tester: "Ɔnam dɛ tsia a yetsiatsia nyimpa ne ndzinoa do no dze ewurkadze"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/akk_Xsux.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/akk_Xsux.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ale_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ale_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/aln_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/aln_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/alt_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/alt_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 exemplar_chars {
   base: "А Б В Г Д Е Ж З И Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ъ Ы Ь Э Ю Я Ё Ј Ҥ Ӧ Ӱ а б в г д е ж з и й к л м н о п р с т у ф х ц ч ш щ ъ ы ь э ю я ё ј ҥ ӧ ӱ"
   marks: "◌̆ ◌̈"
 }
 sample_text {
   masthead_full: "ОоНн"
   masthead_partial: "Чч"
-  styles: "Кижилик билезиниҥ  ончо турчыларыныҥ јарамыкту,"
+  styles: "Кижилик билезиниҥ ончо турчыларыныҥ јарамыкту,"
   tester: "Ончо улус ак-јарыкка јайым ла теҥ-тай тап-эриктӱ туулат. Олор санааукаалу"
   poster_sm: "Кажы ла кижиде"
   poster_md: "Ого ӱзеери"
   poster_lg: "Ончо"
   specimen_48: "Кажы ла кижи јадын-јӱрӱмге, јайымга ла таҥынаҥ бойына тийерге јарабас"
-  specimen_36: "Кем де кандый да кыйынга эмезе оныҥ учурын, тоомјызын тӱжӱрип турган кижи  кӱӱни јок базынышка алдыртпас учурлу."
-  specimen_32: "Кажы ла кижи ого Конституцияла эмезе јасакла берилген тӧс тап-эриктери бузулган тужында ийделӱ, тоомјылу эл јаргыларда  тап-эриктерин једимдӱ орныктырарга тап-эриктӱ."
+  specimen_36: "Кем де кандый да кыйынга эмезе оныҥ учурын, тоомјызын тӱжӱрип турган кижи кӱӱни јок базынышка алдыртпас учурлу."
+  specimen_32: "Кажы ла кижи ого Конституцияла эмезе јасакла берилген тӧс тап-эриктери бузулган тужында ийделӱ, тоомјылу эл јаргыларда тап-эриктерин једимдӱ орныктырарга тап-эриктӱ."
   specimen_21: "Кемди де тууразынаҥ олјолоорго, тударга эмезе сӱрерге јарабас.\nКажы ла кижи оныҥ тап-эриктерин ле молјуларын чокымдаарга, онойдо ок ого эдилген уголовный бурулаштыҥ тӧзӧгӧзин чокымдаарга толо теҥ-тайга тайанып, оныҥ кереги ачык-јарык айалгада кӧрӱлзин ле јаргы ак-чек, кемнеҥ де камаанду эмес чындык болзын деп тап-эриктӱ."
-  specimen_16: "Оныҥ таҥынаҥ ла билелик јӱрӱмине тууразынаҥ кем де киришпес учурлу. Онойдо ок кем де оныҥ айыл-јуртына, корреспонденциязыныҥ  јажыдына эмезе оныҥ ады-јолына, јӱрӱмине тууразынаҥ кирижер учуры јок. Кажы ла кижи ондый табарудаҥ, кирижеринеҥ коруланар јасакка тап-эриктӱ.\nКажы ла кижи јайым кӱӱн-санаага, ак-чекке ле кудай јаҥына тап-эриктӱ; бу тап-эрикке бойыныҥ кудай јаҥын эмезе кӧрӱмин солыыры кирет, бойыныҥ јаҥын јайым јаҥдаары эмезе кӧрӱмин таҥынаҥ бойы, эмезе ӧскӧ улусла кожо јаҥдаары база кирет. Кудайлык чӱм-јаҥ јаҥжыгуларды ӧткӱреринде тапэриктӱ.\nКажы ла кижи амыраарга ла бош ӧйгӧ тап-эриктӱ. Онойдо ок иштеер кӱнди керектӱ кеминде тузаланары ла тӧлӧлип турган јаҥжыккан  амыралта (отпуск) керегинде тап-эрик база кирет."
+  specimen_16: "Оныҥ таҥынаҥ ла билелик јӱрӱмине тууразынаҥ кем де киришпес учурлу. Онойдо ок кем де оныҥ айыл-јуртына, корреспонденциязыныҥ јажыдына эмезе оныҥ ады-јолына, јӱрӱмине тууразынаҥ кирижер учуры јок. Кажы ла кижи ондый табарудаҥ, кирижеринеҥ коруланар јасакка тап-эриктӱ.\nКажы ла кижи јайым кӱӱн-санаага, ак-чекке ле кудай јаҥына тап-эриктӱ; бу тап-эрикке бойыныҥ кудай јаҥын эмезе кӧрӱмин солыыры кирет, бойыныҥ јаҥын јайым јаҥдаары эмезе кӧрӱмин таҥынаҥ бойы, эмезе ӧскӧ улусла кожо јаҥдаары база кирет. Кудайлык чӱм-јаҥ јаҥжыгуларды ӧткӱреринде тапэриктӱ.\nКажы ла кижи амыраарга ла бош ӧйгӧ тап-эриктӱ. Онойдо ок иштеер кӱнди керектӱ кеминде тузаланары ла тӧлӧлип турган јаҥжыккан амыралта (отпуск) керегинде тап-эрик база кирет."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/am_Ethi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/am_Ethi.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 name: "Amharic"
 autonym: "አማርኛ"
 population: 35728475
 region: "ET"
 region: "IL"
 exemplar_chars {
   base: "ሀ ሁ ሂ ሃ ሄ ህ ሆ ለ ሉ ሊ ላ ሌ ል ሎ ሏ ሐ ሑ ሒ ሓ ሔ ሕ ሖ ሗ መ ሙ ሚ ማ ሜ ም ሞ ሟ ሠ ሡ ሢ ሣ ሤ ሥ ሦ ሧ ረ ሩ ሪ ራ ሬ ር ሮ ሯ ሰ ሱ ሲ ሳ ሴ ስ ሶ ሷ ሸ ሹ ሺ ሻ ሼ ሽ ሾ ሿ ቀ ቁ ቂ ቃ ቄ ቅ ቆ ቈ ቊ ቋ ቌ ቍ በ ቡ ቢ ባ ቤ ብ ቦ ቧ ቨ ቩ ቪ ቫ ቬ ቭ ቮ ቯ ተ ቱ ቲ ታ ቴ ት ቶ ቷ ቸ ቹ ቺ ቻ ቼ ች ቾ ቿ ኀ ኁ ኂ ኃ ኄ ኅ ኆ ኈ ኊ ኋ ኌ ኍ ነ ኑ ኒ ና ኔ ን ኖ ኗ ኘ ኙ ኚ ኛ ኜ ኝ ኞ ኟ አ ኡ ኢ ኣ ኤ እ ኦ ኧ ከ ኩ ኪ ካ ኬ ክ ኮ ኰ ኲ ኳ ኴ ኵ ኸ ኹ ኺ ኻ ኼ ኽ ኾ ወ ዉ ዊ ዋ ዌ ው ዎ ዐ ዑ ዒ ዓ ዔ ዕ ዖ ዘ ዙ ዚ ዛ ዜ ዝ ዞ ዟ ዠ ዡ ዢ ዣ ዤ ዥ ዦ ዧ የ ዩ ዪ ያ ዬ ይ ዮ ደ ዱ ዲ ዳ ዴ ድ ዶ ዷ ጀ ጁ ጂ ጃ ጄ ጅ ጆ ጇ ገ ጉ ጊ ጋ ጌ ግ ጎ ጐ ጒ ጓ ጔ ጕ ጠ ጡ ጢ ጣ ጤ ጥ ጦ ጧ ጨ ጩ ጪ ጫ ጬ ጭ ጮ ጯ ጰ ጱ ጲ ጳ ጴ ጵ ጶ ጷ ጸ ጹ ጺ ጻ ጼ ጽ ጾ ጿ ፀ ፁ ፂ ፃ ፄ ፅ ፆ ፈ ፉ ፊ ፋ ፌ ፍ ፎ ፏ ፐ ፑ ፒ ፓ ፔ ፕ ፖ ፗ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "‐ – , ፡ ፣ ፤ ፥ ፦ ! ? . ። ‹ › « » ( ) [ ]"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "– , ፡ ፣ ፤ ፥ ፦ ! ? . ። ‹ › « » ( ) [ ]"
   index: "ሀ ለ ሐ መ ሠ ረ ሰ ሸ ቀ ቈ በ ቨ ተ ቸ ኀ ኈ ነ ኘ አ ከ ኰ ኸ ወ ዐ ዘ ዠ የ ደ ጀ ገ ጐ ጠ ጨ ጰ ጸ ፀ ፈ ፐ"
 }
 sample_text {
   masthead_full: "የሰውል"
   masthead_partial: "ጅሁ"
   styles: "የሰው፡ልጅ፡ሁሉ፡ሲወለድ፡ነጻና፡በክብርና፡በመብትም፡እኩልነት፡ያለው፡ነው።፡የተፈጥሮ፡ማስተዋልና"
   tester: "እያንዳንዱ፡ሰው፡የዘር፡የቀለም፡የጾታ፡የቋንቋ፡የሃይማኖት፡የፖለቲካ፡ወይም፡የሌላ፡ዓይነት፡አስተሳሰብ፡የብሔራዊ፡ወይም፡የኀብረተሰብ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/amc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/amc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ame_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ame_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ami_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ami_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/amr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/amr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/an_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/an_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ang_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ang_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ar_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ar_Arab.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 region: "TJ"
 region: "TN"
 region: "TR"
 region: "YE"
 exemplar_chars {
   base: "ً ٌ ٍ َ ُ ِ ّ ْ ٰ ء أ ؤ إ ئ ا آ ب ة ت ث ج ح خ د ذ ر ز س ش ص ض ط ظ ع غ ف ق ك ل م ن ه و ى ي"
   auxiliary: "ـ‌‍‎‏ پ چ ژ ڜ ڢ ڤ ڥ ٯ ڧ ڨ ک گ ی"
-  numerals: "؜‎ - ‑ , ٫ ٬ . % ٪ ‰ ؉ + 0٠ 1١ 2٢ 3٣ 4٤ 5٥ 6٦ 7٧ 8٨ 9٩"
-  punctuation: "- ‐ ‑ – — ، ؛ : ! ؟ . … \' \" « » ( ) [ ]"
+  numerals: "؜‎ - , ٫ ٬ . % ٪ ؉ + 0٠ 1١ 2٢ 3٣ 4٤ 5٥ 6٦ 7٧ 8٨ 9٩"
+  punctuation: "- – — ، ؛ : ! ؟ . … \' \" « » ( ) [ ]"
   index: "ا ب ت ث ج ح خ د ذ ر ز س ش ص ض ط ظ ع غ ف ق ك ل م ن ه و ي"
 }
 sample_text {
   masthead_full: "يولد"
   masthead_partial: "جم"
   styles: "لمّا كان الاعتراف بالكرامة المتأصلة في جميع"
   tester: "ولما كان تناسي حقوق الإنسان وازدراؤها قد أفضيا إلى أعمال همجية"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/arb_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/arb_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/arc_Armi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/arc_Armi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/arc_Nbat.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/arc_Nbat.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/arc_Palm.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/arc_Palm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/arl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/arl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/arn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/arn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/arp_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/arp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/art_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/art_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/arz_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/arz_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/as_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/as_Beng.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "অসমীয়া"
 population: 17239170
 region: "IN"
 exemplar_chars {
   base: "় অ আ ই ঈ উ ঊ ঋ এ ঐ ও ঔ ং ঁ ঃ ক খ গ ঘ ঙ চ ছ জ ঝ ঞ ট ঠ ড {ড়} ঢ {ঢ়} ণ ত থ দ ধ ন প ফ ব ভ ম য {য়} ৰ ল ৱ শ ষ স হ {ক্ষ} া ি ী ু ূ ৃ ে ৈ ো ৌ ্"
   auxiliary: "‌‍ ৲ ৎ র"
   marks: "◌ঁ ◌ং ◌ঃ ◌় ◌া ◌ি ◌ী ◌ু ◌ূ ◌ৃ ◌ৄ ◌ে ◌ৈ ◌্ ◌ৗ ◌ৢ ◌ৣ"
-  numerals: "- ‑ , . % ‰ + 0০ 1১ 2২ 3৩ 4৪ 5৫ 6৬ 7৭ 8৮ 9৯"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … । \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0০ 1১ 2২ 3৩ 4৪ 5৫ 6৬ 7৭ 8৮ 9৯"
+  punctuation: "- – — , ; : ! ? . … । \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "় অ আ ই ঈ উ ঊ ঋ এ ঐ ও ঔ ং ঃ ক খ গ ঘ ঙ চ ছ জ ঝ ঞ ট ঠ ড ঢ ণ ৎ ত থ দ ধ ন প ফ ব ভ ম য ৰ ল ৱ শ ষ স হ ্"
 }
 sample_text {
   masthead_full: "জনমগ"
   masthead_partial: "তভ"
   styles: "জন্মগতভাৱে সকলো মানুহ মৰ্য্যদা আৰু অধিকাৰত সমান আৰু স্বতন্ত্ৰ।"
   tester: "জন্মগতভাৱে সকলো মানুহ মৰ্য্যদা আৰু অধিকাৰত সমান আৰু স্বতন্ত্ৰ। তেওঁলোকৰ বিবেক আছে, বুদ্ধি"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ast_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ast_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Asturianu"
 population: 650205
 region: "ES"
 exemplar_chars {
   base: "a á b c d e é f g h ḥ i í l ḷ m n ñ o ó p q r s t u ú ü v x y z"
   auxiliary: "ª à ă â å ä ã ā æ ç è ĕ ê ë ē ì ĭ î ï ī j k º ò ŏ ô ö ø ō œ ù ŭ û ū w ÿ"
   marks: "◌́ ◌̃ ◌̈ ◌̣"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ¡ ? ¿ . … \' ‘ ’ \" “ ” « » ( ) [ ] § @ * / \\ & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ¡ ? ¿ . … \' ‘ ’ \" “ ” « » ( ) [ ] @ * / \\ & #"
   index: "A B C D E F G H I L M N Ñ O P Q R S T U V X Y Z"
 }
 sample_text {
   masthead_full: "TtOo"
   masthead_partial: "Ll"
   styles: "Visto que la llibertá, la xusticia y la paz"
   tester: "Visto que desconocer o facer de menos los drechos humanos foi"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/auc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/auc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/awa_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/awa_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ay_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ay_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/az_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/az_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 population: 1142175
 region: "AZ"
 region: "RU"
 exemplar_chars {
   base: "а ә б в г ғ д е ж з и й ј к ҝ л м н о ө п р с т у ү ф х һ ч ҹ ш ы"
   auxiliary: "ц щ ъ ь э ю я"
   marks: "◌̆"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "А Ә Б В Г Ғ Д Е Ж З И Й Ј К Ҝ Л М Н О Ө П Р С Т У Ү Ф Х Һ Ч Ҹ Ш Ы"
 }
 sample_text {
   masthead_full: "БбҮү"
   masthead_partial: "Тт"
   styles: "Бәшәр аиләсинин бүтүн үзвләринә хас олан"
   tester: "инсан һүгугларына етинасызлыг вә нифрәтин бәшәријјәти дәһшәтә"
   poster_sm: "инсанын сон"
   poster_md: "халглар"
   poster_lg: "Бүтүн"
   specimen_48: "Бирләшмиш Милләтләрин халгларынын БМТ Низамнамәсиндә"
   specimen_36: "Һеч ким көлә вә ја асылы вәзијјәтдә сахланыла билмәз; гулдарлыг вә гул тиҹарәти бүтүн формаларда гадаған едилир."
   specimen_32: "Һәр бир шәхс Конститусијанын вә ја ганунун она вердији һүгугларын позулмасы заманы сәләаһијјәтли милли мәһкәмәләр тәрәфиндән һүгугларынын бәрпа олунмасы һүгугуна маликдир."
   specimen_21: "Һеч ким өзбашына һәбсә, тутулмаја вә ја сүрҝүнә мәруз гала билмәз.\nҺәр бир шәхс онун һүгуг вә вәзифәләринин тәјини вә она гаршы ирәли сүрүлмүш ҹинајәт иттиһамынын әсаслылығынын мүәјјәнләшдирилмәси үчүн онун ишинин мүстәгил вә битәрәф мәһкәмәдә, там бәрабәрлик әсасында, ашкарлыг вә әдаләтин бүтүн тәләбләринин ҝөзләнилмәси шәраитиндә бахылмасы һүгугуна маликдир."
-  specimen_16: "Һеч ким шәхси вә аилә һәјатына мүдахиләјә, евинин тохунулмазлығына, мәктублашмасынын ҝизлилијинә, шәрәф вә нүфузуна өзбашына гәсдә мәруз гала билмәз. Һәр бир шәхсин белә мүдахилә вә гәсдән ганун тәрәфиндән мүдафиә олунмаг һүгугу вар.\nҺәр бир шәхс  дүшүнҹә, виҹдан вә дин азадлығы һүгугуна маликдир; бу һүгуга өз динини вә етигадыны дәјишмәк азадлығы вә өз дининә вә инанҹларына тәһсил, дуа вә дини вә ритуал ајинләр заманы тәкликдә вә ја башгалары илә бирликдә, ашкар вә ја фәрди шәкилдә етигад етмәк азадлығы дахилдир.\nҺәр бир шәхсин истираһәт вә асудә вахт, о ҹүмләдән иш ҝүнүнүн ағлабатан һүдуду вә өдәнилән мүтамади мәзунијјәт һүгугу вар."
+  specimen_16: "Һеч ким шәхси вә аилә һәјатына мүдахиләјә, евинин тохунулмазлығына, мәктублашмасынын ҝизлилијинә, шәрәф вә нүфузуна өзбашына гәсдә мәруз гала билмәз. Һәр бир шәхсин белә мүдахилә вә гәсдән ганун тәрәфиндән мүдафиә олунмаг һүгугу вар.\nҺәр бир шәхс дүшүнҹә, виҹдан вә дин азадлығы һүгугуна маликдир; бу һүгуга өз динини вә етигадыны дәјишмәк азадлығы вә өз дининә вә инанҹларына тәһсил, дуа вә дини вә ритуал ајинләр заманы тәкликдә вә ја башгалары илә бирликдә, ашкар вә ја фәрди шәкилдә етигад етмәк азадлығы дахилдир.\nҺәр бир шәхсин истираһәт вә асудә вахт, о ҹүмләдән иш ҝүнүнүн ағлабатан һүдуду вә өдәнилән мүтамади мәзунијјәт һүгугу вар."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/az_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/az_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 region: "AM"
 region: "AZ"
 region: "TR"
 exemplar_chars {
   base: "a b c ç d e ə f g ğ h x ı i İ j k q l m n o ö p r s ş t u ü v y z"
   auxiliary: "w"
   marks: "◌̆ ◌̇ ◌̈ ◌̧"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C Ç D E Ə F G Ğ H X I İ J K Q L M N O Ö P R S Ş T U Ü V Y Z W"
 }
 sample_text {
   masthead_full: "BbÜü"
   masthead_partial: "Tt"
   styles: "Bəşər ailəsinin bütün üzvlərinə xas olan"
   tester: "insan hüquqlarına etinasızlıq və nifrətin bəşəriyyəti dəhşətə"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/azb_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/azb_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/azj_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/azj_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ba_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ba_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ba_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ba_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ban_Bali.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ban_Bali.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ban_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ban_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bap_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bap_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bas_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bas_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 autonym: "Basaa"
 population: 332940
 region: "CM"
 exemplar_chars {
   base: "a A á Á à À â Â ǎ Ǎ ā Ā {a᷆} {a᷇} {A᷆} {A᷇} b B ɓ Ɓ c C d D e E é É è È ê Ê ě Ě ē Ē {e᷆} {e᷇} {E᷆} {E᷇} ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̀} {Ɛ̀} {ɛ̂} {Ɛ̂} {ɛ̌} {Ɛ̌} {ɛ̄} {Ɛ̄} {ɛ᷆} {ɛ᷇} {Ɛ᷆} {Ɛ᷇} f F g G h H i I í Í ì Ì î Î ǐ Ǐ ī Ī {i᷆} {i᷇} {I᷆} {I᷇} j J k K l L m M n N ń Ń ǹ Ǹ ŋ Ŋ o O ó Ó ò Ò ô Ô ǒ Ǒ ō Ō {o᷆} {o᷇} {O᷆} {O᷇} ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̀} {Ɔ̀} {ɔ̂} {Ɔ̂} {ɔ̌} {Ɔ̌} {ɔ̄} {Ɔ̄} {ɔ᷆} {ɔ᷇} {Ɔ᷆} {Ɔ᷇} p P r R s S t T u U ú Ú ù Ù û Û ǔ Ǔ ū Ū {u᷆} {u᷇} {U᷆} {U᷇} v V w W y Y z Z"
   auxiliary: "q Q x X"
   marks: "◌̀ ◌́ ◌̂ ◌̄ ◌̌ ◌᷆ ◌᷇"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B Ɓ C D E Ɛ F G H I J K L M N Ŋ O Ɔ P R S T U V W Y Z"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bax_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bax_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bba_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bba_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bci_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bci_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/be_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/be_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 region: "BY"
 region: "PL"
 region: "UA"
 exemplar_chars {
   base: "а б в г д {дж} {дз} е ё ж з і й к л м н о п р с т у ў ф х ц ч ш ы ь э ю я"
   auxiliary: "{а́} {е́} {ё́} {і́} {о́} {у́} {ы́} {э́} {ю́} {я́}"
   marks: "◌̆ ◌̈"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ , ; : ! ? . « » ( ) [ ] { }"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- , ; : ! ? . « » ( ) [ ] { }"
   index: "А Б В Г Д Е Ё Ж З І Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Ы Ь Э Ю Я"
 }
 sample_text {
   masthead_full: "УуСс"
   masthead_partial: "Ее"
   styles: "Прымаючы пад увагу, што прызнанне годнасці,"
   tester: "прымаючы пад увагу, што грэбаванне і пагарда да правоў чалавека"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/be_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/be_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bem_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bem_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bew_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bew_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bfa_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bfa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bg_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bg_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 region: "RO"
 region: "TR"
 region: "UA"
 exemplar_chars {
   base: "а б в г д е ж з и й к л м н о п р с т у ф х ц ч ш щ ъ ь ю я"
   auxiliary: "{а̀} ѐ ё ѝ {о̀} {у̀} {ъ̀} ы ѣ э {ю̀} {я̀} ѫ"
   marks: "◌̀ ◌̆"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ ( ) [ ] § @ * / ″ №"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ ( ) [ ] @ * /№"
   index: "А Б В Г Д Е Ж З И Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ю Я"
 }
 sample_text {
   masthead_full: "ВвСс"
   masthead_partial: "Ии"
   styles: "Като взе предвид, че признаването на достойнството,"
   tester: "Като взе предвид, че пренебрегването и неуважаването на правата"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bho_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bho_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bik_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bik_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bin_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bin_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bjj_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bjj_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/blt_Tavt.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/blt_Tavt.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 autonym: "傣担语"
 population: 0
 region: "VN"
 sample_text {
   masthead_full: "ꪹꪕꪉꪀ"
   masthead_partial: "ꪱꪋ"
   styles: "ꪫꪸꪀ ꪶꪀꪉ ꪐꪽ ꪻꪬ ꪩꪾꪣ ꫛ ꪶꪔꪙ ꪠꪴ ꪝꪳꪉ ꪁꪫꪸꪙ ꪹꪋꪷꪉ ꪝꪸꪉ ꪹꪚꪱ"
-  tester: "ꪫꪸꪀ ꪹꪤꪸꪒ ꪩꪳꪚ ꪩꪱꪙ ꪀꪾꪚ ꪒꪴ ꪉꪱꪥ  ꪩꪾꪣ ꫛ ꪶꪔꪙ ꪠꪴ ꪭꪳ ꪝꪱ ꪼꪝ ꪭꪮꪒ ꪝꪳꪉ ꪄꪴ ꪹꪤꪸꪒ ꪶꪏꪥ ꪚꪱꪚ"
+  tester: "ꪫꪸꪀ ꪹꪤꪸꪒ ꪩꪳꪚ ꪩꪱꪙ ꪀꪾꪚ ꪒꪴ ꪉꪱꪥ ꪩꪾꪣ ꫛ ꪶꪔꪙ ꪠꪴ ꪭꪳ ꪝꪱ ꪼꪝ ꪭꪮꪒ ꪝꪳꪉ ꪄꪴ ꪹꪤꪸꪒ ꪶꪏꪥ ꪚꪱꪚ"
   poster_sm: "ꪩꪾꪣ ꫛ ꪶꪔꪙ ꪠꪴ"
   poster_md: "ꪹꪜꪸꪙ ꪹꪊꪉ ꪹꪋ"
   poster_lg: "ꪹꪕꪸꪉ"
-  specimen_48: "ꪝꪳꪉ ꪹꪘꪀ ꪹꪊꪱ ꪹꪭꪙ ꪼꪒ ꪐꪽ ꪝꪱꪫ, ꪝꪮꪣ ꪀꪾꪚ ꪩꪺꪉ ꪜꪴꪙ ꪵꪔꪉ  ꪨꪸꪙ ꪹꪭꪷꪚ ꪀꪺꪀ, ꪹꪬꪙ ꪭꪳꪒ"
-  specimen_36: "ꪹꪚꪱ ꪣꪲ ꪻꪠ ꪜꪰꪒ ꪄꪮꪥ ꪹꪏꪷ ꪭꪳ ꪫꪱ ꪊꪺꪚ ꪶꪄꪣ ꪙꪱꪚ ꪹꪏꪉ ꫛ ꪄꪮꪥ  ꪹꪏꪷ, ꪋꪴ ꪮꪽ ꪹꪏꪉ ꪹꪜꪸꪙ ꪄꪮꪥ ꪹꪏꪷ ꪀꪾꪚ ꪁꪱ ꪄꪱꪥ ꪄꪮꪥ ꪹꪏꪷ ꪒꪷ ꪹꪜꪸꪙ ꪄꪴ ꪹꪀꪷꪣ ꪀꪰꪒ ꪹꪁꪸꪉ."
-  specimen_32: "ꪹꪕꪸꪉ ꪀꪱ ꪋꪴ ꫛ ꪻꪠ ꪁꪷ ꪼꪒ ꪹꪋꪷꪉ ꪝꪸꪉ  ꪕꪮꪥ ꪠꪱꪚ ꪨꪺꪒ ꪼꪜ ꪵꪊ ꪹꪏꪉ ꪒꪸꪫ ꪹꪚꪱ ꪣꪲ ꪄꪴ ꪻꪒ ꪜꪽ ꪵꪊꪀ ꪹꪕꪸꪉ ꪀꪱ ꪋꪴ ꫛ ꪝꪮꪣ ꪼꪒ ꪼꪜ ꪵꪊ ꪹꪏꪉ ꪒꪸꪫ ꪼꪒ ꪁꪾꪣ ꪔꪷ ꪝꪳꪉ ꪄꪴ ꪜꪽ ꪵꪊꪀ ꪄꪮꪉ ꪁꪫꪱꪣ ꪜꪱꪫ ꪙꪲ ꪵꪀꪉ ꪼꪒ ꪁꪾꪣ ꪔꪷ  ꪝꪳꪉ  ꪄꪴ ꪑꪮꪀ ꪑꪺꪙ ꪵꪚꪉ ꪵꪑꪀ ꪎꪸ ꪀꪽ ꪽ."
-  specimen_21: "ꪋꪴ ꫛ ꪻꪠ ꪁꪷ ꪣꪲ ꪁꪫꪸꪙ ꪼꪒ ꪕꪫꪱ ꪮꪱꪙ ꪹꪣꪉ ꪽ ꪼꪜ  ꪵꪊ ꪕꪮꪥ ꪠꪱꪚ ꪩꪺꪒ ꪁꪾꪣ ꪔꪷ ꪝꪳꪉ ꪄꪴ  ꪹꪥꪸꪒ ꪠꪲꪒ ꪕꪮꪥ ꪭꪲꪒ ꪻꪐ ꪒꪺꪉ ꪄꪮꪉ ꪠꪱꪚ ꪩꪺꪒ ꪕꪰꪒ ꪮꪮꪀ.\nꪹꪚꪱ ꪣꪲ ꪻꪠ ꪊꪺꪚ ꪜꪰꪒ,  ꪎꪰꪉ ꪼꪫ ꪭꪳ ꪫꪱ ꪬꪱꪀ ꪩꪰꪀ ꪶꪎꪉ  ꪼꪜ ꪹꪣꪉ ꪮꪳꪙ\nꪋꪴ ꫛ ꪻꪠ ꪁꪷ ꪻꪬ ꪼꪒ ꪣꪲ ꪁꪫꪸꪙ  ꪹꪋꪷꪉ ꪝꪸꪉ, ꪼꪒ ꪕꪫꪱ ꪮꪱꪙ ꪹꪣꪉ ꪽ ꪵꪔꪉ ꪹꪩꪷꪉ ꪹꪎꪷꪉ ꪋꪮꪚ ꪵꪊꪉ ꪵꪊꪀ ꪹꪚꪱ ꪚꪰꪀ ꪶꪕꪥ ꪎꪴ ꫛ ꪻꪒ ꪁꪫꪸꪙ ꪚꪰꪀ ꪩꪱ ꪫꪱ ꪮꪫꪱꪙ.\nꪹꪚꪱ ꪣꪲ ꪻꪠ ꪊꪺꪚ ꫛ ꪮꪳꪙ ꪮꪱꪉ ꪕꪷ ꪹꪊꪱ ꪵꪙꪉ ꪹꪤꪸꪒ ꪻꪬ ꪋꪺ  ꪹꪩꪷꪥ ꪚꪮꪣ, ꪋꪺ ꪹꪭꪙ,  ꪚꪮꪙ ꪤꪴ ꪵꪀꪉ ꪎꪳ ꪎꪱꪙ ꪄꪮꪉ ꪚꪮꪣ ꫛ ꪽ ꪹꪚꪱ ꪵꪝꪒ ꪝꪱꪙ ꪭꪮꪒ ꪋꪳ ꪎꪸꪉ ꪘꪱ ꪔꪱ ꪄꪮꪉ ꪹꪊꪱ. ꪋꪴ ꫛ ꪝꪮꪣ ꪼꪒ ꪠꪱꪚ ꪩꪺꪒ ꪼꪜ ꪵꪊ ꪹꪮꪱ ꪁꪾꪣ  ꪔꪷ ꪝꪳꪉ  ꪄꪴ  ꪵꪮ  ꪹꪥꪸꪒ ꪒꪴ ꪉꪱꪥ ꪵꪝ  ꪹꪊꪱ ꪹꪏꪉ ꪽ."
-  specimen_16: "ꪋꪴ ꫛ ꪝꪮꪣ ꪼꪒ ꪣꪲ ꪁꪫꪸꪙ ꪈꪾ ꪜꪴꪙ ꪮꪮꪀ ꪒꪰꪀ ꪵꪒꪣ ꪀꪾꪚ ꪎꪱꪉ ꪭꪲꪒ ꪅꪮꪉ, ꪹꪕꪸꪉ ꪀꪱ ꪕꪳ ꪕꪱꪉ ꪜꪸꪙ ꪹꪋ ꪎꪱꪥ ꪵꪀꪉ ꪭꪲꪒ ꪅꪮꪉ, ꪀꪾꪚ ꪼꪒ ꪕꪳ ꪕꪱꪉ ꪮꪮꪀ ꪘꪱ ꫛ ꪹꪋ ꪎꪱꪥ ꪣꪲ ꪭꪳ ꪎꪱꪉ ꪭꪲꪒ ꪅꪮꪉ ꪵꪔ ꪜꪱꪉ ꪒꪱꪥ ꪋꪸꪙ ꪣꪱ ꪹꪤꪸꪒ ꪹꪎꪸꪙ ꪡꪮꪙ, ꪀꪴꪉ ꪹꪏꪷ,ꪹꪜꪸꪙ ꪄꪮꪉ ꪚꪮꪣ ꪹꪊꪱ ꪭꪳ ꪫꪱ ꪄꪮꪉ ꪭꪺꪣ ꪀꪽ ꪹꪜꪸꪙ ꪮꪮꪀ ꪘꪱ ꪭꪳ ꪄꪮꪉ ꪤꪸꪉ ꪚꪮꪣ ꪹꪊꪱ.\nꪋꪴ ꫛ ꪝꪮꪣ ꪣꪲ ꪁꪫꪸꪙ ꪕꪳ ꪕꪱꪉ ꪜꪱꪀ ꪹꪫꪱ ꪎꪳ ꪎꪱꪙ ꪵꪀꪉ ꪵꪀ ꪼꪄ ꪮꪮꪀ  ꪩꪱꪉ ꪈꪾ ꪩꪱꪉ ꪜꪮꪉ ꪕꪳ ꪕꪱꪉ ꪩꪱꪉ ꪈꪾ ꪭꪲꪒ ꪄꪮꪉ ꪹꪊꪱ, ꪹꪚꪱ ꪤꪴ ꪀꪮꪉ ꪄꪴ ꪶꪄꪣ ꪙꪱꪚ ꪻꪒ, ꪕꪳ ꪕꪱꪉ ꪏꪮꪀ ꪎꪱꪫ ꪹꪮꪱ ꪁꪫꪱꪣ ꪭꪴ ꪏꪸꪉ ꪄꪮꪉ ꫛ ꪮꪳꪙ ꪹꪎꪱ ꪜꪱꪫ ꪣꪱ ꪹꪚꪱ ꪁꪫꪱꪣ ꪹꪣꪉ ꪻꪒ.\nꪋꪴ ꫛ ꪹꪜꪸꪙ ꪹꪊꪱ ꪚꪱꪙ ꪹꪣꪉ, ꪝꪮꪣ ꪼꪒ ꪣꪲ ꪁꪫꪸꪙ ꪚꪱꪫ ꪬꪸꪣ ꪎꪱ ꪶꪭꪥ ꪁꪷ ꪹꪏꪉ ꪒꪸꪫ ꪫꪸꪀ ꪹꪥꪸꪒ ꪀꪲꪙ ꪣꪱ ꪕꪱꪉ ꪠꪱꪥ ꪹꪉꪷꪙ ꪘꪰꪉ ꪎꪱ ꪶꪭꪥ ꪀꪾꪚ ꪪꪽ ꪬꪫꪱ ꪹꪚꪱ ꪹꪖꪸ ꪒꪴꪒ ꪖꪸꪫ ꪻꪬ ꪩꪾ ꫛ ꪶꪔꪙ ꪠꪴ ꪄꪮꪉ ꪹꪊꪱ, ꪶꪎ ꪫꪱꪙ ꪀꪫꪱꪉ ꪄꪫꪱꪉ ꪘꪰꪉ ꪒꪮꪣ ꪹꪣꪉ ꪁꪱꪙ ꪠꪱ ꪀꪾꪚ ꪋꪴ ꪹꪣꪉ, ꪋꪮꪚ ꪹꪋꪷꪉ ꪫꪸꪀ ꪔꪰꪉ ꪵꪕꪉ ꪩꪺꪉ ꪜꪴꪙ ꪄꪮꪉ ꪢꪮꪥ ꪹꪣꪉ."
+  specimen_48: "ꪝꪳꪉ ꪹꪘꪀ ꪹꪊꪱ ꪹꪭꪙ ꪼꪒ ꪐꪽ ꪝꪱꪫ, ꪝꪮꪣ ꪀꪾꪚ ꪩꪺꪉ ꪜꪴꪙ ꪵꪔꪉ ꪨꪸꪙ ꪹꪭꪷꪚ ꪀꪺꪀ, ꪹꪬꪙ ꪭꪳꪒ"
+  specimen_36: "ꪹꪚꪱ ꪣꪲ ꪻꪠ ꪜꪰꪒ ꪄꪮꪥ ꪹꪏꪷ ꪭꪳ ꪫꪱ ꪊꪺꪚ ꪶꪄꪣ ꪙꪱꪚ ꪹꪏꪉ ꫛ ꪄꪮꪥ ꪹꪏꪷ, ꪋꪴ ꪮꪽ ꪹꪏꪉ ꪹꪜꪸꪙ ꪄꪮꪥ ꪹꪏꪷ ꪀꪾꪚ ꪁꪱ ꪄꪱꪥ ꪄꪮꪥ ꪹꪏꪷ ꪒꪷ ꪹꪜꪸꪙ ꪄꪴ ꪹꪀꪷꪣ ꪀꪰꪒ ꪹꪁꪸꪉ."
+  specimen_32: "ꪹꪕꪸꪉ ꪀꪱ ꪋꪴ ꫛ ꪻꪠ ꪁꪷ ꪼꪒ ꪹꪋꪷꪉ ꪝꪸꪉ ꪕꪮꪥ ꪠꪱꪚ ꪨꪺꪒ ꪼꪜ ꪵꪊ ꪹꪏꪉ ꪒꪸꪫ ꪹꪚꪱ ꪣꪲ ꪄꪴ ꪻꪒ ꪜꪽ ꪵꪊꪀ ꪹꪕꪸꪉ ꪀꪱ ꪋꪴ ꫛ ꪝꪮꪣ ꪼꪒ ꪼꪜ ꪵꪊ ꪹꪏꪉ ꪒꪸꪫ ꪼꪒ ꪁꪾꪣ ꪔꪷ ꪝꪳꪉ ꪄꪴ ꪜꪽ ꪵꪊꪀ ꪄꪮꪉ ꪁꪫꪱꪣ ꪜꪱꪫ ꪙꪲ ꪵꪀꪉ ꪼꪒ ꪁꪾꪣ ꪔꪷ ꪝꪳꪉ ꪄꪴ ꪑꪮꪀ ꪑꪺꪙ ꪵꪚꪉ ꪵꪑꪀ ꪎꪸ ꪀꪽ ꪽ."
+  specimen_21: "ꪋꪴ ꫛ ꪻꪠ ꪁꪷ ꪣꪲ ꪁꪫꪸꪙ ꪼꪒ ꪕꪫꪱ ꪮꪱꪙ ꪹꪣꪉ ꪽ ꪼꪜ ꪵꪊ ꪕꪮꪥ ꪠꪱꪚ ꪩꪺꪒ ꪁꪾꪣ ꪔꪷ ꪝꪳꪉ ꪄꪴ ꪹꪥꪸꪒ ꪠꪲꪒ ꪕꪮꪥ ꪭꪲꪒ ꪻꪐ ꪒꪺꪉ ꪄꪮꪉ ꪠꪱꪚ ꪩꪺꪒ ꪕꪰꪒ ꪮꪮꪀ.\nꪹꪚꪱ ꪣꪲ ꪻꪠ ꪊꪺꪚ ꪜꪰꪒ, ꪎꪰꪉ ꪼꪫ ꪭꪳ ꪫꪱ ꪬꪱꪀ ꪩꪰꪀ ꪶꪎꪉ ꪼꪜ ꪹꪣꪉ ꪮꪳꪙ\nꪋꪴ ꫛ ꪻꪠ ꪁꪷ ꪻꪬ ꪼꪒ ꪣꪲ ꪁꪫꪸꪙ ꪹꪋꪷꪉ ꪝꪸꪉ, ꪼꪒ ꪕꪫꪱ ꪮꪱꪙ ꪹꪣꪉ ꪽ ꪵꪔꪉ ꪹꪩꪷꪉ ꪹꪎꪷꪉ ꪋꪮꪚ ꪵꪊꪉ ꪵꪊꪀ ꪹꪚꪱ ꪚꪰꪀ ꪶꪕꪥ ꪎꪴ ꫛ ꪻꪒ ꪁꪫꪸꪙ ꪚꪰꪀ ꪩꪱ ꪫꪱ ꪮꪫꪱꪙ.\nꪹꪚꪱ ꪣꪲ ꪻꪠ ꪊꪺꪚ ꫛ ꪮꪳꪙ ꪮꪱꪉ ꪕꪷ ꪹꪊꪱ ꪵꪙꪉ ꪹꪤꪸꪒ ꪻꪬ ꪋꪺ ꪹꪩꪷꪥ ꪚꪮꪣ, ꪋꪺ ꪹꪭꪙ, ꪚꪮꪙ ꪤꪴ ꪵꪀꪉ ꪎꪳ ꪎꪱꪙ ꪄꪮꪉ ꪚꪮꪣ ꫛ ꪽ ꪹꪚꪱ ꪵꪝꪒ ꪝꪱꪙ ꪭꪮꪒ ꪋꪳ ꪎꪸꪉ ꪘꪱ ꪔꪱ ꪄꪮꪉ ꪹꪊꪱ. ꪋꪴ ꫛ ꪝꪮꪣ ꪼꪒ ꪠꪱꪚ ꪩꪺꪒ ꪼꪜ ꪵꪊ ꪹꪮꪱ ꪁꪾꪣ ꪔꪷ ꪝꪳꪉ ꪄꪴ ꪵꪮ ꪹꪥꪸꪒ ꪒꪴ ꪉꪱꪥ ꪵꪝ ꪹꪊꪱ ꪹꪏꪉ ꪽ."
+  specimen_16: "ꪋꪴ ꫛ ꪝꪮꪣ ꪼꪒ ꪣꪲ ꪁꪫꪸꪙ ꪈꪾ ꪜꪴꪙ ꪮꪮꪀ ꪒꪰꪀ ꪵꪒꪣ ꪀꪾꪚ ꪎꪱꪉ ꪭꪲꪒ ꪅꪮꪉ, ꪹꪕꪸꪉ ꪀꪱ ꪕꪳ ꪕꪱꪉ ꪜꪸꪙ ꪹꪋ ꪎꪱꪥ ꪵꪀꪉ ꪭꪲꪒ ꪅꪮꪉ, ꪀꪾꪚ ꪼꪒ ꪕꪳ ꪕꪱꪉ ꪮꪮꪀ ꪘꪱ ꫛ ꪹꪋ ꪎꪱꪥ ꪣꪲ ꪭꪳ ꪎꪱꪉ ꪭꪲꪒ ꪅꪮꪉ ꪵꪔ ꪜꪱꪉ ꪒꪱꪥ ꪋꪸꪙ ꪣꪱ ꪹꪤꪸꪒ ꪹꪎꪸꪙ ꪡꪮꪙ, ꪀꪴꪉ ꪹꪏꪷ,ꪹꪜꪸꪙ ꪄꪮꪉ ꪚꪮꪣ ꪹꪊꪱ ꪭꪳ ꪫꪱ ꪄꪮꪉ ꪭꪺꪣ ꪀꪽ ꪹꪜꪸꪙ ꪮꪮꪀ ꪘꪱ ꪭꪳ ꪄꪮꪉ ꪤꪸꪉ ꪚꪮꪣ ꪹꪊꪱ.\nꪋꪴ ꫛ ꪝꪮꪣ ꪣꪲ ꪁꪫꪸꪙ ꪕꪳ ꪕꪱꪉ ꪜꪱꪀ ꪹꪫꪱ ꪎꪳ ꪎꪱꪙ ꪵꪀꪉ ꪵꪀ ꪼꪄ ꪮꪮꪀ ꪩꪱꪉ ꪈꪾ ꪩꪱꪉ ꪜꪮꪉ ꪕꪳ ꪕꪱꪉ ꪩꪱꪉ ꪈꪾ ꪭꪲꪒ ꪄꪮꪉ ꪹꪊꪱ, ꪹꪚꪱ ꪤꪴ ꪀꪮꪉ ꪄꪴ ꪶꪄꪣ ꪙꪱꪚ ꪻꪒ, ꪕꪳ ꪕꪱꪉ ꪏꪮꪀ ꪎꪱꪫ ꪹꪮꪱ ꪁꪫꪱꪣ ꪭꪴ ꪏꪸꪉ ꪄꪮꪉ ꫛ ꪮꪳꪙ ꪹꪎꪱ ꪜꪱꪫ ꪣꪱ ꪹꪚꪱ ꪁꪫꪱꪣ ꪹꪣꪉ ꪻꪒ.\nꪋꪴ ꫛ ꪹꪜꪸꪙ ꪹꪊꪱ ꪚꪱꪙ ꪹꪣꪉ, ꪝꪮꪣ ꪼꪒ ꪣꪲ ꪁꪫꪸꪙ ꪚꪱꪫ ꪬꪸꪣ ꪎꪱ ꪶꪭꪥ ꪁꪷ ꪹꪏꪉ ꪒꪸꪫ ꪫꪸꪀ ꪹꪥꪸꪒ ꪀꪲꪙ ꪣꪱ ꪕꪱꪉ ꪠꪱꪥ ꪹꪉꪷꪙ ꪘꪰꪉ ꪎꪱ ꪶꪭꪥ ꪀꪾꪚ ꪪꪽ ꪬꪫꪱ ꪹꪚꪱ ꪹꪖꪸ ꪒꪴꪒ ꪖꪸꪫ ꪻꪬ ꪩꪾ ꫛ ꪶꪔꪙ ꪠꪴ ꪄꪮꪉ ꪹꪊꪱ, ꪶꪎ ꪫꪱꪙ ꪀꪫꪱꪉ ꪄꪫꪱꪉ ꪘꪰꪉ ꪒꪮꪣ ꪹꪣꪉ ꪁꪱꪙ ꪠꪱ ꪀꪾꪚ ꪋꪴ ꪹꪣꪉ, ꪋꪮꪚ ꪹꪋꪷꪉ ꪫꪸꪀ ꪔꪰꪉ ꪵꪕꪉ ꪩꪺꪉ ꪜꪴꪙ ꪄꪮꪉ ꪢꪮꪥ ꪹꪣꪉ."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bn_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bn_Beng.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "GB"
 region: "IN"
 region: "NP"
 exemplar_chars {
   base: "় ৺ অ আ ই ঈ উ ঊ ঋ ৠ ঌ ৡ এ ঐ ও ঔ ং ঃ ঁ ক {ক্ষ} খ গ ঘ ঙ চ ছ জ ঝ ঞ ট ঠ ড {ড়} ঢ {ঢ়} ণ ত ৎ থ দ ধ ন প ফ ব ভ ম য {য়} র ল শ ষ স হ ঽ া ি ী ু ূ ৃ ৄ ৢ ৣ ে ৈ ো ৌ ্ ৗ"
   auxiliary: "‌‍ ৲ ৳ ৴ ৵ ৶ ৷ ৸ ৹ ৰ ৱ"
   marks: "◌ঁ ◌ং ◌ঃ ◌় ◌া ◌ি ◌ী ◌ু ◌ূ ◌ৃ ◌ৄ ◌ে ◌ৈ ◌্ ◌ৗ ◌ৢ ◌ৣ"
-  numerals: "- ‑ , . % ‰ + 0০ 1১ 2২ 3৩ 4৪ 5৫ 6৬ 7৭ 8৮ 9৯"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0০ 1১ 2২ 3৩ 4৪ 5৫ 6৬ 7৭ 8৮ 9৯"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "অ আ ই ঈ উ ঊ ঋ এ ঐ ও ঔ ক {ক্ষ} খ গ ঘ ঙ চ ছ জ ঝ ঞ ট ঠ ড ঢ ণ ত থ দ ধ ন প ফ ব ভ ম য র ল শ ষ স হ"
 }
 sample_text {
   masthead_full: "সমতন"
   masthead_partial: "ষব"
   styles: "যেহেতু মানব পরিবারের সকল সদস্যের সমান ও অবিচ্ছেদ্য অধিকারসমূহ"
   tester: "যেহেতু মানব অধিকারের প্রতি অবজ্ঞা এবং ঘৃণার ফলে মানুবের বিবেক লাঞ্ছিত বোধ করে এমন সব বর্বরোচিত"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bo_Tibt.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bo_Tibt.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 region: "CN"
 region: "IN"
 region: "NP"
 exemplar_chars {
   base: "ཾ ཿ ཀ {ཀྵ} ྐ {ྐྵ} ཁ ྑ ག {གྷ} ྒ {ྒྷ} ང ྔ ཅ ྕ ཆ ྖ ཇ ྗ ཉ ྙ ཊ ྚ ཋ ྛ ཌ {ཌྷ} ྜ {ྜྷ} ཎ ྞ ཏ ྟ ཐ ྠ ད {དྷ} ྡ {ྡྷ} ན ྣ པ ྤ ཕ ྥ བ {བྷ} ྦ {ྦྷ} མ ྨ ཙ ྩ ཚ ྪ ཛ {ཛྷ} ྫ {ྫྷ} ཝ ྭ ྺ ཞ ྮ ཟ ྯ འ ྰ ཡ ྱ ྻ ར ཪ ྲ ྼ ལ ླ ཤ ྴ ཥ ྵ ས ྶ ཧ ྷ ཨ ྸ ི {ཱི} ྀ {ཱྀ} ུ {ཱུ} {ྲྀ} ཷ {ླྀ} ཹ ེ ཻ ོ ཽ ྄"
   auxiliary: "ༀ"
   marks: "◌ི ◌ུ ◌ེ ◌ོ"
-  numerals: "- ‑ , . % ‰ + 0༠ 1༡ 2༢ 3༣ 4༤ 5༥ 6༦ 7༧ 8༨ 9༩"
+  numerals: "- , . % + 0༠ 1༡ 2༢ 3༣ 4༤ 5༥ 6༦ 7༧ 8༨ 9༩"
   punctuation: ": ་ །"
   index: "ཀ ཁ ག ང ཅ ཆ ཇ ཉ ཏ ཐ ད ན པ ཕ བ མ ཙ ཚ ཛ ཝ ཞ ཟ འ ཡ ར ལ ཤ ས ཧ ཨ"
 }
 sample_text {
   masthead_full: "འགབམ"
   masthead_partial: "རས"
   styles: "༈ འགྲོ་བ་མིའི་ཁྱིམ་ཚང་ཁག་གི་ནང་མི་ཡོངས་ལ་རང་བཞིན་ཉིད་ནས་ཡོད་པའི་ཆེ་མཐོངས་དང་འདྲ་མཉམ།"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/boa_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/boa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bpy_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bpy_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/br_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/br_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Brezhoneg"
 population: 563140
 region: "FR"
 exemplar_chars {
   base: "a b {cʼh} {ch} d e ê f g h i j k l m n ñ o p r s t u ù v w x y z"
   auxiliary: "á à ă â å ä ã ā æ c ç é è ĕ ë ē í ì ĭ î ï ī ó ò ŏ ô ö ø ō œ q ú ŭ û ü ū ÿ"
   marks: "◌̀ ◌̂ ◌̃"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ , ; : ! ? . ( ) [ ] { }"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- , ; : ! ? . ( ) [ ] { }"
   index: "A B C D E F G H I J K L M N O P R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "DdIi"
   masthead_partial: "Ee"
   styles: "–O vezañ ma’z eo war anaout an dellezegezh"
   tester: "–o vezañ ma’z eo war dizanaout ha dismegañsiñ gwirioù mab-den eo"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/brh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/brh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/brx_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/brx_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/brx_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/brx_Deva.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "बरʼ"
 population: 1856526
 region: "IN"
 exemplar_chars {
   base: "़ ँ ं अ आ इ ई उ ऊ ऍ ए ऐ ऑ ओ औ क ख ग घ च छ ज झ ञ ट ठ ड {ड़} ढ ण त थ द ध न प फ ब भ म य र ल ळ व श ष स ह ा ि ी ु ू ृ ॅ े ै ॉ ो ौ ्"
   auxiliary: "‌‍"
   marks: "◌ँ ◌ं ◌ः ◌़ ◌ा ◌ि ◌ी ◌ु ◌ू ◌ृ ◌े ◌ै ◌ो ◌ौ ◌्"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   punctuation: "। ॥ ॰"
   index: "अ आ इ ई उ ऊ ऍ ए ऐ ऑ ओ औ क ख ग घ च छ ज झ ञ ट ठ ड {ड़} ढ ण त थ द ध न प फ ब भ म य र ल ळ व श ष स ह"
 }
 sample_text {
   masthead_full: "गसबआ"
   masthead_partial: "नउ"
   styles: "गासै सुबुं आनो उदांयै मान सनमान आरो मोनथाय लाना जोनोम लायो। बिसोरो"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/brx_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/brx_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bs_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bs_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Bosnian (Cyrillic)"
 autonym: "Босански"
 population: 3797234
 region: "BA"
 exemplar_chars {
   base: "а б в г д ђ е ж з и ј к л љ м н њ о п р с т ћ у ф х ц ч џ ш"
   auxiliary: ""
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "А Б В Г Д Ђ Е Ж З И Ј К Л Љ М Н Њ О П Р С Т Ћ У Ф Х Ц Ч Џ Ш"
 }
 sample_text {
   masthead_full: "СсВв"
   masthead_partial: "Аа"
   styles: "БУДУЂИ да су признавање урођеног достојанства"
   tester: "БУДУЂИ да су непоштивање и презирање права човјека имали за посљедицу"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bs_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hr_Latn.textproto`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-id: "bs_Latn"
-language: "bs"
+id: "hr_Latn"
+language: "hr"
 script: "Latn"
-name: "Bosnian"
-autonym: "Bosanski"
-population: 3797234
+name: "Croatian"
+autonym: "Hrvatski"
+population: 6767930
+region: "AT"
 region: "BA"
+region: "DE"
+region: "HR"
+region: "HU"
+region: "IT"
+region: "RS"
+region: "SI"
 exemplar_chars {
   base: "a b c č ć d {dž} đ e f g h i j k l {lj} m n {nj} o p r s š t u v z ž"
   auxiliary: "q w x y"
   marks: "◌́ ◌̌"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "‐ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / ′ ″"
-  index: "A B C Č Ć D {DŽ} E F G H I J K L {LJ} M N {NJ} O P Q R S Š T U V W X Y Z Ž"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "– — , ; : ! ? . … \' ‘ ’ ‚ \" “ ” „ ( ) [ ] @ * /"
+  index: "A B C Č Ć D {DŽ} Đ E F G H I J K L {LJ} M N {NJ} O P Q R S Š T U V W X Y Z Ž"
 }
 sample_text {
   masthead_full: "SsVv"
   masthead_partial: "Aa"
-  styles: "BUDUĆI da su priznavanje urođenog dostojanstva"
-  tester: "BUDUĆI da su nepoštivanje i preziranje prava čovjeka imali za"
-  poster_sm: "BUDUĆI da je"
-  poster_md: "BUDUĆI"
+  styles: "Budući da su priznavanje urođenog dostojanstva"
+  tester: "Budući da su nepoštovanje i preziranje prava čovjeka imali za"
+  poster_sm: "Budući da je"
+  poster_md: "Budući da"
   poster_lg: "Sva"
-  specimen_48: "BUDUĆI da su narodi Ujedinjenih nacija ponovo potvrdili"
-  specimen_36: "BUDUĆI da je zajedničko razumijevanje tih prava i sloboda od najveće važnosti za puno ostvarenje te obaveze,"
+  specimen_48: "Budući da su narodi Ujedinjenih naroda ponovno potvrdili u Povelji"
+  specimen_36: "Budući da je zajedničko razumijevanje tih prava i sloboda od najveće važnosti za puno ostvarenje te obveze,"
   specimen_32: "Sva ljudska bića rađaju se slobodna i jednaka u dostojanstvu i pravima. Ona su obdarena razumom i sviješću i treba da jedno prema drugome postupaju u duhu bratstva."
-  specimen_21: "Svakome su dostupna sva prava i slobode navedene u ovoj Deklaraciji bez razlike bilo koje vrste, kao sto su rasa, boja, spol, jezik, vjera, političko ili drugo mišljenje, narodonosno ili društveno porijeklo, imovina, rođenje ili drugi pravni položaj.\nSvako ima pravo na život, slobodu i osobnu sigurnost.\nNiko ne smije biti držan u ropstvu ili ropskom odnosu; ropstvo i trgovina robljem zabranjuje se u svim njihovim oblicima."
-  specimen_16: "Niko ne smije biti podvrgnut mučenju ili okrutnom, nečovječnom ili ponižavajućem postupku ili kažnjavanju.\nSvako ima pravo da se svagdje pred zakonom priznaje kao osoba.\nSvi su pred zakonom jednaki i imaju pravo, bez ikakve diskriminacije, na jednaku zaštitu zakona. Svi imaju pravo na jednaku zaštitu protiv bilo kakve diskriminacije kojom se krši ova Deklaracija i protiv svakog podsticanja na takvu diskriminaciju.\nSvako ima pravo na djelotvorna pravna sredstva putem nadležnih nacionalnih sudova zbog djela kojima se krše osnovna prava koja su mu dodijeljena u Ustavu ili zakonu."
+  specimen_21: "Svakome su dostupna sva prava i slobode navedene u ovoj Deklaraciji bez razlike bilo koje vrste, kao što su rasa, boja, spol, jezik, vjera, političko ili drugo mišljenje, nacionalno ili društveno porijeklo, imovina, rođenje ili drugi pravni položaj.\nSvatko ima pravo na život, slobodu i osobnu sigurnost.\nNitko ne smije biti držan u ropstvu ili ropskom odnosu; ropstvo i trgovina robljem zabranjuju se u svim svojim oblicima."
+  specimen_16: "Nitko ne smije biti podvrgnut mučenju ili okrutnom, nečovječnom ili ponižavajućem postupku ili kažnjavanju.\nSvatko ima pravo da se svagdje pred zakonom priznaje kao osoba.\nSvi su pred zakonom jednaki i imaju pravo, bez ikakve diskriminacije, na jednaku zaštitu zakona. Svi imaju pravo na jednaku zaštitu protiv bilo kakve diskrimininacije kojom se krši ova Deklaracija i protiv svakog poticanja na takvu diskriminaciju.\nSvatko ima pravo na djelotvorna pravna sredstva putem nadležnih nacionalnih sudova zbog djela kojima se krše osnovna prava koja mu pripadaju temeljem ustava i zakona."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bsq_Bass.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bsq_Bass.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bua_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bua_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/buc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/buc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bug_Bugi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bug_Bugi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bug_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bug_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bum_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bum_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bvi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bvi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/bwy_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/bwy_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/byh_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/byh_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ca_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ca_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "ES"
 region: "FR"
 region: "IT"
 exemplar_chars {
   base: "· a à b c ç d e é è f g h i í ï j k l m n o ó ò p q r s t u ú ü v w x y z"
   auxiliary: "á ă â å ä ã ā æ ĕ ê ë ē ì ĭ î ī ŀ ñ º ŏ ô ö ø ō œ ù ŭ û ū ÿ"
   marks: "◌̀ ◌́ ◌̈ ◌̧"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ¡ ? ¿ . … \' ‘ ’ \" “ ” « » ( ) [ ] § @ * / \\ & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ¡ ? ¿ . … \' ‘ ’ \" “ ” « » ( ) [ ] @ * / \\ & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtOo"
   masthead_partial: "Ss"
   styles: "Considerant que el reconeixement de la dignitat"
   tester: "Considerant que el desconeixement i el menyspreu dels drets humans"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cab_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cab_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cak_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cak_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cbi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cbi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cbk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cbk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cbr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cbr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cbs_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cbs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cbt_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cbt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cbu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cbu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ccp_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ccp_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ccp_Cakm.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ccp_Cakm.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
   marks: "◌𑄀 ◌𑄁 ◌𑄂 ◌𑄧 ◌𑄨 ◌𑄩 ◌𑄪 ◌𑄫 ◌𑄬 ◌𑄭 ◌𑄰 ◌𑄱 ◌𑄲 ◌𑄳 ◌𑄴"
   numerals: "𑄶 𑄷 𑄸 𑄹 𑄺 𑄻 𑄼 𑄽 𑄾 𑄿 0 1 2 3 4 5 6 7 8 9"
   punctuation: "𑅁 𑅂 𑅃 𑅀"
 }
 sample_text {
   masthead_full: "𑄝𑄇𑄟𑄚"
   masthead_partial: "𑄌𑄢"
-  styles: " 𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄟𑄚𑄬𑄭 𑄉𑄨𑄢𑄨𑄢𑄴 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄖𑄳𑄠𑄴 𑄥𑄧𑄁 𑄃𑄮 𑄑𑄚𑄑𑄚𑄳𑄠𑄴 𑄝𑄚𑄝𑄚𑄳𑄠𑄴 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄚𑄩"
+  styles: "𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄟𑄚𑄬𑄭 𑄉𑄨𑄢𑄨𑄢𑄴 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄖𑄳𑄠𑄴 𑄥𑄧𑄁 𑄃𑄮 𑄑𑄚𑄑𑄚𑄳𑄠𑄴 𑄝𑄚𑄝𑄚𑄳𑄠𑄴 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄚𑄩"
   tester: "𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄟𑄚𑄬𑄭 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄧𑄢𑄴 𑄛𑄳𑄢𑄧𑄖𑄨 𑄃𑄧𑄣𑄬𑄦𑄧𑄚𑄴 𑄃𑅅 𑄊𑄨𑄚𑄬𑄚𑄢𑄴 𑄜𑄧𑄣𑄬 𑄟𑄚𑄬𑄭𑄦𑄮𑄢𑄴 𑄃𑄬𑄘 𑄣𑄌𑄴𑄈𑄬𑄚𑄬𑄭 𑄃𑄬𑄘𑄮𑄇𑄳𑄠𑄴 𑄉𑄧𑄢𑄨 𑄃𑄬𑄟𑄚𑄴"
   poster_sm: "𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄟𑄚𑄬𑄭 𑄡𑄳𑄠𑄬𑄚𑄴"
   poster_md: "𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄎𑄘𑄧𑄢𑄴"
   poster_lg: "𑄟𑄚𑄪𑄌𑄴"
   specimen_48: "𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄥𑄧𑄘𑄧𑄥𑄳𑄠𑄧 𑄎𑄖𑄴𑄅𑄚𑄴 𑄎𑄖𑄨𑄥𑄧𑄁𑄊𑄧𑄢𑄴 𑄥𑄧𑄚𑄧𑄘𑄬 𑄃𑄢𑄁 𑄟𑄚𑄬𑄭𑄠𑄮𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁, 𑄟𑄚𑄬𑄭 𑄇𑄬𑄠𑄬𑄢𑄴 𑄃𑄨𑄌𑄴𑄎𑄮𑄖𑄴 𑄃𑄮 𑄘𑄟𑄴 𑄃𑅅 𑄟𑄨𑄣𑄬"
   specimen_36: "𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄥𑄧𑄘𑄧𑄥𑄳𑄠𑄧 𑄢𑄬𑄎𑄳𑄠𑄧𑄠𑄚𑄨 𑄎𑄖𑄨𑄥𑄧𑄁𑄊𑄧𑄢𑄴 𑄝𑄧𑄣𑄝𑄧𑄣𑄴𑄘𑄨𑄠𑄬𑄭 𑄟𑄚𑄬𑄭𑄃𑄇𑄴𑄇𑄥𑄁 𑄃𑄮 𑄃𑄢𑄁 𑄥𑄙𑄩𑄚𑄧𑄖𑄃𑄚𑄩𑄢𑄴 𑄛𑄳𑄢𑄧𑄖𑄨 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄖𑄳𑄠𑄴 𑄃𑄨𑄌𑄴𑄎𑄮𑄖𑄴 𑄝𑄢𑄚 𑄃𑅅 𑄃𑄬𑄘𑄢𑄢𑄴 𑄘𑄧𑄟𑄬𑄘𑄣𑄬 𑄈𑄟𑄇𑄭𑄭 𑄛𑄣𑄚𑄢𑄴 𑄖𑄇𑄴𑄉𑄧𑄢𑄨 𑄜𑄬𑄝𑄖𑄳𑄠𑄬 𑄃𑄨𑄟𑄚𑄴𑄎𑄧𑄝𑄚𑄴 𑄃𑄬𑄇𑄴𑄎𑄧𑄙;"
-  specimen_32: "𑄇𑄢𑄧 𑄚𑄨𑄎𑄮𑄢𑄴 𑄉𑄮𑄛𑄧𑄚𑄴 𑄇𑄨𑄁𑄝 𑄖𑄢𑄴 𑄊𑄧𑄢𑄧𑄢𑄴, 𑄉𑄨𑄢𑄨 𑄃𑄮 𑄌𑄨𑄙𑄨𑄛𑄘𑄨𑄢𑄴 𑄃𑄨𑄌𑄳𑄠𑄴𑄟𑄧𑄖𑄧 𑄎𑄨𑄠𑄚𑄴𑄛𑄭 𑄉𑄧𑄢𑄚 𑄇𑄨𑄁𑄝 𑄖𑄢𑄴 𑄥𑄪𑄚𑄟𑄴 𑄃𑄮  𑄃𑄨𑄌𑄴𑄎𑄮𑄘𑄧 𑄅𑄪𑄢𑄪𑄢𑄬 𑄛𑄨𑄢𑄬 𑄜𑄪𑄘𑄬 𑄛𑄢 𑄉𑄧𑄢 𑄚𑄧 𑄌𑄧𑄣𑄨𑄝𑄧𑅁 𑄃𑄬 𑄝𑄝𑄧𑄖𑄳𑄠𑄴 𑄎𑄨𑄠𑄚𑄴𑄛𑄭 𑄉𑄧𑄢𑄚 𑄝 𑄛𑄨𑄢𑄬𑄛𑄚𑄢𑄴 𑄛𑄨𑄌𑄴𑄥𑄨𑄠𑄚𑄴𑄘𑄨 𑄃𑄃𑄨𑄚𑄮𑄢𑄴 𑄃𑄌𑄴𑄥𑄳𑄢𑄧𑄠𑄴 𑄣𑄞𑄧𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄝𑄬𑄇𑄴𑄅𑄚𑄮𑄢𑄴 𑄢𑄧𑄠𑄬𑅁"
+  specimen_32: "𑄇𑄢𑄧 𑄚𑄨𑄎𑄮𑄢𑄴 𑄉𑄮𑄛𑄧𑄚𑄴 𑄇𑄨𑄁𑄝 𑄖𑄢𑄴 𑄊𑄧𑄢𑄧𑄢𑄴, 𑄉𑄨𑄢𑄨 𑄃𑄮 𑄌𑄨𑄙𑄨𑄛𑄘𑄨𑄢𑄴 𑄃𑄨𑄌𑄳𑄠𑄴𑄟𑄧𑄖𑄧 𑄎𑄨𑄠𑄚𑄴𑄛𑄭 𑄉𑄧𑄢𑄚 𑄇𑄨𑄁𑄝 𑄖𑄢𑄴 𑄥𑄪𑄚𑄟𑄴 𑄃𑄮 𑄃𑄨𑄌𑄴𑄎𑄮𑄘𑄧 𑄅𑄪𑄢𑄪𑄢𑄬 𑄛𑄨𑄢𑄬 𑄜𑄪𑄘𑄬 𑄛𑄢 𑄉𑄧𑄢 𑄚𑄧 𑄌𑄧𑄣𑄨𑄝𑄧𑅁 𑄃𑄬 𑄝𑄝𑄧𑄖𑄳𑄠𑄴 𑄎𑄨𑄠𑄚𑄴𑄛𑄭 𑄉𑄧𑄢𑄚 𑄝 𑄛𑄨𑄢𑄬𑄛𑄚𑄢𑄴 𑄛𑄨𑄌𑄴𑄥𑄨𑄠𑄚𑄴𑄘𑄨 𑄃𑄃𑄨𑄚𑄮𑄢𑄴 𑄃𑄌𑄴𑄥𑄳𑄢𑄧𑄠𑄴 𑄣𑄞𑄧𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄝𑄬𑄇𑄴𑄅𑄚𑄮𑄢𑄴 𑄢𑄧𑄠𑄬𑅁"
   specimen_21: "𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄢𑄴 𑄙𑄧𑄢𑄴𑄟𑄧, 𑄃𑄬𑄘 𑄃𑄮 𑄌𑄨𑄘𑄳𑄠𑄬 𑄥𑄙𑄩𑄚𑄧𑄖𑄠𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄢𑄧𑄠𑄬𑅁 𑄃𑄬 𑄃𑄇𑄴𑄇𑄥𑄁 𑄥𑄧𑄟𑄢𑄬 𑄙𑄧𑄢𑄴𑄟𑄧 𑄝 𑄝𑄨𑄌𑄴𑄥𑄬𑄌𑄴 𑄝𑄧𑄘𑄧𑄣𑄚𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄃𑅅 𑄃𑄬𑄭 𑄥𑄧𑄟𑄢𑄬, 𑄘𑄬𑄉𑄬𑄛𑄢 𑄝 𑄟𑄪𑄢𑄬 𑄟𑄪𑄢𑄬, 𑄉𑄭 𑄝 𑄃𑄧𑄚𑄳𑄠𑄧𑄢𑄴 𑄥𑄧𑄟𑄢𑄬 𑄟𑄨𑄣𑄨𑄚𑄬𑄭, 𑄥𑄨𑄇𑄴𑄈𑄬𑄘𑄚𑄴, 𑄣𑄢𑄴𑄌𑄢𑄴, 𑄙𑄨𑄠𑄚𑄴 𑄉𑄧𑄢𑄚 𑄝 𑄛𑄣𑄬𑄝𑄢𑄴 𑄟𑄖𑄴𑄙𑄧𑄟𑄬 𑄙𑄧𑄢𑄴𑄟𑄧 𑄝 𑄝𑄨𑄌𑄴𑄥𑄬𑄌𑄴 𑄉𑄧𑄢𑄨𑄝𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄮 𑄃𑄨𑄠𑄮𑄖𑄴 𑄗𑄬𑄝𑄧𑅁\n𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄢𑄴 𑄟𑄧𑄖𑄴 𑄘𑄨𑄝𑄢𑄴 𑄃𑅅 𑄟𑄧𑄖𑄴 𑄜𑄧𑄉𑄧𑄘𑄁𑄋𑄨𑄢𑄴 𑄥𑄙𑄩𑄚𑄧𑄖𑄠𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄢𑄧𑄠𑄬𑅁 𑄃𑄧𑄉𑄪𑄢𑄴 𑄟𑄧𑄖𑄴 𑄘𑄨𑄘𑄢𑄴 𑄃𑅅 𑄢𑄬𑄎𑄳𑄠𑄧𑄢𑄴 𑄥𑄨𑄟𑄨𑄚𑄬 𑄌𑄯𑄦𑄨𑄖𑄨𑄨 𑄡𑄬 𑄇𑄧𑄚𑄧 𑄟𑄖𑄴𑄙𑄧𑄟𑄬 𑄈𑄧𑄝𑄧𑄢𑄴 𑄛𑄚 𑄘𑄮𑄇𑄳𑄠𑄴 𑄃𑅅 𑄖𑄧𑄖𑄮 𑄉𑄬𑄛𑄧𑄚𑄴, 𑄣𑄧𑄚 𑄃𑄮 𑄃𑄪𑄙𑄮𑄣𑄧𑄚 𑄥𑄙𑄩𑄚𑄧𑄖𑄃𑄮 𑄃𑄬 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄧𑄢𑄴 𑄟𑄧𑄖𑄴𑄙𑄳𑄠 𑄛𑄧𑄢𑄬𑅁\n𑄥𑄧𑄟𑄎𑄧𑄢𑄴 𑄥𑄧𑄘𑄧𑄥𑄳𑄠𑄧 𑄃𑄨𑄏𑄬𑄝𑄬 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄢𑄴 𑄥𑄟𑄎𑄨𑄇𑄴 𑄚𑄨𑄢𑄛𑄧𑄖𑄳𑄦𑄴𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄃𑄊𑄬𑅁 𑄎𑄖𑄩𑄠𑄧 𑄌𑄬𑄢𑄬𑄖𑄳𑄦𑄴 𑄃𑄮 𑄛𑄨𑄖𑄨𑄨𑄟𑄨𑄢𑄴 𑄝𑄧𑄣𑄴𑄘𑄨𑄠𑄘𑄨𑄢𑄴 𑄟𑄖𑄴𑄙𑄧𑄟𑄬 𑄢𑄮𑄎𑄳𑄠𑄧𑄢𑄴 𑄥𑄧𑄁𑄎𑄧𑄙 𑄃𑄮 𑄥𑄧𑄟𑄴𑄛𑄧𑄘𑄧𑄢𑄴 𑄥𑄧𑄟𑄢𑄬 𑄥𑄧𑄟𑄚𑄴 𑄢𑄉𑄬𑄚𑄬𑄭 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄢𑄬 𑄃𑄟𑄧𑄚𑄧𑄢𑄴 𑄃𑄨𑄌𑄎𑄮𑄖𑄴 𑄃𑅅 𑄟𑄚𑄧𑄢𑄴 𑄃𑄧𑄞𑄬𑄘𑄧𑄢𑄴 𑄜𑄧𑄉𑄧𑄘𑄋𑄧𑄖𑄳𑄠𑄬 𑄈𑄟𑄇𑄭𑄭 𑄥𑄟𑄎𑄨𑄇𑄴, 𑄃𑄧𑄢𑄴𑄗𑄧𑄚𑄨𑄖𑄨𑄇𑄴 𑄃𑄮 𑄥𑄁𑄌𑄴𑄇𑄳𑄢𑄨𑄖𑄨𑄇𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄃𑄘𑄠𑄧𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄢𑄧𑄠𑄬𑅁"
-  specimen_16: "𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄢𑄴 𑄏𑄨𑄢𑄬𑄚 𑄃𑄮 𑄃𑄏𑄬𑄢𑄴 𑄗𑄢𑄚𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄢𑄧𑄠𑄬; 𑄘𑄨𑄚𑄴𑄟𑄉𑄬𑄚𑄬 𑄃𑄧𑄇𑄴𑄖𑄧 𑄟𑄪𑄎𑄨𑄟𑄴 𑄝𑄬𑄖𑄧𑄚𑄴𑄥𑄪𑄟𑄪𑄖𑄴𑄘𑄳𑄠𑄧 𑄍𑄪𑄑𑄨 𑄃𑅅 𑄛𑄬𑄥𑄉𑄧𑄖𑄧 𑄇𑄟𑄧𑄢𑄴 𑄡𑄪𑄇𑄴𑄖𑄨𑄥𑄧𑄁 𑄥𑄩𑄟𑄃𑄮 𑄃𑄬 𑄃𑄇𑄴𑄇𑄥𑄁 𑄞𑄨𑄘𑄨𑄢𑄬 𑄢𑄧𑄠𑄬𑅁\n𑄃𑄬 𑄓𑄇𑄴𑄣𑄢𑄬𑄥𑄧𑄚𑄬 𑄘𑄬𑄉𑄬𑄠𑄬 𑄃𑄇𑄴𑄇𑄥𑄁 𑄃𑄮 𑄥𑄙𑄩𑄚𑄧𑄖𑄊𑄚𑄩𑄢𑄴 𑄇𑄟𑄧𑄖𑄴𑄣𑄉𑄚 𑄥𑄧𑄟𑄴𑄞𑄧𑄛𑄴 𑄃𑄬𑄟𑄧𑄚𑄴 𑄃𑄬𑄇𑄳𑄦𑄴𑄚𑄴 𑄥𑄟𑄎𑄨𑄇𑄴 𑄃𑄮 𑄛𑄨𑄖𑄨𑄨𑄟𑄨 𑄝𑄳𑄠𑄝𑄧𑄌𑄴𑄗𑄭 𑄃𑄧𑄁𑄥𑄩𑄘𑄢𑄨𑄖𑄳𑄠𑄬𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄢𑄴 𑄃𑄊𑄬𑅁  \n𑄇𑄧𑄚𑄧 𑄢𑄬𑄎𑄳𑄠𑄧, 𑄉𑄪𑄖𑄨𑄨 𑄝 𑄟𑄚𑄪𑄌𑄴 𑄃𑄬 𑄓𑄨𑄇𑄴𑄣𑄢𑄬𑄥𑄧𑄚𑄧𑄢𑄴 𑄇𑄧𑄚𑄧 𑄇𑄨𑄌𑄴𑄅 𑄃𑄬𑄟𑄧𑄚𑄴𑄞𑄝𑄬 𑄝𑄳𑄠𑄈𑄳𑄠 𑄉𑄧𑄢𑄨 𑄚𑄧 𑄛𑄢𑄨𑄝𑄇𑄴, 𑄡𑄢𑄴 𑄝𑄧𑄣𑄬 𑄖𑄢 𑄃𑄬𑄭 𑄓𑄨𑄇𑄴𑄣𑄢𑄬𑄥𑄧𑄚𑄬 𑄘𑄬𑄉𑄬𑄠𑄬 𑄃𑄇𑄴𑄇𑄥𑄁 𑄃𑄮 𑄥𑄙𑄩𑄚𑄧𑄖𑄃𑄚𑄩 𑄥𑄢𑄚𑄘 𑄉𑄧𑄢𑄨 𑄛𑄢𑄧𑄚𑄴 𑄃𑄬𑄟𑄧𑄚𑄴 𑄇𑄧𑄚𑄧 𑄇𑄟𑄬 𑄣𑄨𑄛𑄴𑄖𑄧 𑄦𑄰𑄠𑄴 𑄛𑄢𑄬 𑄇𑄨𑄁𑄝 𑄥𑄬𑄙𑄮𑄇𑄳𑄠𑄬 𑄇𑄧𑄚𑄧 𑄇𑄟𑄴 𑄃𑄬𑄏𑄣𑄴𑄘𑄬𑄚 𑄉𑄧𑄢𑄨 𑄛𑄢𑄬𑅁\n 𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄟𑄚𑄬𑄭 𑄉𑄨𑄢𑄨𑄢𑄴 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄖𑄳𑄠𑄴 𑄥𑄧𑄁 𑄃𑄮 𑄑𑄚𑄑𑄚𑄳𑄠𑄴 𑄝𑄚𑄝𑄚𑄳𑄠𑄴 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄚𑄩 𑄃𑅅 𑄃𑄟𑄧𑄚𑄧 𑄎𑄘𑄧𑄢𑄴 𑄃𑄨𑄌𑄴𑄎𑄮𑄘𑄧𑄢𑄴 𑄟𑄚𑄚𑄩 𑄦𑄧𑄣𑄧𑄘𑄳𑄠𑄬 𑄛𑄨𑄖𑄨𑄨𑄟𑄨𑄖𑄴 𑄥𑄚𑄴𑄘𑄨, 𑄥𑄙𑄩𑄚𑄧𑄖 𑄃𑅅 𑄉𑄧𑄟𑄴 𑄝𑄨𑄏𑄬𑄢𑄧𑄢𑄴 𑄈𑄪𑄙𑄨 𑄃𑄨𑄝𑄬;\n𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄟𑄚𑄬𑄭 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄧𑄢𑄴 𑄛𑄳𑄢𑄧𑄖𑄨 𑄃𑄧𑄣𑄬𑄦𑄧𑄚𑄴 𑄃𑅅 𑄊𑄨𑄚𑄬𑄚𑄢𑄴 𑄜𑄧𑄣𑄬 𑄟𑄚𑄬𑄭𑄦𑄮𑄢𑄴 𑄃𑄬𑄘 𑄣𑄌𑄴𑄈𑄬𑄚𑄬𑄭 𑄃𑄬𑄘𑄮𑄇𑄳𑄠𑄴 𑄉𑄧𑄢𑄨 𑄃𑄬𑄟𑄚𑄴 𑄟𑄢𑄚 𑄘𑄮𑄇𑄳𑄠𑄴 𑄝𑄬𑄙𑄮𑄇𑄳𑄠𑄴 𑄇𑄟𑄴 𑄉𑄧𑄢𑄨𑄚𑄬𑄭 𑄃𑅅 𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄃𑄬𑄘𑄮𑄇𑄳𑄠𑄴 𑄃𑄬𑄇𑄳𑄦𑄴𑄚𑄴 𑄛𑄨𑄖𑄨𑄨𑄟𑄨𑄢𑄴 𑄜𑄪𑄢𑄨𑄅𑄪𑄘𑄨𑄚𑄬𑄭 𑄃𑄧𑄎𑄧𑄃𑄌𑄴 𑄟𑄚𑄬𑄭𑄦𑄮𑄢𑄴 𑄝𑄬𑄉𑄧 𑄓𑄋𑄧𑄢𑄴 𑄃𑄏 𑄉𑄧𑄢 𑄦𑄧𑄠𑄬, 𑄡𑄨𑄠𑄚𑄧𑄖𑄴 𑄝𑄬𑄇𑄴 𑄟𑄚𑄬𑄭𑄦𑄮𑄢𑄴 𑄙𑄧𑄢𑄴𑄟𑄧 𑄃𑅅 𑄇𑄧𑄙 𑄇𑄧𑄚𑄢𑄴 𑄎𑄪 𑄛𑄬𑄝𑄇𑄴 𑄃𑅅 𑄇𑄧𑄚𑄧 𑄢𑄖𑄴 𑄃𑄮 𑄚𑄧 𑄓𑄮𑄢𑄬𑄠𑄬 𑄎𑄨𑄁𑄇𑄚𑄩 𑄇𑄘𑄬𑄝𑄇𑄴;"
+  specimen_16: "𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄢𑄴 𑄏𑄨𑄢𑄬𑄚 𑄃𑄮 𑄃𑄏𑄬𑄢𑄴 𑄗𑄢𑄚𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄢𑄧𑄠𑄬; 𑄘𑄨𑄚𑄴𑄟𑄉𑄬𑄚𑄬 𑄃𑄧𑄇𑄴𑄖𑄧 𑄟𑄪𑄎𑄨𑄟𑄴 𑄝𑄬𑄖𑄧𑄚𑄴𑄥𑄪𑄟𑄪𑄖𑄴𑄘𑄳𑄠𑄧 𑄍𑄪𑄑𑄨 𑄃𑅅 𑄛𑄬𑄥𑄉𑄧𑄖𑄧 𑄇𑄟𑄧𑄢𑄴 𑄡𑄪𑄇𑄴𑄖𑄨𑄥𑄧𑄁 𑄥𑄩𑄟𑄃𑄮 𑄃𑄬 𑄃𑄇𑄴𑄇𑄥𑄁 𑄞𑄨𑄘𑄨𑄢𑄬 𑄢𑄧𑄠𑄬𑅁\n𑄃𑄬 𑄓𑄇𑄴𑄣𑄢𑄬𑄥𑄧𑄚𑄬 𑄘𑄬𑄉𑄬𑄠𑄬 𑄃𑄇𑄴𑄇𑄥𑄁 𑄃𑄮 𑄥𑄙𑄩𑄚𑄧𑄖𑄊𑄚𑄩𑄢𑄴 𑄇𑄟𑄧𑄖𑄴𑄣𑄉𑄚 𑄥𑄧𑄟𑄴𑄞𑄧𑄛𑄴 𑄃𑄬𑄟𑄧𑄚𑄴 𑄃𑄬𑄇𑄳𑄦𑄴𑄚𑄴 𑄥𑄟𑄎𑄨𑄇𑄴 𑄃𑄮 𑄛𑄨𑄖𑄨𑄨𑄟𑄨 𑄝𑄳𑄠𑄝𑄧𑄌𑄴𑄗𑄭 𑄃𑄧𑄁𑄥𑄩𑄘𑄢𑄨𑄖𑄳𑄠𑄬𑄢𑄴 𑄃𑄇𑄴𑄇𑄥𑄁 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄢𑄴 𑄃𑄊𑄬𑅁 \n𑄇𑄧𑄚𑄧 𑄢𑄬𑄎𑄳𑄠𑄧, 𑄉𑄪𑄖𑄨𑄨 𑄝 𑄟𑄚𑄪𑄌𑄴 𑄃𑄬 𑄓𑄨𑄇𑄴𑄣𑄢𑄬𑄥𑄧𑄚𑄧𑄢𑄴 𑄇𑄧𑄚𑄧 𑄇𑄨𑄌𑄴𑄅 𑄃𑄬𑄟𑄧𑄚𑄴𑄞𑄝𑄬 𑄝𑄳𑄠𑄈𑄳𑄠 𑄉𑄧𑄢𑄨 𑄚𑄧 𑄛𑄢𑄨𑄝𑄇𑄴, 𑄡𑄢𑄴 𑄝𑄧𑄣𑄬 𑄖𑄢 𑄃𑄬𑄭 𑄓𑄨𑄇𑄴𑄣𑄢𑄬𑄥𑄧𑄚𑄬 𑄘𑄬𑄉𑄬𑄠𑄬 𑄃𑄇𑄴𑄇𑄥𑄁 𑄃𑄮 𑄥𑄙𑄩𑄚𑄧𑄖𑄃𑄚𑄩 𑄥𑄢𑄚𑄘 𑄉𑄧𑄢𑄨 𑄛𑄢𑄧𑄚𑄴 𑄃𑄬𑄟𑄧𑄚𑄴 𑄇𑄧𑄚𑄧 𑄇𑄟𑄬 𑄣𑄨𑄛𑄴𑄖𑄧 𑄦𑄰𑄠𑄴 𑄛𑄢𑄬 𑄇𑄨𑄁𑄝 𑄥𑄬𑄙𑄮𑄇𑄳𑄠𑄬 𑄇𑄧𑄚𑄧 𑄇𑄟𑄴 𑄃𑄬𑄏𑄣𑄴𑄘𑄬𑄚 𑄉𑄧𑄢𑄨 𑄛𑄢𑄬𑅁\n 𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄟𑄚𑄬𑄭 𑄉𑄨𑄢𑄨𑄢𑄴 𑄝𑄬𑄇𑄴𑄅𑄚𑄧𑄖𑄳𑄠𑄴 𑄥𑄧𑄁 𑄃𑄮 𑄑𑄚𑄑𑄚𑄳𑄠𑄴 𑄝𑄚𑄝𑄚𑄳𑄠𑄴 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄚𑄩 𑄃𑅅 𑄃𑄟𑄧𑄚𑄧 𑄎𑄘𑄧𑄢𑄴 𑄃𑄨𑄌𑄴𑄎𑄮𑄘𑄧𑄢𑄴 𑄟𑄚𑄚𑄩 𑄦𑄧𑄣𑄧𑄘𑄳𑄠𑄬 𑄛𑄨𑄖𑄨𑄨𑄟𑄨𑄖𑄴 𑄥𑄚𑄴𑄘𑄨, 𑄥𑄙𑄩𑄚𑄧𑄖 𑄃𑅅 𑄉𑄧𑄟𑄴 𑄝𑄨𑄏𑄬𑄢𑄧𑄢𑄴 𑄈𑄪𑄙𑄨 𑄃𑄨𑄝𑄬;\n𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄟𑄚𑄬𑄭 𑄃𑄇𑄴𑄇𑄥𑄁𑄃𑄧𑄢𑄴 𑄛𑄳𑄢𑄧𑄖𑄨 𑄃𑄧𑄣𑄬𑄦𑄧𑄚𑄴 𑄃𑅅 𑄊𑄨𑄚𑄬𑄚𑄢𑄴 𑄜𑄧𑄣𑄬 𑄟𑄚𑄬𑄭𑄦𑄮𑄢𑄴 𑄃𑄬𑄘 𑄣𑄌𑄴𑄈𑄬𑄚𑄬𑄭 𑄃𑄬𑄘𑄮𑄇𑄳𑄠𑄴 𑄉𑄧𑄢𑄨 𑄃𑄬𑄟𑄚𑄴 𑄟𑄢𑄚 𑄘𑄮𑄇𑄳𑄠𑄴 𑄝𑄬𑄙𑄮𑄇𑄳𑄠𑄴 𑄇𑄟𑄴 𑄉𑄧𑄢𑄨𑄚𑄬𑄭 𑄃𑅅 𑄡𑄨𑄠𑄚𑄧𑄖𑄳𑄠𑄬 𑄃𑄬𑄘𑄮𑄇𑄳𑄠𑄴 𑄃𑄬𑄇𑄳𑄦𑄴𑄚𑄴 𑄛𑄨𑄖𑄨𑄨𑄟𑄨𑄢𑄴 𑄜𑄪𑄢𑄨𑄅𑄪𑄘𑄨𑄚𑄬𑄭 𑄃𑄧𑄎𑄧𑄃𑄌𑄴 𑄟𑄚𑄬𑄭𑄦𑄮𑄢𑄴 𑄝𑄬𑄉𑄧 𑄓𑄋𑄧𑄢𑄴 𑄃𑄏 𑄉𑄧𑄢 𑄦𑄧𑄠𑄬, 𑄡𑄨𑄠𑄚𑄧𑄖𑄴 𑄝𑄬𑄇𑄴 𑄟𑄚𑄬𑄭𑄦𑄮𑄢𑄴 𑄙𑄧𑄢𑄴𑄟𑄧 𑄃𑅅 𑄇𑄧𑄙 𑄇𑄧𑄚𑄢𑄴 𑄎𑄪 𑄛𑄬𑄝𑄇𑄴 𑄃𑅅 𑄇𑄧𑄚𑄧 𑄢𑄖𑄴 𑄃𑄮 𑄚𑄧 𑄓𑄮𑄢𑄬𑄠𑄬 𑄎𑄨𑄁𑄇𑄚𑄩 𑄇𑄘𑄬𑄝𑄇𑄴;"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ce_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ce_Cyrl.textproto`

 * *Files 17% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 name: "Chechen"
 autonym: "Нохчийн мотт"
 population: 935365
 region: "RU"
 exemplar_chars {
   base: "а {аь} б в г {гӏ} д е ё ж з и {ий} й к {кк} {ккх} {кх} {кь} {кӏ} л м н о {ов} {оь} п {пп} {пӏ} р {рхӏ} с {сс} т {тт} {тӏ} у {ув} {уь} {уьй} ф х {хь} {хӏ} ц {цӏ} ч {чӏ} ш щ ъ ы ь э ю {юь} я {яь}"
   marks: "◌̆ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
   index: "А Б В Г Д Е Ё Ж З И К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ъ Ы Ь Э Ю Я"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ceb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ceb_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Cebuano"
 autonym: "Binisaya"
 population: 26203440
 region: "PH"
 exemplar_chars {
   base: "a b d e g h i k l m n o p r s t u w y"
   auxiliary: "c f j ñ q v x z"
-  punctuation: "- ‑ , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & # ′ ″"
+  punctuation: "- , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaNn"
   masthead_partial: "Gg"
   styles: "Samtamg ang pag-ila sa tiunay nga kabililhon"
   tester: "Samtang ang wala pagtagad ug pagbiaybiay sa mga tawhanong katungod"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cfm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cfm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ch_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ch_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/chj_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/chj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/chk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/chk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/chr_Cher.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/chr_Cher.textproto`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 name: "Cherokee"
 autonym: "ᏣᎳᎩ ᎦᏬᏂᎯᏍᏗ"
 population: 25613
 region: "US"
 exemplar_chars {
   base: "ꭰ ꭱ ꭲ ꭳ ꭴ ꭵ ꭶ ꭷ ꭸ ꭹ ꭺ ꭻ ꭼ ꭽ ꭾ ꭿ ꮀ ꮁ ꮂ ꮃ ꮄ ꮅ ꮆ ꮇ ꮈ ꮉ ꮊ ꮋ ꮌ ꮍ ꮎ ꮏ ꮐ ꮑ ꮒ ꮓ ꮔ ꮕ ꮖ ꮗ ꮘ ꮙ ꮚ ꮛ ꮜ ꮝ ꮞ ꮟ ꮠ ꮡ ꮢ ꮣ ꮤ ꮥ ꮦ ꮧ ꮨ ꮩ ꮪ ꮫ ꮬ ꮭ ꮮ ꮯ ꮰ ꮱ ꮲ ꮳ ꮴ ꮵ ꮶ ꮷ ꮸ ꮹ ꮺ ꮻ ꮼ ꮽ ꮾ ꮿ ᏸ ᏹ ᏺ ᏻ ᏼ"
   auxiliary: ""
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "Ꭰ Ꭶ Ꭽ Ꮃ Ꮉ Ꮎ Ꮖ Ꮜ Ꮣ Ꮬ Ꮳ Ꮹ Ꮿ"
 }
 sample_text {
   masthead_full: "ᏂꮒᎦꭶ"
   masthead_partial: "Ꮣꮣ"
   styles: "ᎬᏂᏳᏉ ᏗᏓᏂᎸᏨ ᎾᏍᎩ ᎠᏠᏯᏍᏗᏍᎩ ᎠᏢᏉᏙᏗ ᎠᎴ ᎾᏍᎩᏃ ᎢᎦᏘ"
   tester: "ᎬᏂᏳᏉ ᎠᎦᏎᏍᏔᏅᎾ ᎠᎴ ᏂᎦᎸᏉᏛᎾ ᎾᏍᎩᎾ ᎠᏂᏴᏫ ᎤᏂᎲ ᎢᏳᎾᏛᏗᎢ ᎤᏂᎲᎢ ᏫᏂᏚᎵᏍᏔᏅᎩ Ꮎ ᎤᏂᏍᎦᏎᏘ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/chx_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/chx_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cic_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cic_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cjk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cjk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cjs_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cjs_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
   base: "А Б В Г Д Е Ж З И Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ъ Ы Ь Э Ю Я Ё Ғ Қ Ң Ӧ Ӱ а б в г д е ж з и й к л м н о п р с т у ф х ц ч ш щ ъ ы ь э ю я ё ғ қ ң ӧ ӱ"
   marks: "◌̆ ◌̈"
 }
 sample_text {
   masthead_full: "ПпАа"
   masthead_partial: "Рр"
   styles: "Парчын кижини тенъ тоолабазабыс, пош, шын, абыр"
-  tester: "Кижилерди қыстапкел тоолабанчыабыста, улуғ  қан тӧгӱлӱп, кижи сағыжы"
+  tester: "Кижилерди қыстапкел тоолабанчыабыста, улуғ қан тӧгӱлӱп, кижи сағыжы"
   poster_sm: "Наа чадыйыбыс,"
   poster_md: "Кижилерди"
   poster_lg: "Парчын"
   specimen_48: "Ақ чарықта чатчыған чонқалықтар, ӧзере тартышпан, арғыштаныш полып,"
   specimen_36: "Парчын кижи, ол қайдығ да чозақтығ, тиллиғ полза, по декларацияға кӧре, чозақ аны пашқа кижилербе тең кӧртурзын."
   specimen_32: "Парчын кижи ноо ла санарға саназа, аны саназын, ноо ла айдарға саназа, аны айтсын, ноо ла тилерге, табарға саназа, аны тапсын, кем да аны қайдығ черде да тоқтатпазын."
   specimen_21: "Парчын кижи, қалық аразында чӧрӱуп, чақшы чадарға, қатчы поларға, пай поларға керек небелерин алзын.\nПарчын кижи тынанарға керек полза, тынанзын, ойун ойнарға саназа, ойназын, ужыпажы чоқ тем иштебезин, отпусктығ ползын.\nПарчын кижи қалықтар, кижилер араларында, по декларацияда пасқан небелерге кӧре, улуғ тоолаттырзын, асқайлатпазын."
-  specimen_16: "По декларацияда пасқан небелери пир ле қаан черин, пир чонқалықтың керегин тутчаң небелери эбес; кемге да, по декларацияда пасқан небелерин чоқ эдерге чарабас; по декларацияда пасқан небелери,  кижилерге полушкелип,  пистиң чақшы чадыйыбыс пӱдӱрзиннер.\nПарчын кижини тенъ тоолабазабыс, пош, шын, абыр чадыйыбыс пар полбас теп, кӧрӱп;\nКижилерди қыстапкел тоолабанчыабыста, улуғ  қан тӧгӱлӱп, кижи сағыжы қырыл турча теп, кӧрӱп;\nНаа чадыйыбыс, ол парчын кижи айдарын айдар, сананғанын ажар чадыйы, анаң аара кижи қоруқпан, керексинмен чӧрер чадыйы ползын теп, кӧрӱп;\nКижилерди улуғ тоолап, ыларға чозақ полушсын теп,  қыстаған кижилер қыстапчыған кижилердең тоғра турбазыннар, ӧдӱрӱшпезиннер теп, кӧрӱп;"
+  specimen_16: "По декларацияда пасқан небелери пир ле қаан черин, пир чонқалықтың керегин тутчаң небелери эбес; кемге да, по декларацияда пасқан небелерин чоқ эдерге чарабас; по декларацияда пасқан небелери, кижилерге полушкелип, пистиң чақшы чадыйыбыс пӱдӱрзиннер.\nПарчын кижини тенъ тоолабазабыс, пош, шын, абыр чадыйыбыс пар полбас теп, кӧрӱп;\nКижилерди қыстапкел тоолабанчыабыста, улуғ қан тӧгӱлӱп, кижи сағыжы қырыл турча теп, кӧрӱп;\nНаа чадыйыбыс, ол парчын кижи айдарын айдар, сананғанын ажар чадыйы, анаң аара кижи қоруқпан, керексинмен чӧрер чадыйы ползын теп, кӧрӱп;\nКижилерди улуғ тоолап, ыларға чозақ полушсын теп, қыстаған кижилер қыстапчыған кижилердең тоғра турбазыннар, ӧдӱрӱшпезиннер теп, кӧрӱп;"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cjy_Hans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cjy_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ckb_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ckb_Arab.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 name: "Central Kurdish"
 population: 11086548
 region: "IQ"
 region: "IR"
 exemplar_chars {
   base: "ئ ا ب پ ت ج چ ح خ د ر ز ڕ ژ س ش ع غ ف ڤ ق ک گ ل ڵ م ن ھ ە و ۆ ی ێ"
   auxiliary: "‎‏ ً ٌ ٍ َ ُ ِ ّ ْ ء آ أ ؤ إ ة ث ذ ص ض ط ظ ك ه ى ي"
-  numerals: "‎‏ - ‑ , ٫ ٬ . % ٪ ‰ ؉ + 0٠ 1١ 2٢ 3٣ 4٤ 5٥ 6٦ 7٧ 8٨ 9٩"
+  numerals: "‎‏ - , ٫ ٬ . % ٪ ؉ + 0٠ 1١ 2٢ 3٣ 4٤ 5٥ 6٦ 7٧ 8٨ 9٩"
   index: "ئ ا ب پ ت ج چ ح خ د ر ز ڕ ژ س ش ع غ ف ڤ ق ک گ ل ڵ م ن ھ ە و ۆ ی ێ"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cnh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cnh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cni_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cni_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/co_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/co_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cof_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cof_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/con_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/con_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cop_Copt.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cop_Copt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cot_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cot_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cpu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cpu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/crh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/crh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cri_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cri_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/crs_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/crs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cs_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cs_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 13045532
 region: "CZ"
 region: "SK"
 exemplar_chars {
   base: "a á b c č d ď e é ě f g h {ch} i í j k l m n ň o ó p q r ř s š t ť u ú ů v w x y ý z ž"
   auxiliary: "à ă â å ä ã ā æ ç è ĕ ê ë ē ì ĭ î ï ī ľ ł ñ ò ŏ ô ö ø ō œ ŕ ù ŭ û ü ū ÿ"
   marks: "◌́ ◌̊ ◌̌"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] § @ * / &"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] @ * / &"
   index: "A B C Č D E F G H {CH} I J K L M N O P Q R Ř S Š T U V W X Y Z Ž"
 }
 sample_text {
   masthead_full: "VvŠš"
   masthead_partial: "Ii"
   styles: "že uznání přirozené důstojnosti a rovných"
   tester: "že zneuznání lidských práv a pohrdání jimi vedlo k barbarským"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/csa_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/csa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/csb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/csb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/csw_Cans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/csw_Cans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ctd_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ctd_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cu_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cu_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cu_Glag.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cu_Glag.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cv_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cv_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cy_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cy_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 536376
 region: "AR"
 region: "GB"
 exemplar_chars {
   base: "a á à â ä b c {ch} d {dd} e é è ê ë f {ff} g {ng} h i í ì î ï j l {ll} m n o ó ò ô ö p {ph} r {rh} s t {th} u ú ù û ü w ẃ ẁ ŵ ẅ y ý ỳ ŷ ÿ"
   auxiliary: "ă å ã ā æ ç ĕ ē ĭ ī k ñ ŏ ø ō œ q ŭ ū v x z"
   marks: "◌̀ ◌́ ◌̂ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C {CH} D {DD} E F {FF} G {NG} H I J K L {LL} M N O P {PH} Q R {RH} S T {TH} U V W X Y Z"
 }
 sample_text {
   masthead_full: "GgEe"
   masthead_partial: "Nn"
   styles: "Gan mai cydnabod urddas cynhenid a hawliau"
   tester: "Gan i anwybyddu a dirmygu hawliau dynol arwain at weithredoedd"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/cyo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/cyo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/da_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/da_Latn.textproto`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "DK"
 region: "GL"
 region: "IS"
 exemplar_chars {
   base: "a b c d e f g h i j k l m n o p q r s t u v w x y z æ ø å"
   auxiliary: "á à â ç é è ê ë í î ï ñ ó ô œ ú ù û ÿ ü ä ǿ ö"
   marks: "◌̊ ◌́"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z Æ Ø Å"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Ee"
   styles: "Da anerkendelse af den mennesket iboende"
   tester: "da tilsidesættelse af og foragt for menneskerettighederne har"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dag_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dag_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ddn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ddn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/de_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/de_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 region: "PY"
 region: "RO"
 region: "SI"
 region: "SK"
 region: "US"
 exemplar_chars {
   base: "a ä b c d e f g h i j k l m n o ö p q r s ß t u ü v w x y z"
-  auxiliary: "á à ă â å ã ā æ ç é è ĕ ê ë ē ğ í ì ĭ î ï İ ī ı ñ ó ò ŏ ô ø ō œ ş ú ù ŭ û ū ÿ"
+  auxiliary: "á à ă â å ã ā æ ç é è ĕ ê ë ē ğ í ì ĭ î ï İ ī ı ñ ó ò ŏ ô ø ō œ ş ſ ú ù ŭ û ū ÿ"
   marks: "◌̈ ◌̀ ◌́"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
-  index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
+  index: "A B C D E F G H I J K L M N O P Q R S ẞ T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Ee"
   styles: "Alle Menschen sind frei und gleich an Würde"
   tester: "Alle Menschen sind frei und gleich an Würde und Rechten geboren."
   poster_sm: "Alle Menschen"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dga_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dga_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dhi_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dhi_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dhw_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dhw_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dip_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dip_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dmf_Medf.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dmf_Medf.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/doi_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/doi_Deva.textproto`

 * *Files 21% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 name: "Dogri"
 autonym: "𑠖𑠵𑠌𑠤𑠮"
 population: 2652180
 region: "IN"
 exemplar_chars {
   base: "॑ ॒ ़ ँ ं ः ॐ अ आ इ ई उ ऊ ऋ ॠ ऌ ॡ ए ऐ ओ औ क {क्ष} ख ग घ ङ च छ ज झ ञ ट ठ ड {ड़} ढ {ढ़} ण त थ द ध न प फ ब भ म य र ल ळ व श ष स ह ऽ ा ि ी ु ू ृ ॄ ॢ ॣ े ै ो ौ ्"
   auxiliary: "‌‍ ऍ ऑ ॅ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "_ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "_ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) @ * / & #"
   index: "अ आ इ ई उ ऊ ऋ ॠ ऌ ॡ ए ऐ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल ळ व श ष स ह"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dsb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dsb_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Dolnoserbšćina"
 population: 6973
 region: "DE"
 exemplar_chars {
   base: "a b c č ć d e ě f g h {ch} i j k ł l m n ń o ó p q r ŕ s š ś t u v w x y z ž ź"
   auxiliary: "á à ă â å ä ã ą ā æ ç ď đ é è ĕ ê ë ė ę ē ğ í ì ĭ î ï İ ī ı ĺ ľ ň ñ ò ŏ ô ö ő ø ō œ ř ş ß ť ú ù ŭ û ů ü ű ū ý ÿ ż"
   marks: "◌́ ◌̌"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
   index: "A B C Č Ć D E F G H {Ch} I J K Ł L M N O P Q R S Š Ś T U V W X Y Z Ž Ź"
 }
 sample_text {
   masthead_full: "WwŠš"
   masthead_partial: "Yy"
   styles: "Wšykne luźe su lichotne roźone a jadnake"
   tester: "Wšykne luźe su lichotne roźone a jadnake po dostojnosći a pšawach."
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dtp_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dtp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dty_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dty_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/duu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/duu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dv_Thaa.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dv_Thaa.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dyo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dyo_Latn.textproto`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Jóola-Fóoñi"
 population: 409146
 region: "SN"
 exemplar_chars {
   base: "a A á Á b B c C d D e E é É f F g G h H i I í Í j J k K l L m M n N ñ Ñ ŋ Ŋ o O ó Ó p P q Q r R s S t T u U ú Ú v V w W x X y Y"
   auxiliary: "z Z"
   marks: "◌́ ◌̃"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N Ñ Ŋ O P Q R S T U V W X Y"
 }
 sample_text {
   masthead_full: "BbUu"
   masthead_partial: "Kk"
   styles: "Yíneni aat mati faŋaaf fati anau di sidruwaas"
   tester: "Yíneni jaat anau nasonsoŋ mati kàmanjaataak di eñoosey sidruwaas"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dyu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dyu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/dz_Tibt.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/dz_Tibt.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 370341
 region: "BT"
 region: "IN"
 exemplar_chars {
   base: "ཀ ཁ ག ང ཅ ཆ ཇ ཉ ཏ ཐ ད ན པ ཕ བ མ ཙ ཚ ཛ ཝ ཞ ཟ འ ཡ ར ལ ཤ ས ཧ ཨ ི ུ ེ ོ ྐ ྑ ྒ ྔ ྗ ྙ ྟ ྠ ྡ ྣ ྤ ྥ ྦ ྨ ྩ ྪ ྫ ྭ ྱ ྲ ླ ྵ ྶ ྷ"
   auxiliary: "྄ ཊ ཋ ཌ ཎ ཾ ཥ ྀ ཻ ཽ ྚ ྛ ྜ ྞ ྺ ྻ ྼ"
   marks: "◌ི ◌ུ ◌ེ ◌ོ ◌ྵ"
-  numerals: "- ‑ , . % ‰ + 0༠ 1༡ 2༢ 3༣ 4༤ 5༥ 6༦ 7༧ 8༨ 9༩"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] ༼ ༽ § @ * / & # † ‡ ༄ ༅ ༆ ༈ ༉ ༊ ࿐ ࿑ ༒ ࿒ ࿓ ࿔ ༶ ྾ ྿ ༌ ། ༎ ༏ ༐ ༑ ༔ ༴"
+  numerals: "- , . % + 0༠ 1༡ 2༢ 3༣ 4༤ 5༥ 6༦ 7༧ 8༨ 9༩"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] ༼ ༽ @ * / & # ༄ ༅ ༆ ༈ ༉ ༊ ࿐ ࿑ ༒ ࿒ ࿓ ࿔ ༶ ྾ ྿ ༌ ། ༎ ༏ ༐ ༑ ༔ ༴"
   index: "ཀ ཁ ག ང ཅ ཆ ཇ ཉ ཏ ཐ ད ན པ ཕ བ མ ཙ ཚ ཛ ཝ ཞ ཟ འ ཡ ར ལ ཤ ས ཧ ཨ"
 }
 sample_text {
   masthead_full: "འགབམ"
   masthead_partial: "ཚར"
   styles: "དེ་ཡང་ འཛམ་གླིང་ནང་གི་ཞི་བདེ་དང་དྲང་ཁྲིམས། དེ་ལས་དལ་དབང་ཚུ་གི་གཞི་འགྱམ་གཙོ་བོ་དེ་"
   tester: "དེ་ཡང་ འགྲོ་བ་མིའི་དལ་དབང་ལུ་ཆ་གནས་མ་འབད་མི་དང་། བརྩི་བཀུར་མ་འབད་མི་ལུ་བརྟེན་ཏེ་ ཀླ་ཀློའི་སྤྱོད་པ་དང་འབྲེལ་བའི་བྱ་སྤྱོད་ལུ་བརྩོན་བཅུག་སྟེ་"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ee_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ee_Latn.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 4690856
 region: "GH"
 region: "TG"
 exemplar_chars {
   base: "a A á Á à À ã Ã b B d D ɖ Ɖ e E é É è È ẽ Ẽ ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̀} {Ɛ̀} {ɛ̃} {Ɛ̃} f F ƒ Ƒ g G ɣ Ɣ h H x X i I í Í ì Ì ĩ Ĩ k K l L m M n N ŋ Ŋ o O ó Ó ò Ò õ Õ ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̀} {Ɔ̀} {ɔ̃} {Ɔ̃} p P r R s S t T u U ú Ú ù Ù ũ Ũ v V ʋ Ʋ w W y Y z Z"
   auxiliary: "ă Ă â Â å Å ä Ä ā Ā æ Æ c C ç Ç ĕ Ĕ ê Ê ë Ë ĭ Ĭ î Î ï Ï j J ñ Ñ ŏ Ŏ ô Ô ö Ö ø Ø œ Œ q Q ŭ Ŭ û Û ü Ü ÿ Ÿ"
   marks: "◌̀ ◌́ ◌̃ ◌̂ ◌̄ ◌̆ ◌̈ ◌̊ ◌̧"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } @ * / & #"
   index: "A B D Ɖ E Ɛ F Ƒ G Ɣ H X I K L M N Ŋ O Ɔ P R S T U V Ʋ W Y Z"
 }
 sample_text {
   masthead_full: "WwOo"
   masthead_partial: "Dd"
   styles: "Esi woɖe dzesi kɔtɛe be, amegbetɔwo katã ƒe"
   tester: "Esi eme va kɔ ƒãa be, ablɔɖevinyenye si nye amegbetɔ ɖesiaɖe tɔ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/egy_Egyp.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/egy_Egyp.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/el_Grek.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/el_Grek.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 region: "RO"
 region: "TR"
 region: "UA"
 exemplar_chars {
   base: "α ά β γ δ ε έ ζ η ή θ ι ί ϊ ΐ κ λ μ ν ξ ο ό π ρ σ ς τ υ ύ ϋ ΰ φ χ ψ ω ώ"
   auxiliary: "ἀ ἄ ἂ ἆ ἁ ἅ ἃ ἇ ὰ ᾶ ἐ ἔ ἒ ἑ ἕ ἓ ὲ ἠ ἤ ἢ ἦ ἡ ἥ ἣ ἧ ὴ ῆ ἰ ἴ ἲ ἶ ἱ ἵ ἳ ἷ ὶ ῖ ῒ ῗ ὄ ὂ ὃ ὸ ὐ ὔ ὒ ὖ ὑ ὕ ὓ ὗ ὺ ῦ ῢ ῧ ὤ ὢ ὦ ὥ ὣ ὧ ὼ ῶ"
   marks: "◌́ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! . … \" « » ( ) [ ] § @ * / \\ &"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! . … \" « » ( ) [ ] @ * / \\ &"
   index: "Α Β Γ Δ Ε Ζ Η Θ Ι Κ Λ Μ Ν Ξ Ο Π Ρ Σ Τ Υ Φ Χ Ψ Ω"
 }
 sample_text {
   masthead_full: "ΌόΛλ"
   masthead_partial: "Οο"
   styles: "Όλοι οι άνθρωποι γεννιούνται ελεύθεροι και"
   tester: "Όλοι οι άνθρωποι γεννιούνται ελεύθεροι και ίσοι στην αξιοπρέπεια"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/emk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/emk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/en_Brai.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/en_Brai.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/en_Dsrt.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/en_Dsrt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/en_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/en_Latn.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -152,16 +152,16 @@
 region: "ZA"
 region: "ZM"
 region: "ZW"
 exemplar_chars {
   base: "a b c d e f g h i j k l m n o p q r s t u v w x y z"
   auxiliary: "á à ă â å ä ã ā æ ç é è ĕ ê ë ē í ì ĭ î ï ī ñ ó ò ŏ ô ö ø ō œ ú ù ŭ û ü ū ÿ"
   marks: "◌̀ ◌́ ◌̂ ◌̃ ◌̈ ◌̧"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Hh"
   styles: "Whereas recognition of the inherent dignity"
   tester: "Whereas disregard and contempt for human rights have resulted"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/en_Shaw.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/en_Shaw.textproto`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,12 @@
   styles: "𐑢𐑺𐑨𐑟 𐑮𐑧𐑒𐑩𐑜𐑯𐑦𐑖𐑩𐑯 𐑝 𐑞 𐑦𐑯𐑣𐑧𐑮𐑩𐑯𐑑 𐑛𐑦𐑜𐑯𐑦𐑑𐑦 𐑯 𐑝"
   tester: "·𐑢𐑺𐑨𐑟 𐑛𐑦𐑕𐑮𐑦𐑜𐑸𐑛 𐑯 𐑒𐑩𐑯𐑑𐑧𐑥𐑐𐑑 𐑓 𐑣𐑿𐑥𐑩𐑯 𐑮𐑲𐑑𐑕 𐑣𐑨𐑝 𐑮𐑦𐑟𐑳𐑤𐑑𐑩𐑛 𐑦𐑯 𐑚𐑸𐑚𐑼𐑩𐑕"
   poster_sm: "·𐑢𐑺𐑨𐑟 𐑦𐑑 𐑦𐑟"
   poster_md: "·𐑢𐑺𐑨𐑟 ·𐑥𐑧𐑥𐑚𐑼"
   poster_lg: "𐑣𐑿𐑥𐑩𐑯"
   specimen_48: "·𐑢𐑺𐑨𐑟 𐑩 𐑒𐑪𐑥𐑩𐑯 𐑳𐑯𐑛𐑼𐑕𐑑𐑨𐑯𐑛𐑦𐑙 𐑝 𐑞𐑰𐑟 𐑮𐑲𐑑𐑕 𐑯 𐑓𐑮𐑰𐑛𐑩𐑥𐑟 𐑦𐑟 𐑝 𐑞 𐑜𐑮𐑱𐑑𐑩𐑕𐑑"
   specimen_36: "·𐑧𐑝𐑮𐑦𐑢𐑳𐑯 𐑦𐑟 𐑦𐑯𐑑𐑲𐑑𐑩𐑤𐑛 𐑑 𐑩 𐑕𐑴𐑖𐑩𐑤 𐑯 𐑦𐑯𐑑𐑼𐑯𐑨𐑖𐑩𐑯𐑩𐑤 𐑹𐑛𐑼 𐑦𐑯 𐑢𐑦𐑗 𐑞 𐑮𐑲𐑑𐑕 𐑯 𐑓𐑮𐑰𐑛𐑩𐑥𐑟 𐑕𐑧𐑑 𐑓𐑹𐑔 𐑦𐑯 𐑞𐑦𐑕 ·𐑛𐑧𐑒𐑤𐑼𐑱𐑖𐑩𐑯 𐑒𐑨𐑯 𐑚𐑰 𐑓𐑫𐑤𐑦 𐑮𐑾𐑤𐑲𐑟𐑛."
-  specimen_32: "·𐑢𐑺𐑨𐑟 𐑮𐑧𐑒𐑩𐑜𐑯𐑦𐑖𐑩𐑯 𐑝 𐑞 𐑦𐑯𐑣𐑧𐑮𐑩𐑯𐑑 𐑛𐑦𐑜𐑯𐑦𐑑𐑦 𐑯 𐑝 𐑞 𐑰𐑒𐑢𐑩𐑤 𐑯 𐑦𐑯𐑱𐑤𐑾𐑯𐑩𐑚𐑩𐑤 𐑮𐑲𐑑𐑕 𐑝 𐑷𐑤 𐑥𐑧𐑥𐑚𐑼𐑟 𐑝 𐑞 𐑣𐑿𐑥𐑩𐑯 𐑓𐑨𐑥𐑦𐑤𐑦 𐑦𐑟 𐑞 𐑓𐑬𐑯𐑛𐑱𐑖𐑩𐑯 𐑝 𐑓𐑮𐑰𐑛𐑩𐑥, 𐑡𐑳𐑕𐑑𐑦𐑕 𐑯 𐑐𐑰𐑕 𐑦𐑯\n            𐑞 𐑢𐑻𐑤𐑛,"
-  specimen_21: "·𐑢𐑺𐑨𐑟 𐑮𐑧𐑒𐑩𐑜𐑯𐑦𐑖𐑩𐑯 𐑝 𐑞 𐑦𐑯𐑣𐑧𐑮𐑩𐑯𐑑 𐑛𐑦𐑜𐑯𐑦𐑑𐑦 𐑯 𐑝 𐑞 𐑰𐑒𐑢𐑩𐑤 𐑯 𐑦𐑯𐑱𐑤𐑾𐑯𐑩𐑚𐑩𐑤 𐑮𐑲𐑑𐑕 𐑝 𐑷𐑤 𐑥𐑧𐑥𐑚𐑼𐑟 𐑝 𐑞 𐑣𐑿𐑥𐑩𐑯 𐑓𐑨𐑥𐑦𐑤𐑦 𐑦𐑟 𐑞 𐑓𐑬𐑯𐑛𐑱𐑖𐑩𐑯 𐑝 𐑓𐑮𐑰𐑛𐑩𐑥, 𐑡𐑳𐑕𐑑𐑦𐑕 𐑯 𐑐𐑰𐑕 𐑦𐑯\n            𐑞 𐑢𐑻𐑤𐑛,\n·𐑢𐑺𐑨𐑟 𐑛𐑦𐑕𐑮𐑦𐑜𐑸𐑛 𐑯 𐑒𐑩𐑯𐑑𐑧𐑥𐑐𐑑 𐑓 𐑣𐑿𐑥𐑩𐑯 𐑮𐑲𐑑𐑕 𐑣𐑨𐑝 𐑮𐑦𐑟𐑳𐑤𐑑𐑩𐑛 𐑦𐑯 𐑚𐑸𐑚𐑼𐑩𐑕 𐑨𐑒𐑑𐑕 𐑢𐑦𐑗 𐑣𐑨𐑝 𐑬𐑑𐑮𐑱𐑡𐑛 𐑞 𐑒𐑪𐑯𐑖𐑩𐑯𐑕 𐑝 𐑥𐑨𐑯𐑒𐑲𐑯𐑛, 𐑯 𐑞 𐑨𐑛𐑝𐑧𐑯𐑑 𐑝 𐑩 𐑢𐑻𐑤𐑛 𐑦𐑯 𐑢𐑦𐑗 𐑣𐑿𐑥𐑩𐑯 𐑚𐑰𐑦𐑙𐑟\n            𐑖𐑨𐑤 𐑦𐑯𐑡𐑶 𐑓𐑮𐑰𐑛𐑩𐑥 𐑝 𐑕𐑐𐑰𐑗 𐑯 𐑚𐑦𐑤𐑰𐑓 𐑯 𐑓𐑮𐑰𐑛𐑩𐑥 𐑓𐑮𐑪𐑥 𐑓𐑽 𐑯 𐑢𐑪𐑯𐑑 𐑣𐑨𐑟 𐑚𐑰𐑯 𐑐𐑮𐑴𐑒𐑤𐑱𐑥𐑛 𐑨𐑟 𐑞 𐑣𐑲𐑩𐑕𐑑 𐑨𐑕𐑐𐑼𐑱𐑖𐑩𐑯 𐑝 𐑞 𐑒𐑪𐑥𐑩𐑯 𐑐𐑰𐑐𐑩𐑤,"
-  specimen_16: "·𐑢𐑺𐑨𐑟 𐑮𐑧𐑒𐑩𐑜𐑯𐑦𐑖𐑩𐑯 𐑝 𐑞 𐑦𐑯𐑣𐑧𐑮𐑩𐑯𐑑 𐑛𐑦𐑜𐑯𐑦𐑑𐑦 𐑯 𐑝 𐑞 𐑰𐑒𐑢𐑩𐑤 𐑯 𐑦𐑯𐑱𐑤𐑾𐑯𐑩𐑚𐑩𐑤 𐑮𐑲𐑑𐑕 𐑝 𐑷𐑤 𐑥𐑧𐑥𐑚𐑼𐑟 𐑝 𐑞 𐑣𐑿𐑥𐑩𐑯 𐑓𐑨𐑥𐑦𐑤𐑦 𐑦𐑟 𐑞 𐑓𐑬𐑯𐑛𐑱𐑖𐑩𐑯 𐑝 𐑓𐑮𐑰𐑛𐑩𐑥, 𐑡𐑳𐑕𐑑𐑦𐑕 𐑯 𐑐𐑰𐑕 𐑦𐑯\n            𐑞 𐑢𐑻𐑤𐑛,\n·𐑢𐑺𐑨𐑟 𐑛𐑦𐑕𐑮𐑦𐑜𐑸𐑛 𐑯 𐑒𐑩𐑯𐑑𐑧𐑥𐑐𐑑 𐑓 𐑣𐑿𐑥𐑩𐑯 𐑮𐑲𐑑𐑕 𐑣𐑨𐑝 𐑮𐑦𐑟𐑳𐑤𐑑𐑩𐑛 𐑦𐑯 𐑚𐑸𐑚𐑼𐑩𐑕 𐑨𐑒𐑑𐑕 𐑢𐑦𐑗 𐑣𐑨𐑝 𐑬𐑑𐑮𐑱𐑡𐑛 𐑞 𐑒𐑪𐑯𐑖𐑩𐑯𐑕 𐑝 𐑥𐑨𐑯𐑒𐑲𐑯𐑛, 𐑯 𐑞 𐑨𐑛𐑝𐑧𐑯𐑑 𐑝 𐑩 𐑢𐑻𐑤𐑛 𐑦𐑯 𐑢𐑦𐑗 𐑣𐑿𐑥𐑩𐑯 𐑚𐑰𐑦𐑙𐑟\n            𐑖𐑨𐑤 𐑦𐑯𐑡𐑶 𐑓𐑮𐑰𐑛𐑩𐑥 𐑝 𐑕𐑐𐑰𐑗 𐑯 𐑚𐑦𐑤𐑰𐑓 𐑯 𐑓𐑮𐑰𐑛𐑩𐑥 𐑓𐑮𐑪𐑥 𐑓𐑽 𐑯 𐑢𐑪𐑯𐑑 𐑣𐑨𐑟 𐑚𐑰𐑯 𐑐𐑮𐑴𐑒𐑤𐑱𐑥𐑛 𐑨𐑟 𐑞 𐑣𐑲𐑩𐑕𐑑 𐑨𐑕𐑐𐑼𐑱𐑖𐑩𐑯 𐑝 𐑞 𐑒𐑪𐑥𐑩𐑯 𐑐𐑰𐑐𐑩𐑤,\n·𐑢𐑺𐑨𐑟 𐑦𐑑 𐑦𐑟 𐑦𐑕𐑧𐑯𐑖𐑩𐑤, 𐑦𐑓 𐑥𐑨𐑯 𐑦𐑟 𐑯𐑪𐑑 𐑑 𐑚𐑰 𐑒𐑩𐑥𐑐𐑧𐑤𐑛 𐑑 𐑣𐑨𐑝 𐑮𐑦𐑒𐑹𐑕, 𐑨𐑟 𐑩 𐑤𐑭𐑕𐑑 𐑮𐑦𐑟𐑹𐑑, 𐑑 𐑮𐑦𐑚𐑧𐑤𐑘𐑩𐑯 𐑩𐑜𐑱𐑯𐑕𐑑 𐑑𐑦𐑮𐑩𐑯𐑦 𐑯 𐑩𐑐𐑮𐑧𐑖𐑩𐑯, 𐑞𐑨𐑑 𐑣𐑿𐑥𐑩𐑯 𐑮𐑲𐑑𐑕 𐑖𐑫𐑛 𐑚𐑰 𐑐𐑮𐑩𐑑𐑧𐑒𐑑𐑩𐑛\n            𐑚𐑲 𐑞 𐑮𐑵𐑤 𐑝 𐑤𐑷,"
+  specimen_32: "·𐑢𐑺𐑨𐑟 𐑮𐑧𐑒𐑩𐑜𐑯𐑦𐑖𐑩𐑯 𐑝 𐑞 𐑦𐑯𐑣𐑧𐑮𐑩𐑯𐑑 𐑛𐑦𐑜𐑯𐑦𐑑𐑦 𐑯 𐑝 𐑞 𐑰𐑒𐑢𐑩𐑤 𐑯 𐑦𐑯𐑱𐑤𐑾𐑯𐑩𐑚𐑩𐑤 𐑮𐑲𐑑𐑕 𐑝 𐑷𐑤 𐑥𐑧𐑥𐑚𐑼𐑟 𐑝 𐑞 𐑣𐑿𐑥𐑩𐑯 𐑓𐑨𐑥𐑦𐑤𐑦 𐑦𐑟 𐑞 𐑓𐑬𐑯𐑛𐑱𐑖𐑩𐑯 𐑝 𐑓𐑮𐑰𐑛𐑩𐑥, 𐑡𐑳𐑕𐑑𐑦𐑕 𐑯 𐑐𐑰𐑕 𐑦𐑯\n 𐑞 𐑢𐑻𐑤𐑛,"
+  specimen_21: "·𐑢𐑺𐑨𐑟 𐑮𐑧𐑒𐑩𐑜𐑯𐑦𐑖𐑩𐑯 𐑝 𐑞 𐑦𐑯𐑣𐑧𐑮𐑩𐑯𐑑 𐑛𐑦𐑜𐑯𐑦𐑑𐑦 𐑯 𐑝 𐑞 𐑰𐑒𐑢𐑩𐑤 𐑯 𐑦𐑯𐑱𐑤𐑾𐑯𐑩𐑚𐑩𐑤 𐑮𐑲𐑑𐑕 𐑝 𐑷𐑤 𐑥𐑧𐑥𐑚𐑼𐑟 𐑝 𐑞 𐑣𐑿𐑥𐑩𐑯 𐑓𐑨𐑥𐑦𐑤𐑦 𐑦𐑟 𐑞 𐑓𐑬𐑯𐑛𐑱𐑖𐑩𐑯 𐑝 𐑓𐑮𐑰𐑛𐑩𐑥, 𐑡𐑳𐑕𐑑𐑦𐑕 𐑯 𐑐𐑰𐑕 𐑦𐑯\n 𐑞 𐑢𐑻𐑤𐑛,\n·𐑢𐑺𐑨𐑟 𐑛𐑦𐑕𐑮𐑦𐑜𐑸𐑛 𐑯 𐑒𐑩𐑯𐑑𐑧𐑥𐑐𐑑 𐑓 𐑣𐑿𐑥𐑩𐑯 𐑮𐑲𐑑𐑕 𐑣𐑨𐑝 𐑮𐑦𐑟𐑳𐑤𐑑𐑩𐑛 𐑦𐑯 𐑚𐑸𐑚𐑼𐑩𐑕 𐑨𐑒𐑑𐑕 𐑢𐑦𐑗 𐑣𐑨𐑝 𐑬𐑑𐑮𐑱𐑡𐑛 𐑞 𐑒𐑪𐑯𐑖𐑩𐑯𐑕 𐑝 𐑥𐑨𐑯𐑒𐑲𐑯𐑛, 𐑯 𐑞 𐑨𐑛𐑝𐑧𐑯𐑑 𐑝 𐑩 𐑢𐑻𐑤𐑛 𐑦𐑯 𐑢𐑦𐑗 𐑣𐑿𐑥𐑩𐑯 𐑚𐑰𐑦𐑙𐑟\n 𐑖𐑨𐑤 𐑦𐑯𐑡𐑶 𐑓𐑮𐑰𐑛𐑩𐑥 𐑝 𐑕𐑐𐑰𐑗 𐑯 𐑚𐑦𐑤𐑰𐑓 𐑯 𐑓𐑮𐑰𐑛𐑩𐑥 𐑓𐑮𐑪𐑥 𐑓𐑽 𐑯 𐑢𐑪𐑯𐑑 𐑣𐑨𐑟 𐑚𐑰𐑯 𐑐𐑮𐑴𐑒𐑤𐑱𐑥𐑛 𐑨𐑟 𐑞 𐑣𐑲𐑩𐑕𐑑 𐑨𐑕𐑐𐑼𐑱𐑖𐑩𐑯 𐑝 𐑞 𐑒𐑪𐑥𐑩𐑯 𐑐𐑰𐑐𐑩𐑤,"
+  specimen_16: "·𐑢𐑺𐑨𐑟 𐑮𐑧𐑒𐑩𐑜𐑯𐑦𐑖𐑩𐑯 𐑝 𐑞 𐑦𐑯𐑣𐑧𐑮𐑩𐑯𐑑 𐑛𐑦𐑜𐑯𐑦𐑑𐑦 𐑯 𐑝 𐑞 𐑰𐑒𐑢𐑩𐑤 𐑯 𐑦𐑯𐑱𐑤𐑾𐑯𐑩𐑚𐑩𐑤 𐑮𐑲𐑑𐑕 𐑝 𐑷𐑤 𐑥𐑧𐑥𐑚𐑼𐑟 𐑝 𐑞 𐑣𐑿𐑥𐑩𐑯 𐑓𐑨𐑥𐑦𐑤𐑦 𐑦𐑟 𐑞 𐑓𐑬𐑯𐑛𐑱𐑖𐑩𐑯 𐑝 𐑓𐑮𐑰𐑛𐑩𐑥, 𐑡𐑳𐑕𐑑𐑦𐑕 𐑯 𐑐𐑰𐑕 𐑦𐑯\n 𐑞 𐑢𐑻𐑤𐑛,\n·𐑢𐑺𐑨𐑟 𐑛𐑦𐑕𐑮𐑦𐑜𐑸𐑛 𐑯 𐑒𐑩𐑯𐑑𐑧𐑥𐑐𐑑 𐑓 𐑣𐑿𐑥𐑩𐑯 𐑮𐑲𐑑𐑕 𐑣𐑨𐑝 𐑮𐑦𐑟𐑳𐑤𐑑𐑩𐑛 𐑦𐑯 𐑚𐑸𐑚𐑼𐑩𐑕 𐑨𐑒𐑑𐑕 𐑢𐑦𐑗 𐑣𐑨𐑝 𐑬𐑑𐑮𐑱𐑡𐑛 𐑞 𐑒𐑪𐑯𐑖𐑩𐑯𐑕 𐑝 𐑥𐑨𐑯𐑒𐑲𐑯𐑛, 𐑯 𐑞 𐑨𐑛𐑝𐑧𐑯𐑑 𐑝 𐑩 𐑢𐑻𐑤𐑛 𐑦𐑯 𐑢𐑦𐑗 𐑣𐑿𐑥𐑩𐑯 𐑚𐑰𐑦𐑙𐑟\n 𐑖𐑨𐑤 𐑦𐑯𐑡𐑶 𐑓𐑮𐑰𐑛𐑩𐑥 𐑝 𐑕𐑐𐑰𐑗 𐑯 𐑚𐑦𐑤𐑰𐑓 𐑯 𐑓𐑮𐑰𐑛𐑩𐑥 𐑓𐑮𐑪𐑥 𐑓𐑽 𐑯 𐑢𐑪𐑯𐑑 𐑣𐑨𐑟 𐑚𐑰𐑯 𐑐𐑮𐑴𐑒𐑤𐑱𐑥𐑛 𐑨𐑟 𐑞 𐑣𐑲𐑩𐑕𐑑 𐑨𐑕𐑐𐑼𐑱𐑖𐑩𐑯 𐑝 𐑞 𐑒𐑪𐑥𐑩𐑯 𐑐𐑰𐑐𐑩𐑤,\n·𐑢𐑺𐑨𐑟 𐑦𐑑 𐑦𐑟 𐑦𐑕𐑧𐑯𐑖𐑩𐑤, 𐑦𐑓 𐑥𐑨𐑯 𐑦𐑟 𐑯𐑪𐑑 𐑑 𐑚𐑰 𐑒𐑩𐑥𐑐𐑧𐑤𐑛 𐑑 𐑣𐑨𐑝 𐑮𐑦𐑒𐑹𐑕, 𐑨𐑟 𐑩 𐑤𐑭𐑕𐑑 𐑮𐑦𐑟𐑹𐑑, 𐑑 𐑮𐑦𐑚𐑧𐑤𐑘𐑩𐑯 𐑩𐑜𐑱𐑯𐑕𐑑 𐑑𐑦𐑮𐑩𐑯𐑦 𐑯 𐑩𐑐𐑮𐑧𐑖𐑩𐑯, 𐑞𐑨𐑑 𐑣𐑿𐑥𐑩𐑯 𐑮𐑲𐑑𐑕 𐑖𐑫𐑛 𐑚𐑰 𐑐𐑮𐑩𐑑𐑧𐑒𐑑𐑩𐑛\n 𐑚𐑲 𐑞 𐑮𐑵𐑤 𐑝 𐑤𐑷,"
 }
 historical: true
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/eo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/eo_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Esperanto"
 population: 301
 region: "SM"
 exemplar_chars {
   base: "a b c ĉ d e f g ĝ h ĥ i j ĵ k l m n o p r s ŝ t u ŭ v z"
   auxiliary: "q w x y"
   marks: "◌̂ ◌̆"
-  numerals: "  , % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } /"
+  numerals: ", % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } /"
   index: "A B C Ĉ D E F G Ĝ H Ĥ I J Ĵ K L M N O P R S Ŝ T U Ŭ V Z"
 }
 sample_text {
   masthead_full: "ĈĉIi"
   masthead_partial: "Uu"
   styles: "Pro tio, ke agnosko de la esenca digno kaj"
   tester: "Pro tio, ke malagnosko kaj malestimo de la homaj rajtoj rezultigis"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/es_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/es_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 region: "US"
 region: "UY"
 region: "VE"
 exemplar_chars {
   base: "a á b c d e é f g h i í j k l m n ñ o ó p q r s t u ú ü v w x y z"
   auxiliary: "ª à ă â å ä ã ā æ ç è ĕ ê ë ē ì ĭ î ï ī º ò ŏ ô ö ø ō œ ù ŭ û ū ý ÿ"
   marks: "◌́ ◌̃ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ¡ ? ¿ . … \' ‘ ’ \" “ ” « » ( ) [ ] § @ * / \\ & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ¡ ? ¿ . … \' ‘ ’ \" “ ” « » ( ) [ ] @ * / \\ & #"
   index: "A B C D E F G H I J K L M N Ñ O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtOo"
   masthead_partial: "Dd"
   styles: "Considerando que la libertad, la justicia"
   tester: "Considerando que el desconocimiento y el menosprecio de los derechos"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ese_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ese_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/et_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/et_Latn.textproto`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 878449
 region: "EE"
 region: "FI"
 exemplar_chars {
   base: "a b c d e f g h i j k l m n o p q r s š z ž t u v w õ ä ö ü x y"
   auxiliary: "á à â å ã ā æ ç é è ê ë ē í ì î ï ī ñ ó ò ŏ ô ø ō œ ú ù û ū"
   marks: "◌̃ ◌̈ ◌̌"
-  numerals: "  , % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ – , ; : ! ? . “ „ ( ) [ ] { } @"
+  numerals: ", % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . “ „ ( ) [ ] { } @"
   index: "A B C D E F G H I J K L M N O P Q R S Š Z Ž T U V W Õ Ä Ö Ü X Y"
 }
 sample_text {
   masthead_full: "KkÕõ"
   masthead_partial: "Ii"
   styles: "Pidades silmas, et inimkonna kõigi liikmete"
   tester: "pidades silmas, et inimõiguste põlastamine ja hülgamine on viinud"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ett_Ital.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ett_Ital.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/eu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/eu_Latn.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 1088518
 region: "ES"
 region: "FR"
 exemplar_chars {
   base: "a b c ç d e f g h i j k l m n ñ o p q r s t u v w x y z"
   auxiliary: "á à ă â å ä ã ā æ é è ĕ ê ë ē í ì ĭ î ï ī ó ò ŏ ô ö ø ō œ ú ù ŭ û ü ū ÿ"
   marks: "◌̃ ◌̈"
-  numerals: ", . % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: ", . % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "GgIi"
   masthead_partial: "Zz"
   styles: "Kontuan izanik munduko askatasuna, justizia"
   tester: "Kontuan izanik giza eskubideak ez ezagutzearen eta gutxiestearen"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/eve_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/eve_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/evn_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/evn_Cyrl.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 exemplar_chars {
   base: "А Б В Г Д Е Ж З И Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ъ Ы Ь Э Ю Я Ё Ӈ Ә А̄ Е̄ Ә̄ О̄ Ы̄ а б в г д е ж з и й к л м н о п р с т у ф х ц ч ш щ ъ ы ь э ю я ё ӈ ә а̄ е̄ ә̄ о̄ ы̄"
   marks: "◌̄ ◌̆ ◌̈"
 }
 sample_text {
   masthead_full: "УуПп"
   masthead_partial: "Кк"
-  styles: "Эрэвэр ичэтчэнэ,  упкатту илэлду са̄рӣча̄н бисин,"
+  styles: "Эрэвэр ичэтчэнэ, упкатту илэлду са̄рӣча̄н бисин,"
   tester: "эрэвэр ичэтчэнэ, сэлдэн, алтыссадян ичэтмэин илэ тэденду эмэврэ"
   poster_sm: "эрэвэр ичэтчэнэ,"
   poster_md: "Генеральный"
   poster_lg: "Упкат"
   specimen_48: "Упкат илэл ты̄нмукирди, урэ̄лди мэ̄нңи са̄рича̄ди балдыдяра. Нуңартын"
   specimen_36: "Илэтыкин, о̄кин нуңанман сэлэ̄деңэ̄тын, тэдевэ гэлэ̄ктэлдеңэ̄н, нуңанңи о̄мачин тэдэмэт, тоңнот судту ичэвкэ̄нмэчин."
   specimen_32: "Илэтыкин дялдана, һалдяна, бугатки мургунэ тэдет бивки; тар тэденди илэ һ уңту бугатки мургунэ дюгэлдывдеңэ̄; мэ̄нэкэ̄нгу, гелнунгу илэлнун, делӯмнэкэ̄ нңу, тоңнотку бугатки мургумчэ̄н."
   specimen_21: "Илэтыкин тэдэт мэ̄нңи дялдатчэриви, гӯннэтынми бивки; тар тэден илэду бӯ дерэн гэлэ̄ктэдеми, гадями, са̄вкандями улгуври, дялдалви авадытыкирди о̄наяди ӣдувэл биденэ.\nИлэтыкин, о̄н общества илэн, социальнай обеспечениевэ гамча̄, тарит илэ са̄рича̄ нин экономическайду, социальнайду, культурнайдуда һанилду гэлэ̄вдяри бимчэ̄. Международнай сотрудничество бэлэгэдин, государствотыкин дёкиндядин."
-  specimen_16: "Илэтыкин дэрумкичэ̄нма тэдет бимчэ̄, иргэчивэ  камничивунма һавады тырганӣ яда, тамавдяри дэрумкичэ̄нмэдэ̄.\nИлэтыкин социальнай, международнайда итылва тэдет бимчэ̄, туги о̄дяна илэ тэден, ты̄нмукитын эр Декларация дукувнал о̄мачир.\nЭкунмал эр Декларацияду эвки эсин тэдет таңивра, дялданэ – он эмадувал государстводу, умукэнну илэду һавалмигу, омигу таргачир омачилва, эмал илэл тэделвэтын, тынмукилвэтын ачинңими, эр Декларация дукувналватын.\nЭрэвэр ичэтчэнэ,  упкатту илэлду са̄рӣча̄н бисин,  нуңарңитын тэгэ̄̄р ты нмукитын, тэдетын, аяра̄лдынтын;\nэрэвэр ичэтчэнэ, гэлэвкэ̄, илэ тэдевэтын законит дысутчэдэ̄̄н, илэ эдэ̄н илми һ уски болгӣчанду, кэсэгивунду;"
+  specimen_16: "Илэтыкин дэрумкичэ̄нма тэдет бимчэ̄, иргэчивэ камничивунма һавады тырганӣ яда, тамавдяри дэрумкичэ̄нмэдэ̄.\nИлэтыкин социальнай, международнайда итылва тэдет бимчэ̄, туги о̄дяна илэ тэден, ты̄нмукитын эр Декларация дукувнал о̄мачир.\nЭкунмал эр Декларацияду эвки эсин тэдет таңивра, дялданэ – он эмадувал государстводу, умукэнну илэду һавалмигу, омигу таргачир омачилва, эмал илэл тэделвэтын, тынмукилвэтын ачинңими, эр Декларация дукувналватын.\nЭрэвэр ичэтчэнэ, упкатту илэлду са̄рӣча̄н бисин, нуңарңитын тэгэ̄̄р ты нмукитын, тэдетын, аяра̄лдынтын;\nэрэвэр ичэтчэнэ, гэлэвкэ̄, илэ тэдевэтын законит дысутчэдэ̄̄н, илэ эдэ̄н илми һ уски болгӣчанду, кэсэгивунду;"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ewo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ewo_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 autonym: "Ewondo"
 population: 860095
 region: "CM"
 exemplar_chars {
   base: "a A á Á à À â Â ǎ Ǎ b B d D {dz} {DZ} e E é É è È ê Ê ě Ě ə Ə {ə́} {Ə́} {ə̀} {Ə̀} {ə̂} {Ə̂} {ə̌} {Ə̌} ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̀} {Ɛ̀} {ɛ̂} {Ɛ̂} {ɛ̌} {Ɛ̌} f F g G h H i I í Í ì Ì î Î ǐ Ǐ k K {kp} {KP} l L m M n N ń Ń ǹ Ǹ {ng} {NG} {nk} {NK} ŋ Ŋ o O ó Ó ò Ò ô Ô ǒ Ǒ ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̀} {Ɔ̀} {ɔ̂} {Ɔ̂} {ɔ̌} {Ɔ̌} p P r R s S t T {ts} {TS} u U ú Ú ù Ù û Û ǔ Ǔ v V w W y Y z Z"
   auxiliary: "c C j J q Q x X"
   marks: "◌̀ ◌́ ◌̂ ◌̌"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B D E Ə Ɛ F G H I K L M N Ŋ O Ɔ P R S T U V W Y Z"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ext_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ext_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fa_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fa_Arab.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 region: "OM"
 region: "PK"
 region: "QA"
 region: "TJ"
 exemplar_chars {
   base: "ً ٍ ٌ ّ ٔ آ ا ء أ ؤ ئ ب پ ت ث ج چ ح خ د ذ ر ز ژ س ش ص ض ط ظ ع غ ف ق ک گ ل م ن و ه ة ی"
   auxiliary: "ـ‌‍‎‏ َ ِ ُ ْ ٖ ٰ إ ك ى ي"
-  numerals: "‎ , ٫ ٬ . % ٪ ‰ ؉ + − 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
-  punctuation: "- ‐ ‑ ، ٫ ٬ ؛ : ! ؟ . … ‹ › « » ( ) [ ] * / \\"
+  numerals: "‎ , ٫ ٬ . % ٪ ؉ + − 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
+  punctuation: "- ، ٫ ٬ ؛ : ! ؟ . … ‹ › « » ( ) [ ] * / \\"
   index: "آ ا ب پ ت ث ج چ ح خ د ذ ر ز ژ س ش ص ض ط ظ ع غ ف ق ک گ ل م ن و ه ی"
 }
 sample_text {
   masthead_full: "تماف"
   masthead_partial: "رد"
   styles: "از آنجا که شناسائی حیثیت ذاتی کلیهٔ اعضای"
   tester: "از آنجا که عدم شناسائی و تحقیر حقوق بشر منتهی به اعمال وحشیانه‌ای"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ff_Adlm.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ff_Adlm.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 region: "NG"
 region: "SL"
 region: "SN"
 exemplar_chars {
   base: "𞥄𞥅𞥆 𞤢 𞤣 𞤤 𞤥 𞤦 𞤧 𞤨 𞤩 𞤪 𞤫 𞤬 𞤭 𞤮 𞤯 𞤰 𞤱 𞤲 𞤳 𞤴 𞤵 𞤶 𞤷 𞤸 𞤹 𞤺 𞤻 𞤼 𞤽 𞥋"
   auxiliary: "𞤾 𞤿 𞥀 𞥁 𞥂 𞥃"
   numerals: "𞥐 𞥑 𞥒 𞥓 𞥔 𞥕 𞥖 𞥗 𞥘 𞥙"
-  punctuation: "- ‑ 𞥞 𞥟 . % ‰"
+  punctuation: "- 𞥞 𞥟 . % "
   index: "𞤀 𞤛"
 }
 sample_text {
   masthead_full: "𞤋𞤭𞤐𞤲"
   masthead_partial: "𞤀𞤢"
   styles: "𞤚𞤵𞥅𞤺𞤢𞥄𞤣𞤫 𞤱𞤮𞤲𞤣𞤫 𞤸𞤫𞤬𞤼𞤭𞤲𞤺𞤮𞤤 𞤸𞤮𞤪𞤥𞤢 𞤳𞤢𞤤𞤢 𞤲𞤫𞤯𞥆𞤮 𞤫"
   tester: "𞤚𞤵𞥅𞤺𞤢𞥄𞤣𞤫 𞤱𞤮𞤲𞤣𞤫 𞤱𞤢𞥄𞤧𞤵𞤺𞤮𞤤 𞤸𞤫𞤬𞤼𞤭𞤲𞤣𞤫 𞤳𞤢𞤻𞤵𞤲 𞤫 𞤧𞤢𞤤𞤢𞤺𞤮𞤤 𞤼𞤮𞤼𞥆𞤵𞤣𞤫 𞤯𞤫𞤲 𞤶𞤮𞤶𞥆𞤢𞤲𞤯𞤫"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ff_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ff_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 region: "NG"
 region: "SL"
 region: "SN"
 exemplar_chars {
   base: "a b ɓ c d ɗ e f g h i j k l m n ñ ŋ o p r s t u w y ƴ"
   auxiliary: "q v x z"
   marks: "◌̃"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B Ɓ C D Ɗ E F G H I J K L M N Ñ Ŋ O P R S T U W Y Ƴ"
 }
 sample_text {
   masthead_full: "NnEe"
   masthead_partial: "Dd"
   styles: "TAWEEDE NDELO HETTAARE, NUNDHAL E BHUTTU ADUNAAN"
   tester: "TAWEEDE, MADDYEEDE E BIKKHTAARE HANDANDHI NEDDHO WONUNO SABU AAWASEEDYI"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fi_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "FI"
 region: "RU"
 region: "SE"
 exemplar_chars {
   base: "a b c d e f g h i j k l m n o p q r s š t u v w x y z ž å ä ö"
   auxiliary: "á à ă â ã ą ā ć č ċ ç ď ð đ é è ê ě ë ė ę ē ğ ǧ ģ ǥ ȟ ħ í î ï İ į ī ı ǩ ķ ĺ ľ ļ ł ń ň ñ ņ ŋ ó ò ô ő õ œ ŕ ř ś ŝ ş ș ß ť ţ ț ŧ ú ù û ů ű ų ū ý ÿ ü ź ż ʒ ǯ þ æ ø"
   marks: "◌̈ ◌̊ ◌̃ ◌̌"
-  numerals: "  , % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – , ; : ! ? . … ’ ” » ( ) [ ] § @ * / \\ & #"
+  numerals: ", % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … ’ ” » ( ) [ ] @ * / \\ & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z Å Ä Ö"
 }
 sample_text {
   masthead_full: "KkAa"
   masthead_partial: "Ii"
   styles: "Kun ihmiskunnan kaikkien jäsenten luonnollisen"
   tester: "kun ihmisoikeuksia on väheksytty tai ne on jätetty huomiota vaille,"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fil_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fil_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 66905683
 region: "PH"
 region: "US"
 exemplar_chars {
   base: "a b c d e f g h i j k l m n ñ {ng} o p q r s t u v w x y z"
   auxiliary: "á à â é è ê í ì î ó ò ô ú ù û"
   marks: "◌̃"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § * / & # ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] * / & #"
   index: "A B C D E F G H I J K L M N Ñ {Ng} O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaNn"
   masthead_partial: "Gg"
   styles: "Ang lahat ng tao\'y isinilang na malaya at"
   tester: "Ang lahat ng tao\'y isinilang na malaya at pantay-pantay sa karangalan"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fil_Tglg.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fil_Tglg.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fj_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fkv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fkv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fo_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 71350
 region: "DK"
 region: "FO"
 exemplar_chars {
   base: "a á b d ð e f g h i í j k l m n o ó p r s t u ú v y ý æ ø"
   auxiliary: "c q w x z"
   marks: "◌́ ◌̊"
-  numerals: ", . % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ′ ″"
+  numerals: ", . % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A Á B C D Ð E F G H I Í J K L M N O Ó P Q R S T U Ú V W X Y Ý Z Æ Ø"
 }
 sample_text {
   masthead_full: "ØøLl"
   masthead_partial: "Mm"
   styles: "Tað verður at viðurkenna, at menniskjuni er"
   tester: "Har sum mannarættindini hava verið fyri vanbýti og vanvirðing,"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fon_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fon_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fr_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 region: "VU"
 region: "WF"
 region: "YT"
 exemplar_chars {
   base: "a à â æ b c ç d e é è ê ë f g h i î ï j k l m n o ô œ p q r s t u ù û ü v w x y ÿ z"
   auxiliary: "á å ä ã ā ć ē í ì ī ĳ ñ ó ò ö õ ø ř š ſ ß ú ǔ"
   marks: "◌̀ ◌́ ◌̂ ◌̈ ◌̧"
-  numerals: "  - ‑ , . % ‰ + − 0 1 2 ² 3 ³ 4 5 6 7 8 9 ᵈ ᵉ ʳ ˢ"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … ’ \" “ ” « » ( ) [ ] § @ * / & # † ‡"
+  numerals: "- , . % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … ’ \" “ ” « » ( ) [ ] @ * / & # "
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtOo"
   masthead_partial: "Uu"
   styles: "Considérant que la reconnaissance de la dignité"
   tester: "Considérant que la méconnaissance et le mépris des droits de"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fro_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/frp_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/frp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/frr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/frr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fuc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fuc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fuf_Adlm.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fuf_Adlm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fuf_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fuf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fur_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fur_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Furlan"
 population: 37441
 region: "IT"
 exemplar_chars {
   base: "a à â b c ç d e è ê f g h i ì î j k l m n o ò ô p q r s t u ù û v w x y z"
   auxiliary: "å č é ë ğ ï ñ ó š ü"
   marks: "◌̀ ◌̂ ◌̧"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C Ç D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "DdUu"
   masthead_partial: "Cc"
   styles: "Tignût cont che il ricognossi la dignitât"
   tester: "Tignût cont che il dineâ e il spreseâ i derits dal om a an puartât"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fuv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fuv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fvr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fvr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/fy_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/fy_Latn.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Frysk"
 population: 743057
 region: "NL"
 exemplar_chars {
   base: "a á à â ä b c d e é è ê ë f g h i í ï y ý j k l m n o ó ô ö p r s t u ú û ü v w z"
   auxiliary: "æ ò ù"
   marks: "◌́ ◌̂ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P R S T U V W X Z"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Ee"
   styles: "Yn betinken nommen dat it erkennen fan de"
   tester: "Yn betinken nommen dat it oan \'e kant skowen en lytsachtsjen fan"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ga_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ga_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 1155943
 region: "GB"
 region: "IE"
 exemplar_chars {
   base: "a á b c d e é f g h i í l m n o ó p r s t u ú"
   auxiliary: "å ḃ ċ ḋ ḟ ġ j k ṁ ṗ q ṡ ṫ v w x y z"
   marks: "◌́"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "SsAa"
   masthead_partial: "Oo"
   styles: "De Bhrí gurb é aithint dínte dúchais agus"
   tester: "De Bhrí gur thionscain a neamhaird agus an mí-mheas ar chearta"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gaa_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gaa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gag_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gag_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gag_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gag_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gan_Hans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gan_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gbz_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gbz_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gcf_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gcf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gcr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gcr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gd_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gd_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Gàidhlig"
 population: 65103
 region: "GB"
 exemplar_chars {
   base: "a à b c d e è f g h i ì l m n o ò p r s t u ù"
   auxiliary: "á ă â å ä ã ā æ ċ ç ḋ é ĕ ê ë ē ḟ ġ í ĭ î ï ī ı j k ł ṁ ñ ó ŏ ô ö ø ō œ ṗ q ṡ ş ș ṫ ú ŭ û ü ū v w x y ÿ z"
   marks: "◌̀ ◌́"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ¡ ? . … · \' ‘ ’ \" “ ” ( ) [ ] { } § ¶ @ * / & ⁊ # % † ‡ ‧ ° © ® ™"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ¡ ? . … · \' ‘ ’ \" “ ” ( ) [ ] { } ¶ @ * / & ⁊ # % ‧ ° © ® ™"
   index: "A B C D E F G H I L M N O P R S T U"
 }
 sample_text {
   masthead_full: "TtHh"
   masthead_partial: "Aa"
   styles: "Do bhrìgh \'s gu bheil e air aideachadh gu"
   tester: "Do bhrìgh \'s gun do dh\' adhbharaich a bhith a\' cur còirichean dhaoine"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gem_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gem_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gez_Ethi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gez_Ethi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/giw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/giw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gjn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gjn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gju_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gju_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gkp_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gkp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gl_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 3515529
 region: "ES"
 region: "PT"
 exemplar_chars {
   base: "a á b c d e é f g h i í ï j k l m n ñ o ó p q r s t u ú ü v w x y z"
   auxiliary: "ª à ă â å ä ã ā æ ɑ ç è ĕ ê ë ē ì ĭ î ī º ò ŏ ô ö õ ø ō œ ù ŭ û ū"
   marks: "◌́ ◌̃ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ¡ ? ¿ . … \' ‘ ’ \" “ ” « » ( ) [ ] § @ * / \\ & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ¡ ? ¿ . … \' ‘ ’ \" “ ” « » ( ) [ ] @ * / \\ & #"
   index: "A B C D E F G H I J K L M N Ñ O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtÓó"
   masthead_partial: "Dd"
   styles: "A liberdade, a xustiza e a paz no mundo teñen"
   tester: "O descoñecemento e o menosprezo dos dereitos da persoa orixinaron"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gld_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gld_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gmh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gmh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gmy_Linb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gmy_Linb.textproto`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 language: "gmy"
 script: "Linb"
 name: "Mycenaean Greek"
 sample_text {
   masthead_full: "𐀴𐀪𐀡𐀆"
   masthead_partial: "𐁁𐀐"
   styles: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜"
-  tester: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵"
+  tester: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵"
   poster_sm: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐"
-  poster_md: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 "
+  poster_md: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 "
   poster_lg: "\\𐀐𐀩𐁀"
   specimen_48: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀"
-  specimen_36: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇"
-  specimen_32: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇"
-  specimen_21: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇"
-  specimen_16: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/   𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [   𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇"
+  specimen_36: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇"
+  specimen_32: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇"
+  specimen_21: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇"
+  specimen_16: "𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇\n𐀴𐀪𐀡𐀆𐄀𐁁𐀐𐀄𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐 𐃠 𐄈 𐀴𐀪𐀡𐄀𐀁𐀕𐄀𐀡𐀆𐄀𐀃𐀺𐀸 𐃠 𐄇 𐀴𐀪𐀡𐄀𐀐𐀩𐀯𐀍𐄀𐀸𐀐𐄀𐀀𐀢𐄀𐀐𐀏𐀄𐀕𐀜[ \\𐀐𐀩𐁀 𐃠[/ 𐀤𐀵 𐃢 𐄉 𐀇𐀞𐄀𐀕𐀿𐀁𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 𐀇𐀞𐀁𐄀𐀕𐀿𐀁𐄀𐀴𐀪𐀃𐀸𐀁 𐃡 𐄈 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀤𐀵𐀫𐀸 𐃡 𐄇 [ 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀴𐀪𐀍𐀸 𐃡 𐄇 𐀇𐀞𐄀𐀕𐀹𐀍𐄀𐀀𐀜𐀸 𐃡 𐄇"
 }
 historical: true
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/goh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/goh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gom_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gom_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/got_Goth.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/got_Goth.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/got_Runr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/got_Runr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/grc_Cprt.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/grc_Cprt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/grc_Grek.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/grc_Grek.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/grc_Linb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/grc_Linb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gsw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gsw_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 region: "DE"
 region: "FR"
 region: "LI"
 exemplar_chars {
   base: "a ä b c d e f g h i j k l m n o ö p q r s t u ü v w x y z"
   auxiliary: "á à ă â å ā æ ç é è ĕ ê ë ē í ì ĭ î ï ī ñ ó ò ŏ ô ø ō œ ú ù ŭ û ū ÿ"
   marks: "◌̈"
-  numerals: ". ’ % ‰ + − 0 1 2 3 4 5 6 7 8 9"
+  numerals: ". ’ % + − 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "ÀàLl"
   masthead_partial: "Ii"
   styles: "Wil d’Fréiheit, d’Gerachtichkeit ùn de Frìdde"
   tester: "Wil ’s do, wo mr d’Menscherachte nìt gekannt ùn nìt reschpektìert"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gu_Gujr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gu_Gujr.textproto`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 59679028
 region: "IN"
 region: "KE"
 exemplar_chars {
   base: "઼ ૐ ં ઁ ઃ અ આ ઇ ઈ ઉ ઊ ઋ ૠ ઍ એ ઐ ઑ ઓ ઔ ક ખ ગ ઘ ઙ ચ છ જ ઝ ઞ ટ ઠ ડ ઢ ણ ત થ દ ધ ન પ ફ બ ભ મ ય ર લ વ શ ષ સ હ ળ ઽ ા િ ી ુ ૂ ૃ ૄ ૅ ે ૈ ૉ ો ૌ ્"
   auxiliary: "‌‍ ૰"
   marks: "◌ં ◌ઃ ◌ા ◌િ ◌ી ◌ુ ◌ૂ ◌ૃ ◌ે ◌ૈ ◌ો ◌ૌ ◌્"
-  numerals: "- ‑ , . % ‰ + 0૦ 1૧ 2૨ 3૩ 4૪ 5૫ 6૬ 7૭ 8૮ 9૯"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0૦ 1૧ 2૨ 3૩ 4૪ 5૫ 6૬ 7૭ 8૮ 9૯"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "અ {અં} {અઃ} આ ઇ ઈ ઉ ઊ ઋ ઍ એ ઐ ઑ ઓ ઔ ક {ક્ષ} ખ ગ ઘ ઙ ચ છ જ {જ્ઞ} ઝ ઞ ટ ઠ ડ ઢ ણ ત {ત્ર} થ દ ધ ન પ ફ બ ભ મ ય ર લ વ શ ષ સ હ ળ"
 }
 sample_text {
   masthead_full: "પરતષ"
   masthead_partial: "ઠઅ"
   styles: "કેમ કે માનવકુટુંબના દરેક સભ્યની પરંપરાપ્રાપ્ત પ્રતિષ્ઠાને અને"
   tester: "કેમ કે માનવ અધિકારોની ઉપેક્ષા અને અપમાન કરવાથી એવાં જંગલી કત્યો પરિણમ્યાં છે કે જેણે માનવજાતના"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/guc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/guc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/guu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/guu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gv_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Manx"
 autonym: "Gaelg"
 population: 1719
 region: "IM"
 exemplar_chars {
   base: "a b c ç d e f g h i j k l m n o p q r s t u v w x y z"
   marks: "◌̧"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtAa"
   masthead_partial: "Dd"
   styles: "Fakin dy nee cur enney er ooashley beayn"
   tester: "Fakin dy vel mee-ooashley da cairyssyn deiney as craid jeu er"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/gyr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/gyr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ha_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ha_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 region: "GH"
 region: "NE"
 region: "NG"
 exemplar_chars {
   base: "a A b B ɓ Ɓ c C d D ɗ Ɗ e E f F g G h H i I j J k K ƙ Ƙ l L m M n N o O r R s S {sh} {SH} t T {ts} {TS} u U w W y Y ƴ Ƴ z Z ʼ"
   auxiliary: "á Á à À â Â é É è È ê Ê í Í ì Ì î Î ó Ó ò Ò ô Ô p P q Q {r̃} {R̃} ú Ú ù Ù û Û v V x X"
   marks: "◌̃ ◌̀ ◌́ ◌̂"
-  punctuation: "- ‑ , ; : ! ? . \' ‘ ’ \" “ ” ( ) [ ] { } ′ ″"
+  punctuation: "- , ; : ! ? . \' ‘ ’ \" “ ” ( ) [ ] { }"
   index: "A B Ɓ C D Ɗ E F G H I J K Ƙ L M N O R S T U W Y Ƴ Z"
 }
 sample_text {
   masthead_full: "DdUu"
   masthead_partial: "Kk"
   styles: "Duk ‘yan’adan ana haihuwarsu ne a matsayin"
   tester: "Duk ‘yan’adan ana haihuwarsu ne a matsayin ‘yantattun ‘ya’ya, kuma"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hak_Hans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hak_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/haw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/haw_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "’Olelo Hawai’i"
 population: 29604
 region: "US"
 exemplar_chars {
   base: "a ā e ē i ī o ō u ū h k l m n p w ʻ"
   auxiliary: "b c d f g j q r s t v x y z"
   marks: "◌̄"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A E I O U B C D F G H J K L M N P Q R S T V W ʻ X Y Z"
 }
 sample_text {
   masthead_full: "HhĀā"
   masthead_partial: "Nn"
   styles: "‘Oiai, ‘o ka ho’omaopop ‘ana i ka hanohano, a me"
   tester: "‘Oiai, ‘o ka hehikū a me ka ho’owahāwahā i ka pono kīvila o ke kanaka"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/he_Hebr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/he_Hebr.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "עברית"
 population: 8675480
 region: "IL"
 exemplar_chars {
   base: "א ב ג ד ה ו ז ח ט י כ ך ל מ ם נ ן ס ע פ ף צ ץ ק ר ש ת"
   auxiliary: "ֽׄ‎‏ ְ ֱ ֲ ֳ ִ ֵ ֶ ַ ָ ֹ ֻ ׂ ׁ ּ ֿ ״"
   marks: "◌ְ ◌ֱ ◌ֲ ◌ֳ ◌ִ ◌ֵ ◌ֶ ◌ַ ◌ָ ◌ֹ ◌ֻ ◌ּ ◌ׁ ◌ׂ"
-  numerals: "‎ - ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . ׳ \' \" ( ) [ ] / ״ ־"
+  numerals: "‎ - , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . ׳ \' \" ( ) [ ] / ״ ־"
   index: "א ב ג ד ה ו ז ח ט י כ ל מ נ ס ע פ צ ק ר ש ת"
 }
 sample_text {
   masthead_full: "כלבנ"
   masthead_partial: "יא"
   styles: "כל בני אדם נולדו בני חורין ושווים בערכם ובזכויותיהם"
   tester: "כל אדם זכאי לזכויות ולחרויות שנקבעו בהכרזש זו ללא הפליה כלשהיא"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hea_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hea_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hi_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hi_Deva.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 region: "NP"
 region: "UG"
 region: "ZA"
 exemplar_chars {
   base: "़ ॐ ं ँ ः अ आ इ ई उ ऊ ऋ ऌ ऍ ए ऐ ऑ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल ळ व श ष स ह ऽ ा ि ी ु ू ृ ॄ ॅ े ै ॉ ो ौ ्"
   auxiliary: "‌‍"
   marks: "◌ँ ◌ं ◌ः ◌़ ◌ा ◌ि ◌ी ◌ु ◌ू ◌ृ ◌े ◌ै ◌ो ◌ौ ◌्"
-  numerals: "- ‑ , . % ‰ + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
-  punctuation: "- ‑ , ; : ! ? . ‘ ’ “ ” ( ) [ ] { } ॰"
+  numerals: "- , . % + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
+  punctuation: "- , ; : ! ? . ‘ ’ “ ” ( ) [ ] { } ॰"
   index: "अ आ इ ई उ ऊ ऋ ए ऐ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल व श ष स ह"
 }
 sample_text {
   masthead_full: "सभमन"
   masthead_partial: "षय"
   styles: "चूंकि मानव परिवार के सभी सदस्यों के जन्मजात गौरव और समान"
   tester: "चूंकि मानव अधिकारों के प्रति उपेक्षा और घृणा के फलस्वरूप ही ऐसे बर्बर कार्य हुए जिनसे मनुष्य"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hil_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hil_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hit_Xsux.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hit_Xsux.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hlt_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hlt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hlu_Hluw.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hlu_Hluw.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hmd_Plrd.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hmd_Plrd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hmn_Hmng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hmn_Hmng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hmn_Hmnp.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hmn_Hmnp.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hmn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hmn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hms_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hms_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hna_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hna_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hne_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hne_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hni_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hni_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hnj_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hnj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hns_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hns_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hoc_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hoc_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hsb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hsb_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Hornjoserbšćina"
 population: 12825
 region: "DE"
 exemplar_chars {
   base: "a b c č ć d {dź} e ě f g h {ch} i j k ł l m n ń o ó p q r ř s š t u v w x y z ž"
   auxiliary: "á à ă â å ä ã ą ā æ ç ď đ é è ĕ ê ë ė ę ē ğ í ì ĭ î ï İ ī ı ĺ ľ ň ñ ò ŏ ô ö ő ø ō œ ŕ ś ş ß ť ú ù ŭ û ů ü ű ū ý ÿ ż ź"
   marks: "◌́ ◌̌"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
   index: "A B C Č Ć D {DŹ} E F G H {CH} I J K Ł L M N O P Q R S Š T U V W X Y Z Ž"
 }
 sample_text {
   masthead_full: "WwŠš"
   masthead_partial: "Ii"
   styles: "Dokelž twori płipóznaće wšěm čłonam čłowjeskeje"
   tester: "dokelž stej njedopóznaće a znajechanje čłowječich prawow k aktam"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hsn_Hans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hsn_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ht_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ht_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hu_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 region: "SI"
 region: "SK"
 region: "UA"
 exemplar_chars {
   base: "a á b c {cs} {ccs} d {dz} {ddz} {dzs} {ddzs} e é f g {gy} {ggy} h i í j k l {ly} {lly} m n {ny} {nny} o ó ö ő p r s {sz} {ssz} t {ty} {tty} u ú ü ű v z {zs} {zzs}"
   auxiliary: "à ă â å ä ã ā æ ç è ĕ ê ë ē ì ĭ î ï ī ñ ò ŏ ô ø ō œ q ù ŭ û ū w x y ÿ"
   marks: "◌́ ◌̈ ◌̋"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ – , ; : ! ? . … \' ’ \" ” „ « » ( ) [ ] { } ⟨ ⟩ § @ * / & # ~ ⁒"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … \' ’ \" ” „ « » ( ) [ ] { } @ * / & # ~ "
   index: "A Á B C {CS} D {DZ} {DZS} E É F G {GY} H I Í J K L {LY} M N {NY} O Ó Ö Ő P Q R S {SZ} T {TY} U Ú Ü Ű V W X Y Z {ZS}"
 }
 sample_text {
   masthead_full: "MmIi"
   masthead_partial: "Nn"
   styles: "Tekintettel arra, hogy az emberiség családja"
   tester: "Tekintettel arra, hogy az emberi jogok el nem ismerése és semmibevevése"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hus_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/huu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/huu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hy_Armn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hy_Armn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 region: "LB"
 region: "RU"
 region: "SY"
 region: "TR"
 exemplar_chars {
   base: "ա բ գ դ ե զ է ը թ ժ ի լ խ ծ կ հ ձ ղ ճ մ յ ն շ ո չ պ ջ ռ ս վ տ ր ց ւ փ ք օ ֆ"
   auxiliary: "և"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   punctuation: "֊ , ՝ : ՜ ՞ . « » ՚ ՛ ՟"
   index: "Ա Բ Գ Դ Ե Զ Է Ը Թ Ժ Ի Լ Խ Ծ Կ Հ Ձ Ղ Ճ Մ Յ Ն Շ Ո Չ Պ Ջ Ռ Ս Վ Տ Ր Ց Ւ Փ Ք Օ Ֆ"
 }
 sample_text {
   masthead_full: "ԲբՈո"
   masthead_partial: "Լլ"
   styles: "Քանզի մարդկային ընտանիքի բոլոր անդամներին"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/hyw_Armn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/hyw_Armn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ia_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ia_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ibb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ibb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/id_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/id_Latn.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Indonesia"
 population: 171207687
 region: "ID"
 region: "NL"
 exemplar_chars {
   base: "a b c d e f g h i j k l m n o p q r s t u v w x y z"
   auxiliary: "å"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "SsEe"
   masthead_partial: "Mm"
   styles: "Menimbang bahwa pengakuan atas martabat alamiah"
   tester: "Menimbang bahwa mengabaikan dan memandang rendah hak-hak asasi"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/idu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/idu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ie_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ie_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ig_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ig_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Igbo"
 population: 27823640
 region: "NG"
 exemplar_chars {
   base: "a A b B {ch} {CH} d D e E ẹ Ẹ f F g G {gb} {GB} {gh} {GH} {gw} {GW} h H i I ị Ị j J k K {kp} {KP} {kw} {KW} l L m M n N ṅ Ṅ {nw} {NW} {ny} {NY} o O ọ Ọ p P r R s S {sh} {SH} t T u U ụ Ụ v V w W y Y z Z"
   auxiliary: "á Á à À ā Ā c C é É è È ē Ē í Í ì Ì ī Ī {ị́} {Ị́} {ị̀} {Ị̀} ḿ Ḿ {m̀} {M̀} ń Ń ǹ Ǹ ó Ó ò Ò ō Ō {ọ́} {Ọ́} {ọ̀} {Ọ̀} q Q ú Ú ù Ù ū Ū {ụ́} {Ụ́} {ụ̀} {Ụ̀} x X"
   marks: "◌̀ ◌́ ◌̄ ◌̇ ◌̣"
-  punctuation: "- ‑ , ; : ! ? . ‘ ’ “ ” ( ) [ ] { }"
+  punctuation: "- , ; : ! ? . ‘ ’ “ ” ( ) [ ] { }"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaMm"
   masthead_partial: "Ụụ"
   styles: "Ebe ọ bụ na nghọta ugwu ekere uwa na ikike"
   tester: "Ebe nleghara anya na nleli ikike mmadu nwegasịrị emeela ka e"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ii_Yiii.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ii_Yiii.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Sichuan Yi"
 preferred_name: "Nuosu"
 autonym: "ꆈꌠꉙ (ꆈꌠꁱꂷ)"
 population: 8364120
 region: "CN"
 exemplar_chars {
   base: "ꀀ-ꒌ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "ꀀ ꀋ ꀗ ꀣ ꀯ ꀺ ꁆ ꁒ ꁞ ꁩ ꁵ ꂁ ꂍ ꂘ ꂤ ꂰ ꂼ ꃇ ꃓ ꃟ ꃫ ꃶ ꄂ ꄎ ꄚ ꄥ ꄱ ꄽ ꅉ ꅔ ꅠ ꅬ ꅸ ꆃ ꆏ ꆛ ꆧ ꆳ ꆾ ꇊ ꇖ ꇢ ꇭ ꇹ ꈅ ꈑ ꈜ ꈨ ꈴ ꉀ ꉋ ꉗ ꉣ ꉯ ꉺ ꊆ ꊒ ꊞ ꊩ ꊵ ꋁ ꋍ ꋘ ꋤ ꋰ ꋼ ꌇ ꌓ ꌟ ꌫ ꌷ ꍂ ꍎ ꍚ ꍦ ꍱ ꍽ ꎉ ꎕ ꎠ ꎬ ꎸ ꏄ ꏏ ꏛ ꏧ ꏳ ꏾ ꐊ ꐖ ꐢ ꐭ ꐹ ꑅ ꑑ ꑜ ꑨ ꑴ ꒀ ꒋ"
 }
 sample_text {
   masthead_full: "ꊿꂷꃅꄿ"
   masthead_partial: "ꐨꐥ"
   styles: "ꊽꋩꅍꏭꉜꀋꒉꌠꌋꆀꉜꄸꑠꆹꅢꎆꌊꆀꍀꆿꃅꇏꅊꀐꃅꇏꋋꈨꆹꃰꊿꂄꉌꇬꍍꄀꌠꉬꊿꂷꈀꐥꃅꐥꋭꅇꉉꈋꍣꌋꆀꑇꌠꄿꐨꐥ"
   tester: "ꉻꏑꇩꏤꏓꂱꐥꇯꌠꏦꃤꁢꊧꇬꊿꊇꌅꅍꊿꑌꇐꁌꐨꌋꆀꅪꃰꐥꒈꃅꐥꌠꌅꅍꑠꉈꑴꌌꉉꄜꋊ，ꄷꀋꁨꀋꎪꃅꄿꐨꊼꇅꀉꒉꃅꐥꌠꐧꋦꀒꁨꆹꌠꌋꆀꐥꐨꄺꅐꌠꀻꎆꆹꎻ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ijs_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ijs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ilo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ilo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/io_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/io_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/is_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/is_Latn.textproto`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Íslenska"
 population: 350734
 region: "IS"
 exemplar_chars {
   base: "a á b d ð e é f g h i í j k l m n o ó p r s t u ú v x y ý þ æ ö"
   auxiliary: "c q w z"
   marks: "◌́ ◌̈ ◌̨"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ ( ) [ ] @ * / & #"
   index: "A Á B C D Ð E É F G H I Í J K L M N O Ó P Q R S T U Ú V W X Y Ý Z Þ Æ Ö"
 }
 sample_text {
   masthead_full: "HhVv"
   masthead_partial: "Ee"
   styles: "Það ber að viðurkenna, að hver maður sé jafnborinn"
   tester: "Hafi mannréttindi verið fyrir borð borin og lítilsvirt, hefur"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/it_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/it_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 region: "SM"
 region: "US"
 region: "VA"
 exemplar_chars {
   base: "a à b c d e é è f g h i ì j k l m n o ó ò p q r s t u ù v w x y z"
   auxiliary: "ª á â å ä ã æ ç ê ë í î ï ñ º ô ö õ ø œ ß ú û ü ÿ"
   marks: "◌̀ ◌́ ◌̂ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ — , ; : ! ? . … \' ’ \" “ ” « » ( ) [ ] { } @ /"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- — , ; : ! ? . … \' ’ \" “ ” « » ( ) [ ] { } @ /"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtUu"
   masthead_partial: "Ii"
   styles: "Considerato che il riconoscimento della dignità"
   tester: "Considerato che il disconoscimento e il disprezzo dei diritti"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/iu_Cans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/iu_Cans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ja_Hira.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ja_Hira.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ja_Jpan.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ja_Jpan.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "日本語 (日本)"
 population: 119676253
 region: "BR"
 region: "JP"
 exemplar_chars {
   base: "々 ゝヽ ゞヾ ー ぁァ あア ぃィ いイ ぅゥ うウ ヴ ぇェ えエ ぉォ おオ ヵ かカ がガ きキ ぎギ くク ぐグ ヶ けケ げゲ こコ ごゴ さサ ざザ しシ じジ すス ずズ せセ ぜゼ そソ ぞゾ たタ だダ ちチ ぢヂ っッ つツ づヅ てテ でデ とト どド なナ にニ ぬヌ ねネ のノ はハ ばバ ぱパ ひヒ びビ ぴピ ふフ ぶブ ぷプ へヘ べベ ぺペ ほホ ぼボ ぽポ まマ みミ むム めメ もモ ゃャ やヤ ゅュ ゆユ ょョ よヨ らラ りリ るル れレ ろロ ゎヮ わワ ゐヰ ゑヱ をヲ んン 一 丁 七 万-下 不 与 且 世 丘 丙 両 並 中 串 丸 丹 主 丼 久 乏 乗 乙 九 乞 乱 乳 乾 亀 了 予 争 事 二 互 五 井 亜 亡 交 享-亭 人 仁 今 介 仏 仕 他 付 仙 代-以 仮 仰 仲 件 任 企 伎-休 会 伝 伯 伴 伸 伺 似 但 位-佐 体 何 余 作 佳 併 使 例 侍 供 依 価 侮 侯 侵 侶 便 係 促 俊 俗 保 信 修 俳 俵 俸 俺 倉 個 倍 倒 候 借 倣 値 倫 倹 偉 偏 停 健 側-偶 偽 傍 傑 傘 備 催 傲 債 傷 傾 僅 働 像 僕 僚 僧 儀 億 儒 償 優 元-兆 先 光 克 免 児 党 入 全 八-六 共 兵 具 典 兼 内 円 冊 再 冒 冗 写 冠 冥 冬 冶 冷 凄 准 凍 凝 凡 処 凶 凸-出 刀 刃 分-刈 刊 刑 列 初 判 別 利 到 制-刻 則 削 前 剖 剛 剣-剥 副 剰 割 創 劇 力 功 加 劣 助 努 励 労 効 劾 勃 勅 勇 勉 動 勘 務 勝 募 勢 勤 勧 勲 勾 匂 包 化 北 匠 匹-医 匿 十 千 升 午 半 卑-協 南 単 博 占 印 危 即-卵 卸 厄 厘 厚 原 厳 去 参 又 及-収 叔 取 受 叙 口-句 叫 召 可-右 号 司 各 合 吉 同-向 君 吟 否 含 吸 吹 呂 呈-告 周 呪 味 呼 命 和 咲 咽 哀 品 員 哲 哺 唄 唆 唇 唐 唯 唱 唾 商 問 啓 善 喉 喚 喜 喝 喩-喫 営 嗅 嗣 嘆 嘱 嘲 器 噴 嚇 囚 四 回 因 団 困 囲 図 固 国 圏 園 土 圧 在 地 坂 均 坊 坑 坪 垂 型 垣 埋 城 域 執 培 基 埼 堀 堂 堅 堆 堕 堤 堪 報 場 塀 塁 塊 塑 塔 塗 塚 塞 塩 填 塾 境 墓 増 墜 墨 墳 墾 壁 壇 壊 壌 士 壮 声-売 変 夏 夕 外 多 夜 夢 大 天-夫 央 失 奇-奉 奏 契 奔 奥 奨 奪 奮 女 奴 好 如-妄 妊 妖 妙 妥 妨 妬 妹 妻 姉 始 姓 委 姫 姻 姿 威 娘 娠 娯 婆 婚 婦 婿 媒 媛 嫁 嫉 嫌 嫡 嬢 子 孔 字 存 孝 季 孤 学 孫 宅 宇-安 完 宗-宝 実 客-室 宮 宰 害-家 容 宿 寂 寄 密 富 寒 寛 寝 察 寡 寧 審 寮 寸 寺 対 寿 封 専 射 将 尉-尋 導 小 少 尚 就 尺-局 居 屈 届 屋 展 属 層 履 屯 山 岐 岡 岩 岬 岳 岸 峠 峡 峰 島 崇 崎 崖 崩 嵐 川 州 巡 巣 工-巨 差 己 巻 巾 市 布 帆 希 帝 帥 師 席 帯 帰 帳 常 帽 幅 幕 幣 干-年 幸 幹 幻-幾 庁 広 床 序 底 店 府 度 座 庫 庭 庶-庸 廃 廉 廊 延 廷 建 弁 弄 弊 式 弐 弓-引 弟 弥-弧 弱 張 強 弾 当 彙 形 彩 彫 彰 影 役 彼 往 征 径 待 律 後 徐 徒 従 得 御 復 循 微 徳 徴 徹 心 必 忌 忍 志-忙 応 忠 快 念 怒 怖 思 怠 急 性 怨 怪 恋 恐 恒 恣 恥 恨 恩 恭 息 恵 悔 悟 悠 患 悦 悩 悪 悲 悼 情 惑 惜 惧 惨 惰 想 愁 愉 意 愚 愛 感 慄 慈 態 慌 慎 慕 慢 慣 慨 慮 慰 慶 憂 憎 憤 憧 憩 憬 憲 憶 憾 懇 懐 懲 懸 成-戒 戚 戦 戯 戴 戸 戻 房 所 扇 扉 手 才 打 払 扱 扶 批 承 技 抄 把 抑 投 抗 折 抜 択 披 抱 抵 抹 押 抽 担 拉 拍 拐 拒 拓 拘 拙 招 拝 拠 拡 括 拭 拳 拶 拷 拾 持 指 挑 挙 挟 挨 挫 振 挿 捉 捕 捗 捜 捨 据 捻 掃 授 掌 排 掘 掛 採 探 接 控 推 措 掲 描 提 揚 換 握 揮 援 揺 損 搬 搭 携 搾 摂 摘 摩 摯 撃 撤 撮 撲 擁 操 擦 擬 支 改 攻 放 政 故 敏 救 敗 教 敢 散 敬 数 整 敵 敷 文 斉 斎 斑 斗 料 斜 斤 斥 斬 断 新 方 施 旅 旋 族 旗 既 日-早 旬 旺 昆 昇 明 易 昔 星 映 春 昧 昨 昭 是 昼 時 晩 普 景 晴 晶 暁 暇 暑 暖 暗 暦 暫 暮 暴 曇 曖 曜 曲 更 書 曹 曽 替 最 月 有 服 朕 朗 望 朝 期 木 未-札 朱 朴 机 朽 杉 材 村 束 条 来 杯 東 松 板 析 枕 林 枚 果 枝 枠 枢 枯 架 柄 某 染 柔 柱 柳 柵 査 柿 栃 栄 栓 校 株 核 根 格 栽 桁 桃 案 桑 桜 桟 梅 梗 梨 械 棄 棋 棒 棚 棟 森 棺 椅 植 椎 検 業 極 楷 楼 楽 概 構 様 槽 標 模 権 横 樹 橋 機 欄 欠 次 欧 欲 欺 款 歌 歓 止 正 武 歩 歯 歳 歴 死 殉-残 殖 殴 段 殺 殻 殿 毀 母 毎 毒 比 毛 氏 民 気 水 氷 永 氾 汁 求 汎 汗 汚 江 池 汰 決 汽 沃 沈 沖 沙 没 沢 河 沸 油 治 沼 沿 況 泉 泊 泌 法 泡-泣 泥 注 泰 泳 洋 洗 洞 津 洪 活 派 流 浄 浅 浜 浦 浪 浮 浴 海 浸 消 涙 涯 液 涼 淑 淡 淫 深 混 添 清 渇-渉 渋 渓 減 渡 渦 温 測 港 湖 湧 湯 湾-満 源 準 溝 溶 溺 滅 滋 滑 滝 滞 滴 漁 漂 漆 漏 演 漠 漢 漫 漬 漸 潔 潜 潟 潤 潮 潰 澄 激 濁 濃 濫 濯 瀬 火 灯 灰 災 炉 炊 炎 炭 点 為 烈 無 焦 然 焼 煎 煙 照 煩 煮 熊 熟 熱 燃 燥 爆 爪 爵 父 爽 片 版 牙 牛 牧 物 牲 特 犠 犬 犯 状 狂 狙 狩 独 狭 猛 猟 猫 献 猶 猿 獄 獣 獲 玄 率 玉 王 玩 珍 珠 班 現 球 理 琴 瑠 璃 璧 環 璽 瓦 瓶 甘 甚 生 産 用 田-申 男 町 画 界 畏 畑 畔 留 畜 畝 略 番 異 畳 畿 疎 疑 疫 疲 疾 病 症 痕 痘 痛 痢 痩 痴 瘍 療 癒 癖 発 登 白 百 的 皆 皇 皮 皿 盆 益 盗 盛 盟 監 盤 目 盲 直 相 盾 省 眉 看 県 真 眠 眺 眼 着 睡 督 睦 瞬 瞭 瞳 矛 矢 知 短 矯 石 砂 研 砕 砲 破 硝 硫 硬 碁 碑 確 磁 磨 礁 礎 示 礼 社 祈 祉 祖 祝 神 祥 票 祭 禁 禅 禍 福 秀 私 秋 科 秒 秘 租 秩 称 移 程 税 稚 種 稲 稼 稽 稿 穀 穂 積 穏 穫 穴 究 空 突 窃 窒 窓 窟 窮 窯 立 竜 章 童 端 競 竹 笑 笛 符 第 筆 等 筋 筒 答 策 箇 箋 算 管 箱 箸 節 範 築 篤 簡 簿 籍 籠 米 粉 粋 粒 粗 粘 粛 粧 精 糖 糧 糸 系 糾 紀 約 紅 紋 納 純 紙-紛 素-索 紫 累 細 紳 紹 紺 終 組 経 結 絞 絡 給 統 絵 絶 絹 継 続 維 綱 網 綻 綿 緊 総 緑 緒 線 締 編 緩 緯 練 緻 縁 縄 縛 縦 縫 縮 績 繁 繊 織 繕 繭 繰 缶 罪 置 罰 署 罵 罷 羅 羊 美 羞 群 羨 義 羽 翁 翌 習 翻 翼 老 考 者 耐 耕 耗 耳 聖 聞 聴 職 肉 肌 肖 肘 肝 股 肢 肥 肩 肪 肯 育 肺 胃 胆 背 胎 胞 胴 胸 能 脂 脅 脇 脈 脊 脚 脱 脳 腎 腐 腕 腫 腰 腸-腺 膚 膜 膝 膨 膳 臆 臓 臣 臨 自 臭 至 致 臼 興 舌 舎 舗 舞 舟 航 般 舶 舷 船 艇 艦 良 色 艶 芋 芝 芯 花 芳 芸 芽 苗 苛 若 苦 英 茂 茎 茨 茶 草 荒 荘 荷 菊 菌 菓 菜 華 萎 落 葉 著 葛 葬 蒸 蓄 蓋 蔑 蔵 蔽 薄 薦 薪-薬 藍 藤 藩 藻 虎 虐 虚 虜 虞 虫 虹 蚊 蚕 蛇 蛍 蛮 蜂 蜜 融 血 衆 行 術 街 衛 衝 衡 衣 表 衰 衷 袋 袖 被 裁 裂 装 裏 裕 補 裸 製 裾 複 褐 褒 襟 襲 西 要 覆 覇 見 規 視 覚 覧 親 観 角 解 触 言 訂 訃 計 討 訓 託 記 訟 訪 設 許 訳 訴 診 証 詐 詔 評 詞 詠 詣 試 詩 詮 詰-詳 誇 誉 誌 認 誓 誕 誘 語 誠 誤 説 読 誰 課 調 談 請 論 諦 諧 諭 諮 諸 諾 謀 謁 謄 謎 謙 講 謝 謡 謹 識 譜 警 議 譲 護 谷 豆 豊 豚 象 豪 貌 貝 貞 負-貢 貧-責 貯 貴 買 貸 費 貼 貿 賀 賂-賄 資 賊 賓 賛 賜 賞 賠 賢 賦 質 賭 購 贈 赤 赦 走 赴 起 超 越 趣 足 距 跡 路 跳 践 踊 踏 踪 蹴 躍 身 車 軌 軍 軒 軟 転 軸 軽 較 載 輝 輩 輪 輸 轄 辛 辞 辣 辱 農 辺 込 迅 迎 近 返 迫 迭 述 迷 追 退 送 逃 逆 透 逐 逓 途 通 逝 速 造 連 逮 週 進 逸 遂 遅 遇 遊 運 遍 過 道-違 遜 遠 遡 遣 適 遭 遮 遵 遷 選 遺 避 還 那 邦 邪 邸 郊 郎 郡 部 郭 郵 郷 都 酌-酎 酒 酔 酢 酪 酬 酵 酷 酸 醒 醜 醸 采 釈 里-量 金 釜 針 釣 鈍 鈴 鉄 鉛 鉢 鉱 銀 銃 銅 銘 銭 鋭 鋳 鋼 錠 錦 錬 錮 錯 録 鍋 鍛 鍵 鎌 鎖 鎮 鏡 鐘 鑑 長 門 閉 開 閑 間 関 閣 閥 閲 闇 闘 阜 阪 防 阻 附 降 限 陛 院-陥 陪 陰 陳 陵 陶 陸 険 陽 隅 隆 隊 階 随 隔 隙 際 障 隠 隣 隷 隻 雄-雇 雌 雑 離 難 雨 雪 雰 雲 零 雷 電 需 震 霊 霜 霧 露 青 静 非 面 革 靴 韓 音 韻 響 頂 頃 項 順 須 預-頓 領 頬 頭 頻 頼 題-顎 顔 顕 願 類 顧 風 飛 食 飢 飯 飲 飼-飾 餅 養 餌 餓 館 首 香 馬 駄-駆 駐 駒 騎 騒 験 騰 驚 骨 骸 髄 高 髪 鬱 鬼 魂 魅 魔 魚 鮮 鯨 鳥 鳴 鶏 鶴 鹿 麓 麗 麦 麺 麻 黄 黒 黙 鼓 鼻 齢"
   auxiliary: "丑 亥 亨 兌 兎 凧 剃 卯 嘉 嘔 嘘 壬 壺 嬉 寅 巳 庚 庵 弘 彗 悶 愕 戊 戌 拼 揃 斧 昌 杖 桶 梵 楔 湘 焚 燭 爬 牌 牝 牡 狐 狗 狼 猪 獅 癸 瞑 碇 祚 禄 禎 秤 竿 絆 繍 罫 膏 芒 蟄 蟹 蠍 蠣 贛 蹄 辰 酉 鋲 錄 錨 閏 閩 雀 雉 鳳 鼠 龍"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "‾ _＿ -－ ‐ ‑ — ― 〜 ・ ･ ,， 、､ ;； :： !！ ?？ .． ‥ … 。｡ ＇ ‘ ’ \"＂ “ ” (（ )） [［ ]］ {｛ }｝ 〈 〉 《 》 「｢ 」｣ 『 』 【 】 〔 〕 ‖ § ¶ @＠ *＊ /／ \\＼ &＆ #＃ %％ ‰ † ‡ ′ ″ 〃 ※ }"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "‾ _＿ -－ — ― 〜 ・ ･ ,， 、､ ;； :： !！ ?？ .． ‥ … 。｡ ＇ ‘ ’ \"＂ “ ” (（ )） [［ ]］ {｛ }｝ 〈 〉 《 》 「｢ 」｣ 『 』 【 】 〔 〕 ‖ ¶ @＠ *＊ /／ \\＼ &＆ #＃ %％ 〃 ※ }"
   index: "あ か さ た な は ま や ら わ"
 }
 sample_text {
   masthead_full: "すべての"
   masthead_partial: "人間"
   styles: "人類社会のすべての構成員の固有の尊厳と平等で譲ることのできない権利とを承認することは"
   tester: "人権の無視及び軽侮が、人類の良心を踏みにじった野蛮行為をもたらし、言論及び信仰の自由が受けられ、恐怖及び欠乏のない世界の到来が"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ja_Kana.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ja_Kana.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/jbo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/jbo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/jgo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/jgo_Latn.textproto`

 * *Files 12% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 autonym: "Cú-Mbɔ́ndaa"
 population: 94333
 region: "CM"
 exemplar_chars {
   base: "a A á Á â Â ǎ Ǎ b B c C d D ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̀} {Ɛ̀} {ɛ̂} {Ɛ̂} {ɛ̌} {Ɛ̌} {ɛ̄} {Ɛ̄} f F g G h H i I í Í î Î ǐ Ǐ j J k K l L m M ḿ Ḿ {m̀} {M̀} {m̄} {M̄} n N ń Ń ǹ Ǹ {n̄} {N̄} ŋ Ŋ {ŋ́} {Ŋ́} {ŋ̀} {Ŋ̀} {ŋ̄} {Ŋ̄} ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̂} {Ɔ̂} {ɔ̌} {Ɔ̌} p P {pf} {PF} s S {sh} {SH} t T {ts} {TS} u U ú Ú û Û ǔ Ǔ ʉ Ʉ {ʉ́} {Ʉ́} {ʉ̂} {Ʉ̂} {ʉ̌} {Ʉ̌} {ʉ̈} {Ʉ̈} v V w W ẅ Ẅ y Y z Z ꞌ Ꞌ"
   auxiliary: "e E o O q Q r R x X"
   marks: "◌̀ ◌́ ◌̂ ◌̄ ◌̈ ◌̌"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ , ; : ! ? . ‹ › « »"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- , ; : ! ? . ‹ › « »"
   index: "A B C D Ɛ F G H I J K L M N Ŋ Ɔ P {Pf} S {Sh} T {Ts} U Ʉ {Ʉ̈} V W Ẅ Y Z Ꞌ"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/jiv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/jiv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/jra_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/jra_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/jv_Java.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/jv_Java.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/jv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/jv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ka_Geok.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ka_Geok.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ka_Geor.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ka_Geor.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 3543645
 region: "GE"
 region: "IR"
 region: "TR"
 exemplar_chars {
   base: "ა ბ გ დ ე ვ ზ თ ი კ ლ მ ნ ო პ ჟ რ ს ტ უ ფ ქ ღ ყ შ ჩ ც ძ წ ჭ ხ ჯ ჰ"
   auxiliary: "ⴀ ⴁ ⴂ ⴃ ⴄ ⴅ ⴆ ჱ ⴡ ⴇ ⴈ ⴉ ⴊ ⴋ ⴌ ჲ ⴢ ⴍ ⴎ ⴏ ⴐ ⴑ ⴒ ჳ ⴣ ⴓ ⴔ ⴕ ⴖ ⴗ ⴘ ⴙ ⴚ ⴛ ⴜ ⴝ ⴞ ჴ ⴤ ⴟ ⴠ ჵ ⴥ ჶ ჷ ჸ ჹ ჺ"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … ჻ \' ‘ ‚ “ „ « » ( ) [ ] { } § @ * / & # † ‡ ′ ″ №"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … ჻ \' ‘ ‚ “ „ « » ( ) [ ] { } @ * / & #№"
   index: "ა ბ გ დ ე ვ ზ თ ი კ ლ მ ნ ო პ ჟ რ ს ტ უ ფ ქ ღ ყ შ ჩ ც ძ წ ჭ ხ ჯ ჰ"
 }
 sample_text {
   masthead_full: "ყოვე"
   masthead_partial: "ლი"
   styles: "ვინაიდან ადამიანთა ოჯახის ყველა წევრისათვის"
   tester: "ვინაიდან, ადამიანის უფლებათა უგულებელყოფამ და აბუჩად აგდებამ გამოიწვია"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kaa_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kaa_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kab_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kab_Latn.textproto`

 * *Files 12% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 autonym: "Taqbaylit"
 population: 3351886
 region: "DZ"
 exemplar_chars {
   base: "a A b B c C č Č d D ḍ Ḍ e E ɛ Ɛ f F g G ǧ Ǧ ɣ Ɣ h H ḥ Ḥ i I j J k K l L m M n N p P q Q r R ṛ Ṛ s S ṣ Ṣ t T ṭ Ṭ u U w W x X y Y z Z ẓ Ẓ"
   auxiliary: "o O v V"
   marks: "◌̌ ◌̣"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C Č D Ḍ E Ɛ F G Ǧ Ɣ H Ḥ I J K L M N P Q R Ṛ S Ṣ T Ṭ U W X Y Z Ẓ"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kab_Tfng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kab_Tfng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kbd_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kbd_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kbp_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kbp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kde_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kde_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kdh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kdh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kea_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kea_Latn.textproto`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Kabuverdianu"
 population: 530762
 region: "CV"
 exemplar_chars {
   base: "a b d {dj} e f g h i j k l {lh} m n ñ {nh} o p r s t {tx} u v x y z"
   auxiliary: "ª á à ă â å ä ã ā æ c ç é è ĕ ê ë ẽ ē í ì ĭ î ï ĩ ī {n̈} º ó ò ŏ ô ö õ ø ō œ q {rr} ú ù ŭ û ü ũ ū w ÿ"
   marks: "◌̀ ◌́ ◌̂ ◌̃ ◌̈ ◌̧"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” « » ( ) [ ] § @ * / & # † ‡"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” « » ( ) [ ] @ * / & # "
   index: "A B D E F G H I J K L M N O P R S T U V X Z"
 }
 sample_text {
   masthead_full: "TtUu"
   masthead_partial: "Dd"
   styles: "Nu ta considrâ qui, riconhecimento di dignidadi"
   tester: "Nu ta considrâ qui, disconhecimento e disprezo di drêto di tudo"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kek_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kek_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kg_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kgj_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kgj_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kha_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kha_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,10 @@
   tester: "Kumba ka jingibeiñ bad jingbymsuidkhai ïa ki hok longbriew manbriew"
   poster_sm: "Kumba ka long"
   poster_md: "Kumba ka"
   poster_lg: "bynriew"
   specimen_48: "Kumba ki briew jong ka Synjuk Ki Ri ha ka Kyrmit ki la pynskhem"
   specimen_36: "Kumba ka long kaba donkam ban kyntiew ïa ka jingroi ka jingïadei lok para ri,\nNamarkata, Mynta,\nKa Dorbar Bah,"
   specimen_32: "Ym don uwei ne kawei ki ban shah teh mraw ne long mraw hano hano; la khang pyrshah ïa ka jinglongmraw bad ka jingkhaïi mraw la ki dei ha kano kano ka dur ne rukom."
-  specimen_21: "Kumba ka jingithuh ïa ka kyrdan long tynrai bad ïa ki marryngkat bad bashongkhien jong baroh ki dkhot longïing u  dei ka tlong jong ka jinglaitluid, ka jingbishar hok, bad ka jingsuk shisnieh pyrthei,\nKumba ka long kaba donkam ba ïa u/ka briew ym dei ban pynbor ban shim ki lynti, kum ka khen khatduh, da ka jingïaleh pyrshah ïa ka jingbanbeiñ bad jingsynshar runar, ba ïa ki hok longbriew manbriew dei ban ïada da ka aiñ ka kanun,"
-  specimen_16: "Kumba ka jingithuh ïa ka kyrdan long tynrai bad ïa ki marryngkat bad bashongkhien jong baroh ki dkhot longïing u  dei ka tlong jong ka jinglaitluid, ka jingbishar hok, bad ka jingsuk shisnieh pyrthei,\nKumba ka jingibeiñ bad jingbymsuidkhai ïa ki hok longbriew manbriew la pynkha ïa ki kam riewkhlaw kiba la pynkhih win ïa ka jingïatiplem u bynriew, bad ka jingkylla ka pyrthei ha kaba u khun bynriew un leh kmen laitluid ha ka kren ka khana bad jingngeit bad jinglaitluid na ka tieng ka syier bad ka kyrduh la pynbna kum ka jingangnud ba ha khlieh tam jong u luk u lak,"
+  specimen_21: "Kumba ka jingithuh ïa ka kyrdan long tynrai bad ïa ki marryngkat bad bashongkhien jong baroh ki dkhot longïing u dei ka tlong jong ka jinglaitluid, ka jingbishar hok, bad ka jingsuk shisnieh pyrthei,\nKumba ka long kaba donkam ba ïa u/ka briew ym dei ban pynbor ban shim ki lynti, kum ka khen khatduh, da ka jingïaleh pyrshah ïa ka jingbanbeiñ bad jingsynshar runar, ba ïa ki hok longbriew manbriew dei ban ïada da ka aiñ ka kanun,"
+  specimen_16: "Kumba ka jingithuh ïa ka kyrdan long tynrai bad ïa ki marryngkat bad bashongkhien jong baroh ki dkhot longïing u dei ka tlong jong ka jinglaitluid, ka jingbishar hok, bad ka jingsuk shisnieh pyrthei,\nKumba ka jingibeiñ bad jingbymsuidkhai ïa ki hok longbriew manbriew la pynkha ïa ki kam riewkhlaw kiba la pynkhih win ïa ka jingïatiplem u bynriew, bad ka jingkylla ka pyrthei ha kaba u khun bynriew un leh kmen laitluid ha ka kren ka khana bad jingngeit bad jinglaitluid na ka tieng ka syier bad ka kyrduh la pynbna kum ka jingangnud ba ha khlieh tam jong u luk u lak,"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/khb_Talu.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/khb_Talu.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/khr_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/khr_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/khr_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/khr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/khr_Orya.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/khr_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/khw_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/khw_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/khw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/khw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kjh_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kjh_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
   base: "А Б В Г Д Е Ж З И Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ъ Ы Ь Э Ю Я Ё І Ғ Ң Ӌ Ӧ Ӱ а б в г д е ж з и й к л м н о п р с т у ф х ц ч ш щ ъ ы ь э ю я ё і ғ ң ӌ ӧ ӱ"
   marks: "◌̆ ◌̈"
 }
 sample_text {
   masthead_full: "ПпОо"
   masthead_partial: "Лл"
   styles: "Санға алып, постың синін пілінгенін саназарынын,"
-  tester: "санға  алып,  нимее салбанын паза хырт кјріргенін кізі тјреелеріне"
+  tester: "санға алып, нимее салбанын паза хырт кјріргенін кізі тјреелеріне"
   poster_sm: "санға алып,"
   poster_md: "Искірче пу"
   poster_lg: "Полған"
   specimen_48: "Полған на кізі пос паза тиң тјріпче паза тиң постың синін пілінгенін"
   specimen_36: "Пірдеезін иреелирге алай чабал, кізі нимес чіли, пазынарға постың синін пілінгенін тезірерге чарадылбинча."
   specimen_32: "Полған на кізінің социальнай паза чоннар аразындағы чаа чох, амыр чуртасха, хаҷ ан пу Декларацияда пазылған праволар паза свободалар тооза толдырарға чарир,тјре пар."
-  specimen_21: "Пу Декларацияда пір дее ниме пасха хазнаның, чонның, хайдағда јменең алай алынҷа кізнең  хайдағ даа тоғыстаң айғазар алай пу Декларацияда пазылғанны сайбир  право чоннарның праволарын чох идер педінін сайбабчатхан тіп  саба чарыдылбазын.\nСанға алып, постың синін пілінгенін саназарынын, хайзы  прай кізілерде чоннар тјлінде пар, оларның тиң паза пыластырбас тјрее (право) пос чуртастың, пос оңдай чуртастың, сын паза прай тиксі амыр чуртас тјстігі (основа) полча; паза"
-  specimen_16: "Санға алып, постың синін пілінгенін саназарынын, хайзы  прай кізілерде чоннар тјлінде пар, оларның тиң паза пыластырбас тјрее (право) пос чуртастың, пос оңдай чуртастың, сын паза прай тиксі амыр чуртас тјстігі (основа) полча; паза\nсанға  алып,  нимее салбанын паза хырт кјріргенін кізі тјреелеріне (праволарға) нимее салбас оңдай чабал актарға ағылғаннар,  хайзы чоннардың ах сағысты еректірчелер, паза андағ чир чарыхты педіргені хайда кізілер сјс паза киртініс (убеждение) пос оңдайы пар полар паза хорғыс чох  паза хызылғаны чох чуртирлар паза, кізілерні пјзік кестеніске искірілген; паза"
+  specimen_21: "Пу Декларацияда пір дее ниме пасха хазнаның, чонның, хайдағда јменең алай алынҷа кізнең хайдағ даа тоғыстаң айғазар алай пу Декларацияда пазылғанны сайбир право чоннарның праволарын чох идер педінін сайбабчатхан тіп саба чарыдылбазын.\nСанға алып, постың синін пілінгенін саназарынын, хайзы прай кізілерде чоннар тјлінде пар, оларның тиң паза пыластырбас тјрее (право) пос чуртастың, пос оңдай чуртастың, сын паза прай тиксі амыр чуртас тјстігі (основа) полча; паза"
+  specimen_16: "Санға алып, постың синін пілінгенін саназарынын, хайзы прай кізілерде чоннар тјлінде пар, оларның тиң паза пыластырбас тјрее (право) пос чуртастың, пос оңдай чуртастың, сын паза прай тиксі амыр чуртас тјстігі (основа) полча; паза\nсанға алып, нимее салбанын паза хырт кјріргенін кізі тјреелеріне (праволарға) нимее салбас оңдай чабал актарға ағылғаннар, хайзы чоннардың ах сағысты еректірчелер, паза андағ чир чарыхты педіргені хайда кізілер сјс паза киртініс (убеждение) пос оңдайы пар полар паза хорғыс чох паза хызылғаны чох чуртирлар паза, кізілерні пјзік кестеніске искірілген; паза"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kk_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kk_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kk_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kk_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 12219390
 region: "KZ"
 region: "TR"
 exemplar_chars {
   base: "а ә б в г ғ д е ё ж з и й к қ л м н ң о ө п р с т у ұ ү ф х һ ц ч ш щ ъ ы і ь э ю я"
   auxiliary: ""
   marks: "◌̆ ◌̈"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” « » ( ) [ ] { } @ * / & #"
   index: "А Ә Б В Г Ғ Д Е Ё Ж З И Й К Қ Л М Н Ң О Ө П Р С Т У Ұ Ү Ф Х Һ Ц Ч Ш Щ Ъ Ы І Ь Э Ю Я"
 }
 sample_text {
   masthead_full: "БбАа"
   masthead_partial: "Рр"
   styles: "Адам баласы үйелменінің барлық мүшелеріне"
   tester: "адам құқықтарына деген елемеушілік, менсінбеушілік адам баласы"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kkh_Lana.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kkh_Lana.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kkj_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kkj_Latn.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 autonym: "Kakɔ"
 population: 149823
 region: "CM"
 exemplar_chars {
   base: "a á à â {a̧} b ɓ c d ɗ {ɗy} e é è ê ɛ {ɛ́} {ɛ̀} {ɛ̂} {ɛ̧} f g {gb} {gw} h i í ì î {i̧} j k {kp} {kw} l m {mb} n {nd} ǌ {ny} ŋ {ŋg} {ŋgb} {ŋgw} o ó ò ô ɔ {ɔ́} {ɔ̀} {ɔ̂} {ɔ̧} p r s t u ú ù û {u̧} v w y A Á À Â {A̧} B Ɓ C D Ɗ {Ɗy} E É È Ê Ɛ {Ɛ́} {Ɛ̀} {Ɛ̂} {Ɛ̧} F G {Gb} {Gw} H I Í Ì Î {I̧} J K {Kp} {Kw} L M {Mb} N {Nd} Ǌ {Ny} Ŋ {Ŋg} {Ŋgb} {Ŋgw} O Ó Ò Ô Ɔ {Ɔ́} {Ɔ̀} {Ɔ̂} {Ɔ̧} P R S T U Ú Ù Û {U̧} V W Y"
   auxiliary: "q Q x X z Z"
   marks: "◌́ ◌̀ ◌̂ ◌̧ ◌̌"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   punctuation: ", : ! ? . … ‘ ‹ › “ ” « » ( ) *"
   index: "A B Ɓ C D Ɗ {Ɗy} E Ɛ F G {Gb} {Gw} H I {I̧} J K {Kp} {Kw} L M {Mb} N {Nd} ǋ {Ny} Ŋ {Ŋg} {Ŋgb} {Ŋgw} O Ɔ {Ɔ̧} P R S T U {U̧} V W Y"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kl_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 population: 55440
 region: "DK"
 region: "GL"
 exemplar_chars {
   base: "a b c d e f g h i j k l m n o p q r s t u v w x y z æ ø å"
   auxiliary: "á â ã é ê ẽ í î ĩ ô õ ĸ ú û ũ"
   marks: "◌́ ◌̂ ◌̃ ◌̊ ◌̀"
-  numerals: ", . % ‰ + − 0 1 2 3 4 5 6 7 8 9"
+  numerals: ", . % + − 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z Æ Ø Å"
 }
 sample_text {
   masthead_full: "IiNn"
   masthead_partial: "Uu"
   styles: "Ataqqinassusermik inuup nammineq pigisaanik"
-  tester: "pingaaruteqarluinnar mat  inuiaqatigiit akornanni ikinngutinnersumik"
+  tester: "pingaaruteqarluinnar mat inuiaqatigiit akornanni ikinngutinnersumik"
   poster_sm: "Naalagaaffiit"
   poster_md: "taamaattumik"
   poster_lg: "Inuit"
   specimen_48: "Inuit tamarmik inunngorput nammineersinnaassuseqarlutik assigiimmillu"
   specimen_36: "Kinaluunniit inuunermut, nammineersinnaassuseqarnissamut isumakuluuteqaranilu inuuniarnissamut pisinnaatitaavoq."
   specimen_32: "Kinaluunniit inussiaatigineqaraniluunniit namminersorsinnaassusiiagaassanngilaq; inussiaateqarneq inussiaarniarnerlu sutigut tamatigut inerteqqutigineqassapput."
   specimen_21: "Kinaluunniit naalliutserujussuarneqassanngilaq aammalu peqqarniitsumik, naakkittaatsumik narrunarsaataasumillu pineqassananilu pillarneqassanani.\nInuk kinaluunniit nunarsuarmi sumiluunniit eqqartuussisarnermi pisassalittut pisussaasutulluunniit isigineqarsinnaatitaanissamut pisinnaatitaavoq.\nKinaluunniit namminissarsiortumik tigusarineqassanngliq, tigummigallagassanngortitaassanani imaluunniit nunagisamit peersitaassanani."
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/km_Khmr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/km_Khmr.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "ភាសាខ្មែរ"
 population: 15065030
 region: "KH"
 exemplar_chars {
   base: "័ ៈ ់ ៉ ៊ ៍ ក ខ គ ឃ ង ច ឆ ជ ឈ ញ ដ ឋ ឌ ឍ ណ ត ថ ទ ធ ន ប ផ ព ភ ម យ រ ឫ ឬ ល ឭ ឮ វ ស ហ ឡ អ {អា} ឥ ឦ ឧ {ឧក} ឩ ឪ ឯ ឰ ឱ ឲ ឳ ា ិ ី ឹ ឺ ុ ូ ួ ើ ឿ ៀ េ ែ ៃ ោ ៅ ំ ះ ្"
   auxiliary: "឴឵​ ៌ ៎ ៏ ៑ ឝ ឞ"
   marks: "◌឴ ◌឵ ◌ា ◌ិ ◌ី ◌ឹ ◌ឺ ◌ុ ◌ូ ◌ួ ◌ើ ◌ឿ ◌ៀ ◌េ ◌ែ ◌ៃ ◌ោ ◌ៅ ◌ំ ◌ះ ◌ៈ ◌៉ ◌៊ ◌់ ◌៍ ◌័ ◌្"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ , ៖ ! ? . ។ ៕ ‘ ’ \" “ ” ( ) [ ] { } ៙ ៚"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- , ៖ ! ? . ។ ៕ ‘ ’ \" “ ” ( ) [ ] { } ៙ ៚"
   index: "ក ខ គ ឃ ង ច ឆ ជ ឈ ញ ដ ឋ ឌ ឍ ណ ត ថ ទ ធ ន ប ផ ព ភ ម យ រ ឫ ឬ ល ឭ ឮ វ ស ហ ឡ អ ឥ ឦ ឧ ឩ ឪ ឯ ឰ ឱ ឳ"
 }
 sample_text {
   masthead_full: "មនសទ"
   masthead_partial: "ងអ"
   styles: "ដោយយល់ឃើញថា ការទទួលស្គាល់សេចក្ដីថ្លៃថ្នូរជាប់ពីកំណើត និងសិទ្ធិស្មើភាពគ្នា"
   tester: "ដោយយល់ឃើញថា ការមិនទទួលស្គាល់ និងការប្រមាថមើលងាយសិទ្ធិមនុស្ស នាំឱ្យមានអំពើ ព្រៃផ្សៃសាហាវយង់ឃ្នង ធ្វើឱ្យក្ដៅក្រហាយដល់សតិសម្បជញ្ញៈមនុស្សជាតិ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kmb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kmb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kn_Knda.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kn_Knda.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "ಕನ್ನಡ"
 population: 49065330
 region: "IN"
 exemplar_chars {
   base: "಼ ೦ ೧ ೨ ೩ ೪ ೫ ೬ ೭ ೮ ೯ ಅ ಆ ಇ ಈ ಉ ಊ ಋ ೠ ಌ ೡ ಎ ಏ ಐ ಒ ಓ ಔ ಂ ಃ ಕ ಖ ಗ ಘ ಙ ಚ ಛ ಜ ಝ ಞ ಟ ಠ ಡ ಢ ಣ ತ ಥ ದ ಧ ನ ಪ ಫ ಬ ಭ ಮ ಯ ರ ಱ ಲ ವ ಶ ಷ ಸ ಹ ಳ ಽ ಾ ಿ ೀ ು ೂ ೃ ೄ ೆ ೇ ೈ ೊ ೋ ೌ ್ ೕ ೖ"
   auxiliary: "‌‍ ೞ"
   marks: "◌ಂ ◌ಃ ◌ಾ ◌ಿ ◌ು ◌ೂ ◌ೃ ◌ೄ ◌ೆ ◌ೌ ◌್ ◌ೕ ◌ೖ"
-  numerals: "- ‑ , . % ‰ + 0೦ 1೧ 2೨ 3೩ 4೪ 5೫ 6೬ 7೭ 8೮ 9೯"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & # ′ ″"
+  numerals: "- , . % + 0೦ 1೧ 2೨ 3೩ 4೪ 5೫ 6೬ 7೭ 8೮ 9೯"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "ಅ ಆ ಇ ಈ ಉ ಊ ಋ ೠ ಌ ೡ ಎ ಏ ಐ ಒ ಓ ಔ ಕ ಖ ಗ ಘ ಙ ಚ ಛ ಜ ಝ ಞ ಟ ಠ ಡ ಢ ಣ ತ ಥ ದ ಧ ನ ಪ ಫ ಬ ಭ ಮ ಯ ರ ಱ ಲ ವ ಶ ಷ ಸ ಹ ಳ ೞ"
 }
 sample_text {
   masthead_full: "ಎಲಮನ"
   masthead_partial: "ವರ"
   styles: "ಎಲ್ಲಾ ಮಾನವರೂ ಸ್ವತಂತ್ರರಾಗಿಯೇ ಜನಿಸಿದ್ದಾರೆ. ಹಾಗೂ ಘನತೆ ಮತ್ತು ಹಕ್ಕುಗಳಲ್ಲಿ"
   tester: "ಜಾತಿ, ವರ್ಣ, ಸ್ತ್ರೀಪುರುಷ ಭೇದ, ಭಾಷೆ, ಧರ್ಮ, ರಾಜಕೀಯಾಭಿಪ್ರಾಯ ಅಥವಾ ಅನ್ಯಾಭಿಪ್ರಾಯ, ರಾಷ್ಟ್ರೀಯ ಮೂಲ ಅಥವಾ ಸಾಮಾಜಿಕ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/knc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/knc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ko_Kore.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ko_Kore.textproto`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 population: 78187423
 region: "CN"
 region: "KP"
 region: "KR"
 exemplar_chars {
   base: "가-힣"
   auxiliary: "ᄀ-ᄒ ᅡ-ᅵ ᆨ-ᇂ 丘 串 乃 久 乖 九 乞 乫 乾 亂 亘 交 京 仇 今 介 件 价 企 伋 伎 伽 佳 佶 侃 來 侊 供 係 俓 俱 個 倞 倦 倨 假 偈 健 傀 傑 傾 僅 僑 價 儆 儉 儺 光 克 兢 內 公 共 其 具 兼 冀 冠 凱 刊 刮 券 刻 剋 剛 劇 劍 劒 功 加 劤 劫 勁 勍 勘 勤 勸 勻 勾 匡 匣 區 南 卦 却 卵 卷 卿 厥 去 及 口 句 叩 叫 可 各 吉 君 告 呱 呵 咎 咬 哥 哭 啓 喀 喇 喝 喫 喬 嗜 嘉 嘔 器 囊 困 固 圈 國 圭 圻 均 坎 坑 坤 坰 坵 垢 基 埼 堀 堅 堈 堪 堺 塊 塏 境 墾 壙 壞 夔 奇 奈 奎 契 奸 妓 妗 姑 姜 姦 娘 娜 嫁 嬌 孔 季 孤 宏 官 客 宮 家 寄 寇 寡 寬 尻 局 居 屆 屈 岐 岡 岬 崎 崑 崗 嵌 嵐 嶇 嶠 工 巧 巨 己 巾 干 幹 幾 庚 庫 康 廊 廐 廓 廣 建 弓 强 彊 徑 忌 急 怪 怯 恐 恝 恪 恭 悸 愆 感 愧 愷 愾 慊 慣 慤 慨 慶 慷 憩 憬 憾 懃 懇 懦 懶 懼 戈 戒 戟 戡 扱 技 抉 拉 拏 拐 拒 拘 括 拮 拱 拳 拷 拿 捏 据 捲 捺 掘 掛 控 揀 揆 揭 擊 擎 擒 據 擧 攪 攷 改 攻 故 敎 救 敢 敬 敲 斛 斤 旗 旣 昆 昑 景 晷 暇 暖 暠 暻 曠 曲 更 曷 朗 朞 期 机 杆 杞 杰 枏 果 枯 架 枸 柑 柩 柬 柯 校 根 格 桀 桂 桔 桿 梏 梗 械 梱 棄 棋 棍 棘 棨 棺 楗 楠 極 槁 構 槐 槨 槪 槻 槿 樂 橄 橋 橘 機 檄 檎 檢 櫃 欄 權 欺 款 歌 歐 歸 殼 毆 毬 氣 求 江 汨 汲 決 汽 沂 沽 洛 洸 浪 涇 淃 淇 減 渠 渴 湳 溝 溪 滑 滾 漑 潔 潰 澗 激 濫 灌 灸 炅 炚 炬 烙 烱 煖 爛 牽 犬 狂 狗 狡 狼 獗 玖 玘 珂 珏 珖 珙 珞 珪 球 琦 琨 琪 琯 琴 瑾 璂 璟 璣 璥 瓊 瓘 瓜 甄 甘 甲 男 畇 界 畸 畺 畿 疆 疥 疳 痂 痙 痼 癎 癩 癸 皆 皎 皐 盖 監 看 眷 睾 瞰 瞼 瞿 矜 矩 矯 硅 硬 碁 碣 磎 磬 磯 磵 祁 祇 祈 祛 祺 禁 禽 科 稈 稼 稽 稿 穀 究 穹 空 窘 窟 窮 窺 竅 竟 竭 競 竿 筋 筐 筠 箇 箕 箝 管 簡 粳 糠 系 糾 紀 納 紘 級 紺 絅 結 絞 給 絳 絹 絿 經 綱 綺 緊 繫 繭 繼 缺 罐 罫 羅 羈 羌 羔 群 羹 翹 考 耆 耉 耕 耭 耿 肌 肝 股 肩 肯 肱 胛 胱 脚 脛 腔 腱 膈 膏 膠 臘 臼 舅 舊 舡 艮 艱 芎 芥 芩 芹 苛 苟 苦 苽 茄 莖 菅 菊 菌 菓 菫 菰 落 葛 葵 蓋 蕎 蕨 薑 藁 藍 藿 蘭 蘿 虔 蚣 蛟 蝎 螺 蠟 蠱 街 衢 衲 衾 衿 袈 袞 袴 裙 裸 褐 襁 襟 襤 見 規 覡 覲 覺 觀 角 計 記 訣 訶 詭 誇 誡 誥 課 諫 諾 謙 講 謳 謹 譏 警 譴 谷 谿 豈 貢 貫 貴 賈 購 赳 起 跏 距 跨 踞 蹇 蹶 躬 軀 車 軌 軍 軻 較 輕 轎 轟 辜 近 迦 迲 适 逑 逕 逵 過 遣 遽 邏 那 邯 邱 郊 郎 郡 郭 酪 醵 金 鈐 鈞 鉀 鉅 鉗 鉤 銶 鋸 鋼 錡 錤 錦 錮 鍋 鍵 鎌 鎧 鏡 鑑 鑒 鑛 開 間 閘 閣 閨 闕 關 降 階 隔 隙 雇 難 鞏 鞠 鞨 鞫 頃 頸 顆 顧 飢 餃 館 饉 饋 饑 駒 駕 駱 騎 騏 騫 驅 驕 驚 驥 骨 高 鬼 魁 鮫 鯤 鯨 鱇 鳩 鵑 鵠 鷄 鷗 鸞 麒 麴 黔 鼓 龕 龜"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "‾ _ ＿ - － ‐ ‑ — ― 〜 ・ , ， 、 ; ； : ： ! ！ ¡ ? ？ ¿ . ． ‥ … 。 · ＇ ‘ ’ \" ＂ “ ” ( （ ) ） [ ［ ] ］ { ｛ } ｝ 〈 〉 《 》 「 」 『 』 【 】 〔 〕 § ¶ @ ＠ * ＊ / ／ \\ ＼ & ＆ # ＃ % ％ ‰ † ‡ ′ ″ 〃 ※"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "‾ _ ＿ - － — ― 〜 ・ , ， 、 ; ； : ： ! ！ ¡ ? ？ ¿ . ． ‥ … 。 · ＇ ‘ ’ \" ＂ “ ” ( （ ) ） [ ［ ] ］ { ｛ } ｝ 〈 〉 《 》 「 」 『 』 【 】 〔 〕 ¶ @ ＠ * ＊ / ／ \\ ＼ & ＆ # ＃ % ％ 〃 ※"
   index: "ㄱ ㄴ ㄷ ㄹ ㅁ ㅂ ㅅ ㅇ ㅈ ㅊ ㅋ ㅌ ㅍ ㅎ"
 }
 sample_text {
   masthead_full: "모든인간"
   masthead_partial: "은태"
   styles: "모든 인류 구성원의 천부의 존엄성과 동등하고 양도할 수 없는 권리를 인정하는"
   tester: "인권에 대한 무시와 경멸이 인류의 양심을 격분시키는 만행을 초래하였으며, 인간이 언론과 신앙의 자유, 그리고 공포와"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/koi_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/koi_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -13,13 +13,13 @@
   masthead_full: "БбЫы"
   masthead_partial: "Дд"
   styles: "Медбы тӧдны, что морт семьяись быд членлӧн"
   tester: "медбы тӧдны, что колӧ керны быдӧс, медбы мортлӧн пра воэз дозирайтсисӧ"
   poster_sm: "медбы тӧдны,"
   poster_md: "ГЕНЕРАЛЬНӦЙ"
   poster_lg: "Быдӧс"
-  specimen_48: "Быдӧс отирыс чужӧны вольнӧйезӧн да ӧткоддезӧн  достоинствоын"
+  specimen_48: "Быдӧс отирыс чужӧны вольнӧйезӧн да ӧткоддезӧн достоинствоын"
   specimen_36: "Некинӧс оз позь видзны рабствоын нето пӧдан сайын; раб видзӧм да раббезӧн вузасьӧм оз вермӧ вӧвны миян оланын."
-  specimen_32: "Мийӧ быдӧнным законыс одзын ӧткодьӧсь и ӧтмоза  дорйӧмӧсь. Миян быдӧннымлӧн эта Декларация сьӧрті  право дорйыны асьнымӧс быдӧс умӧльсянь, кинсянь бы сія эз лок."
-  specimen_21: "Быд мортлӧн эм право бертны аслыс ӧштӧм правоэз, кӧдна сетӧмӧсь сылӧ конституцияӧн нето законӧн, тӧдчана национальнӧй суддэзын.\nНекинӧс оз позь законтӧг арестуйтны, кутны нето вӧтлыны.\nБыд мортлӧн, кӧр сійӧ винитӧны уголовнӧй статья сьӧрті,  право тӧдны справедливӧй независимӧй судын ассис правоэз да обязанносттез и эм я мыйкӧ сэтшӧмыс, мед сійӧ винитны."
-  specimen_16: "Некин оз вермы дзугны мортлісь ассис да семейнӧй вӧрзьӧтны сылісь оланін, честь да бур ним. Быдыслӧн эм право сайӧвтны асьсӧ вӧрзьӧтлӧммезсянь законӧн.\nБыд мортыс вермӧ асмознас авйыны, совеститчыны да  ны енлӧ; эта правоыс сетӧ вежны ассит ен, мӧднеж вежӧртны олан, ӧтнатлӧ и ӧтлаын мӧдіккезкӧт донтны кӧть кытшӧм енӧс да ассиныт арт, велӧтчыны, юрбитны да чулӧтны религиознӧй да ритуальнӧй обряддэз йӧз дырни нето дзир аскӧттят.\nБыдыс вермӧ артавны асмознас и кӧть кытӧн баитны эта йылісь йӧзлӧ; эта правоыс сетӧ мортыслӧ воля овны аслас юрӧн, повтӧг кошшыны, адззыны да новйӧтны омӧн юӧ да ассис арттэз кыдз сія только кужӧ и кытшӧм бы границаэз сайын эз вӧв."
+  specimen_32: "Мийӧ быдӧнным законыс одзын ӧткодьӧсь и ӧтмоза дорйӧмӧсь. Миян быдӧннымлӧн эта Декларация сьӧрті право дорйыны асьнымӧс быдӧс умӧльсянь, кинсянь бы сія эз лок."
+  specimen_21: "Быд мортлӧн эм право бертны аслыс ӧштӧм правоэз, кӧдна сетӧмӧсь сылӧ конституцияӧн нето законӧн, тӧдчана национальнӧй суддэзын.\nНекинӧс оз позь законтӧг арестуйтны, кутны нето вӧтлыны.\nБыд мортлӧн, кӧр сійӧ винитӧны уголовнӧй статья сьӧрті, право тӧдны справедливӧй независимӧй судын ассис правоэз да обязанносттез и эм я мыйкӧ сэтшӧмыс, мед сійӧ винитны."
+  specimen_16: "Некин оз вермы дзугны мортлісь ассис да семейнӧй вӧрзьӧтны сылісь оланін, честь да бур ним. Быдыслӧн эм право сайӧвтны асьсӧ вӧрзьӧтлӧммезсянь законӧн.\nБыд мортыс вермӧ асмознас авйыны, совеститчыны да ны енлӧ; эта правоыс сетӧ вежны ассит ен, мӧднеж вежӧртны олан, ӧтнатлӧ и ӧтлаын мӧдіккезкӧт донтны кӧть кытшӧм енӧс да ассиныт арт, велӧтчыны, юрбитны да чулӧтны религиознӧй да ритуальнӧй обряддэз йӧз дырни нето дзир аскӧттят.\nБыдыс вермӧ артавны асмознас и кӧть кытӧн баитны эта йылісь йӧзлӧ; эта правоыс сетӧ мортыслӧ воля овны аслас юрӧн, повтӧг кошшыны, адззыны да новйӧтны омӧн юӧ да ассис арттэз кыдз сія только кужӧ и кытшӧм бы границаэз сайын эз вӧв."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kok_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kok_Deva.textproto`

 * *Files 16% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 script: "Deva"
 name: "Konkani"
 population: 4906533
 region: "IN"
 exemplar_chars {
   base: "़ ० १ २ ३ ४ ५ ६ ७ ८ ९ ॐ ं ँ ः अ आ इ ई उ ऊ ऋ ऌ ऍ ए ऐ ऑ ओ औ क {क़} ख {ख़} ग {ग़} घ ङ च छ ज {ज़} झ ञ ट ठ ड {ड़} ढ {ढ़} ण त थ द ध न प फ {फ़} ब भ म य {य़} र ल व श ष स ह ळ ऽ ा ि ी ु ू ृ ॄ ॅ े ै ॉ ो ौ ्"
   auxiliary: "‌‍"
-  numerals: "- ‑ , . % ‰ + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "अ आ इ ई उ ऊ ऋ ऌ ऍ ए ऐ ऑ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल व श ष स ह ळ"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/koo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/koo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kqn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kqn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kqs_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kqs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/krc_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/krc_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kri_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kri_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/krl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/krl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kru_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kru_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ks_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ks_Arab.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 population: 5723030
 region: "GB"
 region: "IN"
 region: "PK"
 exemplar_chars {
   base: "ء آ أ ٲ ؤ ا ب پ ت ث ٹ ج چ ح خ د ذ ڈ ر ز ڑ ژ س ش ص ض ط ظ ع غ ف ق ک گ ل م ن ں ھ ہ و ۄ ۆ ی ۍ ؠ ے"
   auxiliary: "‎‏ َ ُ ِ ٔ ٕ ٟ ٖ ٗ"
-  numerals: "‎ - ‑ , . % ‰ + 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
+  numerals: "‎ - , . % + 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
 }
 sample_text {
   masthead_full: "سریل"
   masthead_partial: "کھ"
   styles: "سٔری لُکھ چهہٕ حقوٗق تِہ عزت لِحاظٕ ہِہیٖ ژامِت تِمن"
   tester: "سٔری لُکھ چهہٕ حقوٗق تِہ عزت لِحاظٕ ہِہیٖ ژامِت. تِمن چه‍ہِ ضمير تِہ عَقل دِنِ"
   poster_sm: "سٔری لُکھ چهہٕ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ksh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ksh_Latn.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 autonym: "Kölsch"
 population: 240479
 region: "DE"
 exemplar_chars {
   base: "a å ä æ b c d e ë ė f g h i j k l m n o ö œ p q r s ß t u ů ü v w x y z"
   auxiliary: "á à ă â ã ā ç é è ĕ ê ē ğ í ì ĭ î ï ī ĳ ı ł ñ ó ò ŏ ô ø ō ú ù ŭ û ū ÿ"
   marks: "◌̇ ◌̈ ◌̊ ◌̀ ◌́ ◌̂ ◌̃ ◌̄ ◌̆ ◌̧"
-  numerals: "  , % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "_ ‐ – — ⸗ , ; : ! ? . … \' ‘ ‚ \" “ „ ( ) [ ] { } § @ * / & # % † ‡ ° < = > ~"
+  numerals: ", % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "_ – — ⸗ , ; : ! ? . … \' ‘ ‚ \" “ „ ( ) [ ] { } @ * / & # % ° < = > ~"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ksw_Mymr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ksw_Mymr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ktu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ktu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ku_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ku_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ku_Yezi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ku_Yezi.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 language: "ku"
 script: "Yezi"
 name: "Kurdish, Yezidi"
 region: "GE"
 sample_text {
   masthead_full: "𐺍𐺁𐺄𐺀"
   masthead_partial: "𐺍𐺁"
-  styles: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
-  tester: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆"
-  poster_sm: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁"
-  poster_md: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍"
+  styles: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
+  tester: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆"
+  poster_sm: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁"
+  poster_md: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍"
   poster_lg: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍"
-  specimen_48: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍"
-  specimen_36: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
-  specimen_32: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
-  specimen_21: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
-  specimen_16: " 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
+  specimen_48: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍"
+  specimen_36: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
+  specimen_32: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
+  specimen_21: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
+  specimen_16: "𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀 𐺀𐺁𐺍𐺄𐺆𐺍𐺦𐺍 𐺀𐺍𐺁 𐺆𐺀𐺆𐺄𐺁𐺆 𐺦𐺆𐺦 𐺦𐺀𐺍 𐺍𐺦𐺆𐺍𐺁𐺀𐺄𐺍𐺀 𐺆𐺆𐺀𐺀"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kwi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kwi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ky_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ky_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ky_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ky_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Кыргызча"
 population: 2863152
 region: "KG"
 exemplar_chars {
   base: "а б г д е ё ж з и й к л м н ң о ө п р с т у ү х ч ш ъ ы э ю я"
   auxiliary: "в ф ц щ ь"
   marks: "◌̆ ◌̈"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
   index: "А Б В Г Д Е Ё Ж З И Й К Л М Н Ң О Ө П Р С Т У Ү Ф Х Ц Ч Ш Щ Ъ Ы Ь Э Ю Я"
 }
 sample_text {
   masthead_full: "БбАа"
   masthead_partial: "Рр"
   styles: "Адамзат үй бүлөсүнүн бардык мүчөлөрүнөтаандык"
   tester: "адам укуктарын этибарга албоо жана жеккөрүү адамзатынын абийирин"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kyu_Kali.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kyu_Kali.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kyw_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kyw_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/kyw_Orya.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/kyw_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/la_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/la_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lad_Hebr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lad_Hebr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lad_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lad_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lah_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lah_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lb_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Lëtzebuergesch"
 population: 421015
 region: "LU"
 exemplar_chars {
   base: "a ä b c d e é ë f g h i j k l m n o p q r s t u v w x y z"
   auxiliary: "á à ă â å ã ā æ ç è ĕ ê ē ğ í ì ĭ î ï İ ī ı ñ ó ò ŏ ô ö ø ō œ ş ß ú ù ŭ û ü ū ÿ"
   marks: "◌̀ ◌́ ◌̂ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Mm"
   styles: "Well d\'Unerkennong vun der Dignitéit, déi all"
   tester: "Well et do, wou d\'Mënscherechter nët unerkannt an nët respektéiert"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lfn_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lfn_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lfn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lfn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lg_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lhm_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lhm_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lia_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lia_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lif_Limb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lif_Limb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lij_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lij_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lis_Lisu.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lis_Lisu.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/liv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/liv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ljp_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ljp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lkt_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lkt_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Lakȟótiyapi"
 population: 8315
 region: "US"
 exemplar_chars {
   base: "a á {aŋ} b č {čh} {čʼ} e é g ǧ h ȟ i í {iŋ} k {kh} {kȟ} {kʼ} l m n ŋ o ó p {ph} {pȟ} {pʼ} s š t {th} {tȟ} {tʼ} u ú {uŋ} w y z ž ʼ"
   auxiliary: "c d f {ȟʼ} j q r {sʼ} {šʼ} v x"
   marks: "◌́ ◌̌"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . \" “ ” ( ) [ ] @ * / & #"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . \" “ ” ( ) [ ] @ * / & #"
   index: "A B Č E G Ǧ H Ȟ I K L M N Ŋ O P S Š T U W Y Z Ž"
 }
 sample_text {
   masthead_full: "WwIi"
   masthead_partial: "Čč"
   styles: "Wičháša na wíŋyaŋ otóiyohi iglúhapi na iyéhaŋyaŋ"
   tester: "Wičháša na wíŋyaŋ otóiyohi iglúhapi na iyéhaŋyaŋ wówažapi. Tȟaŋmáhel"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lld_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lld_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lmo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lmo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ln_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ln_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 region: "CD"
 region: "CF"
 region: "CG"
 exemplar_chars {
   base: "a A á Á â Â ǎ Ǎ b B c C d D e E é É ê Ê ě Ě ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̂} {Ɛ̂} {ɛ̌} {Ɛ̌} f F g G {gb} {GB} h H i I í Í î Î ǐ Ǐ k K l L m M {mb} {MB} {mp} {MP} n N {nd} {ND} {ng} {NG} {nk} {NK} {ns} {NS} {nt} {NT} {ny} {NY} {nz} {NZ} o O ó Ó ô Ô ǒ Ǒ ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̂} {Ɔ̂} {ɔ̌} {Ɔ̌} p P r R s S t T u U ú Ú v V w W y Y z Z"
   auxiliary: "j J q Q x X"
   marks: "◌́ ◌̂ ◌̌"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E Ɛ F G {Gb} H I K L M {Mb} {Mp} N {Nd} {Ng} {Nk} {Ns} {Nt} {Ny} {Nz} O Ɔ P R S T U V W Y Z"
 }
 sample_text {
   masthead_full: "BbAa"
   masthead_partial: "Tt"
   styles: "Na botáláká ’te kondima limɛmya ya bato nyɔ́nsɔ"
   tester: "Na botáláká ’te na káti ya Mokandá ya Mibéko ya Lisangá ya Bikólo"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lns_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lns_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lo_Laoo.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lo_Laoo.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "ພາສາລາວ"
 population: 5138706
 region: "LA"
 exemplar_chars {
   base: "່ ້ ໊ ໋ ໌ ໍ ໆ ກ ຂ ຄ ງ ຈ ສ ຊ ຍ ດ ຕ ຖ ທ ນ ບ ປ ຜ ຝ ພ ຟ ມ ຢ ຣ ລ ວ ຫ ໜ ໝ ອ ຮ ຯ ະ ັ າ ຳ ິ ີ ຶ ື ຸ ູ ົ ຼ ຽ ເ ແ ໂ ໃ ໄ"
   auxiliary: "​ ໐ ໑ ໒ ໓ ໔ ໕ ໖ ໗ ໘ ໙"
   marks: "◌ັ ◌ິ ◌ີ ◌ຶ ◌ື ◌ຸ ◌ູ ◌ົ ◌ຼ ◌່ ◌້ ◌໊ ◌໋ ◌໌ ◌ໍ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "ກ ຂ ຄ ງ ຈ ສ ຊ ຍ ດ ຕ ຖ ທ ນ ບ ປ ຜ ຝ ພ ຟ ມ ຢ ຣ ລ ວ ຫ {ຫງ} {ຫຍ} {ຫນ} {ຫມ} {ຫລ} {ຫວ} ອ ຮ"
 }
 sample_text {
   masthead_full: "ມະນດ"
   masthead_partial: "ເກ"
   styles: "ດ້ວຍເຫດວ່າ ການຮັບຮູ້ກຽດຕິສັກອັນມີປະຈຳຢູ່ຕົວບຸກຄົນໃນວົງສະກຸນຂອງມະນຸດທຸກໆຄົນ"
   tester: "ດ້ວຍເຫດວ່າ: ໃນກົດໝາຍໂລກນັ້ນປະຊາຊົນແຫ່ງສະຫະປະຊາຊາດໄດ້ປະກາດຢືນຢັນຄວາມເຊື່ອຖືຂອງຕົນອີກໃນສິດສຳຄັນຂອງມະນຸດ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lob_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lob_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lot_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lot_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/loz_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/loz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lrc_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lrc_Arab.textproto`

 * *Files 25% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 name: "Northern Luri"
 population: 2020512
 region: "IQ"
 region: "IR"
 exemplar_chars {
   base: "ٙ ٛ آ أ ؤ ئ ا ب پ ت ث ج چ ح خ د ذ ر ز ژ س ش ص ض ط ظ ع غ ف ڤ ق ک گ ل م ن ھ ە و ۉ ۊ ی ؽ"
   auxiliary: "​‌‍‎‏ ً ٌ ٍ َ ُ ِ ّ ْ ٔ إ ة ك ه ى ي"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ ، ٫ ٬ ؛ : ! ؟ . … ‹ › « » ( ) [ ] * / \\"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- ، ٫ ٬ ؛ : ! ؟ . … ‹ › « » ( ) [ ] * / \\"
   index: "آ ا ب پ ت ث ج چ ح خ د ذ ر ز ژ س ش ص ض ط ظ ع غ ف ق ک گ ل م ن ھ و ی"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lt_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lt_Latn.textproto`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 name: "Lithuanian"
 autonym: "Lietuviškai"
 population: 2357094
 region: "LT"
 region: "PL"
 exemplar_chars {
   base: "a ą b c č d e ę ė f g h i į y j k l m n o p r s š t u ų ū v z ž"
-  auxiliary: "á à ã {ą́} {ą̃} {ch} {dz} {dž} é è ẽ {ę́} {ę̃} {ė́} {ė̃} {i̇́}í {i̇̀}ì {i̇̃}ĩ {į́}{į̇́} {į̃}{į̇̃} {j̃}{j̇̃} {l̃} {m̃} ñ ó ò õ q {r̃} ú ù ũ {ų́} {ų̃} {ū́} {ū̃} w x {i̇́} {i̇̀} {i̇̃} {į́} {į̇́} {į̃} {į̇̃} {j̃} {j̇̃}"
+  auxiliary: "á à ã {ą́} {ą̃} {ch} {dz} {dž} é è ẽ {ę́} {ę̃} {ė́} {ė̃} {i̇́} í {i̇̀} ì {i̇̃} ĩ {į́} {į̇́} {į̃} {į̇̃} {j̃} {j̇̃} {l̃} {m̃} ñ ó ò õ q {r̃} ú ù ũ {ų́} {ų̃} {ū́} {ū̃} w x"
   marks: "◌̄ ◌̇ ◌̌ ◌̨"
-  numerals: "  , % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … “ „ ( ) [ ] { }"
+  numerals: ", % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … “ „ ( ) [ ] { }"
   index: "A Ą B C Č D E Ę Ė F G H I Į Y J K L M N O P R S Š T U Ų Ū V Z Ž"
 }
 sample_text {
   masthead_full: "VvIi"
   masthead_partial: "Ss"
   styles: "Atsižvelgdama į tai, kad visiems žmonių giminės"
   tester: "atsižvelgdama į tai, kad žmogaus teisių visiškas nepaisymas ir"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lu_Latn.textproto`

 * *Files 20% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 autonym: "Kiluba"
 population: 2340939
 region: "CD"
 exemplar_chars {
   base: "a A á Á à À b B c C d D e E é É è È ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̀} {Ɛ̀} f F h H i I í Í ì Ì j J k K l L m M n N {ng} {NG} {ny} {NY} o O ó Ó ò Ò ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̀} {Ɔ̀} p P {ph} {PH} q Q s S {shi} {SHI} t T u U ú Ú ù Ù v V w W y Y z Z"
   auxiliary: "g G r R x X"
   marks: "◌̀ ◌́"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F H I J K L M N O P Q S T U V W Y Z"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lua_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lua_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lue_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lue_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lun_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lun_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lus_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lut_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lut_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/lv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/lv_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Latviešu"
 population: 1147550
 region: "LV"
 exemplar_chars {
   base: "a ā b c č d e ē f g ģ h i ī j k ķ l ļ m n ņ o p r s š t u ū v z ž"
   auxiliary: "y ō q ŗ w x"
   marks: "◌̄ ◌̌ ◌̧"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ ‚ \" “ ” „ ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ ‚ \" “ ” „ ( ) [ ] @ * / & #"
   index: "A Ā B C Č D E Ē F G Ģ H I Ī Y J K Ķ L Ļ M N Ņ O P Q R S Š T U Ū V W X Z Ž"
 }
 sample_text {
   masthead_full: "VvIi"
   masthead_partial: "Ss"
   styles: "Ievērojot, ka visiem cilvēku sabiedrības locekļiem"
   tester: "ievērojot, ka cilvēku tiesību necienīšana un nicināšana noved"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mad_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mad_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mag_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mag_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mai_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mai_Deva.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 region: "IN"
 region: "NP"
 exemplar_chars {
   base: "़ ं ः क {क्ष} ख ग घ च छ ज {ज्ञ} झ ञ ट ठ ड {डं} ढ ण त {त्र} थ द ध न प फ ब भ म य र ल व श {श्र} ष स ह ा ि ी ु ू े ै ो ौ"
   auxiliary: "अ {अं} {अः} आ इ ई उ ऊ ऋ ऌ ॡ ए ऐ ओ औ"
   marks: "◌ँ ◌ं ◌ः ◌ऺ ◌ऻ ◌़ ◌ा ◌ि ◌ी ◌ु ◌ू ◌ृ ◌ॆ ◌े ◌ै ◌ॊ ◌ो ◌ौ ◌् ◌ॏ"
   numerals: "० १ २ ३ ४ ५ ६ ७ ८ ९ 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "_ - ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } § @ * / \\ & # ′ ″ ` + | ~"
+  punctuation: "_ - – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } @ * / \\ & #` + | ~"
   index: "़ अ {अं} {अः} आ इ ई उ ऊ ऋ ऌ ॡ ए ऐ ओ औ क {क्ष} ख ग घ च छ ज {ज्ञ} झ ञ ट ठ ड {डं} ढ ण त {त्र} थ द ध न प फ ब भ म य र ल व श {श्र} ष स ह"
 }
 sample_text {
   masthead_full: "सभमन"
   masthead_partial: "वज"
   styles: "जेँ कि मानव परिवारक सकल सदस्यक जन्मजात गरिमा आओर समान"
   tester: "जेँ कि मानवाधिकारक अवहेलना आʼ अवमाननाक परिणाम होइछ एहन नृशंस आचरण जाहिसँ मानवक अन्तःकरण"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mak_Maka.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mak_Maka.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mam_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mam_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/man_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/man_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mas_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mas_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/maz_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/maz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mcd_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mcd_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mcf_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mcf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/men_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/men_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/men_Mend.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/men_Mend.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mfe_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mfe_Latn.textproto`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Morisyen"
 preferred_name: "Mauritian Creole"
 autonym: "Kreol Morisien"
 population: 1241433
 region: "MU"
 exemplar_chars {
   base: "a b c d e f g h i j k l m n o p r s t u v w x y z"
-  numerals: "  - ‑ . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N O P R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtOo"
   masthead_partial: "Uu"
   styles: "Tou bann imin ne lib ek egal dan dinite ek"
   tester: "Tou bann imin ne lib ek egal dan dinite ek dan bann drwa. Zot"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mfq_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mfq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mg_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mg_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Malagasy"
 population: 24260130
 region: "MG"
 exemplar_chars {
   base: "a A à À â Â b B d D e E é É è È ê Ê ë Ë f F g G h H i I ì Ì î Î ï Ï j J k K l L m M n N ñ Ñ o O ô Ô p P r R s S t T v V y Y z Z"
   auxiliary: "c C q Q u U w W x X"
   marks: "◌̀ ◌́ ◌̂ ◌̃ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B D E F G H I J K L M N O P R S T V Y Z"
 }
 sample_text {
   masthead_full: "TtEe"
   masthead_partial: "Rr"
   styles: "Heverina fa ny fankatoavana ny fahamendrehan\'olombelona"
   tester: "Firenena Mikambana izy amin\'izany, Heverina fa tao anatin\'ny Dina"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mgo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mgo_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 autonym: "Mɨta’"
 population: 130401
 region: "CM"
 exemplar_chars {
   base: "a A à À b B {ch} {CH} d D e E è È ə Ə {ə̀} {Ə̀} f F g G {gh} {GH} i I ì Ì j J k K m M n N ŋ Ŋ o O ò Ò ɔ Ɔ {ɔ̀} {Ɔ̀} p P r R s S t T u U ù Ù w W y Y z Z ʼ"
   auxiliary: "c C h H l L q Q v V x X"
   marks: "◌̀"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   punctuation: ", ; : ! ? . \' ‘ ’ \" “ ”"
   index: "A B {CH} D E Ə F G {GH} I J K M N Ŋ O Ɔ P R S T U W Y Z ʼ"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mic_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mic_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/min_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/min_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/min_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/min_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/miq_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/miq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mis_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mis_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mis_Hatr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mis_Hatr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mis_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mis_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mis_Nshu.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mis_Nshu.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mk_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mk_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 region: "AL"
 region: "GR"
 region: "MK"
 exemplar_chars {
   base: "а б в г д ѓ е ж з ѕ и ј к л љ м н њ о п р с т ќ у ф х ц ч џ ш"
   auxiliary: "ѐ ѝ"
   marks: "◌́ ◌̀"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] { }"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] { }"
   index: "А Б В Г Д Ѓ Е Ж З Ѕ И Ј К Л Љ М Н Њ О П Р С Т Ќ У Ф Х Ц Ч Џ Ш"
 }
 sample_text {
   masthead_full: "СсИи"
   masthead_partial: "Тт"
   styles: "Бидејќи признавањето на вроденото достоинство,"
   tester: "Бидејќи непочитувањето и омаловажувањето на човековите права"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ml_Mlym.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ml_Mlym.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 region: "MY"
 region: "QA"
 region: "SG"
 exemplar_chars {
   base: "‌‍ ഃ അ ആ ഇ ഈ ഉ ഊ ഋ ൠ ഌ ൡ എ ഏ ഐ ഒ ഓ ഔ ക ൿ ഖ ഗ ഘ ങ ച ഛ ജ ഝ ഞ ട ഠ ഡ ഢ ണ ൺ ത ഥ ദ ധ ന ൻ പ ഫ ബ ഭ മ ം യ ര ർ ല ൽ വ ശ ഷ സ ഹ ള ൾ ഴ റ ാ ി ീ ു ൂ ൃ െ േ ൈ ൊ ോ ൌ ൗ ്"
   auxiliary: ""
   marks: "◌ം ◌ഃ ◌ാ ◌ി ◌ീ ◌ു ◌ൂ ◌ൃ ◌െ ◌േ ◌ൈ ◌് ◌ൗ"
-  numerals: "- ‑ , . % ‰ + 0൦ 1൧ 2൨ 3൩ 4൪ 5൫ 6൬ 7൭ 8൮ 9൯"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0൦ 1൧ 2൨ 3൩ 4൪ 5൫ 6൬ 7൭ 8൮ 9൯"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "അ ആ ഇ ഈ ഉ ഊ ഋ എ ഏ ഐ ഒ ഓ ഔ ക ഖ ഗ ഘ ങ ച ഛ ജ ഝ ഞ ട ഠ ഡ ഢ ണ ത ഥ ദ ധ ന പ ഫ ബ ഭ മ യ ര ല വ ശ ഷ സ ഹ ള ഴ റ"
 }
 sample_text {
   masthead_full: "മനഷയ"
   masthead_partial: "രല"
   styles: "മനുഷ്യ സമുദായത്തിൻ്റെ ജന്മസിദ്ധമായ അന്തസ്സും സമാവകാശവും ലോകത്തിൽ"
   tester: "മനുഷ്യാവകാശങ്ങളെ കുറിക്കുന്ന ഈ പൊതുപ്രഖ്യാപനത്തെ ഒരു പ്രമാണമായി കരുതി ഏതൊരു വ്യക്തിക്കും സംഘടനക്കും"
   poster_sm: "ജാതി, മതം, നിറം, ഭാഷ,"
-  poster_md: " സ്വയരക്ഷാബോധത്തോടും"
+  poster_md: "സ്വയരക്ഷാബോധത്തോടും"
   poster_lg: "അന്തസ്സോടും"
   specimen_48: "നിയമത്തിനു മുൻപിൽ എല്ലാവരും തുല്യരാണ്‌. യാതൊരു ഭേദവും കൂടാതെ നിയമാനുസൃതമായ രക്ഷക്ക്‌ എല്ലാവർക്കും അർഹതയുള്ളതുമാണ്‌."
   specimen_36: "വ്യവസ്ഥാപിതമായ ഭരണത്താലും നിയമത്താലും സമ്മതിക്കപ്പെട്ട അവകാശങ്ങളെ ലംഘിച്ചു ആരെങ്കിലും പ്രവർത്തിക്കുകയാണെങ്കിൽ നിയമാനുസൃതമായ പ്രതിവിധി തേടുന്നതിനുള്ള അധികാരം എല്ലാവർക്കും ഉണ്ടായിരിക്കുന്നതാണ്‌."
   specimen_32: "സ്വതന്ത്രചിന്തക്കും സ്വതന്ത്ര മതവിശ്വാസത്തിനും എല്ലാവർക്കും അധികാരമുണ്ട്‌. ഒറ്റക്കായോ കൂട്ടമായിത്തന്നേയോ മതം മാറുവാനും പരസ്യമായോ രഹസ്യമായോ തൻ്റെ മതവിശ്വാസങ്ങളെ പ്രകടിപ്പിക്കുവാനും ആചരിക്കുവാനും ആരാധിക്കാനുമുള്ള അധികാരവും ഇതിൽതന്നെ അടങ്ങിയിരിക്കുന്നു."
   specimen_21: "സ്വതന്ത്രമായ അഭിപ്രായപ്രകടനത്തിന്നു എല്ലാവർക്കും അധികാരമുണ്ട്‌. അതായത്‌ യാതൊരു തടസ്സവുംകൂടാതെ അഭിപ്രായങ്ങളെ ആരായുവാനും മറ്റുള്ളവർക്ക്‌ ഏതൊരുപാധിയിൽ കൂടിയും യാതൊരതിർത്തികളെയും കണക്കാക്കാതെ എല്ലായിടത്തുമെത്തിക്കുവാനുള്ള അധികാരവുമുണ്ടെന്നു താൽപ്പര്യം.\nസമുദായത്തിലെ ഒരംഗമായതുകൊണ്ടു സമുദായത്തിൽനിന്നുമുള്ള രക്ഷക്ക്‌ ഏതൊരാൾക്കും അർഹതയുണ്ട്‌. അതാതു രാജ്യത്തിൻ്റെ കഴിവുകൾക്കനുസരിച്ചും ദേശീയ സംരംഭങ്ങളെക്കൊണ്ടും അന്തർദേശീയ സഹകരണം കൊണ്ടും അവരവരുടെ അന്തസ്സിന്നു അപരിത്യാജ്യമായ സാമുദായികവും സാംസ്കാരികവും സാമ്പത്തികവുമായ അവകാശങ്ങളെ നേടുന്നതിന്നും തൻ്റെ സ്വതന്ത്രമായ വ്യക്തിത്വത്തെ പരിപോഷിപ്പിക്കുന്നതിന്നും ഏതൊരാൾക്കും അധികാരമുള്ളതാണ്‌."
   specimen_16: "ന്യായമായ പ്രവൃത്തിസമയം ഇടക്കിടക്കു ശമ്പളത്തോടുകൂടിയ ഒഴിവുദിവസങ്ങൾ, ഒഴിവുസമയം, വിശ്രമം ഇതുകൾക്ക്‌ ഏതൊരാൾക്കും അവകാശമുള്ളതാണ്‌.\nഈ പ്രഖ്യാപനത്തിൽ പ്രതിപാദിച്ചിട്ടുള്ള അധികാരസ്വാതന്ത്ര്യങ്ങളെ കൈവരുത്തക്ക രീതിയിലുള്ള സാമുദായികവും അന്തർരാഷ്ട്രീയവുമായ ഒരു ജീവിതത്തോതിന്ന് എല്ലാവരും അർഹരാണ്‌.\nഒരു രാജ്യത്തിന്നോ, വകുപ്പിന്നോ, വ്യക്തിക്കോ ഇഷ്ടമുള്ള പ്രവൃത്തികളിലെല്ലാമേർപ്പെടാമെന്നോ, ഇതിലടങ്ങിയിരിക്കുന്ന തത്വങ്ങൾക്കെതിരായിത്തന്നെ എന്തെങ്കിലും പ്രവർത്തിക്കാമെന്നോ ഉള്ള രീതിയിൽ ഈ പ്രഖ്യാപനത്തെ വ്യാഖ്യാനിക്കാൻ പാടുള്ളതല്ല.\nമനുഷ്യാവകാശങ്ങളെ കുറിക്കുന്ന ഈ പൊതുപ്രഖ്യാപനത്തെ ഒരു പ്രമാണമായി കരുതി ഏതൊരു വ്യക്തിക്കും സംഘടനക്കും അവരുടെ പ്രയത്നംകൊണ്ടു മനുഷ്യാവകാശങ്ങളെ ബഹുമാനിച്ചു വകവെച്ചു കൊടുക്കാൻ യത്നിക്കേണ്ടതാണ്‌. ക്രമേണ രാഷ്ട്രീയവും അന്തർരാഷ്ട്രീയവുമായ പ്രവർത്തനങ്ങളെക്കൊണ്ടു ഈ പ്രഖ്യാപനത്തിലടങ്ങിയിരിക്കുന്ന അവകാശങ്ങളെ ഐക്യരാഷ്ട്ര സംഘടനയിലെ അംഗങ്ങളെക്കൊണ്ടും അവരുടെ അധികാരത്തിലിരിക്കുന്ന ജനങ്ങളെക്കൊണ്ടും ഫലപ്രദമാകത്തക്ക രീതിയിൽ അംഗീകരിപ്പിക്കുവാൻ ശ്രമിക്കേണ്ടതുമാണ്‌."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mn_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mn_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 2948393
 region: "MN"
 region: "RU"
 exemplar_chars {
   base: "а б в г д е ё ж з и й к л м н о ө п р с т у ү ф х ц ч ш щ ъ ы ь э ю я"
   auxiliary: "ә җ ӊ һ"
   marks: "◌̆ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "А Б В Г Д Е Ж З И Й К Л М Н О Ө П Р С Т У Ү Ф Х Ц Ч Ш Щ Ъ Ы Ь Э Ю Я"
 }
 sample_text {
   masthead_full: "ХхҮү"
   masthead_partial: "Нн"
   styles: "Хүн төрөлхтөний гэр бүлийн бүх гишүүнд угаас"
   tester: "хүний эрхийг үл тоомсорлох, басамжлах нь зон олны жигшлийг төрүүлсэн"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mn_Mong.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mn_Mong.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mni_Mtei.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mni_Mtei.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mnw_Mymr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mnw_Mymr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mor_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mor_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mos_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mos_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mr_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mr_Deva.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "मराठी"
 population: 92826300
 region: "IN"
 exemplar_chars {
   base: "़ ॐ ं ँ ः अ आ इ ई उ ऊ ऋ ऌ ऍ ए ऐ ऑ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ऱ ल व श ष स ह ळ ऽ ा ि ी ु ू ृ ॄ ॅ े ै ॉ ो ौ ्"
   auxiliary: "‌‍"
   marks: "◌ँ ◌ं ◌ः ◌़ ◌ा ◌ि ◌ी ◌ु ◌ू ◌ृ ◌े ◌ै ◌ो ◌ौ ◌्"
-  numerals: "- ‑ , . % ‰ + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & # ′ ″"
+  numerals: "- , . % + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "‍ ॐ ं ः अ आ इ ई उ ऊ ऋ ऌ ए ऐ ऑ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल व श ष स ह ळ ऽ ॅ ्"
 }
 sample_text {
   masthead_full: "सरवम"
   masthead_partial: "नय"
   styles: "ज्या अर्थी मानव कुटुँवातील सर्व व्यक्तींची स्वाभाविक प्रतिष्ठा व"
   tester: "ज्या अर्थी, मानवी अधिकारांची अबहेलना व अप्रतिष्ठा झाल्याने अमानुष कृत्ये घडून आली आणि त्यायोगे"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mr_Modi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mr_Modi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mrw_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mrw_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mrw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mrw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ms_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ms_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mt_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mt_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Malti"
 population: 457267
 region: "MT"
 exemplar_chars {
   base: "a à b ċ d e è f ġ g {għ} h ħ i ì j k l m n o ò p q r s t u ù v w x ż z"
   auxiliary: "c y"
   marks: "◌̀ ◌̂ ◌̇"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ , ; : ! ? . \' ‘ ’ \" “ ” ( ) [ ] { }"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- , ; : ! ? . \' ‘ ’ \" “ ” ( ) [ ] { }"
   index: "A B Ċ C D E F Ġ G {GĦ} H Ħ I {IE*} J K L M N O P Q R S T U V W X Y Ż Z"
 }
 sample_text {
   masthead_full: "IiLl"
   masthead_partial: "Bb"
   styles: "Billi l-għarfien tad-dinjità proprja tal-membri"
   tester: "Billi t-tkasbir u ż-żebliħ tal-jeddijiet tal-bniedem ġabu magħhom"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mto_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mto_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mui_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mui_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mus_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mxi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mxi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mxv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mxv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/my_Mymr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/my_Mymr.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "မြန်မာ"
 population: 36559231
 region: "BD"
 region: "MM"
 exemplar_chars {
   base: "က ခ ဂ ဃ င စ ဆ ဇ ဈ ဉ ည ဋ ဌ ဍ ဎ ဏ တ ထ ဒ ဓ န ပ ဖ ဗ ဘ မ ယ ရ လ ဝ သ ဟ ဠ အ ဣ ၏ ဤ ဥ ဦ ဧ ဩ ဪ ာ ါ ိ ီ ု ူ ေ ဲ ံ ဿ ျ ြ ွ ှ ္ ် ့ း"
   auxiliary: "၀႐ ၁႑ ၂႒ ၃႓ ၄႔ ၅႕ ၆႖ ၇႗ ၈႘ ၉႙ ၵ ၚ ၽ ၾ ၐ ၑ ၥ ဨ ဢ ၒ ၓ ၔ ၕ ဳ ၖ ၗ ၘ ၙ ဴ ၢ ႆ ၤ ႈ ႊ ႏ"
-  numerals: "- ‑ , . % ‰ + 0၀ 1၁ 2၂ 3၃ 4၄ 5၅ 6၆ 7၇ 8၈ 9၉"
+  numerals: "- , . % + 0၀ 1၁ 2၂ 3၃ 4၄ 5၅ 6၆ 7၇ 8၈ 9၉"
   punctuation: "၊ ။ ‘ ’ “ ”"
   index: "က ခ ဂ ဃ င စ ဆ ဇ ဈ ဉ ည ဋ ဌ ဍ ဎ ဏ တ ထ ဒ ဓ န ပ ဖ ဗ ဘ မ ယ ရ လ ဝ သ ဟ ဠ အ"
 }
 sample_text {
   masthead_full: "လတငသ"
   masthead_partial: "ညပ"
   styles: "လူခပ်သိမ်း၏ မျိုးရိုးဂုဏ်သိက္ခာနှင့်တကွ လူတိုင်းအညီအမျှခံစားခွင့်ရှိသည့် အခွင့်အရေးများကို"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/myz_Mand.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/myz_Mand.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/mzi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/mzi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nan_Hans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nan_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nan_Hant.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nan_Hant.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nap_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nap_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nba_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nba_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nds_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nds_Latn.textproto`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 script: "Latn"
 name: "Low German"
 autonym: "Niedersächsisch"
 population: 11520008
 region: "DE"
 region: "NL"
 exemplar_chars {
-  base: "a å ä b c d e f g h i j k l m n o ö p q r s t u ü v w x y z"
+  base: "a å ä b c d e f g h i j k l m n o ö p q r s ß t u ü v w x y z"
   auxiliary: "á à ă â ā æ ç é è ĕ ê ë ę ē í ì ĭ î ï ī ñ ó ò ŏ ô ø ō œ ú ù ŭ û ū ÿ"
   marks: "◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S ẞ T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Dd"
   styles: "Vunwegen wat dat Anerkennen vun de Wüürd,"
   tester: "vunwegen wat dat Verkennen un Minnachten vun de Minschen rechten"
   poster_sm: "vunwegen wat"
   poster_md: "vunwegen"
   poster_lg: "All"
   specimen_48: "vunwegen wat de Völker vun de Vereenten Natschonen mit düsse"
   specimen_36: "Vunwegen wat dat Anerkennen vun de Wüürd, mit de all Minschen baren sünd, un de Rechten, de all Maten vun"
-  specimen_32: "vunwegen wat dat nödig is, de Minschenrechten dörch dat Regeern vun’t Recht Schuul  geven, dat de Minsch nich dwungen  as lest Middel Wedderpart to hollen Tyrannei un Ünnerdrücken,"
-  specimen_21: "Vunwegen wat dat Anerkennen vun de Wüürd, mit de all Minschen baren sünd, un de Rechten, de all Maten vun de Gemeenschupp vun de Minschen hebbt un de gliek un nich to verköpen sünd, de Grundlaag vun Frieheit un Freden in de Welt is, un wat dat recht und billig togeiht,\nvunwegen wat dat nödig is, de Minschenrechten dörch dat Regeern vun’t Recht Schuul  geven, dat de Minsch nich dwungen  as lest Middel Wedderpart to hollen Tyrannei un Ünnerdrücken,"
+  specimen_32: "vunwegen wat dat nödig is, de Minschenrechten dörch dat Regeern vun’t Recht Schuul geven, dat de Minsch nich dwungen as lest Middel Wedderpart to hollen Tyrannei un Ünnerdrücken,"
+  specimen_21: "Vunwegen wat dat Anerkennen vun de Wüürd, mit de all Minschen baren sünd, un de Rechten, de all Maten vun de Gemeenschupp vun de Minschen hebbt un de gliek un nich to verköpen sünd, de Grundlaag vun Frieheit un Freden in de Welt is, un wat dat recht und billig togeiht,\nvunwegen wat dat nödig is, de Minschenrechten dörch dat Regeern vun’t Recht Schuul geven, dat de Minsch nich dwungen as lest Middel Wedderpart to hollen Tyrannei un Ünnerdrücken,"
   specimen_16: "Vunwegen wat dat Anerkennen vun de Wüürd, mit de all Minschen baren sünd, un de Rechten, de all Maten vun de Gemeenschupp vun de Minschen hebbt un de gliek un nich to verköpen sünd, de Grundlaag vun Frieheit un Freden in de Welt is, un wat dat recht und billig togeiht,\nvunwegen wat dat Verkennen un Minnachten vun de Minschen rechten to unminschlich Doon föhrt hett, un dat Geweten vun de Minschen daarvun vull is vun Schann, is dat vör nehmste Wark vun de Minschen dat Buen vun een Welt, wo elk un een seggen un gloven dröff, wat he will un he frie is vun Bang sien un Noot,"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ne_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ne_Deva.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 region: "BT"
 region: "IN"
 region: "NP"
 exemplar_chars {
   base: "़ ँ ं ः ॐ अ आ इ ई उ ऊ ऋ ऌ ऍ ए ऐ ऑ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल ळ व श ष स ह ऽ ा ि ी ु ू ृ ॄ ॅ े ै ॉ ो ौ ्"
   auxiliary: "‌‍"
   marks: "◌ँ ◌ं ◌ः ◌़ ◌ा ◌ि ◌ी ◌ु ◌ू ◌ृ ◌े ◌ै ◌ो ◌ौ ◌्"
-  numerals: "- ‑ , . % ‰ + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
-  punctuation: "- ‑ — , ; ! ? । \' ‘ ’ \" “ ” ( ) [ ] { }"
+  numerals: "- , . % + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
+  punctuation: "- — , ; ! ? । \' ‘ ’ \" “ ” ( ) [ ] { }"
   index: "अ आ इ ई उ ऊ ऋ ए ऐ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल व श ष स ह"
 }
 sample_text {
   masthead_full: "सबवय"
   masthead_partial: "कत"
   styles: "मानव परिवारका सबै सदस्यहरूको अन्तर्निहित मान तथा सम्मान र"
   tester: "मानव अधिकारहरू प्रति अवहेलना तथा अनादरको परिणामबाटै नै काम भड मानव जातिको अन्त स्करणमा"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/new_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/new_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/new_Newa.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/new_Newa.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ng_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ng_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nhn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nhn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nio_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nio_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/niu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/niu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/njo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/njo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nku_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nku_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nl_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 region: "CW"
 region: "DE"
 region: "FR"
 region: "NL"
 region: "SR"
 region: "SX"
 exemplar_chars {
-  base: "a á ä b c d e é ë f g h i í ï {ij} {íj́} j k l m n o ó ö p q r s t u ú ü v w x y z"
+  base: "a á ä b c d e é ë f g h i í ï {ij} {íj} {íj́} j k l m n o ó ö p q r s t u ú ü v w x y z"
   auxiliary: "à â å ã æ ç è ê î ñ ô ø œ ù û ÿ"
   marks: "◌̀ ◌́ ◌̂ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Ee"
   styles: "Overwegende, dat erkenning van de inherente"
   tester: "Overwegende, dat terzijdestelling van en minachting voor de rechten"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nmg_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nnh_Latn.textproto`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-id: "nmg_Latn"
-language: "nmg"
+id: "nnh_Latn"
+language: "nnh"
 script: "Latn"
-name: "Kwasio"
-autonym: "Kwasio"
-population: 8878
+name: "Ngiemboon"
+autonym: "Ngyɛmbɔɔŋ"
+population: 388430
 region: "CM"
 exemplar_chars {
-  base: "a A á Á â Â ǎ Ǎ ä Ä ā Ā b B ɓ Ɓ c C d D e E é É ê Ê ě Ě ē Ē ǝ Ǝ {ǝ́} {Ǝ́} {ǝ̂} {Ǝ̂} {ǝ̌} {Ǝ̌} {ǝ̄} {Ǝ̄} ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̂} {Ɛ̂} {ɛ̌} {Ɛ̌} {ɛ̄} {Ɛ̄} f F g G h H i I í Í î Î ǐ Ǐ ï Ï ī Ī j J k K l L m M n N ń Ń ŋ Ŋ o O ó Ó ô Ô ǒ Ǒ ö Ö ō Ō ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̂} {Ɔ̂} {ɔ̌} {Ɔ̌} {ɔ̄} {Ɔ̄} p P r R ŕ Ŕ s S t T u U ú Ú û Û ǔ Ǔ ū Ū v V w W y Y"
-  auxiliary: "q Q x X z Z"
-  marks: "◌́ ◌̂ ◌̄ ◌̈ ◌̌"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  index: "A B Ɓ C D E Ǝ Ɛ F G H I J K L M N Ŋ O Ɔ P R S T U V W Y"
+  base: "a A á Á à À â Â ǎ Ǎ b B c C d D e E é É è È ê Ê ě Ě ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̀} {Ɛ̀} {ɛ̂} {Ɛ̂} {ɛ̌} {Ɛ̌} f F g G h H i I í Í ì Ì j J k K l L m M ḿ Ḿ n N ń Ń ŋ Ŋ o O ó Ó ò Ò ô Ô ǒ Ǒ ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̀} {Ɔ̀} {ɔ̂} {Ɔ̂} {ɔ̌} {Ɔ̌} p P {pf} {PF} s S {sh} {SH} t T {ts} {TS} u U ú Ú ù Ù û Û ǔ Ǔ ʉ Ʉ {ʉ́} {Ʉ́} {ʉ̀} {Ʉ̀} {ʉ̂} {Ʉ̂} {ʉ̌} {Ʉ̌} v V w W ẅ Ẅ y Y ÿ Ÿ z Z ʼ"
+  auxiliary: "q Q r R x X"
+  marks: "◌̀ ◌́ ◌̂ ◌̈ ◌̌"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: ", ; : ! ? . \' ‘ ’ « »"
+  index: "A B C D E Ɛ F G H I J K L M N Ŋ O Ɔ P {Pf} R S {Sh} T {Ts} U Ʉ V W Ẅ Y Ÿ Z ʼ"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nn_Latn.textproto`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 script: "Latn"
 name: "Norwegian Nynorsk"
 autonym: "nynorsk"
 population: 1366860
 region: "NO"
 exemplar_chars {
   auxiliary: "á ǎ č ç đ è ê ń ñ ŋ š ŧ ü ž ä ö"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Ee"
   styles: "Då det å godkjenne det naturlege menneskeverdet"
   tester: "og då hån og vørdsløyse mot menneskerettane har ført til barbariske"
   poster_sm: "og då det er"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nnp_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nnp_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nnp_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nnp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nnp_Wcho.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nnp_Wcho.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/non_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/non_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/non_Runr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/non_Runr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/not_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/not_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nqo_Nkoo.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nqo_Nkoo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nrf_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nrf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nso_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nso_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nst_Tnsa.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nst_Tnsa.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nus_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nus_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Nuer"
 autonym: "Naath"
 population: 591427
 region: "SS"
 exemplar_chars {
   base: "a A ä Ä {a̱} {A̱} b B c C d D e E ë Ë {e̱} {E̱} ɛ Ɛ {ɛ̈} {Ɛ̈} {ɛ̱} {Ɛ̱} {ɛ̱̈} {Ɛ̱̈} f F g G ɣ Ɣ h H i I ï Ï {i̱} {I̱} j J k K l L m M n N ŋ Ŋ o O ö Ö {o̱} {O̱} ɔ Ɔ {ɔ̈} {Ɔ̈} {ɔ̱} {Ɔ̱} p P q Q r R s S t T u U v V w W x X y Y z Z"
   marks: "◌̈ ◌̱"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E Ɛ F G Ɣ H I J K L M N Ŋ O Ɔ P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "NnAa"
   masthead_partial: "Tt"
   styles: "Naath dial diethɛ kɛ a lɔr kä päärkɛ kɛ ciaŋ"
   tester: "Naath dial diethɛ kɛ a lɔr kä päärkɛ kɛ ciaŋ malä a mäni cuŋkiɛn."
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ny_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ny_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nym_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nym_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nyn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nyn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/nzi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/nzi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/oaa_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/oaa_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/oc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/oc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ohu_Hung.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ohu_Hung.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 script: "Hung"
 name: "Old Hungarian"
 population: 5000
 region: "HU"
 sample_text {
   masthead_full: "𐲪𐳪𐲢𐳢"
   masthead_partial: "𐲙𐳙"
-  styles: "𐲪𐲢𐲙𐲔 𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖 𐲌𐲛𐲍𐲮𐲀𐲙 𐲐𐲢𐲙𐲔 𐲯𐲢𐲞𐲦  𐲥𐲀𐲯𐲎 𐲥𐲦𐲙𐲇𐲞𐲂𐲉 𐲘𐲀𐲨𐲤 𐲒𐲀𐲙𐲛𐲤 𐲤𐲨𐲦𐲙 𐲓𐲛𐲮𐲀𐲆 𐲆𐲐𐲙𐲀𐲖𐲦𐲔 𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢 𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔 𐲍 𐲐𐲒 𐲀 𐲤 𐲐 𐲗 𐲗 𐲖𐲦 𐲀"
+  styles: "𐲪𐲢𐲙𐲔 𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖 𐲌𐲛𐲍𐲮𐲀𐲙 𐲐𐲢𐲙𐲔 𐲯𐲢𐲞𐲦 𐲥𐲀𐲯𐲎 𐲥𐲦𐲙𐲇𐲞𐲂𐲉 𐲘𐲀𐲨𐲤 𐲒𐲀𐲙𐲛𐲤 𐲤𐲨𐲦𐲙 𐲓𐲛𐲮𐲀𐲆 𐲆𐲐𐲙𐲀𐲖𐲦𐲔 𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢 𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔 𐲍 𐲐𐲒 𐲀 𐲤 𐲐 𐲗 𐲗 𐲖𐲦 𐲀"
   tester: "𐲪𐲢𐲙𐲔⁝𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖⁝𐲌𐲛𐲍𐲮𐲀𐲙⁝𐲐𐲢𐲙𐲔⁝𐲯𐲢𐲞𐲦 ⁝𐲥𐲀𐲯𐲎⁝𐲥𐲦𐲙𐲇𐲞𐲂𐲉⁝𐲘𐲀𐲨𐲤⁝𐲒𐲀𐲙𐲛𐲤⁝𐲤𐲨𐲦𐲙⁝𐲓𐲛𐲮𐲀𐲆⁝𐲆𐲐𐲙𐲀𐲖𐲦𐲔⁝𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢⁝𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔"
   poster_sm: "𐲪𐲢𐲙𐲔⁝𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖⁝𐲌𐲛𐲍𐲮𐲀𐲙⁝𐲐𐲢𐲙𐲔⁝𐲯𐲢𐲞𐲦 ⁝𐲥𐲀𐲯𐲎⁝𐲥𐲦𐲙𐲇𐲞𐲂𐲉⁝𐲘𐲀𐲨𐲤⁝𐲒𐲀𐲙𐲛𐲤⁝𐲤𐲨𐲦𐲙⁝𐲓𐲛𐲮𐲀𐲆⁝𐲆𐲐𐲙𐲀𐲖𐲦𐲔⁝𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢⁝𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔 𐲍·𐲐𐲒·𐲀·𐲤·𐲐·𐲗·𐲗·𐲖𐲦·𐲀"
   poster_md: "𐲪𐲢𐲙𐲔⁝𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖⁝𐲌𐲛𐲍𐲮𐲀𐲙⁝𐲐𐲢𐲙𐲔⁝𐲯𐲢𐲞𐲦 ⁝𐲥𐲀𐲯𐲎⁝𐲥𐲦𐲙𐲇𐲞𐲂𐲉⁝𐲘𐲀𐲨𐲤⁝𐲒𐲀𐲙𐲛𐲤⁝𐲤𐲨𐲦𐲙⁝𐲓𐲛𐲮𐲀𐲆⁝𐲆𐲐𐲙𐲀𐲖𐲦𐲔⁝𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢⁝𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔 𐲍·𐲐𐲒·𐲀·𐲤·𐲐·𐲗·𐲗·𐲖𐲦·𐲀"
   poster_lg: "𐲪𐲢𐲙𐲔⁝𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖⁝𐲌𐲛𐲍𐲮𐲀𐲙⁝𐲐𐲢𐲙𐲔⁝𐲯𐲢𐲞𐲦 ⁝𐲥𐲀𐲯𐲎⁝𐲥𐲦𐲙𐲇𐲞𐲂𐲉⁝𐲘𐲀𐲨𐲤⁝𐲒𐲀𐲙𐲛𐲤⁝𐲤𐲨𐲦𐲙⁝𐲓𐲛𐲮𐲀𐲆⁝𐲆𐲐𐲙𐲀𐲖𐲦𐲔⁝𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢⁝𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔 𐲍·𐲐𐲒·𐲀·𐲤·𐲐·𐲗·𐲗·𐲖𐲦·𐲀"
   specimen_48: "𐲪𐲢𐲙𐲔⁝𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖⁝𐲌𐲛𐲍𐲮𐲀𐲙⁝𐲐𐲢𐲙𐲔⁝𐲯𐲢𐲞𐲦 ⁝𐲥𐲀𐲯𐲎⁝𐲥𐲦𐲙𐲇𐲞𐲂𐲉⁝𐲘𐲀𐲨𐲤⁝𐲒𐲀𐲙𐲛𐲤⁝𐲤𐲨𐲦𐲙⁝𐲓𐲛𐲮𐲀𐲆⁝𐲆𐲐𐲙𐲀𐲖𐲦𐲔⁝𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢⁝𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔 𐲍·𐲐𐲒·𐲀·𐲤·𐲐·𐲗·𐲗·𐲖𐲦·𐲀"
   specimen_36: "𐲪𐲢𐲙𐲔⁝𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖⁝𐲌𐲛𐲍𐲮𐲀𐲙⁝𐲐𐲢𐲙𐲔⁝𐲯𐲢𐲞𐲦 ⁝𐲥𐲀𐲯𐲎⁝𐲥𐲦𐲙𐲇𐲞𐲂𐲉⁝𐲘𐲀𐲨𐲤⁝𐲒𐲀𐲙𐲛𐲤⁝𐲤𐲨𐲦𐲙⁝𐲓𐲛𐲮𐲀𐲆⁝𐲆𐲐𐲙𐲀𐲖𐲦𐲔⁝𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢⁝𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔 𐲍·𐲐𐲒·𐲀·𐲤·𐲐·𐲗·𐲗·𐲖𐲦·𐲀·"
   specimen_32: "𐲪𐲢𐲙𐲔⁝𐲥𐲬𐲖𐲦𐲤𐲦𐲬𐲖⁝𐲌𐲛𐲍𐲮𐲀𐲙⁝𐲐𐲢𐲙𐲔⁝𐲯𐲢𐲞𐲦 ⁝𐲥𐲀𐲯𐲎⁝𐲥𐲦𐲙𐲇𐲞𐲂𐲉⁝𐲘𐲀𐲨𐲤⁝𐲒𐲀𐲙𐲛𐲤⁝𐲤𐲨𐲦𐲙⁝𐲓𐲛𐲮𐲀𐲆⁝𐲆𐲐𐲙𐲀𐲖𐲦𐲔⁝𐲘𐲀𐲨𐲀𐲤𐲘𐲤𐲦𐲢⁝𐲍𐲢𐲍𐲗𐲘𐲤𐲦𐲢𐲆𐲐𐲙𐲀𐲖𐲦𐲀𐲔 𐲍·𐲐𐲒·𐲀·𐲤·𐲐·𐲗·𐲗·𐲖𐲦·𐲀·"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ojb_Cans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ojb_Cans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/oki_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/oki_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/om_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/om_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Afaan Oromoo"
 population: 34897120
 region: "ET"
 region: "KE"
 region: "SO"
 exemplar_chars {
   base: "a A b B c C d D e E f F g G h H i I j J k K l L m M n N o O p P q Q r R s S t T u U v V w W x X y Y z Z"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "NnAa"
   masthead_partial: "Mm"
   styles: "Ulfinni fi wal-qixxummaan ilmoo namaa kan"
   tester: "Mirga namummaa irra ijjechuun yookaan tuffachuun yeroo hunda"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/or_Orya.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/or_Orya.textproto`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 name: "Odia"
 autonym: "ଓଡ଼ିଆ"
 population: 42434880
 region: "IN"
 exemplar_chars {
   base: "଼ ଅ ଆ ଇ ଈ ଉ ଊ ଋ ଏ ଐ ଓ ଔ ଁ ଂ ଃ କ ଖ ଗ ଘ ଙ ଚ ଛ ଜ ଝ ଞ ଟ ଠ ଡ {ଡ଼} ଢ {ଢ଼} ଣ ତ ଥ ଦ ଧ ନ ପ ଫ ବ ଭ ମ ଯ ୟ ର ଲ ଳ ଵ ୱ ଶ ଷ ସ ହ ା ି ୀ ୁ ୂ ୃ େ ୈ ୋ ୌ ୍"
   auxiliary: "‌‍"
-  numerals: "- ‑ , . % ‰ + 0୦ 1୧ 2୨ 3୩ 4୪ 5୫ 6୬ 7୭ 8୮ 9୯"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0୦ 1୧ 2୨ 3୩ 4୪ 5୫ 6୬ 7୭ 8୮ 9୯"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "ଅ ଆ ଇ ଈ ଉ ଊ ଋ ଏ ଐ ଓ ଔ କ ଖ ଗ ଘ ଙ ଚ ଛ ଜ ଝ ଞ ଟ ଠ ଡ ଢ ଣ ତ ଥ ଦ ଧ ନ ପ ଫ ବ ଭ ମ ଯ ର ଲ ଳ ଶ ଷ ସ ହ {କ୍ଷ}"
 }
 sample_text {
   masthead_full: "ସବମନ"
   masthead_partial: "ଷୟ"
   styles: "ସବୁ ମନୁଷ୍ୟ ଜନ୍ମକାଳରୁ ସ୍ୱାଧୀନ. ସେମାନଙ୍କର ମର୍ଯ୍ୟାଦା ଓ ଅଧିକାର ସମାନ."
   tester: "ସବୁ ମନୁଷ୍ୟ ଜନ୍ମକାଳରୁ ସ୍ୱାଧୀନ. ସେମାନଙ୍କର ମର୍ଯ୍ୟାଦା ଓ ଅଧିକାର ସମାନ. ସେମାନଙ୍କଠାରେ ପ୍ରଜ୍ଞା ଓ ବିବେକ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/orh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/orh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/orv_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/orv_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/os_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/os_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 616987
 region: "GE"
 region: "RU"
 exemplar_chars {
   base: "а ӕ б в г {гъ} д {дж} {дз} е ё ж з и й к {къ} л м н о п {пъ} р с т {тъ} у ф х {хъ} ц {цъ} ч {чъ} ш щ ъ ы ь э ю я"
   auxiliary: ""
   marks: "◌̆ ◌̈"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
   index: "А Ӕ Б В Г {Гъ} Д {Дж} {Дз} Е Ё Ж З И Й К {Къ} Л М Н О П {Пъ} Р С Т {Тъ} У Ф Х {Хъ} Ц {Цъ} Ч {Чъ} Ш Щ Ы Э Ю Я"
 }
 sample_text {
   masthead_full: "АаДд"
   masthead_partial: "Ӕӕ"
   styles: "Нӕй рохуаты уадзӕн ӕппӕт дзыллӕджын бинонты"
   tester: "Адӕймӕгтӕ се \'ппӕт дӕр райгуырынц сӕрибарӕй ӕмӕ ӕмхуызонӕй сӕ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/osa_Osge.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/osa_Osge.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/osc_Ital.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/osc_Ital.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ota_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ota_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ote_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ote_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/otk_Orkh.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/otk_Orkh.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/otn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/otn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/owl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/owl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pa_Guru.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pa_Guru.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "IN"
 region: "KE"
 region: "SG"
 exemplar_chars {
   base: "ੱ ੰ ਼ ੦ ੧ ੨ ੩ ੪ ੫ ੬ ੭ ੮ ੯ ੴ ੳ ਉ ਊ ਓ ਅ ਆ ਐ ਔ ੲ ਇ ਈ ਏ ਸ {ਸ਼} ਹ ਕ ਖ {ਖ਼} ਗ {ਗ਼} ਘ ਙ ਚ ਛ ਜ {ਜ਼} ਝ ਞ ਟ ਠ ਡ ਢ ਣ ਤ ਥ ਦ ਧ ਨ ਪ ਫ {ਫ਼} ਬ ਭ ਮ ਯ ਰ ਲ ਵ ੜ ੍ ਾ ਿ ੀ ੁ ੂ ੇ ੈ ੋ ੌ"
   auxiliary: "‌‍ ਃ ਂ ਁ {ਲ਼}"
   marks: "◌਼ ◌ਾ ◌ਿ ◌ੀ ◌ੁ ◌ੂ ◌ੇ ◌ੈ ◌ੋ ◌ੌ"
-  numerals: "- ‑ , . % ‰ + 0੦ 1੧ 2੨ 3੩ 4੪ 5੫ 6੬ 7੭ 8੮ 9੯"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . \' ‘ ’ \" “ ” ( ) [ ] / & ′ ″"
+  numerals: "- , . % + 0੦ 1੧ 2੨ 3੩ 4੪ 5੫ 6੬ 7੭ 8੮ 9੯"
+  punctuation: "- – — , ; : ! ? . \' ‘ ’ \" “ ” ( ) [ ] / &"
   index: "ੳ ਅ ੲ ਸ ਹ ਕ ਖ ਗ ਘ ਙ ਚ ਛ ਜ ਝ ਞ ਟ ਠ ਡ ਢ ਣ ਤ ਥ ਦ ਧ ਨ ਪ ਫ ਬ ਭ ਮ ਯ ਰ ਲ ਵ ੜ"
 }
 sample_text {
   masthead_full: "ਸਰਮਨ"
   masthead_partial: "ਖਪ"
   styles: "ਜਦ ਕਿ ਮਨੁੱਖੀ ਪਰਿਵਾਰ ਦੇ ਸਾਰੇ ਮੈਂਬਰਾਂ ਦੀ ਧੁਰ ਅੰਦਰਲੀ ਅੰਤਰੀਵ ਸ਼ਾਨ"
   tester: "ਜਦ ਕਿ ਮਨੁੱਖੀ ਅਧਿਕਾਰਾਂ ਪ੍ਰਤੀ ਨਿਰਾਦਰ ਅਤੇ ਨਫ਼ਰਤ ਦਾ ਸਿੱਟਾ ਉਜੱਡ ਕਿਸਮ ਦੀਆਂ ਕਾਰਵਾਈਆਂ ਨਿਕਲਿਆ ਹੈ ਜਿਸ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pal_Phli.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pal_Phli.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pam_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pam_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pap_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pap_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pau_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pau_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pbb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pbb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pcd_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pcd_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pck_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pck_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pcm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pcm_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 script: "Latn"
 name: "Nigerian Pidgin"
 population: 44945880
 region: "NG"
 exemplar_chars {
   base: "a á b {ch} d e é ẹ {ẹ́} f g {gb} h i í j k {kp} l m n o ó ọ {ọ́} p r s {sh} t u ú v w y z {zh}"
   auxiliary: "à c è {ẹ̀} ì ò {ọ̀} q ù x"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B {CH} D E F G H I J K L M N O P R S T U V W Y Z"
 }
 sample_text {
   masthead_full: "EeVv"
   masthead_partial: "Rr"
   styles: "Dem recognise say human beings get dignity"
   tester: "Since e be like say, dem no see our right as any ting and dem"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/phn_Phnx.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/phn_Phnx.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pis_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pis_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/piu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/piu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pl_Latn.textproto`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 region: "RO"
 region: "SK"
 region: "UA"
 exemplar_chars {
   base: "a ą b c ć d e ę f g h i j k l ł m n ń o ó p r s ś t u w y z ź ż"
   auxiliary: "à â å ä æ ç é è ê ë î ï ô ö œ q ß ù û ü v x ÿ"
   marks: "◌́ ◌̇ ◌̨"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' \" ” „ « » ( ) [ ] { } § @ * / & # % † ‡ ′ ″ ° ~"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' \" ” „ « » ( ) [ ] { } @ * / & # %° ~"
   index: "A B C Ć D E F G H I J K L Ł M N O Ó P Q R S Ś T U V W X Y Z Ź Ż"
 }
 sample_text {
   masthead_full: "WwSs"
   masthead_partial: "Zz"
   styles: "ZWAŻYWSZY, że uznanie przyrodzonej godności"
   tester: "ZWAŻYWSZY, że nieposzanowanie i nieprzestrzeganie praw człowieka"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pms_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pms_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pon_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pon_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pov_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pov_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ppl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ppl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pro_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/prq_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/prq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ps_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ps_Arab.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 region: "AE"
 region: "AF"
 region: "IR"
 region: "PK"
 exemplar_chars {
   base: "َ ِ ُ ً ٍ ٌ ّ ْ ٔ ٰ آ ا أ ء ب پ ت ټ ث ج ځ چ څ ح خ د ډ ذ ر ړ ز ژ ږ س ش ښ ص ض ط ظ ع غ ف ق ک ګ گ ل م ن ڼ ه ة و ؤ ی ي ې ۍ ئ"
   auxiliary: "‌ ‍ ‎‏ ے"
-  numerals: "‎ - ‑ , ٫ ٬ . % ٪ ‰ ؉ + − 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
+  numerals: "‎ - , ٫ ٬ . % ٪ ؉ + − 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
   punctuation: "، ; : ! ۔ \' ‘ ( ) [ ] { } /"
   index: "آ ا ء ب پ ت ټ ث ج ځ چ څ ح خ د ډ ذ ر ړ ز ژ ږ س ش ښ ص ض ط ظ ع غ ف ق ک ګ ل م ن ڼ ه و ی"
 }
 sample_text {
   masthead_full: "دبشر"
   masthead_partial: "ټو"
   styles: "څرنګه چې دبشري کورنۍ دټولو غړو ذاتي حېثيت"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pt_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pt_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 region: "PT"
 region: "ST"
 region: "TL"
 exemplar_chars {
   base: "a á à â ã b c ç d e é ê f g h i í j k l m n o ó ò ô õ p q r s t u ú v w x y z"
   auxiliary: "ª ă å ä ā æ è ĕ ë ē ì ĭ î ï ī ñ º ŏ ö ø ō œ ù ŭ û ü ū ÿ"
   marks: "◌̀ ◌́ ◌̂ ◌̃ ◌̈ ◌̧"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtOo"
   masthead_partial: "Dd"
   styles: "Todos os seres humanos nascem livres e iguais"
   tester: "Todos os seres humanos nascem livres e iguais em dignidade e"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/pwo_Mymr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/pwo_Mymr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qu_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 region: "BO"
 region: "EC"
 region: "PE"
 exemplar_chars {
   base: "a {ch} {chʼ} h i k {kʼ} l {ll} m n ñ p {pʼ} q {qʼ} s t {tʼ} u w y"
   auxiliary: "á à ă â å ä ã ā æ b c ç d e é è ĕ ê ë ē f g í ì ĭ î ï ī j o ó ò ŏ ô ö ø ō œ r ú ù ŭ û ü ū v x ÿ z"
   marks: "◌̃ ◌̂ ◌̌"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A {Ch} H I K L {Ll} M N Ñ P Q S T U W Y"
 }
 sample_text {
   masthead_full: "LlAa"
   masthead_partial: "Pp"
   styles: "Pachantin ayllu wawaq allin kausaypi kananta"
   tester: "Runaq runa kayninta sarunchasqata rikuspan, wakin ima mil lay"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/quc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/quc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qud_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qud_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qug_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qug_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/quh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/quh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/quy_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/quy_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/quz_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/quz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qva_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qva_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qvc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qvc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qvh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qvh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qvm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qvm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qvn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qvn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qwh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qwh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qxn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qxn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/qxu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/qxu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rab_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rab_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rar_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rar_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ray_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ray_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rcf_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rcf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rej_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rej_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rej_Rjng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rej_Rjng.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 language: "rej"
 script: "Rjng"
 name: "Rejang, Rejang"
 population: 0
 sample_text {
   masthead_full: "ꤰꤳꤾꥁ"
   masthead_partial: "ꤸꤴ"
-  styles: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ"
-  tester: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ"
+  styles: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ"
+  tester: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ"
   poster_sm: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ,"
   poster_md: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸ"
   poster_lg: "ꤸꥎꥑꤴꥉꤰ,"
-  specimen_48: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ"
-  specimen_36: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓."
-  specimen_32: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓."
-  specimen_21: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓."
-  specimen_16: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ.  ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓."
+  specimen_48: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ"
+  specimen_36: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓."
+  specimen_32: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓."
+  specimen_21: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓."
+  specimen_16: "ꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓.\nꤰꥈꤳꥎ ꤳꥈꥐ ꤾꥁꥉꥑ ꤸꥎꥑꤴꥉꤰ, ꤳ꥓ꤸꥈꥆꥐ ꥁꥋꤰ꥓ꥁꥋꤰ꥓ ꤴꥎ ꤼ꥓ꤽꥊ. ꤰꥈꤳꥎ ꤵꤱꥇꥒꤰ꥓ꤷꥒ ꥆꤰꥎꥒ ꤶꥉꤰꥉꥑ ꤲꥉꥐ ꥆꤳꥊꥎ, ꤰꥎꥑꤵꥋ ꥆꥋ ꤰꥎꤾꥋꤰ꥓ꤵꥎ ꤷꥎꥒꤰꥈꥆꤳ꥓ꤷꥒ ꤴꥋ ꤲꥉꥐ ꤾꥈꤿꥎꥐ ꤾꥎꤸ꥓ ꥆꤼꥊ ꤼꥎꤶꤼꥈꥒꤰ꥓."
 }
 historical: true
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rgn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rgn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rhg_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rhg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rhg_Rohg.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rhg_Rohg.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -7,12 +7,12 @@
   masthead_partial: "𐴎𐴃"
   styles: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝"
   tester: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌"
   poster_sm: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕"
   poster_md: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 "
   poster_lg: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕"
   specimen_48: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝"
-  specimen_36: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔"
-  specimen_32: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔"
-  specimen_21: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔"
-  specimen_16: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔  𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔"
+  specimen_36: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔"
+  specimen_32: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔"
+  specimen_21: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔"
+  specimen_16: "𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔\n𐴀𐴞𐴕𐴐𐴝𐴦𐴕 𐴁𐴠𐴒𐴧𐴟𐴕 𐴀𐴝𐴎𐴝𐴊𐴢 𐴀𐴝𐴌 𐴀𐴠𐴑𐴧𐴟 𐴉𐴟𐴥𐴖𐴝𐴙𐴕𐴝 𐴇𐴡𐴥𐴑 𐴀𐴝𐴌 𐴀𐴞𐴎𐴧𐴡𐴃𐴢 𐴓𐴡𐴌 𐴉𐴡𐴘𐴊𐴝 𐴀𐴡𐴥𐴘𐴧𐴠 ۔ 𐴀𐴞𐴥𐴃𐴝𐴘𐴝𐴃𐴧𐴟 𐴀𐴝𐴈𐴡𐴓 𐴀𐴝𐴌 𐴁𐴟𐴎 𐴀𐴡𐴥𐴘𐴧𐴠 ، 𐴀𐴠𐴥𐴃𐴡𐴓𐴧𐴝 𐴀𐴞𐴥𐴃𐴝𐴌𐴝𐴃𐴧𐴟 𐴀𐴠𐴑 𐴀𐴡𐴕 𐴀𐴝𐴌 𐴀𐴠𐴑 𐴎𐴡𐴕 𐴓𐴡𐴘 𐴁𐴤𐴝𐴘𐴧𐴡 𐴋𐴧𐴡𐴙𐴓𐴧𐴝 𐴔𐴝𐴦𐴔𐴠𐴓𐴝 𐴒𐴡𐴌𐴡𐴥𐴕 𐴏𐴝𐴀𐴝 ۔"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rkt_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rkt_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rm_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Rumantsch"
 population: 42019
 region: "CH"
 exemplar_chars {
   base: "a à b c d e é è f g h i ì j k l m n o ò p q r s t u ù v w x y z"
   auxiliary: "á ă â å ä ā æ ç ĕ ê ë ē í ĭ î ï ī ñ ó ŏ ô ö ø ō œ ú ŭ û ü ū ÿ"
   marks: "◌̀ ◌́ ◌̂ ◌̈"
-  numerals: ". ’ % ‰ + − 0 1 2 3 4 5 6 7 8 9"
+  numerals: ". ’ % + − 0 1 2 3 4 5 6 7 8 9"
   index: "A À B C D E É È F G H I Ì J K L M N O Ò P Q R S T U Ù V W X Y Z"
 }
 sample_text {
   masthead_full: "TtUu"
   masthead_partial: "Oo"
   styles: "Considerand cha l\'arcugnuschentscha da la"
   tester: "Considerand cha la mancanza da la cugnuschentscha e\'l spredsch"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rmn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rmn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rn_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 script: "Latn"
 name: "Rundi"
 autonym: "Ikirundi"
 population: 7475454
 region: "BI"
 exemplar_chars {
   base: "a A b B c C d D e E f F g G h H i I j J k K l L m M n N o O p P q Q r R s S t T u U v V w W x X y Y z Z"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaBb"
   masthead_partial: "Nn"
   styles: "Ibonye ko kwemera ko abantu bose bategerezwa"
   tester: "Ibonye ko kutemera n\'ukudakwirikiza ingingo zubahiriza zina muntu"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ro_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ro_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ro_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ro_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 region: "RO"
 region: "RS"
 region: "UA"
 exemplar_chars {
   base: "a ă â b c d e f g h i î j k l m n o p r s ș t ț u v w x y z"
   auxiliary: "á à å ä ç é è ê ë ñ ö q ş ţ ü"
   marks: "◌̂ ◌̆ ◌̦ ◌̧"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ \" “ ” „ « » ( ) [ ] @ * /"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ \" “ ” „ « » ( ) [ ] @ * /"
   index: "A Ă Â B C D E F G H I Î J K L M N O P Q R S Ș T Ț U V W X Y Z"
 }
 sample_text {
   masthead_full: "TtOo"
   masthead_partial: "Aa"
   styles: "Considerând că recunoașterea demnității inerente"
   tester: "Considerând că ignorarea și disprețuirea drepturilor omului au"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ru_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ru_Cyrl.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 region: "UA"
 region: "US"
 region: "UZ"
 exemplar_chars {
   base: "а б в г д е ё ж з и й к л м н о п р с т у ф х ц ч ш щ ъ ы ь э ю я"
   auxiliary: "{а́} {е́} {и́} {о́} {у́} {ы́} {э́} {ю́} {я́}"
   marks: "◌̆ ◌̈ ◌́"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } § @ * / & #"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ‚ \" “ „ « » ( ) [ ] { } @ * / & #"
   index: "А Б В Г Д Е Ё Ж З И Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ы Э Ю Я"
 }
 sample_text {
   masthead_full: "ВвСс"
   masthead_partial: "Ее"
   styles: "Принимая во внимание, что признание достоинства,"
   tester: "принимая во внимание, что пренебрежение и презрение к правам человека"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rue_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rue_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rup_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rup_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/rw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/rw_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Kinyarwanda"
 population: 11083625
 region: "CD"
 region: "RW"
 region: "UG"
 exemplar_chars {
   base: "a A b B c C d D e E f F g G h H i I j J k K l L m M n N o O p P q Q r R s S t T u U v V w W x X y Y z Z"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "AaBb"
   masthead_partial: "Nn"
   styles: "- Ugushyira ukizana, ituze n\'ubutungane mu bihugu"
   tester: "- Gusuzugura no kwirengagiza ako gaciro n\'icyubahiro bya buli muntu"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Ahom.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Ahom.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Bali.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Bali.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Bhks.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Bhks.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Brah.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Brah.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Bugi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Bugi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Cham.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Cham.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Deva.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "संस्कृतम्"
 population: 15913
 region: "IN"
 exemplar_chars {
   base: "॑ ॒ ़ ँ ं ः ॐ अ आ इ ई उ ऊ ऋ ॠ ऌ ॡ ए ऐ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल ळ व श ष स ह ऽ ा ि ी ु ू ृ ॄ ॢ ॣ े ै ो ौ ्"
   auxiliary: "‌‍ ऍ ऑ ॅ ॉ"
   marks: "◌ँ ◌ं ◌ः ◌़ ◌ा ◌ि ◌ी ◌ु ◌ू ◌ृ ◌े ◌ै ◌ो ◌ौ ◌्"
-  numerals: "- ‑ , . % ‰ + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
-  punctuation: "_ - ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } § @ * / \\ & # ′ ″ ` + | ~"
+  numerals: "- , . % + 0० 1१ 2२ 3३ 4४ 5५ 6६ 7७ 8८ 9९"
+  punctuation: "_ - – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } @ * / \\ & #` + | ~"
   index: "अ आ इ ई उ ऊ ऋ ॠ ऌ ॡ ए ऐ ओ औ क ख ग घ ङ च छ ज झ ञ ट ठ ड ढ ण त थ द ध न प फ ब भ म य र ल ळ व श ष स ह"
 }
 sample_text {
   masthead_full: "सरवम"
   masthead_partial: "नत"
   styles: "यत्र जगति शान्तिन्यायस्वातन्त्र्याणां आधारः मानवपरिवारस्य सर्वेषामपि"
   tester: "सर्वे मानवाः स्वतन्त्राः समुत्पन्नाः वर्तन्ते अपि च, गौरवदृशा अधिकारदृशा च समानाः एव वर्तन्ते।"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Gonm.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Gonm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Gran.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Gran.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Khar.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Khar.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Limb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Limb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Marc.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Marc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Modi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Modi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mong.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Mong.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mroo.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Mroo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mtei.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Mtei.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Mult.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Mult.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Nand.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Nand.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 language: "sa"
 script: "Nand"
 name: "Sanskrit"
 autonym: "𑧍𑧞𑧍𑧠𑦮𑧖𑦽𑧆𑧠"
 region: "IN"
 exemplar_chars {
 base: "𑧟 𑦬 𑦠 𑦡 𑦢 𑦣 𑦤 𑦥 𑦦 𑦧 𑦪 𑦫 𑦭 𑦮 𑦯 𑦰 𑦱 𑦲 𑦳 𑦴 𑦵 𑦶 𑦷 𑦸 𑦹 𑦺 𑦻 𑦼 𑦽 𑦾 𑦿 𑧀 𑧁 𑧂 𑧃 𑧄 𑧅 𑧆 𑧇 𑧈 𑧉 𑧏 𑧊 𑧋 𑧌 𑧍 𑧎"
-auxiliary: " 𑦪 𑦡 𑧑 𑧚"
+auxiliary: "𑦪 𑦡 𑧑 𑧚"
 marks: "◌𑧞 ◌𑧟 ◌ ◌𑧑 ◌𑧒 ◌𑧓 ◌𑧔 ◌𑧕 ◌𑧖 ◌𑧚 ◌𑧛 ◌𑧜 ◌𑧝 ◌𑧠"
-punctuation: "_ - ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } § @ * / \\ & # ′ ″ ` + | ~"
+punctuation: "_ - – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] { } @ * / \\ & #` + | ~"
 index: "𑦠 𑦡 𑦢 𑦣 𑦤 𑦥 𑦦 𑦧 𑧉𑧔 𑧉𑧕 𑦪 𑦫 𑦬 𑦭 𑦮 𑦯 𑦰 𑦱 𑦲 𑦳 𑦴 𑦵 𑦶 𑦷 𑦸 𑦹 𑦺 𑦻 𑦼 𑦽 𑦾 𑦿 𑧀 𑧁 𑧂 𑧃 𑧄 𑧅 𑧆 𑧇 𑧈 𑧉 𑧏 𑧊 𑧋 𑧌 𑧍 𑧎"
 }
 sample_text {
 masthead_full: "𑧍𑧈𑧊𑧆"
 masthead_partial: "𑧁𑦽"
 styles: "𑧇𑦽𑧠𑧈 𑦵𑦰𑦽𑧒 𑧋𑧑𑧞𑦽𑧒𑧁𑧠𑧇𑧑𑧇𑧍𑧠𑧊𑧑𑦽𑧞𑦽𑧠𑧈𑧠𑧇𑧑𑦼𑧑𑧞 𑦡𑧀𑧑𑧈𑧟 𑧆𑧑𑧁𑧊𑧂𑧈𑧒𑧊𑧑𑧈𑧍𑧠𑧇 𑧍𑧈𑧠𑧊𑧚𑧌𑧑𑧆𑧂𑧒"
 tester: "𑧍𑧈𑧠𑧊𑧚 𑧆𑧑𑧁𑧊𑧑𑧟 𑧍𑧠𑧊𑦽𑧞𑦽𑧠𑧈𑧑𑧟 𑧍𑧆𑧔𑦽𑧠𑧂𑧁𑧠𑧁𑧑𑧟 𑧊𑧈𑧠𑦽𑧞𑦽𑧚 𑦠𑧂𑧒 𑦳, 𑦰𑧝𑧈𑧊𑦿𑧖𑧋𑧑 𑦠𑧀𑧒𑦮𑧑𑧈𑦿𑧖𑧋𑧑 𑦳 𑧍𑧆𑧑𑧁𑧑𑧟 𑦪𑧊 𑧊𑧈𑧠𑦽𑧞𑦽𑧚।"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Newa.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Newa.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Orya.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Phag.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Phag.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Ranj.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Ranj.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Rjng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Rjng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Shrd.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Shrd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sidd.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sidd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sind.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sind.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sinh.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sinh.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sora.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sora.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Soyo.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Soyo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sund.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sund.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Sylo.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Sylo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Tagb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Tagb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Tirh.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Tirh.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Wara.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Wara.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Wcho.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Wcho.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Xpeo.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Xpeo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sa_Zanb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sa_Zanb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sah_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sah_Cyrl.textproto`

 * *Files 7% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 autonym: "Сахалыы"
 population: 453510
 region: "RU"
 exemplar_chars {
   base: "а б г ҕ д {дь} и й к л м н {нь} ҥ о ө п р с т у ү х һ ч ы э"
   auxiliary: "в е ё ж з ф ц ш щ ъ ь ю я"
   marks: "◌̆ ◌̈"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   punctuation: ":"
   index: "А Б Г Ҕ Д {Дь} И Й К Л М Н {Нь} Ҥ О Ө П Р С Т У Ү Х Һ Ч Ы Э"
 }
 sample_text {
   masthead_full: "ДдЬь"
   masthead_partial: "Оо"
   styles: "Киһи аймах бэйэ суолтатын өйдөбулэ, тэҥ уонна"
   tester: "киһи быраабын ахсарбат буолуу уонна сэнээһин түмүгэр дьон аймах"
   poster_sm: "киһи бырааба"
   poster_md: "норуоттар"
   poster_lg: "Дьон"
   specimen_48: "Холбоһуктаах Нациялар норуоттара Устааптарыгар киһи сүрүн быраабыгар,"
   specimen_36: "Киһи аймах бэйэ суолтатын өйдөбулэ, тэҥ уонна быстыспат бырааба аан дойдуга көҥүл уонна кырдьык биир төрүтэ"
-  specimen_32: "ыйыллыбыт быраап уонна көҥүл диэн эйдэбуллэри дириҥник өйдөөһүн бу бэриллибит бигэ тыллары олоххо киллэриигэ улахан суолталааҕын болҕомтоҕо ылан туран.  Генеральнай Ассамблея,"
-  specimen_21: "Киһи аймах бэйэ суолтатын өйдөбулэ, тэҥ уонна быстыспат бырааба аан дойдуга көҥүл уонна кырдьык биир төрүтэ буоларын болҕомтоҕо ылан туран,\nкиһи быраабын ахсарбат буолуу уонна сэнээһин түмүгэр дьон аймах суобаһын абардар варвардыы  быһыылар  тахсыбаттарынан,  тыл  уонна  санаа  көҥүлүгэр,  кыһалҕата,  куттала суох олоххо дьон дьулуһарын болҕомтоҕо ылан туран,"
-  specimen_16: "Киһи аймах бэйэ суолтатын өйдөбулэ, тэҥ уонна быстыспат бырааба аан дойдуга көҥүл уонна кырдьык биир төрүтэ буоларын болҕомтоҕо ылан туран,\nкиһи быраабын ахсарбат буолуу уонна сэнээһин түмүгэр дьон аймах суобаһын абардар варвардыы  быһыылар  тахсыбаттарынан,  тыл  уонна  санаа  көҥүлүгэр,  кыһалҕата,  куттала суох олоххо дьон дьулуһарын болҕомтоҕо ылан туран,\nкиһи бырааба сокуон былааһынан харыстаныахтааҕын, киһи батталлаах былааһы утары өрө турууну бүтэһик ньыма курдук туһамматын туһугар,\nноруоттар икки ардыларыгар доҕордоһууну күүһүрдэр туһугар,\nыйыллыбыт быраап уонна көҥүл диэн эйдэбуллэри дириҥник өйдөөһүн бу бэриллибит бигэ тыллары олоххо киллэриигэ улахан суолталааҕын болҕомтоҕо ылан туран.  Генеральнай Ассамблея,"
+  specimen_32: "ыйыллыбыт быраап уонна көҥүл диэн эйдэбуллэри дириҥник өйдөөһүн бу бэриллибит бигэ тыллары олоххо киллэриигэ улахан суолталааҕын болҕомтоҕо ылан туран. Генеральнай Ассамблея,"
+  specimen_21: "Киһи аймах бэйэ суолтатын өйдөбулэ, тэҥ уонна быстыспат бырааба аан дойдуга көҥүл уонна кырдьык биир төрүтэ буоларын болҕомтоҕо ылан туран,\nкиһи быраабын ахсарбат буолуу уонна сэнээһин түмүгэр дьон аймах суобаһын абардар варвардыы быһыылар тахсыбаттарынан, тыл уонна санаа көҥүлүгэр, кыһалҕата, куттала суох олоххо дьон дьулуһарын болҕомтоҕо ылан туран,"
+  specimen_16: "Киһи аймах бэйэ суолтатын өйдөбулэ, тэҥ уонна быстыспат бырааба аан дойдуга көҥүл уонна кырдьык биир төрүтэ буоларын болҕомтоҕо ылан туран,\nкиһи быраабын ахсарбат буолуу уонна сэнээһин түмүгэр дьон аймах суобаһын абардар варвардыы быһыылар тахсыбаттарынан, тыл уонна санаа көҥүлүгэр, кыһалҕата, куттала суох олоххо дьон дьулуһарын болҕомтоҕо ылан туран,\nкиһи бырааба сокуон былааһынан харыстаныахтааҕын, киһи батталлаах былааһы утары өрө турууну бүтэһик ньыма курдук туһамматын туһугар,\nноруоттар икки ардыларыгар доҕордоһууну күүһүрдэр туһугар,\nыйыллыбыт быраап уонна көҥүл диэн эйдэбуллэри дириҥник өйдөөһүн бу бэриллибит бигэ тыллары олоххо киллэриигэ улахан суолталааҕын болҕомтоҕо ылан туран. Генеральнай Ассамблея,"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sas_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sas_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sat_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sat_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sc_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/scn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/scn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sco_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sco_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sd_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sd_Arab.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "سنڌي (عربي)"
 population: 31467954
 region: "IN"
 region: "PK"
 exemplar_chars {
   base: "ء آ ا ب ٻ پ ڀ ت ث ٺ ٽ ٿ ج {جھ} ڃ ڄ چ ڇ ح خ د ذ ڊ ڌ ڍ ڏ ر ز ڙ س ش ص ض ط ظ ع غ ف ڦ ق ک ڪ گ {گھ} ڱ ڳ ل م ن ڻ ه ھ و ي"
   auxiliary: "َ ُ ِ ئ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   punctuation: "⹁ ⁏ : ! ۔ ‘ ( ) [ ] { } /"
   index: "ا ب ٻ پ ڀ ت ث ٺ ٽ ٿ ج {جھ} ڃ ڄ چ ڇ ح خ د ذ ڊ ڌ ڍ ڏ ر ز ڙ س ش ص ض ط ظ ع غ ف ڦ ق ک ڪ گ {گھ} ڱ ڳ ل م ن ڻ ه ھ و ي"
 }
 sample_text {
   masthead_full: "سمور"
   masthead_partial: "ان"
   styles: "سمورا انسان آزاد ءِ عزت ءِ حقن ڄي حوالي ڪان"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sd_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sd_Deva.textproto`

 * *Files 14% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 autonym: "सिन्धी"
 population: 344783
 region: "IN"
 exemplar_chars {
   base: "़ ं अ आ इ ई उ ऊ ए ऐ ओ औ क ख ग ॻ घ ङ च छ ज ॼ झ ञ ट ठ ड ॾ ढ ण त थ द ध न प फ ब ॿ भ म य र ल व श ष स ह ा ि ी ु ू ृ ॄ ॅ े ै ॉ ो ौ ्"
   auxiliary: "‌‍"
   marks: "◌ँ ◌ं ◌ः ◌़ ◌ा ◌ि ◌ी ◌ु ◌ू ◌ृ ◌े ◌ै ◌ो ◌ौ ◌्"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/se_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/se_Latn.textproto`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 region: "FI"
 region: "NO"
 region: "SE"
 exemplar_chars {
   base: "a á b c č d đ e f g h i j k l m n ŋ o p r s š t ŧ u v z ž"
   auxiliary: "à ç é è í ń ñ ó ò q ú w x y ü ø æ å ä ã ö"
   marks: "◌́ ◌̈ ◌̊ ◌̌"
-  numerals: "  , % ‰ + − 0 1 2 3 4 5 6 7 8 9"
+  numerals: ", % + − 0 1 2 3 4 5 6 7 8 9"
   index: "A Á B C Č D Đ E É F G H I J K L M N Ŋ O P Q R S Š T Ŧ U V W X Y Z Ž Ø Æ Å Ä Ö"
 }
 sample_text {
   masthead_full: "BbUu"
   masthead_partial: "Oo"
   styles: "Buot olbmot leat riegádan friddjan ja olmmošárvvu"
   tester: "Juohkehaš lea vuoigaduvvon buot daid vuoigatvuođaide ja friddjavuođaide,"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sey_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sey_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sg_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sg_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Sängö"
 population: 2935521
 region: "CF"
 exemplar_chars {
   base: "a A â Â ä Ä b B d D e E ê Ê ë Ë f F g G h H i I î Î ï Ï j J k K l L m M n N o O ô Ô ö Ö p P r R s S t T u U ù Ù û Û ü Ü v V w W y Y z Z"
   auxiliary: "c C q Q x X"
   marks: "◌̂ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B D E F G H I J K L M N O P R S T U V W Y Z"
 }
 sample_text {
   masthead_full: "AaDd"
   masthead_partial: "Üü"
   styles: "Na hïngängö bîanî atene nëngö terê tî zo"
   tester: "Na hïngängö nî pëpëe na këngö ândiä tî bata nëngö terë tî zo"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sga_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sga_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sga_Ogam.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sga_Ogam.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/shk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/shk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/shn_Mymr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/shn_Mymr.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -13,9 +13,9 @@
   poster_sm: "ယွၼ်ႉပိူဝ်ႈ ၶီႇၼဵၵ်းတဵၵ်းတဵင်ပေႉၵိၼ်"
   poster_md: "ၼင်ႇႁိုဝ်ၸိုင်ႈမိူင်းၸိူဝ်းၼႆႉ"
   poster_lg: "ၵူၼ်းၵူႊၵေႃႉၼႆႉ"
   specimen_48: "လုၵ်ႈၸုမ်း ၸၢတ်ႈၸိုင်ႈလုမ်ႈၾႃႉၶဝ်ၼႆႉ ၼင်ႇႁိုဝ် ၼႂ်းလုမ်ႈၾႃႉၵူႊတီႈတီႈ တေႁၵ်ႉသႃပႂ်ႉပႃး သုၼ်ႇလႆႈသုၼ်ႇပဵၼ်ၵူၼ်း၊ သုၼ်ႇလႆႈသုၼ်ႇပဵၼ်ပိုၼ်ႉထၢၼ်ၽၢႆႇလွတ်ႈလႅဝ်းထၢင်ႇႁၢင်ႊၵႂႃႇၼၼ်ႉ"
   specimen_36: "ၵူၼ်းၵူႊၵေႃႉၼႆႉ ပဵၼ်ဢၼ်ၵိူတ်ႇမႃးလူၺ်ႈၵုင်ႇမုၼ်ဢၼ်လွတ်ႈလႅဝ်းၽဵင်ႇပဵင်းၵၼ် လႄႈ သုၼ်ႇလႆႈဢၼ် လွတ်ႈလႅဝ်းၽဵင်ႇ ပဵင်းၵၼ်။ ၶဝ်ၼႆႉ မီးၺၢၼ်ႇဢၼ်မေႃထတ်းသၢင် လႄႈ ၸႂ်ဢၼ်ႁူႉၸၵ်းၾိင်ႈတိုဝ်းၵမ် ၼၼ်ႉလႄႈ ထုၵ်ႇဝႆႉၸႂ်ပီႈဢွၵ်ႇ ၼွင်ႉၶႆႇၵၼ်သေ တိတ်းတေႃႇၵၼ်။"
   specimen_32: "ၵူၼ်းၵူႊၵေႃႉၼႆႉ မီးသုၼ်ႇလႆႈတႃႇၶုၺ်ႉႁၼ်ပိူင်ႇငမ်းသုၼ်ႇလႆႈလႄႈ လွင်ႈလွတ်ႈလႅဝ်းတင်းသဵင်ႈ ဢၼ်ပိုတ်ႇၼေဝႆႉ ၼႂ်း လိၵ်ႈပိုၼ်ၽၢဝ်ႇၼႆႉသေ တေဢမ်ႇလႆႈမီးလွင်ႈၸႅၵ်ႇၼႄလူၺ်ႈ ၸၢဝ်းၶိူဝ်း၊ သီၽိဝ်၊ ၶိူင်ႈၽွၵ်ႇ၊ ၵႂၢမ်းလၢတ်ႈ၊ ၸၢဝ်းၵိူဝ်း ယမ်၊ ပၢႆးႁပ်ႉႁၼ်ၵၢၼ်မိူင်း ဢိၵ်ႇတၢင်ႇလွင်ႈ၊ ငဝ်ႈႁၢၵ်ႈ ဢၼ်ၵဵဝ်ႇလူၺ်ႈ ၸိုင်ႈမိူင်း ႁိုဝ် ၸၼ်ႉထၢၼ်ႈၵၼ်ႊၵူၼ်း၊ လွင်ႈ မၢၵ်ႈမီးလီပဵၼ်၊ လွင်ႈၶိူဝ်းႁိူၼ်း လႄႈ ၸၼ်ႉထၢၼ်ႈတၢင်ႇၸိူဝ်ႉတၢင်ႇပိူင် ၸိူဝ်းၼႆႉ။"
   specimen_21: "လိူဝ်ၼၼ်ႉ ဢိင်ၼိူဝ် ၾၢႆႇပၢႆးမိူင်း၊ ၾၢႆႇတတ်းသိၼ်တွၼ်ႇၾိင်ႈ ဢမ်ႇၼၼ် ၾၢႆႇၶဝ်ႈဢွၵ်ႇတေႃႇၵူႊမိူင်းမိူင်း ၶွင်ၸိုင်ႈမိူင်း ႁိုဝ်ၼႃႈတီႈဢၼ်ၵူၼ်းၵေႃႉၼိုင်ႈယူႇသဝ်းၼၼ်ႉသေ တေဢမ်ႇလႆႈမီးလွင်ႈၸႅၵ်ႇၽႄၵၼ်။ ဝႆႉဝႃႈၼႃႈတီႈ ၼၼ်ႉ ပဵၼ်ဢၼ်လွတ်ႈလႅဝ်းသဝ်းၶေႃ ၵေႃႈလီ၊ ပဵၼ်ဢၼ်မီးဢႃႇၼႃႇတႃႇ ၽွင်းငမ်းၵမ်ႈၽွင်ႈၵွၺ်း ႁိုဝ် ပဵၼ်ၼႃႈတီႈ ဢၼ်ၸၢတ်ႈၸိုင်ႈလုမ်ႈၾႃႉၵုမ်းၵႂၢၼ်းတူၺ်းထိုင်ဝႆႉၼၼ်ႉ ၵေႃႈယႃႇ တႃႇတေဢိင်ၼိူဝ် လွင်ႈဝႃႈ ၸႂ်ႈဢမ်ႇၸႂ်ႈၼႃႈတီႈၸိူ ဝ်းၼၼ်ႉသေ ၸႅၵ်ႇၽႄၵၼ်ၼႆႉ တိုၼ်းတေဢမ်ႇလႆႈမီး။\nၵူၼ်းၵူႊၵေႃႉ မီးသုၼ်ႇလႆႈ တႃႇၶီးၸိုၼ်ႈ၊ တႃႇလွတ်ႈလႅဝ်းထၢင်ႇႁၢင်ႊ လႄႈ တႃႇႁူမ်ႇလူမ်ႈၸူဝ်ႊပၢၼ်မၼ်း။\nတေဢမ်ႇလႆႈတဵၵ်းႁႂ်ႈၽူႈလႂ်ႁဵတ်းၶႃႈၸႂ်ႉ ဢမ်ႇၼၼ် တဵၵ်းႁဵတ်းၼင်ႇၶႃႈၸႂ်ႉ။ ၵႃႊပဵၼ်လွင်ႈတဵၵ်း ႁႂ်ႈႁဵတ်း ၶႃႈၸႂ်ႉ လႄႈ လွင်ႈၵႃႉၶၢႆၶႃႈၸႂ်ႉၼႆႉ တေလႆႈဢိုတ်းႁၢမ်ႈပႅတ်ႈ ႁႂ်ႈပႃးၸဵမ် ၼႃႈၵၢၼ် ဢၼ်ငၢႆးမိူၼ်ၼႆ။"
-  specimen_16: "တေဢမ်ႇလႆႈၶႃၸႂ်ဢမ်ႇၼၼ် တိတ်းတေႃႇႁၢဝ်ႈႁၢဝ်ႈႁႅင်းႁႅင်း ထၢၼ်ႈပေႃးဢမ်ႇမိူၼ်ၵူၼ်းသေ ႁဵတ်းႁႂ်ႈတိူဝ်ႉ သရေႇၼႃႈ တႃ ဢမ်ႇၼၼ် တေဢမ်ႇလႆႈပၼ်တူတ်ႈတၢမ်ႇ မိူၼ်ၼႆ တီႈၽူႈလႂ်ၽႂ်သေၵေႃႉ။\nတီႈပၵ်းပိူင်ၼၼ်ႉ ၵူၼ်းၵူႊၵေႃႉၼႆႉ မီးသုၼ်ႇလႆႈ ထုၵ်ႇမၵ်းမၼ်ႈၼင်ႇ ၵူၼ်းၵေႃႉၼိုင်ႈ တႃႇၵူႊလွင်ႈ။\nၵူၼ်းတင်းသဵင်ႈၼႆႉ တီႈပၵ်းပိူင်ၾိင်ႈမိူင်းၼၼ်ႉ ၽဵင်ႇပဵင်းဢၼ်သေဢမ်ႇၵႃး လွင်ႈဢၼ်ပၵ်းပိူင် ၾိင်ႈမိူင်း ၵႅတ်ႇၶေပၼ် ၼၼ်ႉၵေႃႈ ဢမ်ႇမီးလွင်ႈပႅၵ်ႇပိူင်ႈၵၼ်သေ မီးသုၼ်ႇလႆႈ တႃႇၶုၺ်ႉႁၼ်ၽဵင်ႇပဵင်းၵၼ်။ ၵူၼ်းတင်းသဵင်ႈၼႆႉ မီးသုၼ်ႇလႆႈ ၽဵင်ႇၽဵင်ႇပဵင်းပဵင်း တႃႇၶုၺ်ႉႁၼ် ဢၼ်ၵႅတ်ႇၶေပၼ် လွင်ႈပူၼ်ႉပႅၼ်တေႃႇလိၵ်ႈပိုၼ်ၽၢဝ်ႇၼႆႉသေ ၸႅၵ်ႇၽႄၵၼ်လႂ်၊ လွင်ႈသူၼ်းႁူၺ်ႈ ႁႂ်ႈၸႅၵ်ႇၽႄၵၼ်လႂ်ၼၼ်ႉယူႇ။\nသင်ဝႃႈ လႆႈပူၼ်ႉပႅၼ်တေႃႇ သုၼ်ႇလႆႈပိုၼ်ႉငဝ်ႈ ဢၼ်လၵ်းမိူင်း ဢမ်ႇၼၼ် ၾိင်ႈမိူင်း ဢၼ်ႁပ်ႉႁွင်းပၼ်ဝႆႉၼၼ်ႉၸိုင် ၵူၼ်းၵူႊၵေႃႉၼႆႉ တၵ်းမီး သုၼ်ႇလႆႈတႃႇႁပ်ႉဢဝ် ဢၼ်လုမ်းတွၼ်ႇၾိင်ႈၸိုင်ႈမိူင်း ၶိုၼ်းၵေႈ သၢႆလူတ်းလူမ်ပၼ် ထိုင်တီႈ လီငၢမ်းၼၼ်ႉယူႇ။\nဢမ်ႇၶဝ်ႈတၢင်းၵၢၼ်ပၵ်းပိူင်ၾိင်ႈမိူင်းသေ ၽူႈလႂ်ၵေႃႈ တေဢမ်ႇႁႂ်ႈလႆႈထုၵ်ႇတီႉၺွပ်း  ႁိုဝ် လိုပ်ႈဢွၵ်ႇမိူင်း။\nမိူဝ်ႈလႆႈထုၵ်ႇတတ်းၶၢၼ်း သုၼ်ႇလႆႈ လႄႈ ၼႃႈၶွင်ပုၼ်ႈၽွၼ်းမၼ်းၼၼ်ႉလႂ်၊ မိူဝ်ႈလႆႈထုၵ်ႇမၢပ်ႇမႂ်ထိုင် ယွၼ်ႉလိူင်ႈၽိတ်း ၾိင်ႈၼၼ်ႉလႂ် ၵူၼ်းၵူႊၵေႃႉၼႆႉ မီးသုၼ်ႇလႆႈၽဵင်ႇပဵင်းမိူၼ်ၵၼ် တႃႇလႆႈထုၵ်ႇလုမ်းတွၼ်ႇၾိင်ႈ ဢၼ်လွတ်ႈလႅဝ်း လႄႈ ဢၼ်ဢမ်ႇၸွမ်းပႃႈၽၢႆႇၼၼ်ႉ ၵူတ်ႇထတ်းၽဵင်ႇၽဵၼ်ႈ တီႈၼႃႈၵူၼ်းၼမ်။\nၵူၼ်းၵူႊၵေႃႉၼႆႉ မီးသုၼ်ႇလႆႈ တႃႇဝူၼ်ႉၶႆႈ၊ ႁပ်ႉႁၼ်၊ ၵိူဝ်းယမ် လွတ်ႈလွတ်ႈလႅဝ်းလႅဝ်းသေ ၼႂ်းၼၼ်ႉ ပႃးဝႆႉသုၼ်ႇလႆႈ တႃႇလႅၵ်ႈလၢႆႈၸၢဝ်းၵိူဝ်းယမ် လႄႈ ပၢႆးယုမ်ႇယမ်ၸဝ်ႈၵဝ်ႇၼၼ်ႉ လွတ်ႈလွတ်ႈလႅဝ်းလႅဝ်းယူႇ။ လိူဝ်ၼၼ်ႉ ယူႇတီႈၵေႃႉ လႂ်ၽႂ်မၼ်းလႄႈသင် ႁူမ်ႈလူၺ်ႈတင်းတၢင်ႇၵေႃႉသေလႄႈသင် ၸွမ်းၼင်ႇ  ၸဝ်ႈၵဝ်ႇ ၵိူဝ်းယမ် ဢမ်ႇၼၼ် ပူင်သွၼ်လႆႈ၊ ၽိုၵ်းၵမ်လႆႈ၊ ၵိူဝ်းယမ်ၼပ်ႉထိုဝ်လႆႈ တီႈၽၢႆႇၼႃႈၵူၼ်းမိူင်း တင်းလၢႆ လႄႈ တီႈလပ်ႉလင်ၶဝ်ၼၼ်ႉ လွတ်ႈလွတ်ႈလႅဝ်း လႅဝ်းယူႇ။"
+  specimen_16: "တေဢမ်ႇလႆႈၶႃၸႂ်ဢမ်ႇၼၼ် တိတ်းတေႃႇႁၢဝ်ႈႁၢဝ်ႈႁႅင်းႁႅင်း ထၢၼ်ႈပေႃးဢမ်ႇမိူၼ်ၵူၼ်းသေ ႁဵတ်းႁႂ်ႈတိူဝ်ႉ သရေႇၼႃႈ တႃ ဢမ်ႇၼၼ် တေဢမ်ႇလႆႈပၼ်တူတ်ႈတၢမ်ႇ မိူၼ်ၼႆ တီႈၽူႈလႂ်ၽႂ်သေၵေႃႉ။\nတီႈပၵ်းပိူင်ၼၼ်ႉ ၵူၼ်းၵူႊၵေႃႉၼႆႉ မီးသုၼ်ႇလႆႈ ထုၵ်ႇမၵ်းမၼ်ႈၼင်ႇ ၵူၼ်းၵေႃႉၼိုင်ႈ တႃႇၵူႊလွင်ႈ။\nၵူၼ်းတင်းသဵင်ႈၼႆႉ တီႈပၵ်းပိူင်ၾိင်ႈမိူင်းၼၼ်ႉ ၽဵင်ႇပဵင်းဢၼ်သေဢမ်ႇၵႃး လွင်ႈဢၼ်ပၵ်းပိူင် ၾိင်ႈမိူင်း ၵႅတ်ႇၶေပၼ် ၼၼ်ႉၵေႃႈ ဢမ်ႇမီးလွင်ႈပႅၵ်ႇပိူင်ႈၵၼ်သေ မီးသုၼ်ႇလႆႈ တႃႇၶုၺ်ႉႁၼ်ၽဵင်ႇပဵင်းၵၼ်။ ၵူၼ်းတင်းသဵင်ႈၼႆႉ မီးသုၼ်ႇလႆႈ ၽဵင်ႇၽဵင်ႇပဵင်းပဵင်း တႃႇၶုၺ်ႉႁၼ် ဢၼ်ၵႅတ်ႇၶေပၼ် လွင်ႈပူၼ်ႉပႅၼ်တေႃႇလိၵ်ႈပိုၼ်ၽၢဝ်ႇၼႆႉသေ ၸႅၵ်ႇၽႄၵၼ်လႂ်၊ လွင်ႈသူၼ်းႁူၺ်ႈ ႁႂ်ႈၸႅၵ်ႇၽႄၵၼ်လႂ်ၼၼ်ႉယူႇ။\nသင်ဝႃႈ လႆႈပူၼ်ႉပႅၼ်တေႃႇ သုၼ်ႇလႆႈပိုၼ်ႉငဝ်ႈ ဢၼ်လၵ်းမိူင်း ဢမ်ႇၼၼ် ၾိင်ႈမိူင်း ဢၼ်ႁပ်ႉႁွင်းပၼ်ဝႆႉၼၼ်ႉၸိုင် ၵူၼ်းၵူႊၵေႃႉၼႆႉ တၵ်းမီး သုၼ်ႇလႆႈတႃႇႁပ်ႉဢဝ် ဢၼ်လုမ်းတွၼ်ႇၾိင်ႈၸိုင်ႈမိူင်း ၶိုၼ်းၵေႈ သၢႆလူတ်းလူမ်ပၼ် ထိုင်တီႈ လီငၢမ်းၼၼ်ႉယူႇ။\nဢမ်ႇၶဝ်ႈတၢင်းၵၢၼ်ပၵ်းပိူင်ၾိင်ႈမိူင်းသေ ၽူႈလႂ်ၵေႃႈ တေဢမ်ႇႁႂ်ႈလႆႈထုၵ်ႇတီႉၺွပ်း ႁိုဝ် လိုပ်ႈဢွၵ်ႇမိူင်း။\nမိူဝ်ႈလႆႈထုၵ်ႇတတ်းၶၢၼ်း သုၼ်ႇလႆႈ လႄႈ ၼႃႈၶွင်ပုၼ်ႈၽွၼ်းမၼ်းၼၼ်ႉလႂ်၊ မိူဝ်ႈလႆႈထုၵ်ႇမၢပ်ႇမႂ်ထိုင် ယွၼ်ႉလိူင်ႈၽိတ်း ၾိင်ႈၼၼ်ႉလႂ် ၵူၼ်းၵူႊၵေႃႉၼႆႉ မီးသုၼ်ႇလႆႈၽဵင်ႇပဵင်းမိူၼ်ၵၼ် တႃႇလႆႈထုၵ်ႇလုမ်းတွၼ်ႇၾိင်ႈ ဢၼ်လွတ်ႈလႅဝ်း လႄႈ ဢၼ်ဢမ်ႇၸွမ်းပႃႈၽၢႆႇၼၼ်ႉ ၵူတ်ႇထတ်းၽဵင်ႇၽဵၼ်ႈ တီႈၼႃႈၵူၼ်းၼမ်။\nၵူၼ်းၵူႊၵေႃႉၼႆႉ မီးသုၼ်ႇလႆႈ တႃႇဝူၼ်ႉၶႆႈ၊ ႁပ်ႉႁၼ်၊ ၵိူဝ်းယမ် လွတ်ႈလွတ်ႈလႅဝ်းလႅဝ်းသေ ၼႂ်းၼၼ်ႉ ပႃးဝႆႉသုၼ်ႇလႆႈ တႃႇလႅၵ်ႈလၢႆႈၸၢဝ်းၵိူဝ်းယမ် လႄႈ ပၢႆးယုမ်ႇယမ်ၸဝ်ႈၵဝ်ႇၼၼ်ႉ လွတ်ႈလွတ်ႈလႅဝ်းလႅဝ်းယူႇ။ လိူဝ်ၼၼ်ႉ ယူႇတီႈၵေႃႉ လႂ်ၽႂ်မၼ်းလႄႈသင် ႁူမ်ႈလူၺ်ႈတင်းတၢင်ႇၵေႃႉသေလႄႈသင် ၸွမ်းၼင်ႇ ၸဝ်ႈၵဝ်ႇ ၵိူဝ်းယမ် ဢမ်ႇၼၼ် ပူင်သွၼ်လႆႈ၊ ၽိုၵ်းၵမ်လႆႈ၊ ၵိူဝ်းယမ်ၼပ်ႉထိုဝ်လႆႈ တီႈၽၢႆႇၼႃႈၵူၼ်းမိူင်း တင်းလၢႆ လႄႈ တီႈလပ်ႉလင်ၶဝ်ၼၼ်ႉ လွတ်ႈလွတ်ႈလႅဝ်း လႅဝ်းယူႇ။"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/shp_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/shp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/si_Sinh.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/si_Sinh.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 name: "Sinhala"
 autonym: "සිංහල"
 population: 15564656
 region: "LK"
 exemplar_chars {
   base: "අ ආ ඇ ඈ ඉ ඊ උ ඌ ඍ එ ඒ ඓ ඔ ඕ ඖ ං ඃ ක ඛ ග ඝ ඞ ඟ ච ඡ ජ ඣ ඥ ඤ ට ඨ ඩ ඪ ණ ඬ ත ථ ද ධ න ඳ ප ඵ බ භ ම ඹ ය ර ල ව ශ ෂ ස හ ළ ෆ ා ැ ෑ ි ී ු ූ ෘ ෲ ෟ ෙ ේ ෛ ො ෝ ෞ ්"
   auxiliary: "​‌‍ ඎ ඏ ඐ ඦ ෳ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "අ ආ ඇ ඈ ඉ ඊ උ ඌ ඍ එ ඒ ඓ ඔ ඕ ඖ ක ඛ ග ඝ ඞ ඟ ච ඡ ජ ඣ ඥ ඤ ට ඨ ඩ ඪ ණ ඬ ත ථ ද ධ න ඳ ප ඵ බ භ ම ඹ ය ර ල ව ශ ෂ ස හ ළ ෆ"
 }
 sample_text {
   masthead_full: "සයලම"
   masthead_partial: "නෂ"
   styles: "ලෝකයේ පවත්නා නිදහස, යුක්තිය සහ සාමය යන්නෙහි පදනම මිනිස් පවුලේ"
   tester: "මානව අයිතිවාසිකම් නොතැකීම හා අවඥාවට ලක්කිරීමේ ප්‍රතිඵලයක් වශයෙන් මිනිස් වර්ගයාගේ හෘදය සාක්ෂිය"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sja_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sja_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sk_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "HU"
 region: "RS"
 region: "SK"
 exemplar_chars {
   base: "a á ä b c č d ď {dz} {dž} e é f g h {ch} i í j k l ĺ ľ m n ň o ó ô p q r ŕ s š t ť u ú v w x y ý z ž"
   auxiliary: "à ă â å ā æ ç è ĕ ê ë ē ì ĭ î ï ī ñ ò ŏ ö ő ø ō œ ř ù ŭ û ü ű ū ÿ"
   marks: "◌́ ◌̂ ◌̈ ◌̌"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] § @ * / &"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] @ * / &"
   index: "A Ä B C Č D Ď E F G H {CH} I J K L Ľ M N O Ô P Q R S Š T Ť U V W X Y Z Ž"
 }
 sample_text {
   masthead_full: "VvŠš"
   masthead_partial: "Ee"
   styles: "Vo vedomí že uznanie prirodzenej dôstojnosti"
   tester: "že zneuznanie ľudských práv a pohrdanie nimi viedlo k barbarským"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/skr_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/skr_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sl_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "HU"
 region: "IT"
 region: "SI"
 exemplar_chars {
   base: "a b c č d e f g h i j k l m n o p r s š t u v z ž"
   auxiliary: "á à ă â å ä ā æ ç ć đ é è ĕ ê ë ē í ì ĭ î ï ī ñ ó ò ŏ ô ö ø ō œ q ú ù ŭ û ü ū w x y ÿ"
   marks: "◌́ ◌̈ ◌̌"
-  numerals: ", . % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ – , ; : ! ? . … \' \" „ ‟ « » ( ) [ ] { } @ *"
+  numerals: ", . % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … \' \" „ ‟ « » ( ) [ ] { } @ *"
   index: "A B C Č Ć D Đ E F G H I J K L M N O P Q R S Š T U V W X Y Z Ž"
 }
 sample_text {
   masthead_full: "VvSs"
   masthead_partial: "Ii"
   styles: "ker pomeni priznanje prirojenega človeškega"
   tester: "ker sta zanikanje in teptanje človekovih pravic pripeljala do"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sla_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sla_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/slr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/slr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/smn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/smn_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Anarâškielâ"
 population: 612
 region: "FI"
 exemplar_chars {
   base: "a â b c č d đ e f g h i j k l m n ŋ o p r s š t u v y z ž ä á"
   auxiliary: "à ç é è í ñ ń ó ò q ú ü w x æ ø å ã ö"
   marks: "◌́ ◌̂ ◌̈ ◌̊ ◌̌"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "A Â B C Č D Đ E F G H I J K L M N Ŋ O P R S Š T U V Y Z Ž Ä Á"
 }
 sample_text {
   masthead_full: "BbUu"
   masthead_partial: "Oo"
   styles: "Buot olbmot leat riegádan friddjan ja olmmošárvvu"
   tester: "Buot olbmot leat riegádan friddjan ja olmmošárvvu ja olmmošvuoigatvuođaid"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/smp_Samr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/smp_Samr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sn_Latn.textproto`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Shona"
 autonym: "Chishona"
 population: 11782503
 region: "ZW"
 exemplar_chars {
   base: "a A b B c C d D e E f F g G h H i I j J k K l L m M n N o O p P r R s S t T u U v V w W y Y z Z"
   auxiliary: "q Q x X"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N O P R S T U V W Y Z"
 }
 sample_text {
   masthead_full: "VvAa"
   masthead_partial: "Nn"
   styles: "Sezvo kucherechedza hunhu nekodzero yakayenzana"
   tester: "Sezvo kusatevera nekusvora kodzero dzevanhu zvakamboita kuti"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/snk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/snk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/snn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/snn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/so_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/so_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 region: "DJ"
 region: "ET"
 region: "KE"
 region: "SO"
 exemplar_chars {
   base: "b B c C d D f F g G h H j J k K l L m M n N q Q r R s S t T w W x X y Y"
   auxiliary: "a A e E i I o O p P u U v V z Z"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "B C D F G H J K L M N Q R S T W X Y"
 }
 sample_text {
   masthead_full: "AaDd"
   masthead_partial: "Nn"
   styles: "Iyadoo aqoonsiga sharafta uu ku dhashay iyo"
   tester: "Iyadoo aqoonsi la\'aanta iyo ku tumashada xuquuqda aadanuhu ay"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/so_Osma.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/so_Osma.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sq_Elba.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sq_Elba.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sq_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sq_Latn.textproto`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 region: "RS"
 region: "TR"
 region: "XK"
 exemplar_chars {
   base: "a b c ç d {dh} e ë f g {gj} h i j k l {ll} m n {nj} o p q r {rr} s {sh} t {th} u v x {xh} y z {zh}"
   auxiliary: "w"
   marks: "◌̈ ◌̧"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” « » ( ) [ ] § @ * / & # ′ ″ ~"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” « » ( ) [ ] @ * / & #~"
   index: "A B C Ç D {DH} E Ë F G {GJ} H I J K L {LL} M N {NJ} O P Q R {RR} S {SH} T {TH} U V X {XH} Y Z {ZH}"
 }
 sample_text {
   masthead_full: "TtËë"
   masthead_partial: "Gg"
   styles: "Të gjithë njerëzit lindin të lirë dhe të"
   tester: "Të gjithë njerëzit lindin të lirë dhe të barabartë në dinjitet"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sr_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sr_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "ME"
 region: "RS"
 region: "XK"
 exemplar_chars {
   base: "а б в г д ђ е ж з и ј к л љ м н њ о п р с т ћ у ф х ц ч џ ш"
   auxiliary: "{а̂} {е̂} ё й {и̂} {о̂} {у̂} щ ъ ы ь э ю я"
   marks: "◌́"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] { } * #"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] { } * #"
   index: "А Б В Г Д Ђ Е Ж З И Ј К Л Љ М Н Њ О П Р С Т Ћ У Ф Х Ц Ч Џ Ш"
 }
 sample_text {
   masthead_full: "СсВв"
   masthead_partial: "Аа"
   styles: "Пошто је признавање урођеног достојанства"
   tester: "пошто је непоштовање и презирање права човека водило варварским"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sr_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 region: "RS"
 region: "RU"
 region: "TR"
 region: "XK"
 exemplar_chars {
   base: "a b c č ć d {dž} đ e f g h i j k l {lj} m n {nj} o p r s š t u v z ž"
   auxiliary: "å q w x y"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] { } * #"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . … ‘ ‚ “ „ ( ) [ ] { } * #"
   index: "A B C Č Ć D {DŽ} E F G H I J K L {LJ} M N {NJ} O P Q R S Š T U V W X Y Z Ž"
 }
 sample_text {
   masthead_full: "SsVv"
   masthead_partial: "Aa"
   styles: "Pošto je priznavanje urođenog dostojanstva"
   tester: "pošto je nepoštovanje i preziranje prava čoveka vodilo varvarskim"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/srn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/srn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/srr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/srr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ss_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ss_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/st_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/st_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/stq_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/stq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/str_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/str_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/su_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/su_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Basa Sunda"
 population: 32043120
 region: "ID"
 exemplar_chars {
   base: "a b c d e é f g h i j k l m n o p q r s t u v w x y z"
   auxiliary: "á à ă â å ä ã ā æ ç è ĕ ê ë ē í ì ĭ î ï ī ñ ó ò ŏ ô ö ø ō œ ú ù ŭ û ü ū ÿ"
   marks: "◌́"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E É F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "SsAa"
   masthead_partial: "Kk"
   styles: "Dumasar ku ayana timbangan yen pangakuan"
   tester: "Ku ayana timbangan yen ngalelewodehkeun katut nganggap enteng"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/su_Sund.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/su_Sund.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/suk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/suk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sus_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sv_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "DK"
 region: "FI"
 region: "SE"
 exemplar_chars {
   base: "a à b c d e é f g h i j k l m n o p q r s t u v w x y z å ä ö"
   auxiliary: "á â ã ā ç è ë í î ï ī ñ ó ú ÿ ü æ ø"
   marks: "◌̀ ◌́ ◌̈ ◌̊"
-  numerals: "  , % ‰ + − 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: ", % + − 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z Å Ä Ö"
 }
 sample_text {
   masthead_full: "AaLl"
   masthead_partial: "Mm"
   styles: "Enär erkännandet av det inneboende värdet"
   tester: "enär ringaktning och förakt för de mänskliga rättigheterna lett"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/sw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/sw_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 region: "TZ"
 region: "UG"
 region: "YT"
 region: "ZA"
 exemplar_chars {
   base: "a A b B {ch} {CH} d D e E f F g G h H i I j J k K l L m M n N o O p P r R s S t T u U v V w W y Y z Z"
   auxiliary: "c C q Q x X"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ , ; : ! ? . \' \" ( ) [ ] { }"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- , ; : ! ? . \' \" ( ) [ ] { }"
   index: "A B {CH} D E F G H I J K L M N O P R S T U V W Y Z"
 }
 sample_text {
   masthead_full: "WwAa"
   masthead_partial: "Tt"
   styles: "Kwa kuwa kukiri heshima ya asili na haki"
   tester: "Kwa kuwa kutojali na kudharau haki za binadamu kumeletea vitendo"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/swb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/swb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/syc_Syrc.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/syc_Syrc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/syl_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/syl_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/syl_Sylo.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/syl_Sylo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/szl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/szl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ta_Taml.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ta_Taml.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 region: "MY"
 region: "RE"
 region: "SG"
 exemplar_chars {
   base: "அ ஆ இ ஈ உ ஊ எ ஏ ஐ ஒ ஓ ஔ ஃ க ங ச ஞ ட ண த ந ப ம ய ர ல வ ழ ள ற ன ஜ ஷ ஸ ஹ ா ி ீ ு ூ ெ ே ை ொ ோ ௌ ்"
   auxiliary: "‌‍"
   marks: "◌ா ◌ி ◌ீ ◌ு ◌ூ ◌ெ ◌ே ◌ை ◌் ◌ௗ"
-  numerals: "- ‑ , . % ‰ + 0௦ 1௧ 2௨ 3௩ 4௪ 5௫ 6௬ 7௭ 8௮ 9௯"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0௦ 1௧ 2௨ 3௩ 4௪ 5௫ 6௬ 7௭ 8௮ 9௯"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "அ ஆ இ ஈ உ ஊ எ ஏ ஐ ஒ ஓ ஔ க ங ச ஞ ட ண த ந ப ம ய ர ல வ ழ ள ற ன"
 }
 sample_text {
   masthead_full: "மனதப"
   masthead_partial: "றவ"
   styles: "மனிதக் குடும்பத்தினைச் சேர்ந்த யாவரதும் உள்ளார்ந்த மரியாதையையும், அவர்கள்"
   tester: "மனித உரிமைகளை அவமதித்தலும் இகழ்தலும், மனிதகுலத்தின் மனசாட்சியை சீற்றத்திற்குள்ளாக்கியுள்ள காட்டுமிராண்டித்தனமான"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/taj_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/taj_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/taj_Tibt.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/taj_Tibt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/taq_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/taq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/taq_Tfng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/taq_Tfng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tbw_Tagb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tbw_Tagb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tbz_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tbz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tca_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tca_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tdd_Tale.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tdd_Tale.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tdt_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tdt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/te_Telu.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/te_Telu.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "తెలుగు"
 population: 95478480
 region: "IN"
 exemplar_chars {
   base: "అ ఆ ఇ ఈ ఉ ఊ ఋ ౠ ఌ ౡ ఎ ఏ ఐ ఒ ఓ ఔ ఁ ం ః క ఖ గ ఘ ఙ చ ఛ జ ఝ ఞ ట ఠ డ ఢ ణ త థ ద ధ న ప ఫ బ భ మ య ర ఱ ల వ శ ష స హ ళ ా ి ీ ు ూ ృ ౄ ె ే ై ొ ో ౌ ్ ౕ ౖ"
   auxiliary: "‌‍ ౦ ౧ ౨ ౩ ౪ ౫ ౬ ౭ ౮ ౯"
   marks: "◌ఁ ◌ం ◌ః ◌ా ◌ి ◌ీ ◌ు ◌ూ ◌ృ ◌ౄ ◌ె ◌ే ◌ొ ◌ో ◌ౌ ◌్ ◌ౖ ◌ౢ ◌ౣ"
-  numerals: "- ‑ , . % ‰ + 0౦ 1౧ 2౨ 3౩ 4౪ 5౫ 6౬ 7౭ 8౮ 9౯"
-  punctuation: "- ‑ , ; : ! ? . \' ‘ ’ \" “ ” ( ) [ ] { }"
+  numerals: "- , . % + 0౦ 1౧ 2౨ 3౩ 4౪ 5౫ 6౬ 7౭ 8౮ 9౯"
+  punctuation: "- , ; : ! ? . \' ‘ ’ \" “ ” ( ) [ ] { }"
   index: "అ ఆ ఇ ఈ ఉ ఊ ఋ ౠ ఎ ఏ ఐ ఒ ఓ ఔ క ఖ గ ఘ ఙ చ ఛ జ ఝ ఞ ట ఠ డ ఢ ణ త థ ద ధ న ప ఫ బ భ మ య ర ఱ ల వ శ ష స హ ళ"
 }
 sample_text {
   masthead_full: "పరతస"
   masthead_partial: "వమ"
   styles: "మానవకుటంబమునందలి వ్యక్తులందరికిని గల ఆజన్మసిద్ధమైన ప్రతిపత్తిని,"
   tester: "మానవజాతి అంతఃకరణమును క్షోభపెట్టిన ఘోరచర్యలు, మానవస్వత్వములయెడ గలిగిన అవజ్ఞా నిరసన భావముల"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tem_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tem_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tet_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tet_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tg_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tg_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tg_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tg_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Тоҷикӣ"
 population: 8873670
 region: "TJ"
 exemplar_chars {
   base: "а б в г ғ д е ё ж з и ӣ й к қ л м н о п р с т у ӯ ф х ҳ ч ҷ ш ъ э ю я"
   auxiliary: "ц щ ы ь"
   marks: "◌̄ ◌̆ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "А Б В Г Ғ Д Е Ё Ж З И Ӣ Й К Қ Л М Н О П Р С Т У Ӯ Ф Х Ҳ Ч Ҷ Ш Ъ Э Ю Я"
 }
 sample_text {
   masthead_full: "ТтАа"
   masthead_partial: "Мм"
   styles: "Бо дарназардошти ин, ки этирофи қадру қимат"
   tester: "бо дарназардошти ин, ки таҳкиру беэътиноӣ ба ҳуқуқи башар боиси"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tg_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/th_Thai.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/th_Thai.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "ภาษาไทย"
 population: 55181920
 region: "TH"
 exemplar_chars {
   base: "ฯ ๆ ๎ ์ ็ ่ ้ ๊ ๋ ก ข ฃ ค ฅ ฆ ง จ ฉ ช ซ ฌ ญ ฎ ฏ ฐ ฑ ฒ ณ ด ต ถ ท ธ น บ ป ผ ฝ พ ฟ ภ ม ย ร ฤ ล ฦ ว ศ ษ ส ห ฬ อ ฮ ํ ะ ั า ๅ ำ ิ ี ึ ื ุ ู เ แ โ ใ ไ ฺ"
   auxiliary: "​"
   marks: "◌ั ◌ิ ◌ุ ◌ู ◌็ ◌ํ"
-  numerals: "% , - . ‑ ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "! \" # \' ( ) * , - . / : @ [ ] ‐ ‑ – — ‘ ’ “ ” … ′ ″"
+  numerals: "% , - . + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "! \" # \' ( ) * , - . / : @ [ ] – — ‘ ’ “ ” …"
   index: "ก ข ฃ ค ฅ ฆ ง จ ฉ ช ซ ฌ ญ ฎ ฏ ฐ ฑ ฒ ณ ด ต ถ ท ธ น บ ป ผ ฝ พ ฟ ภ ม ย ร ฤ ล ฦ ว ศ ษ ส ห ฬ อ ฮ"
 }
 sample_text {
   masthead_full: "มนษย"
   masthead_partial: "ทง"
   styles: "โดยที่การไม่นำพาและการหมิ่นในคุณค่าของสิทธิมนุษยชน"
   tester: "โดยที่ประชาชนแห่งสหประชาชาติได้ยืนยันอีกครั้งไว้ในกฎบัตรถึงศรัทธาในสิทธิมนุษยชนขั้นพื้นฐาน"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/thf_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/thf_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ths_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ths_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ti_Ethi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ti_Ethi.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 population: 10145910
 region: "ER"
 region: "ET"
 region: "IL"
 exemplar_chars {
   base: "፟ ሀ-ሆ ለ-ቆ ቈ ቊ-ቍ ቐ-ቖ ቘ ቚ-ቝ በ-ኆ ኈ ኊ-ኍ ነ-ኮ ኰ ኲ-ኵ ኸ-ኾ ዀ ዂ-ዅ ወ-ዎ ዐ-ዖ ዘ-ዮ ደ-ዷ ጀ-ጎ ጐ ጒ-ጕ ጠ-ፗ"
   auxiliary: "᎐ ᎑ ᎒ ᎓ ᎔ ᎕ ᎖ ᎗ ᎘ ᎙ ሇ ⶀ ᎀ ᎁ ᎂ ᎃ ⶁ ⶂ ⶃ ⶄ ቇ ᎄ ᎅ ᎆ ᎇ ⶅ ⶆ ⶇ ኇ ⶈ ⶉ ⶊ ኯ ዏ ⶋ ዯ ⶌ ዸ ዹ ዺ ዻ ዼ ዽ ዾ ዿ ⶍ ⶎ ጏ ጘ ጙ ጚ ጛ ጜ ጝ ጞ ጟ ⶓ ⶔ ⶕ ⶖ ⶏ ⶐ ⶑ ᎈ ᎉ ᎊ ᎋ ᎌ ᎍ ᎎ ᎏ ⶒ ፘ ፙ ፚ ⶠ ⶡ ⶢ ⶣ ⶤ ⶥ ⶦ ⶨ ⶩ ⶪ ⶫ ⶬ ⶭ ⶮ ⶰ ⶱ ⶲ ⶳ ⶴ ⶵ ⶶ ⶸ ⶹ ⶺ ⶻ ⶼ ⶽ ⶾ ⷀ ⷁ ⷂ ⷃ ⷄ ⷅ ⷆ ⷈ ⷉ ⷊ ⷋ ⷌ ⷍ ⷎ ⷐ ⷑ ⷒ ⷓ ⷔ ⷕ ⷖ ⷘ ⷙ ⷚ ⷛ ⷜ ⷝ ⷞ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "ሀ ለ ሐ መ ሠ ረ ሰ ሸ ቀ ቈ ቐ ቘ በ ቨ ተ ቸ ኀ ኈ ነ ኘ አ ከ ኰ ኸ ዀ ወ ዐ ዘ ዠ የ ደ ጀ ገ ጐ ጠ ጨ ጰ ጸ ፀ ፈ ፐ"
 }
 sample_text {
   masthead_full: "ብመንፅ"
   masthead_partial: "ርክ"
   styles: "ኦብ ዓለም ንናይ ኩሎም ሰባት ተፈጥሮኦዊ ክብሪትን ንማዕሪን ዘይገሃሱን"
   tester: "ንሰብኦዊ መሰላት ኦብ ግምት ዘይምእታውን ምጥሓስን ንሕልና ወዲ ሰብ ዘቑሰለን ኦሪሜናዊ ተግባራት"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tiv_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tiv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tiw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tiw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tjs_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tjs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tk_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tk_Cyrl.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -16,10 +16,10 @@
   tester: "адам хукукларына болан әсгермезлик этмегиң ве йигренҗиң адамзадың"
   poster_sm: "адам өзүниң"
   poster_md: "Бирлешен"
   poster_lg: "Хемме"
   specimen_48: "Бирлешен Миллетлер Гурамасының агзалары-дөвлетлериң"
   specimen_36: "Хич ким гулчулыкда я-да табынлыкда сакланмалы дәлдир: гулчулык ве гул сөвдасы әхли гөрнүшинде гадаган эдилйәр."
   specimen_32: "Хер бир адам Конституция я-да канун тарапындан оңа берлен эсасы хукукларың бозулан ягдайында долы ыгтыярлы милли судлар тарапындан өз хукукларының дикелдилмегине хаклыдыр."
-  specimen_21: "Хич ким эсассыз туссаг эдилип, сакланылып я-да ковулып билинмез.\nХер бир адам өзүниң хукукларының ве борчларының аныкланылмагы үчин ве оңа гөркезилйән җенаят айыпламаның догрулыгыны аныкламак үчин гарашсыз, битарап суд тарапындан адалатлылыгың  хемме талапларына лайыклыкда долы деңлик эсасында өз ишине серетдирмәге хаклыдыр."
+  specimen_21: "Хич ким эсассыз туссаг эдилип, сакланылып я-да ковулып билинмез.\nХер бир адам өзүниң хукукларының ве борчларының аныкланылмагы үчин ве оңа гөркезилйән җенаят айыпламаның догрулыгыны аныкламак үчин гарашсыз, битарап суд тарапындан адалатлылыгың хемме талапларына лайыклыкда долы деңлик эсасында өз ишине серетдирмәге хаклыдыр."
   specimen_16: "Хич кимиң шахсы ве машгала дурмушына эсассыз аралашылып, онуң яшайыш җайының элдегрилмесизлигине, онуң хабар серишделериниң сырына я-да онуң намысына ве абрайына эсассыз каст эдилип билинмез. Хер бир адам шейле аралашылмакдан ве каст эдилмекден канун тарапындан горага хаклыдыр.\nХич бир адам пикир, выҗдан ве дин азатлыгына хаклыдыр, бу хак өз диниңи я-да гарайшыңы эркин үйтгедип билмеклиги, эркинликде өз диниңе я-да гарайышларыңа өзбашдак я-да көпчүликлейин уюп билмеклиги, көпчүликлейин я-да еке-тәк ягдайда өвренмеклиги, худая гуллук этмеклиги хем-де ритуал дәплери ерине етирмеклиги өз ичине аляр."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tk_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tk_Latn.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -16,10 +16,10 @@
   tester: "Adam hukuklarynyň äsgerilmezliginiň we ýigrenilmeginiň adamzat"
   poster_sm: "Agza-döwletleriň"
   poster_md: "Halklaryň"
   poster_lg: "hemmesi"
   specimen_48: "Birleşen Milletleriň halklarynyň esasy adam hukuklaryna,"
   specimen_36: "Hiç kim gulçulykda ýa-da baknalykda saklanyp bilinmez; gulçulygyň we gul söwdasynyň ähli görnüşleri gadagan edilýär."
   specimen_32: "Her bir adam konstitusiýanyň ýa-da kanunyň özüne beren esasy hukuklary bozulan ýagdaýynda öz hukuklaryny başarnykly milli sudlar arkaly netijeli dikeltmäge haklydyr."
-  specimen_21: "Hiç kim eden-ýtdilikli tussag edilmäge, saklanylmaga ýa-da ýurdundan kowulmaga duçar edilip bilinmez.    \nHer bir adam öz hukuklarynyň we borçlarynyň kesgitlenmegi we özüne bildirilen jenaýat aýyplamasynyň esaslydygyny anyklamak üçin doly deňhukuklylyk esasynda öz işiniň açyk we adalatyň ähli talaplaryna laýyklykda garaşsyz we bitarap sudda seredilmegine haklydyr."
+  specimen_21: "Hiç kim eden-ýtdilikli tussag edilmäge, saklanylmaga ýa-da ýurdundan kowulmaga duçar edilip bilinmez. \nHer bir adam öz hukuklarynyň we borçlarynyň kesgitlenmegi we özüne bildirilen jenaýat aýyplamasynyň esaslydygyny anyklamak üçin doly deňhukuklylyk esasynda öz işiniň açyk we adalatyň ähli talaplaryna laýyklykda garaşsyz we bitarap sudda seredilmegine haklydyr."
   specimen_16: "Hiç kim öz şahsy we maşgala durmuşyna eden-ýtdilikli gatyşylmagyna, öz ýaşaýyş jaýynyň eldegrilmezliginiň, hat-habar aragatnaşyklarynyň gizlinliginiň ýa-da öz at-abraýynyň we mertebesiniň garawsyz bozulmagyna duçar edilip bilinmez. Her bir adam öz durmuşyna beýle gatyşmalardan ýa-da kastdan kanun arkaly goranmaga haklydyr.\nHer bir adam pikir, ynam we din azatlygyna haklydyr; bu hukuk diniňi ýa-da ynamyňy üýtgetmek azatlygyny we öz diniňe ýa-da ynamyňa uýmak hem-de oňa ýeke özüň we il bilen bile hususy tertipde, şeýle-de köpçülikde sežde etmek, ýörelge, hudaýa çokunmak we dini ritual dessurlaryň azatlygyny öz içine alýar."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tly_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tly_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tn_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/to_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/to_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 autonym: "Faka Tonga"
 population: 100790
 region: "TO"
 exemplar_chars {
   base: "a á ā e é ē f h i í ī k l m n {ng} o ó ō p s t u ú ū v ʻ"
   auxiliary: "à ă â å ä æ b c ç d è ĕ ê ë g ì ĭ î ï j ñ ò ŏ ô ö ø œ q r ù ŭ û ü w x y ÿ z"
   marks: "◌́ ◌̄"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A E F H I K L M N {NG} O P S T U V ʻ"
 }
 sample_text {
   masthead_full: "KkOo"
   masthead_partial: "Ee"
   styles: "Ko e me’a ‘i he mahino ko e ngeia fakaenatula"
   tester: "Peako e me’a ‘i he mahino ko hono li’ekina mo ta’efaka’apa’apa’i ‘a e"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tob_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tob_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/toi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/toi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/toj_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/toj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/top_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/top_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tpi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tpi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tr_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tr_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 region: "TR"
 region: "UA"
 region: "UZ"
 exemplar_chars {
   base: "a b c ç d e f g ğ h ı i İ j k l m n o ö p r s ş t u ü v y z"
   auxiliary: "á à ă â å ä ã ā æ é è ĕ ê ë ē í ì ĭ î ï ī ñ ó ò ŏ ô ø ō œ q ß ú ù ŭ û ū w x ÿ"
   marks: "◌̂ ◌̆ ◌̇ ◌̈ ◌̦ ◌̧"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B C Ç D E F G H I İ J K L M N O Ö P Q R S Ş T U Ü V W X Y Z"
 }
 sample_text {
   masthead_full: "BbÜü"
   masthead_partial: "Tt"
   styles: "İnsanlık ailesinin bütün üyelerinde bulunan"
   tester: "İnsan haklarının tanınmaması ve hor görülmesinin insanlık vicdanını"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/trp_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/trp_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tru_Syrc.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tru_Syrc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ts_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ts_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tsz_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tsz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tt_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tt_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tt_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tt_Cyrl.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 autonym: "Татарча"
 population: 1984108
 region: "RU"
 exemplar_chars {
   base: "а ә б в г д е ё ж җ з и й к л м н ң о ө п р с т у ү ф х һ ц ч ш щ ъ ы ь э ю я"
   auxiliary: "ғ қ"
   marks: "◌̆ ◌̈"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # ′ ″"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "А Ә Б В Г Д Е Ё Ж Җ З И Й К Л М Н Ң О Ө П Р С Т У Ү Ф Х Һ Ц Ч Ш Щ Ъ Ы Ь Э Ю Я"
 }
 sample_text {
   masthead_full: "БбАа"
   masthead_partial: "Рр"
   styles: "Кешелек гаиләсенең бөтен әгъзаларына хас"
   tester: "кеше хокукларына кимсетеп һәм җирәнеп каруның вәхшилеккә китерүен,"
   poster_sm: "җәберләүгә"
   poster_md: "Кешенең төп"
   poster_lg: "Барлык"
   specimen_48: "Берләшкен Милләтләр Оешмасы әгъзасы булган дәүләтләрнең кеше"
   specimen_36: "әлеге хокукларны һәм ирекләрне анлау бу йөкләмәләрне тулысынча үтәүдә бик зур әһәмияткә ия булуын истә тотып,"
   specimen_32: "Конституция яки закон биргән тон хокуклардан мәхрүм ителгән очракта, һәр кешенең ул хокукларын компетентлы милли судлар аша кире кайтарылып бирелүен таләп итәргә хокукы бар."
   specimen_21: "Беркем дә нигезсез рәвештә кулга алынуга, тоткарлануга, куылуга дучар ителергә тиеш түгел.\nҺәр кешенең үз хокукларын һәм бурычларын билгеләр очен һәм аны җинаять җаваплылыгына тартуның нигезле булуын ачыклар очен, туды титезлелек нигезендә үз эшенең ачык рәвештә, мөстәкыйль, гадел һәм бәйсез суд аша каралуын таләп итәргә хокукы бар."
-  specimen_16: "Бер кеше дә шәхси һәм гаилә тормышына, торак иминлегенә кагылуга, язышү, хәбәрләшү серенә, абруена һәм намусына нигезсез катиашуга дучар ителергә тиеш түгел.  Шундый кысулардан, яисә дучар ителүләрдән һәр кешенең закон белән якланырга хокукы бар.\nҺәр кешенең фикер, вөҗдан һәм дин ирегенә хокукы бар; бу хокук Аллага табынуны, йола куша торган дини тәртипләрне үгәүне эченә ала, һәр кешенең бер үзе генә яисә башкалар белән бергәлән аерым рәвештә яки ачыктаначык үз карашларын, үз динен алыштырырга аки тотарга хокукы бар.\nҺәр кеше ялга хокуклы һәм эш көнең тиешле чикләрдә кыскартуны да кертен, ел саси түләүле ял алырга, эштән буш вакытка хокукы бар."
+  specimen_16: "Бер кеше дә шәхси һәм гаилә тормышына, торак иминлегенә кагылуга, язышү, хәбәрләшү серенә, абруена һәм намусына нигезсез катиашуга дучар ителергә тиеш түгел. Шундый кысулардан, яисә дучар ителүләрдән һәр кешенең закон белән якланырга хокукы бар.\nҺәр кешенең фикер, вөҗдан һәм дин ирегенә хокукы бар; бу хокук Аллага табынуны, йола куша торган дини тәртипләрне үгәүне эченә ала, һәр кешенең бер үзе генә яисә башкалар белән бергәлән аерым рәвештә яки ачыктаначык үз карашларын, үз динен алыштырырга аки тотарга хокукы бар.\nҺәр кеше ялга хокуклы һәм эш көнең тиешле чикләрдә кыскартуны да кертен, ел саси түләүле ял алырга, эштән буш вакытка хокукы бар."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tt_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tvl_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tvl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/txg_Tang.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/txg_Tang.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/txo_Toto.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/txo_Toto.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 region: "IN"
 population: 1411
 exemplar_chars {
   base: "𞊐 𞊑 𞊒 𞊓 𞊔 𞊕 𞊖 𞊗 𞊘 𞊙 𞊚 𞊛 𞊜 𞊝 𞊞 𞊟 𞊠 𞊡 𞊢 𞊣 𞊤 𞊥 𞊦 𞊧 𞊨 𞊩 𞊪 𞊫 𞊬 𞊭"
   marks: "◌𞊮"
 }
 sample_text {
-  masthead_full: "𞊒𞊧𞊜𞊭"  # tehwa, "sweet" (Toto Dictionary app)
-  masthead_partial: "𞊙𞊭"  # saa, "house" (Toto Writer's Guide)
+  masthead_full: "𞊒𞊧𞊜𞊭" # tehwa, "sweet" (Toto Dictionary app)
+  masthead_partial: "𞊙𞊭" # saa, "house" (Toto Writer's Guide)
   styles: "𞊡𞊛𞊥 𞊞𞊭 𞊙𞊣𞊖𞊭𞊑𞊡 𞊞𞊭 𞊥𞊑𞊡𞊔𞊪 𞊙𞊭 𞊑𞊭𞊗𞊭𞊛𞊖𞊡 𞊡𞊚𞊪 𞊙𞊦𞊘𞊒𞊦𞊘𞊔𞊪 𞊒𞊨𞊒𞊭."
   tester: "𞊡𞊛𞊥 𞊞𞊭 𞊙𞊣𞊖𞊭𞊑𞊡 𞊞𞊭 𞊥𞊑𞊡𞊔𞊪 𞊙𞊭 𞊑𞊭𞊗𞊭𞊛𞊖𞊡 𞊡𞊚𞊪 𞊙𞊦𞊘𞊒𞊦𞊘𞊔𞊪 𞊒𞊨𞊒𞊭."
   poster_sm: "𞊞𞊭𞊞𞊭𞊛𞊔𞊨𞊖𞊡"
   poster_md: "𞊒𞊨𞊐𞊭𞊜"
-  poster_lg: "𞊕𞊦𞊮𞊜𞊭"  # géwa, "know" (Toto Dictionary app)
+  poster_lg: "𞊕𞊦𞊮𞊜𞊭" # géwa, "know" (Toto Dictionary app)
   # "styles" above and all specimens below from "Story of the Bees", L2/19-330
   specimen_48: "𞊡𞊛𞊥 𞊞𞊭 𞊙𞊣𞊖𞊭𞊑𞊡 𞊞𞊭 𞊥𞊑𞊡𞊔𞊪 𞊙𞊭 𞊑𞊭𞊗𞊭𞊛𞊖𞊡 𞊡𞊚𞊪 𞊙𞊦𞊘𞊒𞊦𞊘𞊔𞊪 𞊒𞊨𞊒𞊭."
   specimen_36: "𞊡𞊛𞊥 𞊞𞊭 𞊙𞊣𞊖𞊭𞊑𞊡 𞊞𞊭 𞊥𞊑𞊡𞊔𞊪 𞊙𞊭 𞊑𞊭𞊗𞊭𞊛𞊖𞊡 𞊡𞊚𞊪 𞊙𞊦𞊘𞊒𞊦𞊘𞊔𞊪 𞊒𞊨𞊒𞊭. 𞊥𞊑𞊡 𞊞𞊭 𞊒𞊭𞊘𞊙𞊭 𞊛𞊭𞊭𞊮𞊘𞊒𞊭𞊓𞊡𞊘𞊖𞊡 𞊥𞊒𞊭 𞊛𞊥𞊥𞊮𞊘𞊖𞊙𞊭."
   specimen_32: "𞊡𞊛𞊥 𞊞𞊭 𞊙𞊣𞊖𞊭𞊑𞊡 𞊞𞊭 𞊥𞊑𞊡𞊔𞊪 𞊙𞊭 𞊑𞊭𞊗𞊭𞊛𞊖𞊡 𞊡𞊚𞊪 𞊙𞊦𞊘𞊒𞊦𞊘𞊔𞊪 𞊒𞊨𞊒𞊭. 𞊥𞊑𞊡 𞊞𞊭 𞊒𞊭𞊘𞊙𞊭 𞊛𞊭𞊭𞊮𞊘𞊒𞊭𞊓𞊡𞊘𞊖𞊡 𞊥𞊒𞊭 𞊛𞊥𞊥𞊮𞊘𞊖𞊙𞊭. 𞊜𞊫𞊔𞊪𞊒𞊭 𞊞𞊭 𞊝 𞊡𞊛𞊭𞊑𞊡𞊟𞊦 𞊔𞊪𞊪𞊮𞊛𞊔𞊪 𞊜𞊭𞊘𞊚𞊭𞊘𞊖𞊡 𞊠𞊦𞊮𞊘𞊜𞊭."
   specimen_21: "𞊡𞊛𞊥 𞊞𞊭 𞊙𞊣𞊖𞊭𞊑𞊡 𞊞𞊭 𞊥𞊑𞊡𞊔𞊪 𞊙𞊭 𞊑𞊭𞊗𞊭𞊛𞊖𞊡 𞊡𞊚𞊪 𞊙𞊦𞊘𞊒𞊦𞊘𞊔𞊪 𞊒𞊨𞊒𞊭. 𞊥𞊑𞊡 𞊞𞊭 𞊒𞊭𞊘𞊙𞊭 𞊛𞊭𞊭𞊮𞊘𞊒𞊭𞊓𞊡𞊘𞊖𞊡 𞊥𞊒𞊭 𞊛𞊥𞊥𞊮𞊘𞊖𞊙𞊭. 𞊜𞊫𞊔𞊪𞊒𞊭 𞊞𞊭 𞊝 𞊡𞊛𞊭𞊑𞊡𞊟𞊦 𞊔𞊪𞊪𞊮𞊛𞊔𞊪 𞊜𞊭𞊘𞊚𞊭𞊘𞊖𞊡 𞊠𞊦𞊮𞊘𞊜𞊭. 𞊥𞊑𞊡𞊔𞊪 𞊝 𞊡𞊘𞊓𞊭𞊕𞊡𞊛𞊭 𞊛𞊭𞊭𞊮𞊘𞊒𞊭𞊖𞊙𞊭𞊟𞊭𞊘 𞊞𞊫𞊓𞊡𞊘𞊖𞊡."
   specimen_16: "𞊡𞊛𞊥 𞊞𞊭 𞊙𞊣𞊖𞊭𞊑𞊡 𞊞𞊭 𞊥𞊑𞊡𞊔𞊪 𞊙𞊭 𞊑𞊭𞊗𞊭𞊛𞊖𞊡 𞊡𞊚𞊪 𞊙𞊦𞊘𞊒𞊦𞊘𞊔𞊪 𞊒𞊨𞊒𞊭. 𞊥𞊑𞊡 𞊞𞊭 𞊒𞊭𞊘𞊙𞊭 𞊛𞊭𞊭𞊮𞊘𞊒𞊭𞊓𞊡𞊘𞊖𞊡 𞊥𞊒𞊭 𞊛𞊥𞊥𞊮𞊘𞊖𞊙𞊭. 𞊜𞊫𞊔𞊪𞊒𞊭 𞊞𞊭 𞊝 𞊡𞊛𞊭𞊑𞊡𞊟𞊦 𞊔𞊪𞊪𞊮𞊛𞊔𞊪 𞊜𞊭𞊘𞊚𞊭𞊘𞊖𞊡 𞊠𞊦𞊮𞊘𞊜𞊭. 𞊥𞊑𞊡𞊔𞊪 𞊝 𞊡𞊘𞊓𞊭𞊕𞊡𞊛𞊭 𞊛𞊭𞊭𞊮𞊘𞊒𞊭𞊖𞊙𞊭𞊟𞊭𞊘 𞊞𞊫𞊓𞊡𞊘𞊖𞊡. 𞊭𞊓𞊪 𞊥𞊑𞊡𞊔𞊪 𞊛𞊭𞊭𞊮𞊘𞊒𞊭𞊜𞊭 𞊝 𞊡𞊘𞊓𞊭𞊕𞊡𞊛𞊭 𞊞𞊫𞊝𞊦 𞊖𞊫𞊞𞊫𞊗𞊭."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ty_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ty_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tyv_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tyv_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,11 @@
   styles: "Кижи төрелгетен аймааның бүгү кежигүннериниң"
   tester: "кижиниң эргелеринге тоомча чок болгаш көөр хөөн чок чоруктуң"
   poster_sm: "чоннар аразынга"
   poster_md: "Каттышкан"
   poster_lg: "Бүгү"
   specimen_48: "кежигүнкүрүнелерниң Каттышкан Нациялар Организациязыбиле кады"
   specimen_36: "Кымдаа кулданыгга азы хостуг эвес байдалга туттунмас ужурлуг; кулданыгның болгаш кул садарының бүгү хевирлери хоруглуг."
-  specimen_32: "Кижи бүрүзү дыштанылгага база хостуг үеге эргелиг, ооң иштинде  ажыл хүнүн  шын кызыгаарлаарынга база  өйлепөйлеп  бээр төлевирлиг  шөлээге  эргелиг."
-  specimen_21: "Кижи бүрүзү ук Угуулгада айыттынган эргелер болгаш хосталгаларны долузубиле хандырып турар социал болгаш улустар аразының корумчурумунга эргелиг.\nУк Угуулгада чүүдаа чүве кайыбир күрүнеге, бөлүкке азы тус кижилерге ук Угуулгада айыттынган эргелер болгаш хосталгаларны узуткаарынче угланган ажылдар чорударынга азы кылдыныглар кылырынга эрге берип турар деп  тайылбырлаттынып болбас."
-  specimen_16: "Кижи төрелгетен аймааның бүгү кежигүннериниң  кижи мөзүзүн, оларның дең болгаш казып болбас эргелерин хүлээп көөрү хосталганың, чөптүг чоруктуң база бүгүниити тайбыңның үндезини болурун кичээнгейге албышаан; база\nкижиниң эргелеринге тоомча чок болгаш көөр хөөн чок чоруктуң кижи төрелгетенниң сагыжын аартып дүвүреткен дерзии үүлгедиглерге чедиргенин база кижилер  сөстүң болгаш үзелдерниң   хосталгазынга эргелиг, коргуушкун болгаш түрегделден хостуг  делегейни тургузары кижилерниң бедик чүткүлү кылдыр чарлаттынганын  кичээнгейге албышаан; база\nчоннар аразынга эпнайыралдыг харылзааларның сайзыралын деткиириниң эргежок чугулазын кичээнгейге албышаан; база"
+  specimen_32: "Кижи бүрүзү дыштанылгага база хостуг үеге эргелиг, ооң иштинде ажыл хүнүн шын кызыгаарлаарынга база өйлепөйлеп бээр төлевирлиг шөлээге эргелиг."
+  specimen_21: "Кижи бүрүзү ук Угуулгада айыттынган эргелер болгаш хосталгаларны долузубиле хандырып турар социал болгаш улустар аразының корумчурумунга эргелиг.\nУк Угуулгада чүүдаа чүве кайыбир күрүнеге, бөлүкке азы тус кижилерге ук Угуулгада айыттынган эргелер болгаш хосталгаларны узуткаарынче угланган ажылдар чорударынга азы кылдыныглар кылырынга эрге берип турар деп тайылбырлаттынып болбас."
+  specimen_16: "Кижи төрелгетен аймааның бүгү кежигүннериниң кижи мөзүзүн, оларның дең болгаш казып болбас эргелерин хүлээп көөрү хосталганың, чөптүг чоруктуң база бүгүниити тайбыңның үндезини болурун кичээнгейге албышаан; база\nкижиниң эргелеринге тоомча чок болгаш көөр хөөн чок чоруктуң кижи төрелгетенниң сагыжын аартып дүвүреткен дерзии үүлгедиглерге чедиргенин база кижилер сөстүң болгаш үзелдерниң хосталгазынга эргелиг, коргуушкун болгаш түрегделден хостуг делегейни тургузары кижилерниң бедик чүткүлү кылдыр чарлаттынганын кичээнгейге албышаан; база\nчоннар аразынга эпнайыралдыг харылзааларның сайзыралын деткиириниң эргежок чугулазын кичээнгейге албышаан; база"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tzh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tzh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tzm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tzm_Latn.textproto`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "Tamaziɣt"
 population: 3485046
 region: "MA"
 exemplar_chars {
   base: "a A b B c C d D ḍ Ḍ e E ɛ Ɛ f F g G {gʷ} {Gʷ} ɣ Ɣ h H ḥ Ḥ i I j J k K {kʷ} {Kʷ} l L m M n N q Q r R ṛ Ṛ s S ṣ Ṣ t T ṭ Ṭ u U w W x X y Y z Z"
   auxiliary: "o O p P v V"
   marks: "◌̣"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D Ḍ E Ɛ F G Ɣ H Ḥ I J K L M N Q R Ṛ S Ṣ T Ṭ U W X Y Z"
 }
 sample_text {
   masthead_full: "IiMm"
   masthead_partial: "Dd"
   styles: "Imi asmussen n lḥwerma i ttalasen akkw yâggalen"
   tester: "Imi kra n widn nesmussun ara izerfan n wemdan d widn iḥeqqren"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/tzo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/tzo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/udu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/udu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ug_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ug_Arab.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 autonym: "ئۇيغۇرچە (ئەرەب)"
 population: 7670114
 region: "AF"
 region: "CN"
 exemplar_chars {
   base: "{ئا} {ئه} {ئو} {ئۇ} {ئۆ} {ئۈ} {ئې} {ئى} ا ە ب پ ت ج چ خ د ر ز ژ س ش غ ف ق ك گ ڭ ل م ن ھ و ۇ ۆ ۈ ۋ ې ى ي"
   auxiliary: "‎‏ ئ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
   index: "{ئا} {ئه} {ئو} {ئۇ} {ئۆ} {ئۈ} {ئې} {ئى} ا ە ب پ ت ج چ خ د ر ز ژ س ش غ ف ق ك گ ڭ ل م ن ھ و ۇ ۆ ۈ ۋ ې ى ي"
 }
 sample_text {
   masthead_full: "ھەمئ"
   masthead_partial: "اد"
   styles: "ئىنسانلار ئائىلىسىنىڭ بارلىق ئەزالىرنىڭ ئۆزىگە"
   tester: "كىشىلىك ھوقۇقىغا ئېتىبارسىز قاراش ۋە ھاقارەت كەلتۈرۈش ئەۋج ئېلىپ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ug_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ug_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ug_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ug_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/uga_Ugar.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/uga_Ugar.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/uk_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/uk_Cyrl.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 region: "RS"
 region: "SK"
 region: "UA"
 exemplar_chars {
   base: "а б в г ґ д е є ж з и і ї й к л м н о п р с т у ф х ц ч ш щ ь ю я ʼ"
   auxiliary: "{а́} {е́} ё {є́} {и́} {і́} {ї́} {о́} {у́} ъ ы э {ю́} {я́}"
   marks: "◌̆ ◌̈ ◌́"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ – , ; : ! ? . \' ’ \" “ „ « » ( ) [ ] { } § @ * / \\ №"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – , ; : ! ? . \' ’ \" “ „ « » ( ) [ ] { } @ * / \\ №"
   index: "А Б В Г Ґ Д Е Є Ж З И І Ї Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ю Я"
 }
 sample_text {
   masthead_full: "ВвСс"
   masthead_partial: "Іі"
   styles: "Беручи до уваги, що визнання гідності, яка"
   tester: "беручи до уваги, що зневажання і нехтування правами людини призвели"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/umb_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/umb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/unr_Beng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/unr_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/unr_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/unr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/unr_Nagm.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/unr_Nagm.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -15,13 +15,13 @@
   tester: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔 𞓐𞓡𞓐𞓐 𞓕𞓢𞓝𞓚𞓓𞓕𞓣 𞓢𞓐 𞓣𞓤𞓕𞓙 𞓑𞓕𞓚𞓝𞓚𞓗𞓕𞓗𞓕𞓝 𞓣𞓤 𞓖𞓕𞓨𞓕𞓧 𞓖𞓐𞓣𞓐𞓔𞓓𞓤𞓝𞓤 𞓕𞓙𞓡𞓕𞓨𞓕𞓡 𞓐𞓡𞓐𞓐 𞓤𞓢𞓟𞓕𞓒"
   poster_sm: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔"
   poster_md: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐"
   poster_lg: "𞓛𞓐𞓗𞓤𞓨"
   specimen_48: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔 𞓐𞓡𞓐𞓐 𞓕𞓢𞓝𞓚𞓓𞓕𞓣 𞓢𞓐 𞓣𞓤𞓕𞓙 𞓑𞓕𞓚𞓝𞓚𞓗𞓕𞓗𞓕𞓝 𞓣𞓤 𞓖𞓕𞓨𞓕𞓧 𞓖𞓐𞓣𞓐𞓔𞓓𞓤𞓝𞓤 𞓕𞓙𞓡𞓕𞓨𞓕𞓡"
   specimen_36: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔 𞓐𞓡𞓐𞓐 𞓕𞓢𞓝𞓚𞓓𞓕𞓣 𞓢𞓐 𞓣𞓤𞓕𞓙 𞓑𞓕𞓚𞓝𞓚𞓗𞓕𞓗𞓕𞓝 𞓣𞓤 𞓖𞓕𞓨𞓕𞓧 𞓖𞓐𞓣𞓐𞓔𞓓𞓤𞓝𞓤 𞓕𞓙𞓡𞓕𞓨𞓕𞓡 𞓐𞓡𞓐𞓐 𞓤𞓢𞓟𞓕𞓒 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕."
   specimen_32: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔 𞓐𞓡𞓐𞓐 𞓕𞓢𞓝𞓚𞓓𞓕𞓣 𞓢𞓐 𞓣𞓤𞓕𞓙 𞓑𞓕𞓚𞓝𞓚𞓗𞓕𞓗𞓕𞓝 𞓣𞓤 𞓖𞓕𞓨𞓕𞓧 𞓖𞓐𞓣𞓐𞓔𞓓𞓤𞓝𞓤 𞓕𞓙𞓡𞓕𞓨𞓕𞓡 𞓐𞓡𞓐𞓐 𞓤𞓢𞓟𞓕𞓒 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕."
-  specimen_21: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔 𞓐𞓡𞓐𞓐 𞓕𞓢𞓝𞓚𞓓𞓕𞓣 𞓢𞓐 𞓣𞓤𞓕𞓙 𞓑𞓕𞓚𞓝𞓚𞓗𞓕𞓗𞓕𞓝 𞓣𞓤 𞓖𞓕𞓨𞓕𞓧 𞓖𞓐𞓣𞓐𞓔𞓓𞓤𞓝𞓤 𞓕𞓙𞓡𞓕𞓨𞓕𞓡 𞓐𞓡𞓐𞓐 𞓤𞓢𞓟𞓕𞓒 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕.  𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙.  𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙."
-  specimen_16: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔 𞓐𞓡𞓐𞓐 𞓕𞓢𞓝𞓚𞓓𞓕𞓣 𞓢𞓐 𞓣𞓤𞓕𞓙 𞓑𞓕𞓚𞓝𞓚𞓗𞓕𞓗𞓕𞓝 𞓣𞓤 𞓖𞓕𞓨𞓕𞓧 𞓖𞓐𞓣𞓐𞓔𞓓𞓤𞓝𞓤 𞓕𞓙𞓡𞓕𞓨𞓕𞓡 𞓐𞓡𞓐𞓐 𞓤𞓢𞓟𞓕𞓒 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕.  𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙.  𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙.  𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙.  𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓙𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙."
+  specimen_21: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔 𞓐𞓡𞓐𞓐 𞓕𞓢𞓝𞓚𞓓𞓕𞓣 𞓢𞓐 𞓣𞓤𞓕𞓙 𞓑𞓕𞓚𞓝𞓚𞓗𞓕𞓗𞓕𞓝 𞓣𞓤 𞓖𞓕𞓨𞓕𞓧 𞓖𞓐𞓣𞓐𞓔𞓓𞓤𞓝𞓤 𞓕𞓙𞓡𞓕𞓨𞓕𞓡 𞓐𞓡𞓐𞓐 𞓤𞓢𞓟𞓕𞓒 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕. 𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙. 𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙."
+  specimen_16: "𞓛𞓐𞓗𞓤𞓨 𞓙𞓐𞓡𞓐𞓢𞓐 𞓢𞓤 𞓧𞓕𞓨𞓣𞓕𞓔 𞓐𞓡𞓐𞓐 𞓕𞓢𞓝𞓚𞓓𞓕𞓣 𞓢𞓐 𞓣𞓤𞓕𞓙 𞓑𞓕𞓚𞓝𞓚𞓗𞓕𞓗𞓕𞓝 𞓣𞓤 𞓖𞓕𞓨𞓕𞓧 𞓖𞓐𞓣𞓐𞓔𞓓𞓤𞓝𞓤 𞓕𞓙𞓡𞓕𞓨𞓕𞓡 𞓐𞓡𞓐𞓐 𞓤𞓢𞓟𞓕𞓒 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕. 𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙. 𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙. 𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓕𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓛𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙. 𞓚𞓨𞓢𞓟 𞓢𞓤 𞓛𞓤𞓨𞓡𞓐 𞓐𞓡𞓐𞓐𞓖𞓚 𞓑𞓤𞓡𞓤𞓙, 𞓖𞓚𞓟 𞓣𞓤𞓕𞓙 𞓤𞓨𞓤𞓧𞓢𞓐 𞓨𞓕𞓧𞓕 𞓢𞓕𞓨𞓕 𞓐𞓡𞓐𞓐 𞓚𞓨𞓢𞓟 𞓒𞓐𞓐𞓕𞓙𞓝𞓤 𞓙𞓕𞓦𞓤𞓓𞓕𞓮𞓐𞓓𞓕 𞓒𞓤𞓢𞓕 𞓖𞓕𞓦𞓕𞓣 𞓗𞓕𞓢𞓕𞓣 𞓒𞓕𞓦𞓕𞓝𞓚𞓔𞓕𞓕𞓙."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/unr_Orya.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/unr_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/unx_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/unx_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ur_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ur_Arab.textproto`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 population: 288202177
 region: "IN"
 region: "MU"
 region: "PK"
 exemplar_chars {
   base: "ا ب پ ت ٹ ث ج چ ح خ د ڈ ذ ر ڑ ز ژ س ش ص ض ط ظ ع غ ف ق ک گ ل م ن و ہ ھ ء ی ے"
   auxiliary: "؀؁؂؃‌‍‎‏ ً ٌ ٍ َ ُ ِ ّ ْ ٔ ٖ ٗ ٘ ٰ أ آ ں ؤ ۂ ۃ ئ ٻ ة ٺ ټ ٽ ه ي"
-  numerals: "‎ - ‑ , ٫ ٬ . % ‰ + 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
+  numerals: "‎ - , ٫ ٬ . % + 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
   punctuation: "، ؍ ٫ ٬ ؛ : ؟ . ۔ ( ) [ ]"
   index: "ا ب پ ت ٹ ث ج چ ح خ د ڈ ذ ر ڑ ز ژ س ش ص ض ط ظ ع غ ف ق ک گ ل م ن و ہ ھ ء ی ے"
 }
 sample_text {
   masthead_full: "تمان"
   masthead_partial: "سآ"
   styles: "چونکہ ہر انسان کی ذاتی عزت اور حرمت اور انسانوں"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ura_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ura_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/uz_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/uz_Arab.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Uzbek (Arabic)"
 autonym: "اوزبیک (عربی)"
 population: 1722258
 region: "AF"
 exemplar_chars {
   base: "ً ٌ ٍ َ ُ ِ ّ ْ ٔ ٰ ء آ أ ؤ ئ ا ب پ ة ت ث ج چ ح خ د ذ ر ز ژ س ش ص ض ط ظ ع غ ف ق ک گ ل م ن ه و ۇ ۉ ی"
   auxiliary: "‌‍‎‏ ټ ځ څ ډ ړ ږ ښ ګ ڼ ي ۍ ې"
-  numerals: "‎ - ‑ , ٫ ٬ . % ٪ ‰ ؉ + − 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
+  numerals: "‎ - , ٫ ٬ . % ٪ ؉ + − 0۰ 1۱ 2۲ 3۳ 4۴ 5۵ 6۶ 7۷ 8۸ 9۹"
   index: "ء آ أ ؤ ئ ا ب پ ة ت ث ټ ج چ ح خ ځ څ د ذ ډ ر ز ړ ږ ژ س ش ښ ص ض ط ظ ع غ ف ق ک ګ گ ل م ن ڼ ه و ۇ ۉ ي ی ۍ ې"
 }
 sample_text {
   masthead_full: "بهرچ"
   masthead_partial: "آد"
   styles: "به‌رچه آده‌مله‌ر ئېرکىن، قه‌درقىممه‌ت ۋه هۇقۇقله‌رده"
   tester: "به‌رچه آده‌مله‌ر ئېرکىن، قه‌درقىممه‌ت ۋه هۇقۇقله‌رده تېڭ بولىب تۇغىله‌دىله‌ر"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/uz_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/uz_Cyrl.textproto`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 population: 4590386
 region: "CN"
 region: "UZ"
 exemplar_chars {
   base: "а б в г ғ д е ё ж з и й к қ л м н о п р с т у ў ф х ҳ ч ш ъ э ю я"
   auxiliary: "ц щ ы ь"
   marks: "◌̆ ◌̈"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "А Б В Г Ғ Д Е Ж З И Й К Қ Л М Н О П Р С Т У Ў Ф Х Ҳ Ч Ш Ъ Э Ю Я"
 }
 sample_text {
   masthead_full: "БбАа"
   masthead_partial: "Рр"
   styles: "Инсон оиласи барча аъзоларига ҳос бўлган"
   tester: "Инсон ҳуқуқларини менсимаслик ва оёқ-ости қилиш одамзод виждонини"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/uz_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/uz_Latn.textproto`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 26480135
 region: "TM"
 region: "TR"
 region: "UZ"
 exemplar_chars {
   base: "a b d e f g h i j k l m n o p q r s t u v x y z {oʻ} {gʻ} {sh} {ch} ʼ"
   auxiliary: "á à ă â å ä ã ā æ c ç é è ĕ ê ë ē í ì ĭ î ï ī ñ ó ò ŏ ô ö ø ō œ ú ù ŭ û ü ū w ÿ"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A B D E F G H I J K L M N O P Q R S T U V X Y Z {Oʻ} {Gʻ} {Sh} {Ch}"
 }
 sample_text {
   masthead_full: "BbAa"
   masthead_partial: "Rr"
   styles: "Inson oilasi barcha aʼzolariga hos boʻlgan"
   tester: "Inson huquqlarini mensimaslik va oyoq-osti qilish odamzod vijdonini"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/vai_Vaii.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/vai_Vaii.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 name: "Vai"
 autonym: "ꕙꔤ"
 population: 131905
 region: "LR"
 exemplar_chars {
   base: "ꔀ ꔁ ꔂ ꔃ ꔄ ꔅ ꔆ ꔇ ꔈ ꔉ ꔊ ꔋ ꔌ ꔍ ꔎ ꔏ ꔐ ꔑ ꔒ ꔓ ꔔ ꔕ ꔖ ꔗ ꔘ ꔙ ꔚ ꔛ ꔜ ꔝ ꔞ ꔟ ꔠ ꔡ ꔢ ꔣ ꔤ ꔥ ꔦ ꔧ ꔨ ꔩ ꔪ ꔫ ꔬ ꔭ ꔮ ꔯ ꔰ ꔱ ꔲ ꔳ ꔴ ꔵ ꔶ ꔷ ꔸ ꔹ ꔺ ꔻ ꔼ ꔽ ꔾ ꔿ ꕀ ꕁ ꕂ ꕃ ꕄ ꕅ ꕆ ꕇ ꕈ ꕉ ꕊ ꕋ ꕌ ꕍ ꕎ ꕏ ꕐ ꕑ ꕒ ꕓ ꕔ ꕕ ꕖ ꕗ ꕘ ꘐ ꕙ ꕚ ꕛ ꕜ ꕝ ꕞ ꕟ ꕠ ꕡ ꕢ ꕣ ꕤ ꕥ ꕦ ꕧ ꕨ ꕩ ꕪ ꘑ ꕫ ꕬ ꕭ ꕮ ꘪ ꕯ ꕰ ꕱ ꕲ ꕳ ꕴ ꕵ ꕶ ꕷ ꕸ ꕹ ꕺ ꕻ ꕼ ꕽ ꕾ ꕿ ꖀ ꖁ ꖂ ꖃ ꖄ ꖅ ꖆ ꖇ ꘒ ꖈ ꖉ ꖊ ꖋ ꖌ ꖍ ꖎ ꖏ ꖐ ꖑ ꖒ ꖓ ꖔ ꖕ ꖖ ꖗ ꖘ ꖙ ꖚ ꖛ ꖜ ꖝ ꖞ ꖟ ꖠ ꖡ ꖢ ꖣ ꖤ ꖥ ꖦ ꖧ ꖨ ꖩ ꖪ ꖫ ꖬ ꖭ ꖮ ꖯ ꖰ ꖱ ꖲ ꖳ ꖴ ꖵ ꖶ ꖷ ꖸ ꖹ ꖺ ꖻ ꖼ ꖽ ꖾ ꖿ ꗀ ꗁ ꗂ ꗃ ꗄ ꗅ ꗆ ꗇ ꗈ ꗉ ꗊ ꗋ ꗌ ꗍ ꗎ ꗏ ꗐ ꗑ ꘫ ꗒ ꗓ ꗔ ꗕ ꗖ ꗗ ꗘ ꗙ ꗚ ꗛ ꗜ ꗝ ꗞ ꗟ ꗠ ꗡ ꗢ ꗣ ꗤ ꗥ ꗦ ꗧ ꗨ ꗩ ꗪ ꗫ ꗬ ꗭ ꗮ ꗯ ꗰ ꗱ ꗲ ꗳ ꗴ ꗵ ꗶ ꗷ ꗸ ꗹ ꗺ ꗻ ꗼ ꗽ ꗾ ꗿ ꘀ ꘁ ꘂ ꘃ ꘄ ꘅ ꘆ ꘇ ꘈ ꘉ ꘊ ꘋ ꘌ"
   auxiliary: "ꘓ ꘔ ꘕ ꘖ ꘗ ꘘ ꘙ ꘚ ꘛ ꘜ ꘝ ꘞ ꘟ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
 }
 sample_text {
   masthead_full: "ꕉꕜꕮꔔ"
   masthead_partial: "ꘋꖸ"
   styles: "ꕪꘋ ꖷ ꗞꔧ ꕀꔤ ꔻꔤ ꔤ ꗃꗡ ꖸꕊ ꗪꗡ ꔻꔤꘂ ꕮ ꘃꖷ ꕉ ꗋꘋ ꕉꕜꕮ"
   tester: "ꕪꘋ ꖷ ꗞ ꕮ ꗛꖺ ꔧ ꕒꕌ ꕪ ꗞ ꖸꕊ ꗋꖺꕰꕊ ꖸ ꕮ, ꗋꖺꕰꕊ ꗷꔤ ꖷ ꖸ ꗞ ꔇꔀ ꖴꘋ ꕉꕜꕮ ꔔꘋ ꕮ"
   poster_sm: "ꕪꘋ ꖷ ꕉ ꗪ ꗪꗡꕯ"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ve_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ve_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/vec_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/vec_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/vep_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/vep_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/vi_Hani.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/vi_Hani.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -11,11 +11,11 @@
   tester: "人民各渃成員聯合國𥪝本憲章㐌𠬠吝姅肯定念信𧵑𨉟𠓨仍權基本𧵑𡥵𠊛、𠓨人品、𠓨價值𧵑每𠊛、𠓨權平等男女、吧㐌𠍣𤍊決心促𢱜進步社會拱如𡏦𥩯各條件𤯨𡄰欣"
   poster_sm: "每𠊛調𣎏權𤯨、自由吧安全個人"
   poster_md: "空埃被查訊咍被對處"
   poster_lg: "空分別種族"
   specimen_48: "畢哿每𠊛調平等𠓀法律吧得法律保衞如饒空𣎏不據事分別芇。畢哿每𠊛調得保衞如饒𢶢吏每形式分別對處違犯本宣言呢共如𢶢吏每行爲驅𠽖分別對處如丕"
   specimen_36: "𢭲認識哴：\n役承認人品本𣎏、各權平等吧空體㳻𢴐𧵑每成員𥪝家庭人類羅基礎朱自由、公平吧和平𨕭世界、\n事侵犯吧䁛常人權㐌引𦤾仍行動殘暴侵犯𬧐良心𧵑人類、吧役𡏦𥩯𠬠世界𥪝𪦆𡥵𠊛得自由言論吧信仰、空群沛𠹾餒𢜝駭吧窮極得䁛羅願望高哿一𧵑類𠊛、"
   specimen_32: "版宣言全世界𧗱人權呢羅𡱩都終朱畢哿各渃吧畢哿各民族打價役實現目標𦓡每個人吧每組織𥪝社會、𨕭基礎㫻記𢖵版宣言呢、𠱊奮鬥促𢱜事尊重各權吧自由基本𧵑𡥵𠊛通過傳播吧教育、拱如𠱊奮鬥擔保朱 每𠊛民、於正各渃成員𧵑聯合國吧於各領土屬權管理𧵑𨉟、公認吧實現仍權吧自由𪦆𠬠格𣎏效果通過仍辦法積極、𥪝範圍國家咍國際。"
-  specimen_21: "𢭲認識哴：\n役承認人品本𣎏、各權平等吧空體㳻𢴐𧵑每成員𥪝家庭人類羅基礎朱自由、公平吧和平𨕭世界、\n事侵犯吧䁛常人權㐌引𦤾仍行動殘暴侵犯𬧐良心𧵑人類、吧役𡏦𥩯𠬠世界𥪝𪦆𡥵𠊛得自由言論吧信仰、空群沛𠹾餒𢜝駭吧窮極得䁛羅願望高哿一𧵑類𠊛、\n人權沛得法律保衞抵每𠊛空𦄾沛浽亂如羅辦法𡳳窮抵挵吏制度強權吧壓逼、\n勤沛勸激役發展關係朋友𡧲各民族、\n人民各渃成員聯合國𥪝本憲章㐌𠬠吝姅肯定念信𧵑𨉟𠓨仍權基本𧵑𡥵𠊛、𠓨人品、𠓨價值𧵑每𠊛、𠓨權平等男女、吧㐌𠍣𤍊決心促𢱜進步社會拱如𡏦𥩯各條件𤯨𡄰欣、自由欣。\n    各渃成員㐌甘結、共𢭲組織聯合國、奮鬥促𢱜每𠊛尊重吧實現各權拱如仍自由基本𧵑𡥵𠊛。 \n\n    認識統一𧗱仍權吧自由𪦆𧵑𡥵𠊛羅要素關重一朱役實現𠫆踷甘結呢。"
-  specimen_16: "𢭲認識哴：\n役承認人品本𣎏、各權平等吧空體㳻𢴐𧵑每成員𥪝家庭人類羅基礎朱自由、公平吧和平𨕭世界、\n事侵犯吧䁛常人權㐌引𦤾仍行動殘暴侵犯𬧐良心𧵑人類、吧役𡏦𥩯𠬠世界𥪝𪦆𡥵𠊛得自由言論吧信仰、空群沛𠹾餒𢜝駭吧窮極得䁛羅願望高哿一𧵑類𠊛、\n人權沛得法律保衞抵每𠊛空𦄾沛浽亂如羅辦法𡳳窮抵挵吏制度強權吧壓逼、\n勤沛勸激役發展關係朋友𡧲各民族、\n人民各渃成員聯合國𥪝本憲章㐌𠬠吝姅肯定念信𧵑𨉟𠓨仍權基本𧵑𡥵𠊛、𠓨人品、𠓨價值𧵑每𠊛、𠓨權平等男女、吧㐌𠍣𤍊決心促𢱜進步社會拱如𡏦𥩯各條件𤯨𡄰欣、自由欣。\n    各渃成員㐌甘結、共𢭲組織聯合國、奮鬥促𢱜每𠊛尊重吧實現各權拱如仍自由基本𧵑𡥵𠊛。 \n\n    認識統一𧗱仍權吧自由𪦆𧵑𡥵𠊛羅要素關重一朱役實現𠫆踷甘結呢。\n𠉞、大會同聯合國宣布：\n版宣言全世界𧗱人權呢羅𡱩都終朱畢哿各渃吧畢哿各民族打價役實現目標𦓡每個人吧每組織𥪝社會、𨕭基礎㫻記𢖵版宣言呢、𠱊奮鬥促𢱜事尊重各權吧自由基本𧵑𡥵𠊛通過傳播吧教育、拱如𠱊奮鬥擔保朱 每𠊛民、於正各渃成員𧵑聯合國吧於各領土屬權管理𧵑𨉟、公認吧實現仍權吧自由𪦆𠬠格𣎏效果通過仍辦法積極、𥪝範圍國家咍國際。\n畢哿每𠊛生𠚢調得自由吧平等𧗱人品吧權。每𡥵𠊛調得造化頒朱理智吧良心吧勤沛對處𢭲膮𥪝情朋友。\n每𠊛調得享畢哿仍權吧自由標𥪝版宣言呢、空分別種族、𬜝䏧、界性、言語、宗教、觀點政治咍各觀點恪、源㭲國家咍社會、財產、成分出身咍地位社會。"
+  specimen_21: "𢭲認識哴：\n役承認人品本𣎏、各權平等吧空體㳻𢴐𧵑每成員𥪝家庭人類羅基礎朱自由、公平吧和平𨕭世界、\n事侵犯吧䁛常人權㐌引𦤾仍行動殘暴侵犯𬧐良心𧵑人類、吧役𡏦𥩯𠬠世界𥪝𪦆𡥵𠊛得自由言論吧信仰、空群沛𠹾餒𢜝駭吧窮極得䁛羅願望高哿一𧵑類𠊛、\n人權沛得法律保衞抵每𠊛空𦄾沛浽亂如羅辦法𡳳窮抵挵吏制度強權吧壓逼、\n勤沛勸激役發展關係朋友𡧲各民族、\n人民各渃成員聯合國𥪝本憲章㐌𠬠吝姅肯定念信𧵑𨉟𠓨仍權基本𧵑𡥵𠊛、𠓨人品、𠓨價值𧵑每𠊛、𠓨權平等男女、吧㐌𠍣𤍊決心促𢱜進步社會拱如𡏦𥩯各條件𤯨𡄰欣、自由欣。\n 各渃成員㐌甘結、共𢭲組織聯合國、奮鬥促𢱜每𠊛尊重吧實現各權拱如仍自由基本𧵑𡥵𠊛。 \n\n 認識統一𧗱仍權吧自由𪦆𧵑𡥵𠊛羅要素關重一朱役實現𠫆踷甘結呢。"
+  specimen_16: "𢭲認識哴：\n役承認人品本𣎏、各權平等吧空體㳻𢴐𧵑每成員𥪝家庭人類羅基礎朱自由、公平吧和平𨕭世界、\n事侵犯吧䁛常人權㐌引𦤾仍行動殘暴侵犯𬧐良心𧵑人類、吧役𡏦𥩯𠬠世界𥪝𪦆𡥵𠊛得自由言論吧信仰、空群沛𠹾餒𢜝駭吧窮極得䁛羅願望高哿一𧵑類𠊛、\n人權沛得法律保衞抵每𠊛空𦄾沛浽亂如羅辦法𡳳窮抵挵吏制度強權吧壓逼、\n勤沛勸激役發展關係朋友𡧲各民族、\n人民各渃成員聯合國𥪝本憲章㐌𠬠吝姅肯定念信𧵑𨉟𠓨仍權基本𧵑𡥵𠊛、𠓨人品、𠓨價值𧵑每𠊛、𠓨權平等男女、吧㐌𠍣𤍊決心促𢱜進步社會拱如𡏦𥩯各條件𤯨𡄰欣、自由欣。\n 各渃成員㐌甘結、共𢭲組織聯合國、奮鬥促𢱜每𠊛尊重吧實現各權拱如仍自由基本𧵑𡥵𠊛。 \n\n 認識統一𧗱仍權吧自由𪦆𧵑𡥵𠊛羅要素關重一朱役實現𠫆踷甘結呢。\n𠉞、大會同聯合國宣布：\n版宣言全世界𧗱人權呢羅𡱩都終朱畢哿各渃吧畢哿各民族打價役實現目標𦓡每個人吧每組織𥪝社會、𨕭基礎㫻記𢖵版宣言呢、𠱊奮鬥促𢱜事尊重各權吧自由基本𧵑𡥵𠊛通過傳播吧教育、拱如𠱊奮鬥擔保朱 每𠊛民、於正各渃成員𧵑聯合國吧於各領土屬權管理𧵑𨉟、公認吧實現仍權吧自由𪦆𠬠格𣎏效果通過仍辦法積極、𥪝範圍國家咍國際。\n畢哿每𠊛生𠚢調得自由吧平等𧗱人品吧權。每𡥵𠊛調得造化頒朱理智吧良心吧勤沛對處𢭲膮𥪝情朋友。\n每𠊛調得享畢哿仍權吧自由標𥪝版宣言呢、空分別種族、𬜝䏧、界性、言語、宗教、觀點政治咍各觀點恪、源㭲國家咍社會、財產、成分出身咍地位社會。"
 }
 historical: true
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/vi_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/vi_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 86038260
 region: "CN"
 region: "US"
 region: "VN"
 exemplar_chars {
   base: "a à ả ã á ạ ă ằ ẳ ẵ ắ ặ â ầ ẩ ẫ ấ ậ b c d đ e è ẻ ẽ é ẹ ê ề ể ễ ế ệ f g h i ì ỉ ĩ í ị j k l m n o ò ỏ õ ó ọ ô ồ ổ ỗ ố ộ ơ ờ ở ỡ ớ ợ p q r s t u ù ủ ũ ú ụ ư ừ ử ữ ứ ự v w x y ỳ ỷ ỹ ý ỵ z"
   marks: "◌̀ ◌́ ◌̂ ◌̃ ◌̆ ◌̉ ◌̛ ◌̣"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] § @ * / & # † ‡ ′ ″"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) [ ] @ * / & #"
   index: "A Ă Â B C D Đ E Ê F G H I J K L M N O Ô Ơ P Q R S T U Ư V W X Y Z"
 }
 sample_text {
   masthead_full: "TtÂâ"
   masthead_partial: "Cc"
   styles: "Việc thừa nhận nhân phẩm vốn có, các quyền"
   tester: "Sự xâm phạm và coi thường nhân quyền đã dẫn đến những hành động"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/vmw_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/vmw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/vo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/vo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/vro_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/vro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/wa_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/wa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/wae_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/wae_Latn.textproto`

 * *Files 22% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 population: 11376
 region: "CH"
 region: "LI"
 exemplar_chars {
   base: "a á ä ã b c č d e é f g h i í j k l m n o ó ö õ p q r s š t u ú ü ũ v w x y z"
   auxiliary: "à ă â å ā æ ç è ĕ ê ë ē ì ĭ î ï ī ñ ò ŏ ô ø ō œ ß ù ŭ û ū ÿ"
   marks: "◌́ ◌̃ ◌̈ ◌̌ ◌̀ ◌̂ ◌̄ ◌̆ ◌̊ ◌̧"
-  numerals: "- ‑ , ’ % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , ’ % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/war_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/war_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/wo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/wo_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 population: 11025493
 region: "MR"
 region: "SN"
 exemplar_chars {
   base: "a A à À b B c C d D e E é É ë Ë f F g G i I j J k K l L m M n N ñ Ñ ŋ Ŋ o O ó Ó p P q Q r R s S t T u U w W x X y Y"
   auxiliary: "ã Ã h H v V z Z"
   marks: "◌̀ ◌́ ◌̃ ◌̈"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ , ; : ! ? . ( ) [ ] { }"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- , ; : ! ? . ( ) [ ] { }"
   index: "A B C D E F G H I J K L M N Ŋ O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "DdOo"
   masthead_partial: "Mm"
   styles: "Ñu jàpp te nangu ne sagu doomi aadama ak"
   tester: "Ñu jàpp ne ñakk xam ak soofantal sañ-sañi doomi aadama indi na"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/wsg_Gong.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/wsg_Gong.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/wuu_Hans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/wuu_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/wwa_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/wwa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xcr_Cari.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xcr_Cari.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xh_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xlc_Lyci.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xlc_Lyci.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xld_Lydi.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xld_Lydi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xly_Elym.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xly_Elym.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xmn_Mani.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xmn_Mani.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xna_Narb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xna_Narb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xnr_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xnr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xpr_Prti.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xpr_Prti.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xsa_Sarb.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xsa_Sarb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xsm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xsm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/xsr_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/xsr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yad_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yad_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yao_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yao_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yap_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yap_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yav_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yav_Latn.textproto`

 * *Files 3% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 autonym: "Nuasue"
 population: 2302
 region: "CM"
 exemplar_chars {
   base: "a A á Á à À â Â ǎ Ǎ ā Ā b B c C d D e E é É è È ɛ Ɛ {ɛ́} {Ɛ́} {ɛ̀} {Ɛ̀} f F h H i I í Í ì Ì î Î ī Ī k K l L m M {mb} {MB} n N {ny} {NY} ŋ Ŋ {ŋg} {ŊG} o O ó Ó ò Ò ô Ô ǒ Ǒ ō Ō ɔ Ɔ {ɔ́} {Ɔ́} {ɔ̀} {Ɔ̀} p P s S t T u U ú Ú ù Ù û Û ǔ Ǔ ū Ū v V w W y Y"
   auxiliary: "g G j J q Q r R x X z Z"
   marks: "◌̀ ◌́ ◌̂ ◌̄ ◌̌"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "A B C D E Ɛ F H I K L M N Ŋ O Ɔ P S T U V W Y"
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ybh_Deva.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ybh_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yi_Hebr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yi_Hebr.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 region: "SE"
 region: "UA"
 region: "US"
 exemplar_chars {
   base: "א {אַ} {אָ} ב {בֿ} ג ד {דזש} ה ו {וּ} {וו} {וי} ז {זש} ח ט {טש} י {יִ} {יי} {ײַ} {כּ} כ ך ל מ ם נ ן ס ע {פּ} {פֿ} ף צ ץ ק ר ש {שׂ} {תּ} ת"
   auxiliary: "‎‏"
   marks: "◌ְ ◌ֱ ◌ֲ ◌ֳ ◌ִ ◌ֵ ◌ֶ ◌ַ ◌ָ ◌ֹ ◌ֻ ◌ּ ◌ׁ ◌ׂ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . ׳ \' \" ( ) [ ] / ״ ־"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- – — , ; : ! ? . ׳ \' \" ( ) [ ] / ״ ־"
   index: "ׂ ּ ֿ א ב ג ד ה ו ז ח ט י כ ל מ נ ס ע פ צ ק ר ש ת"
 }
 sample_text {
   masthead_full: "יעדר"
   masthead_partial: "מנ"
   styles: "היות װי דער סאַמער גרונט פֿון פֿרײַהײט יושר און"
   tester: "היות װי איגנאָרירן און ביטול צו די מענטשנרעכט האָבן גורם געװען"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ykg_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ykg_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yo_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yo_Latn.textproto`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 population: 28685568
 region: "BJ"
 region: "NG"
 exemplar_chars {
   base: "a A á Á à À b B d D e E é É è È ẹ Ẹ {ẹ́} {Ẹ́} {ẹ̀} {Ẹ̀} f F g G {gb} {GB} h H i I í Í ì Ì j J k K l L m M ḿ Ḿ {m̀} {M̀} n N ń Ń ǹ Ǹ o O ó Ó ò Ò ọ Ọ {ọ́} {Ọ́} {ọ̀} {Ọ̀} p P r R s S ṣ Ṣ t T u U ú Ú ù Ù w W y Y"
   auxiliary: "c C q Q v V x X z Z"
   marks: "◌̀ ◌́ ◌̄ ◌̣"
-  punctuation: "- ‐ ‑ – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) @ * / & # † ‡ ′ ″"
+  punctuation: "- – — , ; : ! ? . … \' ‘ ’ \" “ ” ( ) @ * / & #"
   index: "A B D E F G H I J K L M N O P R S T U W Y"
 }
 sample_text {
   masthead_full: "GgBb"
   masthead_partial: "Oo"
   styles: "Bí ó ti jẹ́ pé ṣíṣe àkíyèsí iyì tó jẹ́ àbímọ́"
   tester: "Bí ó ti jẹ́ pé àìka àwọn ẹ̀tọ́ ọmọnìyàn sí àti ìkẹ́gàn àwọn ẹ̀tọ́ wọ̀nyí"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yrk_Cyrl.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yrk_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yua_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yua_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yue_Hani.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yue_Hani.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yue_Hans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yue_Hans.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 autonym: "粤语（简体）"
 population: 72489040
 region: "CN"
 region: "HK"
 exemplar_chars {
   base: "一 丁 七 万-与 丑 专 且 世 丘-业 东 丝 丢 两 严 个 中 丰 串 临 丸-主 丽 举 乃 久 么 义 之 乌 乎-乐 乔 乖 乘 乙 九 也-乡 书 买 乱 了 予 争 事 二 于 亏 云 互 五 井 亚 些 亡 交-亨 享 京 亮 亲 人 亿-仁 仅 仇 今 介 仍 从 仑 仔 他 付 仙 代-以 仪 们 仰 仲 件 价 任 份 企 伊 伍 伐 休 众-会 伟 传 伤 伦 伯 估 伴 伸 似 伽 但 佉 位-住 体 何 余 佛 作 你 佩 佳 使 例 供 依 侠 侦-侨 侯 侵 便 促 俄 俊 俗 保 信 修 俾 倍 倒 候 倚 借 值 倾 假 偏 做 停 健 偶 偷 傣 傲 傻 像 僧 儒 儿 允 元-充 先 光 克 免 兔 党 入 全 八-兮 兰 共 关-兹 养-兽 内 冈 册 再 冒 写 军 农 冠 冬 冰 冲 决 况 冷 净 准 凉 凌 减 凝 几 凡 凤 凭 凯 凰 凶 出 击 函 刀 分 切 刊 划 列-创 初 删 判 利 别 到 制 刷 刺 刻 剌 前 剑 剧 剩 剪 副 割 力 劝-务 动-劫 励-劳 势 勇 勉 勒 勤 勿 包 匈 化 北 匹-医 十 千 升 午 半 华 协 卒 卓 单-南 博 卜 占-卢 卧 卫 卯-危 即 却 卷 厂 厄-历 厉 压 厌 厘 厚 原 去 县 参 又 及-反 发 叔 取-叙 口-另 只-叭 可 台 史 右 叶-叹 吃 各 合-吊 同-后 吐 向 吓 吕 吗 君 吝-吠 否 吧 含 听 启 吴 吵 吸 吹 吾 呀 呆 告 员 呜 呢 周 味 呵 呼 命 和 咖 咤 咦 咧 咪 咬 咱 哀 品 哇-哉 响 哎 哥 哦 哩 哪 哭 哲 唉 唐 唔 唬 售 唯 唱 唷 商 啊 啡 啥 啦 啪 啰 喀 喂 善 喇 喊 喔 喜 喝 喵 喷 嗨 嗯 嘉 嘛 嘴 嘻 嘿 器 四 回 因 团 园 困 围 固 国 图 圆 圈 圜 土 圣 在 圭 地 场 圾 址 均 坎-坐 块 坚-坜 坡 坤 坦 坪 垂 垃 型 垒 埃 城 埔 域 培 基 堂 堆 堕 堡 堪 塔 塞 填 境 墙 增 墨 壁 士 壬 壮 声 壳 处 备 复 夏 夕 外 多 夜 够 大 天-夫 央 失 头 夷-夺 奇-奉 奋 奎 奏 契 奔 奖 套 奥 女 奴 奶 她 好 如 妆-妈 妙 妥 妨 妮 妳 妹 妻 姆 始 姐 姑 姓 委 姿 威 娃 娄 娘 娱 婆 婚 媒 嫌 嫩 子 孔 字-孙 孝 孟 季 孤 学 孩 宁 它 宅 宇-安 宋 完 宏 宗-实 宠-室 宪 宫 害 家 容 宽-宿 寂 寄-密 富 寒 寝-察 寨 寮 对 寻 导 寿 封 射 将 尊 小 少 尔 尖 尘 尚 尝 尤 就 尺 尼-尾 局-层 居 届 屋 屏 展 属 屠 山 岁 岂 岚 岛 岩 岭 岸 峡 峰 崇 崴 川 州 巡 工-巨 巫 差 己-巴 巷 币-布 帅 师 希 帐 帕 帖 帛 帝 带 席 帮 常 帽 幅 幕 干-年 并 幸 幻-幽 广 庄 庆 庇 床 序 库-底 店 庚 府 废 度 座 庭 康 庸 廉 廖 延 廷 建 开 异-弄 式 引 弗 弘 弟 张 弥 弦 弯 弱 弹 强 彊 归 当 录 彝 形 彦 彩 彬 彭 彰 影 役 彻 彼 往 征 径 待 很 律 徐 徒 得 微 德 心 必 忆 忌 忍 志-忙 忠 忧 快 念 忽 怀 态 怎 怒 怕 怖 怜 思 怡 急 性 怨 怪 总 恋 恐 恒 恢 恨 恩 恭 息 恰 恶 恼 悉 悔 悟 悠 悦 您 悲 情 惊 惑 惜 惠 惧 惨 惯 想 惹 愁 愈 愉 意 愚 感 愿 慈 慕 慢 慧 慰 憾 懂 懒 戈 戊 戌 戏-戒 或 战 截 戴 户 房-扁 扇 手 才 扎 打 托 扣 扥 执 扩 扫-扭 扯 扰 批 找-技 抄 把 抓 投 抗 折 抛 抢 护 报 披 抬 抱 抵 抹 抽 担 拆 拉 拍 拏 拒 拔 拖 招 拜 拟 拥 拨 择 括 拳 拼 拾 拿 持 挂 指 按 挑 挖 挝 挡 挤 挥 挪 振 挺 捐 捕 损 捡 换 据 捷 授 掉 掌 排 探 接 控 推 措 掸 描 提 插 握 援 搜 搞 搬 搭 摄 摆 摇 摘 摩 摸 撑 撒 撞 播 操 擎 擦 支 收 改 攻 放 政 故 效 敌 敍 敏 救 教 敝 敢 散 敦 敬 数 整 文 斋 斐 斗 料 断 斯 新 方 施 旁 旅 旋 族 旗 无 既 日-旧 早 旭 时 旺 昂 昆 昌 明 昏 易 星 映 春 昨 昭 是 显 晋 晒 晓 晚 晨 普 景 晴 晶 智 暂 暑 暖 暗 暴 曰 曲 更 曼 曾-最 月 有 朋 服 朗 望 朝 期 木 未-札 术 朱 朵 机 杀 杂 权 杉 李 材 村 杜 束 条 来 杨 杯 杰 松 板 极 构 析 林 果 枝 枢 枪 枫 架 柏 某 染 柔 查 柬 柯 柳 柴 标 栏 树 校 样-根 格 桃 案 桌 桑 档 桥 梁 梅 梦 梨 梯 械 梵 检 棉 棋 棒 棚 森 椅 植 椰 楚 楼 概 榜 模 横 檀 次-欣 欧 欲 欺 款 歉 歌 止-武 死 殊 残 段 毁 毅 母 每 毒 比 毕 毛 毫 氏 民 气 水 永 求 汉 汗 汝 江-污 汤 汪 汶 汽 沃 沈 沉 沙 沟 没 沧 河 油 治 沿 泄 泉 泊 法 泡 波 泥 注 泪 泰 泳 泽 泾 洁 洋 洗 洛 洞 洪 洲 活 洽 派 流 浅 测 济 浏 浓 浦 浩 浪 浮 海 涂 消 涉 涛 涨 涯 液 涵 淑 淡 深 混 清 渐 渡 温 港 游 湖 湾 源 溪 滋 滑 滚 满 滥 滨 滴 漂 漏 演 漠 漫 潘 潜 潮 澳 激 灌 火 灭 灯 灰 灵 灾 炉 炎 炮 炸 点 烂 烈 烟 烤 烦 烧 热 焦 然 煞 照 熊 熟 燃 爆 爪 爬 爱 爵-爸 爽 片 版 牌 牙 牛 牠 牧 物 牲 牵 特 牺 犯 状 犹 狂 狐 狗 狠 独 狮 狱 狼 猛 猜 猪 猫 献 猴 玄 率 玉 王 玛 玩 玫 环 现 玲 玻 珊 珍 珠 珥 班 球 理 琉 琪 琴 瑙 瑜 瑞 瑟 瑰 瑶 瓜 瓦 瓶 甘 甚 甜 生 用 田-申 电 男 甸 画 界 留 略 番 疆 疏 疑 疗 疯 疼 病 痕 痛 痴 癸 登 白 百 的 皆 皇 皮 益 监 盖-盘 盛 盟 目 盲 直 相 盼 盾 省 眉 看 真 眠 眼 着 睛 睡 督 瞧 矛 矣 知 短 石 矶 码 砂 砍 研 破 础 硕 硬 确 碍 碎 碗 碟 碧 碰 磁 磨 示 礼 社 祖 祚 祛 祝 神 祥 票 祯 祸 禁 禄 禅 福 离 秀 私 秋 种 科 秒 秘 租 秤 秦 积 称 移 程 稍 税 稣 稳 稿 穆 究 穷 穹 空 穿 突 窗 窝 窭 立 站 竞-章 童 端 竹 笑 笔 笛 符 笨 第 等 筋 筑 答 策 筹 签 简 算 管 箫 箭 箱 篇 篮 簿 籍 米 类 粉 粗 粤 精 糊 糕 糟 系 素 索 紧 紫 累 繁 纠 红 约 级 纪 纬 纯 纲 纳 纵 纷 纸 纽 线 练 组 细-终 绍 经 结 绕 绘 给 络 绝 统 继 绩 绪 续 维 综 绿 缅 缓 编 缘 缚 缩 缪 缴 缸 缺 网 罕 罗 罚 罢 罪 置 署 羊 美 羞 群 羽 翁 翔 翘 翰 翻 翼 耀 老 考 者 而 耍 耐 耗 耳 耶 耻 聊 职 联 聚 聪 肉 肚 股 肥 肩 肯 育 胆 背 胎 胖 胜 胞 胡 胸 能 脆 脑 脚 脱 脸 腊 腓 腔 腰 腿 臣 自 臭 至 致 舌 舍 舒 舞 舟 航 般 舰 船 良 色 艺 艾 节 芝 芦 芬 花 芳 苍 苏 若 苦 英 范 茅 茫 茶 草 荐 荒 荣 药 荷 荼 莉 莎 莫 莱 莲 获 菜 菩 菲 萄 萤 营 萧 萨 落 葛 葡 蒂 蒋 蒙 蒲 蓝 蔕 蔡 薄 薪 藏 藤 虎 虑 虚 虫 虽 蛇 蛋 蛙 蛮 蜂 蜜 蝎 蝶 融 蟹 血 行 街 衡 衣 补 表 袋 被 裁 裂 装 裕 裤 西 要 覆 见 观 规 视 览 觉 角 解 触 言 誉 誓 警 计 订 认 讨 让 训-记 讲 讷 许 论 设 访 证 评 识 诉 词 译 试 诗 诚 话 诞 询 该 详 语 误 说 请 诸 诺 读 课 谁 调 谅 谈 谊 谋 谓 谚 谢 谱 谷 豆 象 豪 貌 贝-负 贡-败 货 质 贪 购 贯 贱 贴 贵 费 贺 贾 资 赋 赌 赏 赐 赖 赚 赛 赞 赠 赢 赤 赫 走 赵-起 超 越 趋 趣 足 跃 跌 跎 跑 距 跟 路 跳 踏 踢 踪 身 躲 车 轨 轩 转 轮-轰 轻 载 较 辅 辆 辈 辉 辑 输 辛 辞 辨 辩 辰 辱 边 达 迁 迅 过 迈 迎 运 近 返 还 这 进-迟 迦 迪 迫 述 迷 迹 追 退-逃 逆 选 逊 透 逐 途 通 逛 逝 速 造 逢 逸 逻 逼 遇 遍 道 遗 遥 遭 遮 避 邀 那 邦 邪 邮 邱 邻 郁 郎 郑 部 郭 都 鄂 酉 配 酒 酷 酸 醉 醒 采 释 里-量 金 鉴 针 钓 钟 钢 钦 钱 钵 铁 铃 铜 铢 铭 银 销 锁 锅 锋 锐 错 锡 锦 键 镇 镑 镜 长 门 闪 闭 问 闰 闲 间 闷 闹 闻 阁 阅 阇 阐 阔 阗 队 防-阶 阻 阿 陀 附-陆 陈 降 限 院 除 险 陪 陵-陷 隆 随 隐 隔 障 难 雄-集 雉 雨 雪 雳 零 雷 雾 需 震 霍 露 霸 霹 青 靖 静 非 靠 面 革 靼 鞋 鞑 韦 韩 音 韵 頞 页 顶 项-须 顽-顿 预 领 颇 频 颗 题 颜 额 风 飘 飞 食 餐 饭 饮 饰 饱 饼 馆 首 香 马 驱 驶 驻 驾 骂 验 骑 骗 骚 骨 高 鬼 魁 魂 魅 魔 鱼 鲁 鲜 鸟 鸡 鸣 鸿 鹅 鹰 鹿 麦 麻 黄 黎 黑 默 鼓 鼠 鼻 齐 齿 龄 龙 龟"
   auxiliary: "乍 仂 伏 佐 侣 僳 兆 兑 券 勋 卑 卞 咀 嘅 堤 墎 壤 孜 屿 峇 巽 斜 昙 昼 栗 楔 浑 涅 湘 澎 灿 狄 琳 瑚 甫 碑 礁 绰 芒 苗 茨 茵 蓬 蚩 蛰 蜀 裘 谬 赣 酋 闽 陇 霜"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9 〇 一 七 三 九 二 五 八 六 四"
-  punctuation: "﹉﹊﹋﹌ _ ＿ ﹍﹎﹏ ︳︴ - － ﹣ ‐ ‑ – — ︱ ― , ， ﹐ 、 ﹑ ; ； ﹔ : ： ﹕ ! ！ ﹗ ? ？ ﹖ . ． ﹒ ‥ ︰ … 。 · ＇ ‘ ’ \" ＂ “ ” 〝 〞 ( （ ﹙ ︵ ) ） ﹚ ︶ [ ［ ] ］ { ｛ ﹛ ︷ } ｝ ﹜ ︸ 〈 ︿ 〉 ﹀ 《 ︽ 》 ︾ 「 ﹁ 」 ﹂ 『 ﹃ 』 ﹄ 【 ︻ 】 ︼ 〔 ﹝ ︹ 〕 ﹞ ︺ 〖 〗 ‖ § @ ＠ ﹫ * ＊ ﹡ / ／ \\ ＼ ﹨ & ＆ ﹠ # ＃ ﹟ % ％ ﹪ ‰ ′ ″ ‵ 〃 ※"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9 〇 一 七 三 九 二 五 八 六 四"
+  punctuation: "﹉﹊﹋﹌ _ ＿ ﹍﹎﹏ ︳︴ - － ﹣ – — ︱ ― , ， ﹐ 、 ﹑ ; ； ﹔ : ： ﹕ ! ！ ﹗ ? ？ ﹖ . ． ﹒ ‥ ︰ … 。 · ＇ ‘ ’ \" ＂ “ ” 〝 〞 ( （ ﹙ ︵ ) ） ﹚ ︶ [ ［ ] ］ { ｛ ﹛ ︷ } ｝ ﹜ ︸ 〈 ︿ 〉 ﹀ 《 ︽ 》 ︾ 「 ﹁ 」 ﹂ 『 ﹃ 』 ﹄ 【 ︻ 】 ︼ 〔 ﹝ ︹ 〕 ﹞ ︺ 〖 〗 ‖ @ ＠ ﹫ * ＊ ﹡ / ／ \\ ＼ ﹨ & ＆ ﹠ # ＃ ﹟ % ％ ﹪ ‵ 〃 ※"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "人生出嚟"
   masthead_partial: "就系"
   styles: "人人生出嚟就系自由慨，喺尊严同权利上一律平等。渠哋具有理性同良心，而且应该用兄弟间慨关系嚟互相对待"
   tester: "人人生出嚟就系自由慨，喺尊严同权利上一律平等。渠哋具有理性同良心，而且应该用兄弟间慨关系嚟互相对待"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/yue_Hant.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/yue_Hant.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 autonym: "粵語 (繁體)"
 population: 6524919
 region: "CN"
 region: "HK"
 exemplar_chars {
   base: "一 丁 七 丈-不 丑 且 世 丘 丙 丟 並 中 串 丸 丹 主 乃 久 么 之 乎 乏 乖 乘 乙 九 也 乾 亂 了 予 事 二 于 云 互 五 井 些 亞 亡 交-亦 亨 享 京 亮 人 什 仁 仇 今 介 仍 仔 他 付 仙 代-以 仰 仲 件 任 份 企 伊 伍 伐 休 伙 伯 估 伴 伸 似 伽 但 佈 佉 位-住 佔 何 余 佛 作 你 佩 佳 使 來 例 供 依 侯 侵 便 係-俄 俊 俏 俗 保 俠 信 修 俱 俾 倉 個 倍 們 倒 候 倚 借 倫 值 假 偉 偏 做 停 健 側-偷 偽 傅 傑 傘 備 傢 傣 傲 傳 傷 傻 傾 僅 像 僑 僧 價 儀 億 儒 儘 優 允 元-充 兇-光 克 免 兒 兔 入 內-兩 八-兮 共 兵-典 兼 冊 再 冒 冠 冬 冰 冷 准 凋-凍 凝 凡 凰 凱 出 函 刀 分 切 刊 列 初 判 別 刨-刪 刮 到 制 刷 刺 刻 剃 則 剌 前 剛 剩 剪 副 割 創 劃 劇 劉 劍 力 功 加 助-劫 勁 勇 勉 勒 動 務 勝 勞 勢 勤 勵 勸 勾 勿 包 匈 化 北 匯 匹 區 十 千 升 午 半 卒-協 南 博 卜 卡 卯-危 即 卷 卹 卻 厄 厘 厚 原 厭 厲 去 參 又 及 友 反 叔 取 受 口-另 只-叭 可 台 史 右 司 吃 各 合-吊 同-后 吐-吒 君 吝-吠 否 吧 含 吳 吵 吸 吹 吾 呀 呂 呆 告 呢 周 味 呵 呼 命 和 咖 咦 咧 咪 咬 咱 哀 品 哇-哉 哎 員 哥 哦 哩 哪 哭 哲 唇 唉 唐 唔 唬 售 唯 唱 唵 唷 唸 商 啊 問 啟 啡 啤-啦 啪 喀 喂 善 喇 喊 喔 喜 喝 喪 喬 單 喲 喵 嗎 嗚 嗨 嗯 嘆 嘉 嘗 嘛 嘴 嘻 嘿 噁 噓 器 噴 嚇 嚏 嚴 囉 四 回 因 困 固 圈 國 圍 園 圓 圖 團 圜 土 在 圭 地 圾 址 均 坎 坐 坑 坡 坤 坦 坪 垂 垃 型 埃 城 埔 域 執 培 基 堂 堅 堆 堡 堪 報 場 塊 塔 塗 塞 填 塵 境 墅 墓 增 墟 墨 墮 墳 壁 壇 壓 壘 壞 壢 壩 士 壬 壯 壺 壽 夏 夕 外 多 夜 夠 夢 夥 大 天-夫 央 失 夷 夸 夾 奇-奉 奎 奏 契 奔 套 奧 奪 奮 女 奴 奶 她 好 如 妙 妝 妥 妨 妮 妳 妹 妻 姆 姊 始 姐 姑 姓 委 姿 威 娃 娘 娛 婁 婆 婚 婦 媒 媽 嫌 嫩 子 孔 孕 字 存 孝 孟 季 孤 孩 孫 孵 學 它 宅 宇-安 宋 完 宏 宗-宜 客-室 宮 害 家 容 宿 寂 寄-密 富 寒 寞 察 寢 實-審 寫 寬 寮 寵 寶 寺 封 射 將 專 尊 尋 對-小 少 尖 尚 尤 就 尺 尼 尾-屁 居 屆 屋 屍 屏 屑 展 屠 層 屬 山 岡 岩 岸 峰 島 峽 崇 崙 崴 嵐 嶺 川 州 巡 工-巨 巫 差 己-巴 巷 市 布 希 帕 帖 帚 帛 帝 帥 師 席 帳 帶 常 帽 幅 幕 幟 幣 幫 干-年 幸 幹 幻-幾 庇 床 序 底 店 庚 府 度 座 庫 庭 康 庸 廈 廉 廖 廟 廠 廢 廣 廳 延 廷 建 弄 式 引 弗 弘 弟 弦 弱 張 強 彈 彊 彌 彎 彝 彞 形 彥 彩 彬 彭 彰 影 役 彼 往 征 待 很 律 後 徐-徒 得 從 復 微 徵 德 徹 心 必 忌 忍 志-忙 忠 忡 快 念 忽 怎 怒 怕 怖 思 怡 急 性 怨 怪 恆 恐 恢 恥 恨 恩 恭 息 恰 悅 悉 悔 悟 悠 您 悲 悶 情 惑 惜 惠 惡 惱 想 惹 愁 愈 愉 意 愚 愛 感 慈 態 慕 慘 慢 慣 慧 慮 慰 慶 慾 憂 憊 憐 憑 憲 憶 憾 懂 應 懨 懶 懷 懼 戀 戈 戊 戌 成-戒 或 截 戰 戲 戴 戶 房-扁 扇 手 才 扎 打 托 扣 扥 扭-扯 批 找-技 抄 把 抓 投 抗 折 披 抬 抱 抵 抹 抽 拆 拉 拋 拍 拏 拒 拔 拖 招 拜 括 拳 拼 拾 拿 持 指 按 挑 挖 挪 振 挺 捏 捐 捕 捧 捨 捲 捷 掃 授 掉 掌 排 掛 掠-探 接 控 推 措 掰 描 提 插 揚 換 握 揮 援 揹 損 搏 搖 搜 搞 搬 搭 搶 摀 摘 摩 摸 撐 撒 撕 撞 撣 撥 播 撲 撾 撿 擁 擇 擊 擋 操 擎 擔 據 擠 擦 擬 擴 擺 擾 攀 攝 攤 支 收 改 攻 放 政 故 效 敍 敏 救 敗-教 敝 敞 敢 散 敦 敬 整 敵 數 文 斐 斑 斗 料 斜 斧 斯 新 斷 方 於 施 旁 旅 旋 族 旗 既 日 旦 早 旭 旺 昂 昆 昇 昌 明 昏 易 星 映 春 昨 昭 是 時 晉 晒 晚 晨 普 景 晴 晶 智 暑 暖 暗 暫 暮 暴 曆 曇 曉 曬 曰 曲-更 書 曼 曾-最 會 月 有 朋 服 朔 朗 望 朝 期 木 未-札 朱 朵 杉 李 材 村 杖 杜 束 杯-東 松 板 析 林 果 枝 枯 架 柏 某 染 柔 查 柬 柯 柳 柴 栓 校 核 根 格 栽 桃 案 桌 桑 梁 梅 條 梨 梯 械 梵 棄 棉 棋 棍 棒 棕 棚 森 棺 椅 植 椒 椰 楊 楓 楚 業 極 概 榜 榮 構-槍 樂 樓 標 樞 模 樣 樹 橄 橇 橋 橘 橙 機 橫 檀 檔 檢 檬 檸 櫚 櫻 欄 權 欖 欠 次 欣 欲 欺 欽 款 歉 歌 歐 歡-武 歲 歷 歸 死 殊 残 殘 殭 段 殺 殼 毀 毅 母 每 毒 比 毛 毫 氏 民 氣 水 永 汁 求 汗 汝 江-污 汪 汶 決 汽 沃 沈 沉 沒 沖 沙 沫 沮 河 油 治 沿 況 泉 泊 法 泡-泣 泥 注 泰 泳 洋 洗 洛 洞 洩 洪 洲 活 洽 派 流 浣 浦 浩 浪 浮 浴 海 涇-涉 涎 涮 涯 液 涵 涼 淇 淋 淑 淚 淡 淨 深 混 淺 清 減 渡 測 港 游 湖 湘 湯 源 準 溜 溝 溪 溫 滄 滅 滋 滑 滴 滾 滿 漂 漏 演 漠 漢 漫 漲 漸 漿 潔 潘 潛 潮 澡 澤 澳 激 濃 濕 濟 濤 濫 濱 瀏 灌 灣 火 灰 災 炎 炮 炸 為 烈 烏 烘 烤 烹 焊 焙 無 焦 焰 然 煙 煞 照 煩 煮 熊 熟 熱 燃 燈 燒 燙 營 爆 爍 爐 爛 爪 爬 爭 爵 父 爸 爺 爽 爾 牆-版 牌 牙 牛 牠 牧 物 牲 特 牽 犀 犧 犬 犯 狀 狂 狐 狗 狠 狡 狸 狼 猛 猜 猩 猴 猶 猾 猿 獄 獅 獎 獨 獲 獸 獺 獻 獾 玄 率 玉 王 玩 玫 玲 玻 珊 珍 珠 珥 班 現 球 理 琉 琪 琴 瑙 瑜 瑞 瑟 瑤 瑪 瑰 環 瓜 瓢 瓦 瓶 甕 甘 甚 甜 生 產 用 田-申 男 甸 界 留 畢 略 番 畫 異 當 疆 疏 疑 疲 疼 疾 病 痕 痛 痴 瘋 瘦 瘧 療 癡 癸 登-百 皂 的 皆 皇 皮 皿 盃 盆 盈 益 盔 盛 盜 盟 盡 監-盥 盧 目 盲 直 相 盼 盾 省 眉 看 真 眠 眼 眾 睏 睛 睡 督 瞇 瞌 瞧 瞪 瞭 矛 矣 知 短 石 砂 砍 研 砲 破 硬 碎 碗 碟 碧 碩 碰 確 碼 磁 磚 磨 磯 礎 礙 礫 示 社 祈 祕 祖 祚 祛 祝 神 祥 票 祿 禁 禍-福 禪 禮 禱 禿-私 秋 科 秒 秘 租 秤 秦 移 稅 程 稍 種 稱 稻 稿 穀 穆 穌 積 穩 究 穹 空 穿 突 窄 窗 窩 窮 窶 立 站 竟 章 童 端 競 竹 竿 笑 笛 符 笨 第 筆 等 筋 答 策 筷 简 箏 箔 算 管 箭 箱 節 範 篇 築 篷 簡 簫 簽 簿 籃 籌 籍 籠 籤 米 粉 粗 粵 精 糊 糕 糖 糟 糥 系 糾 紀 約 紅 紉 納 紐 純 紙-紛 素 索 紫 紮-細 紳 紹 終 組 結 絕 絡 給 統 絲 經 綜 綠 維 綱 網 綽 綿 緊 緒 線 緣 編 緩 緬 緯 練 縛 縣 縫 縮 縱 總 績 繁 繃 繆 織 繞 繡 繩 繪 繳 繼 續 纖 缸 缺 罈 罐 罕 罩 罪 置 罰 署 罵 罷 羅 羊 美 羞 群 義 羽 翁 習 翔 翰 翹 翻 翼 耀 老 考 者 而 耍 耐 耗 耳 耶 聊 聖 聚 聞 聯 聰 聲 職 聽 聾 肉 肌 肚 股 肥 肩 肯 育 肺 背 胎 胖 胞 胡 胸 能 脆 脈 脖 脫 腐 腓 腔 腦 腰 腳 腹 腿 膚 膠 膽 臂 臉 臘 臟 臣 臥 臨 自 臭 至 致 臺 與-舊 舌 舍 舒 舞 舟 航 般 船 艦 良 色 艾 芙 芝 芬 芭 花 芳 芽 苣 若 苦 英 茄 茅 茫 茲 茵 茶 茸 草 荒 荷 荼 莉 莊 莎 莓 莖 莫 菇 菌 菜 菩 華 菲 萄 萊 萎 萬 萵 落 葉 著 葛 葡 葵 蒂 蒙 蒜 蒲 蒸 蒼 蓄 蓉 蓋 蓮 蔔 蔕 蔡 蔣 蔥 蔬 蕉 蕭 蕾 薄 薑 薦 薩 薪 薯 藉 藍 藏 藝 藤 藥 蘆 蘇 蘋 蘑 蘭 蘿 虎 處 虛 號 虧 蚊 蚓 蚯 蛇 蛋 蛙 蜂 蜜 蜥 蜴 蝙 蝟 蝠 蝦 蝶 螂 螃 融 螞 螢 螺 蟀 蟄 蟋 蟑 蟲 蟳 蟹 蟻 蠅 蠍 蠕 蠣 蠻 血 行 術 街 衛 衝 衡 衣 表 衫 袋 袍 被 裁 裂 裏 裕 補 裝 裡 裱 裹 製 複 褐 褲 襪 襯 西 要 覆 見 規 視 親 覺 覽 觀 角 解 觸 言 訂 計 訊 討 訓 託 記 訝 訥 訪 設 許 訴 診-証 評 詞 詢 試 詩 話-詳 誇 誌 認 誓 誕 語 誠 誤 說 誰 課 誼 調 談 請 諒 論 諸 諺 諾 謀 謂 謎 講 謝 證 識 譜 警 譯 議 護 譽 讀 變 讓 讚 谷 豆 豈 豎 豐 豔 象 豪 豬 豹 貌 貓 貝 貞 負-貢 貨 貪-責 貴 買 費 貼 賀 資 賈 賓 賜 賞 賢-賤 賦 質 賭 賴 賺 購 賽 贈 贊 贏 贛 赤 赫 走 起 超 越 趕 趙 趣 趨 足 跆 跌 跎 跑 距 跟 跡 跪 路 跳 踏 踢 踩 蹟 蹤 躍 身 躲 車 軌 軍 軒 軟 軸 較 載 輔 輕 輛 輝 輩 輪 輯 輸 轉 轎 轟 辛 辜 辣 辦 辨 辭 辯-農 迅 迎 近 返 迦 迪 迫 述 迴 迷 追 退 送 逃 逆 透 逐 途 這-逛 逝 速 造 逢 連 週 進 逸 逼 遇 遊 運 遍 過 道-違 遙 遜 遠 適 遭 遮 遲 遷 選 遺 避-邁 還 邊 邏 那 邦 邪 邱 郎 部 郭 郵 都 鄂 鄉 鄙 鄭 鄰 酉 配 酒 酪 酷 酸 醉 醒 醜 醫 醬 采 釋-量 金 針 釣 鈴 鉅 鉢 鉤 銀 銅 銖 銘 銳 銷 鋁 鋒 鋼 錄 錢 錦 錨 錫 錯 錶 鍊 鍋 鍵 鍾 鎊 鎖 鎮 鏈 鏡 鏢 鐘 鐡 鐵 鑑 鑿 長 門 閃 閉 開 閏 閒 間 閣 閩 閱 闆 闊 闍 闐 關 闡 阱 防 阻 阿 陀 附 降 限 院-除 陪 陰 陳 陵-陸 陽 隆 隊 階 隔 際 障 隨 險 隱 隻 雄-集 雉 雌 雖 雙 雜 雞 離 難 雨 雪 雲 零 雷 電 需 震 霍 霜 霧 露 霸 霹 靂 靈 青 靖 静 靜 非 靠 面 革 靴 靼 鞋 鞭 韃 韋 韓 音 韻 響 頁 頂 項 順 須 頌 預 頑 頓 頗 領 頞 頭 頸 頻 顆 題 額 顏 願 顛 類 顧 顯 風 颱 飄 飆 飛 食 飪 飯 飲 飽 飾 餃 餅 養 餌 餐 餘 餚 館 餾 首 香 馬 駐 駕 駛 駝 駱 騎 騙 騷 驅 驕 驗 驚 骨 體 高 髮 鬆 鬍 鬥 鬧 鬱 鬼 魁 魂 魅 魔 魚 魯 魷 鮑 鮮 鯊 鯨 鱷 鳥 鳩 鳳 鳴 鴨 鴻 鵝 鵡 鶴 鷹 鸚 鹽 鹿 麗 麥 麵 麻 麼 黃 黎 黑 默 黛 點 黨 鼓 鼠 鼬 鼻 齊 齋 齒 齡 龍 龐 龜"
   auxiliary: "乍 仂 伏 佐 侶 僳 兆 兌 兹 凸 别 券 勳 卑 卞 占 叶 嘅 堤 墎 壤 奥 孜 峇 嶼 巽 栗 楔 涅 渾 澎 灘 燦 狄 琳 瑚 甫 碑 礁 纜 艇 芒 苗 茨 蓬 蚩 蜀 裘 謬 酋 隴 雀 髪"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9 〇 一 七 三 九 二 五 八 六 四"
-  punctuation: "‾ ﹉﹊﹋﹌ _ ＿ ﹍﹎﹏ ︳︴ - － ﹣ ‐ ‑ – ︲ — ﹘ ︱ , ， ﹐ 、 ﹑ ; ； ﹔ : ： ﹕ ! ！ ﹗ ? ？ ﹖ . ． ﹒ ‥ ︰ … 。 · ＇ ‘ ’ \" ＂ “ ” 〝 〞 ( （ ﹙ ︵ ) ） ﹚ ︶ [ ［ ] ］ { ｛ ﹛ ︷ } ｝ ﹜ ︸ 〈 ︿ 〉 ﹀ 《 ︽ 》 ︾ 「 ﹁ 」 ﹂ 『 ﹃ 』 ﹄ 【 ︻ 】 ︼ 〔 ﹝ ︹ 〕 ﹞ ︺ § @ ＠ ﹫ * ＊ ﹡ / ／ \\ ＼ ﹨ & ＆ ﹠ # ＃ ﹟ % ％ ﹪ ‰ † ‡ ‧ ′ ″ ‵ 〃 ※"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9 〇 一 七 三 九 二 五 八 六 四"
+  punctuation: "‾ ﹉﹊﹋﹌ _ ＿ ﹍﹎﹏ ︳︴ - － ﹣ – ︲ — ﹘ ︱ , ， ﹐ 、 ﹑ ; ； ﹔ : ： ﹕ ! ！ ﹗ ? ？ ﹖ . ． ﹒ ‥ ︰ … 。 · ＇ ‘ ’ \" ＂ “ ” 〝 〞 ( （ ﹙ ︵ ) ） ﹚ ︶ [ ［ ] ］ { ｛ ﹛ ︷ } ｝ ﹜ ︸ 〈 ︿ 〉 ﹀ 《 ︽ 》 ︾ 「 ﹁ 」 ﹂ 『 ﹃ 』 ﹄ 【 ︻ 】 ︼ 〔 ﹝ ︹ 〕 ﹞ ︺ @ ＠ ﹫ * ＊ ﹡ / ／ \\ ＼ ﹨ & ＆ ﹠ # ＃ ﹟ % ％ ﹪ ‧‵ 〃 ※"
   index: "一 丁 丈 不 且 丞 並 串 乘 乾 亂 亭 傀 僎 僵 儐 償 儳 儷 儻 叢 嚴 囌 囑 廳"
 }
 sample_text {
   masthead_full: "人生而平"
   masthead_partial: "等喺"
   styles: "鉴于对人类家庭所有嘅成员固有尊严同埋佢哋嘅平等嘅兼不移嘅权利嘅承认，係世界自由、正义同埋和平嘅基础"
   tester: "鉴于对人权嘅无视同埋侮蔑经已发展成为野蛮暴行，呢些暴行玷污咗人类嘅良心，而一个人人都有言论同埋信仰自由而且冇惊冇穷嘅世界嘅嚟临"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/za_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/za_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zam_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zam_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zdj_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zdj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zgh_Tfng.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zgh_Tfng.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 script: "Tfng"
 name: "Standard Moroccan Tamazight"
 autonym: "ⵜⴰⵎⴰⵣⵉⵖⵜ"
 population: 7823574
 region: "MA"
 exemplar_chars {
   base: "ⴰ ⴱ ⴳ {ⴳⵯ} ⴷ ⴹ ⴻ ⴼ ⴽ {ⴽⵯ} ⵀ ⵃ ⵄ ⵅ ⵇ ⵉ ⵊ ⵍ ⵎ ⵏ ⵓ ⵔ ⵕ ⵖ ⵙ ⵚ ⵛ ⵜ ⵟ ⵡ ⵢ ⵣ ⵥ"
-  numerals: "  - ‑ , % ‰ + 0 1 2 3 4 5 6 7 8 9"
+  numerals: "- , % + 0 1 2 3 4 5 6 7 8 9"
   index: "ⴰ ⴱ ⴳ ⴷ ⴹ ⴻ ⴼ ⴽ ⵀ ⵃ ⵄ ⵅ ⵇ ⵉ ⵊ ⵍ ⵎ ⵏ ⵓ ⵔ ⵕ ⵖ ⵙ ⵚ ⵛ ⵜ ⵟ ⵡ ⵢ ⵣ ⵥ"
 }
 sample_text {
   masthead_full: "ⴰⵔⴷⵜ"
   masthead_partial: "ⵍⵏ"
   styles: "ⵍⵍⵉⵖ ⵜⴳⴰ ⵜⵓⴽⵣⴰ ⵏ ⵓⵍⵍⴰⵍⵓ ⵏ ⴽⴰⵢⴳⴰⵜ ⵢⴰⵏ ⵖ ⵜⴰⵡⵊⴰ"
   tester: "ⵜⴳ ⵜⴰⵎⵜⵜⴰⵡⵜ ⵏ ⵉⵣⵔⴼⴰⵏ ⵏ ⵓⴼⴳⴰⵏ ⴰⴷ ⵉⵜⵜⴰⵡⵉⵏ ⵜⵓⴳⵜⵜ ⵏ ⵎⴰⴷ ⵉⵀⵔⵛⵏ ⴰⵔ"
   poster_sm: "ⴷ ⵍⵍⵉⵖ ⵉⴳⴰ"
   poster_md: "ⴷ ⵍⵍⵉⵖ ⵉⵍⵍⴰ"
   poster_lg: "ⵜⵜⵍⴰⵍⴰⵏ"
   specimen_48: "ⴷ ⵍⵍⵉⵖ ⵎⵙⵓⵛⴽⴰⵏ ⵉⵡⴰⵏⴽⵏ ⵉⴳⵎⴰⵎⵏ, ⵙ ⵜⵡⵙⵉⵏ ⵏ ⵜⵎⴰⴷⴷⴰⵙⵜ ⵏ ⵜⵎⵜⵜⴰ ⵉⵎⵓⵏⵏ,"
   specimen_36: "ⴽⵓ ⵢⴰⵏ ⵉⵍⵍⴰ ⴷⴰⵔⵙ ⵓⵣⵔⴼ ⴰⴷ ⵉⴼⵜⵓ ⵙ ⵜⵉⵏⴼⴳⴰⵔⵉⵏ ⵜⵉⵏⴰⵎⵓⵔⵉⵏ ⵉⵖ ⵉⵍⵍⴰ ⴽⵔⴰ ⵓⵣⴳⴳⴰⵍ ⵖ ⵉⵣⵔⴼⴰⵏ ⵏⵏⵙ ⵍⵍⵉ ⵢⴰⵙ ⵉⴼⴽⴰ ⵓⵍⵓⴳⵏ."
   specimen_32: "ⵓⵔ ⵉⵅⵚⵚⴰ ⴰⴷ ⵢⵉⵍⵉ ⴽⵔⴰ ⵓⴽⵛⵛⵎ ⵉⵅⵛⵛⵏ ⵖ ⵜⵓⴷⵔⵜ ⵉⵥⵍⵉⵏ ⵙ ⴽⵔⴰ ⵏ ⵢⴰⵏ ⵏⵖⴷ ⵜⵉⵏ ⵜⵡⵊⴰ ⵏⵏⵙ ⵏⵖⴷ ⴰⵣⴷⴷⵓⵖ ⵏⵏⵙ ⵏⵖⴷ ⵉⵎⵢⴰⵡⴰⴹⵏ ⵏⵏⵙ ⵖⴷ ⴰⴷⴷⵓⵔ ⵏⵏⵙ. ⵢⵉⵍⵉ ⴷⴰⵔ ⴽⵓ ⵢⴰⵏ ⵓⵣⵔⴼ ⵏ ⵓⵃⵟⵟⵓ ⵏ ⵓⵍⵓⴳⵏ ⵖ ⵣⵓⵏⴷ ⴰⴽⵛⵛⵓⵎ ⴰⴷ."
-  specimen_21: "ⴽⵓ ⵢⴰⵏ ⵉⵍⵍⴰ ⴷⴰⵔⵙ ⵓⵣⵔⴼ ⵏ ⴳ ⵜⴷⵔⴼⵉⵜ ⵏ ⵓⵙⵡⵉⵏⴳⵎ ⴷ ⵜⵉⵏ ⵜⴰⵏⵏⴰⵢⵜ, ⴷ ⵜⵉⵏ ⵓⵙⴳⴷ ⵖⵉⵍⵍⴰ ⵉⵍⵍⴰ ⵓⵣⵔⴼ ⴰⴷ ⵉⵙⵏⴼ ⴰⵙⴳⵖⵏⵏⵙ, ⵢⵉⵍⵍⵉ ⴷⴰⵔⵙ ⴰⵡⴷ ⵓⵣⵔⴼ ⵏ ⵜⵡⵏⵏⵉⵜ ⵜⴰⵏⴼⵔⵓⵜ ⵙ ⴽⵔⴰ ⵉⴳⴰⵜ ⴰⵏⴰ ⵏⵏⵙ.\nⴽⵓ ⵢⴰⵏ ⵉⵍⵍⴰ ⴷⴰⵔⵙ ⵓⵣⵔⴼ ⵏ ⵜⴷⵔⴼⵉⵜ ⵏ ⵜⴰⵏⵏⴰⵢⵜ ⴷ ⵜⵡⵏⵏⵉⵜ, ⴰⴷ ⵉⵜⵜⵉⴽⵚⵓⴹ ⵅⴼ ⵜⴰⵏⵏⴰⵢⵉⵏ ⵏⵏⵙ ⵓⵍⴰ ⴰⵔⵣⵣⵓ ⵏⵏⵙ ⴰⴷ ⵢⴰⵎⵥ ⵏⵖ ⴰⴷ ⵉⵣⵓⵣⵣⵔ, ⴰⴱⵍⴰ ⵉⵡⵜⵜⴰ, ⵉⵏⵖⵎⵉⵙⵏ ⴷ ⵜⵡⵏⴳⵉⵎⵉⵏ ⵙ ⴰⴽⵯ ⵉⵎⴰⵙⵙⵏ  ⵓⵙⵓⵙⵙⵏ."
+  specimen_21: "ⴽⵓ ⵢⴰⵏ ⵉⵍⵍⴰ ⴷⴰⵔⵙ ⵓⵣⵔⴼ ⵏ ⴳ ⵜⴷⵔⴼⵉⵜ ⵏ ⵓⵙⵡⵉⵏⴳⵎ ⴷ ⵜⵉⵏ ⵜⴰⵏⵏⴰⵢⵜ, ⴷ ⵜⵉⵏ ⵓⵙⴳⴷ ⵖⵉⵍⵍⴰ ⵉⵍⵍⴰ ⵓⵣⵔⴼ ⴰⴷ ⵉⵙⵏⴼ ⴰⵙⴳⵖⵏⵏⵙ, ⵢⵉⵍⵍⵉ ⴷⴰⵔⵙ ⴰⵡⴷ ⵓⵣⵔⴼ ⵏ ⵜⵡⵏⵏⵉⵜ ⵜⴰⵏⴼⵔⵓⵜ ⵙ ⴽⵔⴰ ⵉⴳⴰⵜ ⴰⵏⴰ ⵏⵏⵙ.\nⴽⵓ ⵢⴰⵏ ⵉⵍⵍⴰ ⴷⴰⵔⵙ ⵓⵣⵔⴼ ⵏ ⵜⴷⵔⴼⵉⵜ ⵏ ⵜⴰⵏⵏⴰⵢⵜ ⴷ ⵜⵡⵏⵏⵉⵜ, ⴰⴷ ⵉⵜⵜⵉⴽⵚⵓⴹ ⵅⴼ ⵜⴰⵏⵏⴰⵢⵉⵏ ⵏⵏⵙ ⵓⵍⴰ ⴰⵔⵣⵣⵓ ⵏⵏⵙ ⴰⴷ ⵢⴰⵎⵥ ⵏⵖ ⴰⴷ ⵉⵣⵓⵣⵣⵔ, ⴰⴱⵍⴰ ⵉⵡⵜⵜⴰ, ⵉⵏⵖⵎⵉⵙⵏ ⴷ ⵜⵡⵏⴳⵉⵎⵉⵏ ⵙ ⴰⴽⵯ ⵉⵎⴰⵙⵙⵏ ⵓⵙⵓⵙⵙⵏ."
   specimen_16: "ⴽⵓ ⵢⴰⵏ ⵉⵍⵍⴰ, ⵖⵉⴽⵍⵍⵉ ⵉⴳⴰ ⵢⴰⵏ ⵓⴼⵔⴷⵉⵙ ⵖ ⵡⴰⵎⵓⵏ, ⴷⴰⵔⵙ ⴰⵣⵔⴼ ⵖ ⵓⵏⴼⵔⵓ ⴰⵏⴰⵎⵓⵏ :ⴰⵣⵔⴼ ⴰⴷ ⵉⴱⴷⴷⴰ ⵅⴼ ⵃⵎⴰ ⴰⴷ ⵜⵉⵍⵉ ⵜⵓⵎⵔⵜ ⵏ ⵉⵣⵔⴼⴰⵏ ⵉⴷⴰⵎⵙⴰⵏⵏ, ⵉⵏⴰⵎⵓⵏⵏ ⴷ ⵉⴷⵍⵙⴰⵏⵏ ⵉⵥⵍⵉⵏ ⵙ ⴰⴷⴷⵓⵔ ⵏⵏⵙ ⴷ ⵓⵙⴱⵓⵖⵍⵓ ⵏ ⵡⵓⴷⵎ ⵏⵏⵙ, ⴰⵢⴰⴷ ⵙ ⵜⴷⵓⵙⵉ ⵜⴰⵏⴰⵎⵓⵔⵜ ⴷ ⵜⵡⵉⵙⵉ ⵜⴰⴳⵔⴰⵖⵍⴰⵏⵜ, ⵏⵏⴰ ⵉⵙⵏⵏⴷⵏ ⵅⴼ ⵓⵙⵏⵎⴰⵍⴰ ⴷ ⵉⵙⵓⴳⵉⵎ ⵏ ⴽⵓ ⵜⴰⵎⵓⵔⵜ.\nⴽⵓ ⵢⴰⵏ ⵉⵍⵍⴰ ⴷⴰⵔⵙ ⵓⵣⵔⴼ ⵏ ⵓⵙⵙⵓⵏⴼⵓ, ⵖ ⵜⵉⵣⵉ ⵍⵍⵉ ⵉⵅⵡⴰⵏ, ⴷ ⵎⵏⵛⴽ ⵏ ⵜⵙⵔⴰⴳⵉⵏ ⵏ ⵜⵡⵓⵔⵉ ⴷ ⵓⵙⵙⵏⴼⵓ ⵉⵎⵓⵏ ⴷ ⵜⵖⵔⴰⴷ.\nⴽⵓ ⵢⴰⵏ ⵉⵍⵍⴰ ⴷⴰⵔⵙ ⵓⵣⵔⴼ ⴰⴷ ⵉⵙⴼⴰⵢⴷ ⵖ ⵓⵖⴰⵡⴰⵙ ⴰⵏⴰⵎⵓⵏ ⴰⴳⵔⴰⵖⵍⴰⵏ ⵍⵍⵉⵖ ⵍⵍⴰⵏ ⵉⵣⵔⴼⴰⵏ ⴷ ⵜⴷⵔⴼⵉⵢⵉⵏ ⵍⵍⵉ ⴷ ⵢⵓⵛⴽⴰⵏ ⵖ ⴰⵍⵖⵓ ⴰⴷ.\nⵓⵔ ⵉⵍⵍⵉ ⵖ ⵓⵍⵖⵓ ⴰⴷ ⴽⵔⴰ ⵏ ⵓⴹⵕⵉⵚ ⴰⴼⴰⴷ ⴰⴷ ⵉⵙⵎⴷⵢⴰ ⴽⵔⴰ ⵏ ⵓⵡⴰⵏⴽ ⵏⵖⴷ ⴽⵔⴰ ⵏ ⵓⴳⴷⵓⴷ ⵏⵖⴷ ⵓⴼⴳⴰⵏ ⵙ ⵖⵉⴽⵍⵍⵉ ⵉⵔⴰ ⴷ ⵓⵔ ⴷⴰⵔⵙ ⴽⵔⴰ ⵏ ⵓⵣⵔⴼ ⴰⴼⴰⴷ ⵉⵙⴽⵔ ⵜⴰⵡⵔⵉ ⵏⵏⴰ ⵉⵔⴰ ⵍⵍⵉ ⵉⵜⵜⵔⵥⵥⴰⵏ ⵉⵣⵔⴼⴰⵏ ⴷ ⵜⴷⵔⴼⵢⵉⵏ ⵍⵍⵉ ⴷ ⵢⵉⵡⵉ ⵖ ⵓⵍⵖⵓ ⴰⴷ."
 }
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zh_Hans.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zh_Hans.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 region: "MN"
 region: "MO"
 region: "MY"
 region: "SG"
 exemplar_chars {
   base: "一 丁 七 万-与 丑 专 且 世 丘-业 东 丝 丢 两 严 丧 个 中 丰 串 临 丸-主 丽 举 乃 久 么 义 之-乐 乔 乖 乘 乙 九 也-乡 书 买 乱 乾 了 予 争 事 二 于 亏 云 互 五 井 亚 些 亡 交-亨 享 京 亮 亲 人 亿-仁 仅 仇 今 介 仍 从 仔 他 付 仙 代-以 仪 们 仰 仲 件 价 任 份 仿 企 伊 伍 伏-休 众-会 伟 传 伤 伦 伯 估 伴 伸 似 伽 但 位-佑 体 何 余 佛 作 你 佤 佩 佳 使 例 供 依 侠 侦-侨 侬 侯 侵 便 促 俄 俊 俗 保 信 俩 修 俱 俾 倍 倒 候 倚 借 倦 值 倾 假 偌 偏 做 停 健 偶 偷 储 催 傲 傻 像 僧 儒 儿 允 元-兆 先 光 克 免 兑 兔 党 入 全 八-兮 兰 共 关-兹 养-兽 内 冈 册 再 冒 写 军 农 冠 冬 冰 冲 决 况 冷 准 凌 减 凝 几 凡 凤 凭 凯 凰 出 击 函 刀 分 切 刊 刑 划 列-创 初 判 利 别 到 制-券 刺 刻 剂 前 剑 剧 剩 剪 副 割 力 劝-务 劣 动-劫 励-劳 势 勇 勉 勋 勒 勤 勾 勿 包 匆 匈 化 北 匙 匹-医 十 千 升 午 半 华 协 卒 卓 单-南 博 占-卢 卫 卯-危 即 却 卷 厂 厄-历 厉 压-厍 厚 原 去 县 参 又-反 发 叔 取-叙 口-另 只-叭 可 台 史 右 叶-叹 吃 各 合-吊 同-后 吐 向 吓 吗 君 吝 吟 否 吧 含 听 启 吵 吸 吹 吻 吾 呀 呆 呈 告 呐 员 呜 呢 呦 周 味 呵 呼 命 和 咖 咦-咨 咪 咬 咯 咱 哀 品 哇-哉 响 哎 哟 哥 哦 哩 哪 哭 哲 唉 唐 唤 唬 售 唯 唱 唷 商 啊 啡 啥 啦 啪 喀 喂 善 喇 喊 喏 喔 喜 喝 喵 喷 喻 嗒 嗨 嗯 嘉 嘛 嘴 嘻 嘿 器 四 回 因 团 园 困 围 固 国 图 圆 圈 土 圣 在 圭 地 圳 场 圾 址 均 坎 坐 坑 块 坚-坜 坡 坤 坦 坪 垂 垃 型 垒 埃 埋 城 埔 域 培 基 堂 堆 堕 堡 堪 塑 塔 塞 填 境 增 墨 壁 壤 士 壬 壮 声 处 备 复 夏 夕 外 多 夜 够 夥 大 天-夫 央 失 头 夷-夺 奇-奉 奋 奏 契 奔 奖 套 奥 女 奴 奶 她 好 如 妇 妈 妖 妙 妥 妨 妮 妹 妻 姆 姊 始 姐 姑 姓 委 姿 威 娃 娄 娘 娜 娟 娱 婆 婚 媒 嫁 嫌 嫩 子 孔 孕 字-孙 孜 孝 孟 季 孤 学 孩 宁 它 宇-安 宋 完 宏 宗-实 审-室 宪 害 宴 家 容 宽-宿 寂 寄-寇 富 寒 寝-察 寡 寨 寸 对 寻 导 寿 封 射 将 尊 小 少 尔 尖 尘 尚 尝 尤 就 尺 尼-尾 局-层 居 屋 屏 展 属 屠 山 岁 岂 岗 岘 岚 岛 岳 岸 峡 峰 崇 崩 崴 川 州 巡 工-巨 巫 差 己-巴 巷 币-布 帅 师 希 帐 帕 帖 帝 带 席 帮 常 帽 幅 幕 干-年 并 幸 幻-幽 广 庆 床 序 库-底 店 庙 庚 府 庞 废 度 座 庭 康 庸 廉 廖 延 廷 建 开 异-弄 弊 式 引 弗 弘 弟 张 弥 弦 弯 弱 弹 强 归 当 录 彝 形 彩 彬 彭 彰 影 彷 役 彻 彼 往 征 径 待 很 律 後 徐 徒 得 循 微 徵 德 心 必 忆 忌 忍 志-忙 忠 忧 快 念 忽 怀 态 怎 怒 怕 怖 思 怡 急 性 怨 怪 总 恋 恐 恢 恨 恩 恭 息 恰 恶 恼 悄 悉 悔 悟 悠 患 您 悲 情 惑 惜 惠 惧 惨 惯 想 惹 愁 愈 愉 意 愚 感 愧 慈 慎 慕 慢 慧 慰 憾 懂 懒 戈 戊 戌 戏-戒 或 战 截 戴 户 房-扁 扇 手 才 扎 扑 打 托 扣 执 扩 扫-扯 批 找-技 抄 把 抑 抓 投 抗 折 抢 护 报 披 抬 抱 抵 抹 抽 担 拆 拉 拍 拒 拔 拖 拘 招 拜 拟 拥 拦 拨 择 括 拳 拷 拼 拾 拿 持 指 按 挑 挖 挝 挡 挤 挥 挪 振 挺 捉 捐 捕 损 捡 换 据 捷 授 掉 掌 排 探 接 控-措 掸 描 提 插 握 援 搜 搞 搬 搭 摄 摆 摊 摔 摘 摩 摸 撒 撞 播 操 擎 擦 支 收 改 攻 放 政 故 效 敌 敏 救 教 敝 敢 散 敦 敬 数 敲 整 文 斋 斐 斗 料 斜 斥 断 斯 新 方 於 施 旁 旅 旋 族 旗 无 既 日-早 旭 时 旺 昂 昆 昌 明 昏 易 星 映 春 昨 昭 是 显 晃 晋 晒 晓 晚 晨 普 景 晴 晶 智 暂 暑 暖 暗 暮 暴 曰 曲 更 曹 曼 曾-最 月 有 朋 服 朗 望 朝 期 木 未-札 术 朱 朵 机 杀 杂 权 杉 李 材 村 杜 束 条 来 杨 杯 杰 松 板 极 构 析 林 果 枝 枢 枪 枫 架 柏 某 染 柔 查 柬 柯 柳 柴 标 栋 栏 树 校 样-根 格 桃 框 案 桌 桑 档 桥 梁 梅 梦 梯 械 梵 检 棉 棋 棒 棚 森 椅 植 椰 楚 楼 概 榜 模 樱 檀 欠-欣 欧 欲 欺 款 歉 歌 止-武 歪 死 殊 残 段 毅 母 每 毒 比 毕 毛 毫 氏 民 气 氛 水 永 求 汇 汉 汗 汝 江-污 汤 汪 汶 汽 沃 沈 沉 沙 沟 没 沧 河 油 治 沿 泉 泊 法 泛 泡-泣 泥 注 泰 泳 泽 洋 洗 洛 洞 津 洪 洲 活 洽 派 流 浅 测 济 浏 浑 浓 浙 浦 浩 浪 浮 浴 海 涅 消 涉 涛 涨 涯 液 涵 淋 淑 淘 淡 深 混 添 清 渐 渡 渣 温 港 渴 游 湖 湾 源 溜 溪 滋 滑 满 滥 滨 滴 漂 漏 演 漠 漫 潘 潜 潮 澎 澳 激 灌 火 灭 灯 灰 灵 灿 炉 炎 炮 炸 点 烂 烈 烤 烦 烧 热 焦 然 煌 煞 照 煮 熊 熟 燃 燕 爆 爪 爬 爱 爵-爸 爽 片 版 牌 牙 牛 牡 牢 牧 物 牲 牵 特 牺 犯 状 犹 狂 狐 狗 狠 独 狮 狱 狼 猛 猜 猪 献 猴 玄 率 玉 王 玛 玩 玫 环 现 玲 玻 珀 珊 珍 珠 班 球 理 琊 琪 琳 琴 琼 瑙 瑜 瑞 瑟 瑰 瑶 璃 瓜 瓦 瓶 甘 甚 甜 生 用 田-申 电 男 甸 画 畅 界 留 略 番 疆 疏 疑 疗 疯 疲 疼 疾 病 痕 痛 痴 癸 登 白 百 的 皆 皇 皮 盈 益 监 盒 盖 盘 盛 盟 目 直 相 盼 盾 省 眉 看 真 眠 眼 着 睛 睡 督 瞧 矛 矣 知 短 石 矶 码 砂 砍 研 破 础 硕 硬 确 碍 碎 碗 碟 碧 碰 磁 磅 磨 示 礼 社 祖 祚 祝 神 祥 票 祯 祸 禁 禅 福 离 秀 私 秋 种 科 秒 秘 租 秤 秦 秩 积 称 移 稀 程 稍 税 稣 稳 稿 穆 究 穷 穹 空 穿 突 窗 窝 立 站 竞-章 童 端 竹 笑 笔 笛 符 笨 第 等 筋 筑 答 策 筹 签 简 算 管 箭 箱 篇 篮 簿 籍 米 类 粉 粒 粗 粤 粹 精 糊 糕 糖 糟 系 素 索 紧 紫 累 繁 红 约 级 纪 纯 纲 纳 纵 纷 纸 纽 线 练 组 细-终 绍 经 结 绕 绘 给 络 绝 统 继 绩 绪 续 维 绵 综 绿 缅 缓 编 缘 缠 缩 缴 缶 缸 缺 罐 网 罕 罗 罚 罢 罪 置 署 羊 美 羞 群 羯 羽 翁 翅 翔 翘 翠 翰 翻 翼 耀 老 考 者 而 耍 耐 耗 耳 耶 聊 职 联 聘 聚 聪 肉 肖 肚 股 肤 肥 肩 肯 育 胁 胆 背 胎 胖 胜 胞 胡 胶 胸 能 脆 脑 脱 脸 腊 腐 腓 腰 腹 腾 腿 臂 臣 自 臭 至 致 舌 舍 舒 舞 舟 航 般 舰 船 良 色 艺 艾 节 芒 芝 芦 芬 芭 花 芳 苍 苏 苗 若 苦 英 茂 范 茨 茫 茶 草 荐 荒 荣 药 荷 莉 莎 莪 莫 莱 莲 获 菜 菩 菲 萄 萍 萤 营 萧 萨 落 著 葛 葡 蒂 蒋 蒙 蓉 蓝 蓬 蔑 蔡 薄 薪 藉 藏 藤 虎 虑 虫 虹 虽 虾 蚁 蛇 蛋 蛙 蛮 蜂 蜜 蝶 融 蟹 蠢 血 行 街 衡 衣 补 表 袋 被 袭 裁 裂 装 裕 裤 西 要 覆 见 观 规 视 览 觉 角 解 言 誉 誓 警 计 订 认 讨 让 训-记 讲 讷 许 论 设 访 证 评 识 诉 词 译 试 诗 诚 话 诞 询 该 详 语 误 说 请 诸 诺 读 课 谁 调 谅 谈 谊 谋 谓 谜 谢 谨 谱 谷 豆 象 豪 貌 贝-负 贡-败 货-贪 购 贯 贱 贴 贵 贸-贺 贼 贾 资 赋 赌 赏 赐 赔 赖 赚 赛 赞 赠 赢 赤 赫 走 赵 起 趁 超 越 趋 趣 足 跃 跌 跑 距 跟 路 跳 踏 踢 踩 身 躲 车 轨 轩 转 轮-轰 轻 载 较 辅 辆 辈 辉 辑 输 辛 辞 辨 辩 辰 辱 边 达 迁 迅 过 迈 迎 运 近 返 还 这 进-迟 迦 迪 迫 述 迷 追 退-逃 逆 选 逊 透 逐 递 途 通 逛 逝 速 造 逢 逸 逻 逼 遇 遍 道 遗 遭 遮 遵 避 邀 邓 那 邦 邪 邮 邱 邻 郎 郑 部 郭 都 鄂 酉 酋 配 酒 酷 酸 醉 醒 采 释 里-量 金 针 钓 钟 钢 钦 钱 钻 铁 铃 铜 铢 铭 银 铺 链 销 锁 锅 锋 错 锡 锦 键 锺 镇 镜 镭 长 门 闪 闭 问 闰 闲 间 闷 闹 闻 阁 阅 阐 阔 队 阮 防-阶 阻 阿 陀 附-陆 陈 降 限 院 除 险 陪 陵-陷 隆 随 隐 隔 障 难 雄-集 雉 雨 雪 雯 雳 零 雷 雾 需 震 霍 霖 露 霸 霹 青 靖 静 非 靠 面 革 靼 鞋 鞑 韦 韩 音 页 顶 项-须 顽-顿 预 领 颇 频 颗 题 额 风 飘 飙 飞 食 餐 饭 饮 饰 饱 饼 馆 首 香 馨 马 驱 驶 驻 驾 验 骑 骗 骚 骤 骨 高 鬼 魂 魅 魔 鱼 鲁 鲜 鸟 鸡 鸣 鸭 鸿 鹅 鹤 鹰 鹿 麦 麻 黄 黎 黑 默 鼓 鼠 鼻 齐 齿 龄 龙 龟"
   auxiliary: "乒 乓 乳 仂 仓 伞 伪 侣 傈 傣 僳 僵 冥 冻 净 凉 凸 刨 刮 剃 剽 劈 勺 匕 匠 匮 卑 卜 卞 卦 厕 厘 厦 厨 叮 吕 吴 呕 呣 咒 哨 哺 唇 啤 啮 喱 嗅 嘘 嘟 噘 噜 噢 嚏 坏 坝 垫 堤 堵 墅 墓 墙 墟 壳 壶 奎 奸 妆 姜 娥 婴 媚 孪 宅 宠 宫 寺 尬 尴 尸 屈 屎 屑 屡 履 屿 岩 巽 巾 帆 帚 帜 帧 庇 庵 弓 彗 御 徽 怜 恒 恤 恳 悬 悯 惊 惫 愤 戟 扔 扰 扳 抖 抛 拄 拇 拐 挂 挎 捂 捏 掘 掠 揭 搏 携 摇 撅 撕 撤 攀 敞 斑 斧 昙 晕 朔 杆 杖 杠 枯 柄 柑 柜 柠 柩 柱 柿 栓 栗 栽 桔 桶 梨 棍 棕 棺 椒 楔 楠 榄 榈 槌 槟 槿 横 橄 橇 橘 橙 橡 檬 汁 沐 沫 泪 泵 洁 洒 浆 浣 涂 涌 涎 涕 涩 淇 渗 湘 滕 滚 滩 澡 灾 炽 烘 烙 烛 烟 烹 焊 焙 焰 煎 熏 燥 犀 犄 犬 犸 狡 狸 猎 猕 猩 猫 猬 猾 猿 獭 獾 瑚 瓢 瓮 甫 畜 疟 皂 皱 皿 盆 盐 盔 盗 盥 盲 眨 眩 眯 睿 瞌 瞒 瞪 矿 砖 砸 碑 祈 祭 祷 禄 禽 秃 稻 稽 窃 窄 窥 竖 竿 笆 笺 笼 筐 筒 筝 筷 箸 篓 篱 篷 粑 粟 粥 粮 粽 絮 纠 纫 纬 纱 纹 绒 绣 绳 绷 缄 缆 缎 缝 罩 羹 翱 耸 聋 肌 肢 肺 脏 脚 腋 腕 腮 膀 膏 舔 舵 艇 艮 艳 芙 芽 苜 苞 苣 苹 茄 莓 莴 菇 菌 菠 菱 萎 萝 葩 葫 葬 葱 葵 蒜 蒲 蒸 蓄 蓿 蔬 蔽 蕉 蕾 薯 蘑 蚂 蚊 蚓 蚝 蚯 蛆 蛎 蛐 蛛 蛰 蛾 蜗 蜘 蜡 蜥 蜴 蝇 蝎 蝙 蝠 蝴 螂 螃 螺 蟀 蟋 蟑 蠕 衫 衬 袜 裙 裹 褂 讶 讽 诊 诱 谍 谎 谚 谬 豚 豹 账 贷 赣 趾 跆 跛 跤 跨 跪 踪 蹄 蹈 蹦 蹬 躬 躺 轴 轿 辐 辣 迹 郁 鄙 酢 酥 酪 酱 醺 钉 钞 钥 钩 钮 钯 钳 铂 铅 铛 铰 锄 锑 锚 锤 锯 镐 镑 镖 闺 闽 阱 隧 雀 雌 雕 霜 霾 靴 靶 鞠 颈 颜 颠 颤 飓 饪 饵 饺 馍 馏 驰 驼 骂 骄 骆 骰 骷 骼 髅 髦 鬈 魁 鱿 鲤 鲨 鲸 鳄 鸢 鸵 鸽 鹉 鹦 黏 黛 鼬 龇"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9 〇 一 七 三 九 二 五 八 六 四"
-  punctuation: "﹉﹊﹋﹌ _ ＿ ﹍﹎﹏ ︳︴ - － ﹣ ‐ ‑ – — ︱ ― , ， ﹐ 、 ﹑ ; ； ﹔ : ： ﹕ ! ！ ﹗ ? ？ ﹖ . ． ﹒ ‥ ︰ … 。 · ＇ ‘ ’ \" ＂ “ ” 〝 〞 ( （ ﹙ ︵ ) ） ﹚ ︶ [ ［ ] ］ { ｛ ﹛ ︷ } ｝ ﹜ ︸ 〈 ︿ 〉 ﹀ 《 ︽ 》 ︾ 「 ﹁ 」 ﹂ 『 ﹃ 』 ﹄ 【 ︻ 】 ︼ 〔 ﹝ ︹ 〕 ﹞ ︺ 〖 〗 ‖ § @ ＠ ﹫ * ＊ ﹡ / ／ \\ ＼ ﹨ & ＆ ﹠ # ＃ ﹟ % ％ ﹪ ‰ ′ ″ ‵ 〃 ※"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9 〇 一 七 三 九 二 五 八 六 四"
+  punctuation: "﹉﹊﹋﹌ _ ＿ ﹍﹎﹏ ︳︴ - － ﹣ – — ︱ ― , ， ﹐ 、 ﹑ ; ； ﹔ : ： ﹕ ! ！ ﹗ ? ？ ﹖ . ． ﹒ ‥ ︰ … 。 · ＇ ‘ ’ \" ＂ “ ” 〝 〞 ( （ ﹙ ︵ ) ） ﹚ ︶ [ ［ ] ］ { ｛ ﹛ ︷ } ｝ ﹜ ︸ 〈 ︿ 〉 ﹀ 《 ︽ 》 ︾ 「 ﹁ 」 ﹂ 『 ﹃ 』 ﹄ 【 ︻ 】 ︼ 〔 ﹝ ︹ 〕 ﹞ ︺ 〖 〗 ‖ @ ＠ ﹫ * ＊ ﹡ / ／ \\ ＼ ﹨ & ＆ ﹠ # ＃ ﹟ % ％ ﹪ ‵ 〃 ※"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "人生而自"
   masthead_partial: "由在"
   styles: "鉴于对人类家庭所有成员的固有尊严及其平等的和不移的权利的承认,乃是世界自由、正义与和平的基础"
   tester: "鉴于对人权的无视和侮蔑已发展为野蛮暴行,这些暴行玷污了人类的良心,而一个人人享有言论和信仰自由并免予恐惧和匮乏的世界的来临,已被宣布为普通人民的最高愿望"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zh_Hant.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zh_Hant.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 region: "TH"
 region: "TW"
 region: "US"
 region: "VN"
 exemplar_chars {
   base: "一 丁 七 丈-不 丑 且 世 丘 丙 丟 並 中 串 丸 丹 主 乃 久 么 之 乎 乏 乖 乘 乙 九 也 乾 亂 了 予 事 二 于 云 互 五 井 些 亞 亡 交-亦 亨 享 京 亮 人 什 仁 仇 今 介 仍 仔 他 付 仙 代-以 仰 仲 件 任 份 企 伊 伍 伐 休 伙 伯 估 伴 伸 似 伽 但 佈 佉 位-住 佔 何 余 佛 作 你 佩 佳 使 來 例 供 依 侯 侵 便 係-俄 俊 俗 保 俠 信 修 俱 俾 個 倍 們 倒 候 倚 借 倫 值 假 偉 偏 做 停 健 側-偷 傑 備 傢 傣 傲 傳 傷 傻 傾 僅 像 僑 僧 價 儀 億 儒 儘 優 允 元-充 兇-光 克 免 兒 兔 入 內-兩 八-兮 共 兵-典 兼 冊 再 冒 冠 冬 冰 冷 准 凌 凝 凡 凰 凱 出 函 刀 分 切 刊 列 初 判 別 利 刪 到 制 刷 刺 刻 則 剌 前 剛 剩 剪 副 割 創 劃 劇 劉 劍 力 功 加 助-劫 勁 勇 勉 勒 動 務 勝 勞 勢 勤 勵 勸 勿 包 匈 化 北 匹 區 十 千 升 午 半 卒-協 南 博 卜 卡 卯-危 即 卷 卻 厄 厘 厚 原 厭 厲 去 參 又 及 友 反 叔 取 受 口-另 只-叭 可 台 史 右 司 吃 各 合-吊 同-后 吐-吒 君 吝-吠 否 吧 含 吳 吵 吸 吹 吾 呀 呂 呆 告 呢 周 味 呵 呼 命 和 咖 咦 咧 咪 咬 咱 哀 品 哇-哉 哎 員 哥 哦 哩 哪 哭 哲 唉 唐 唔 唬 售 唯 唱 唷 唸 商 啊 問 啟 啡 啥 啦 啪 喀 喂 善 喇 喊 喔 喜 喝 喬 單 喵 嗎 嗚 嗨 嗯 嘆 嘉 嘗 嘛 嘴 嘻 嘿 器 噴 嚇 嚴 囉 四 回 因 困 固 圈 國 圍 園 圓 圖 團 圜 土 在 圭 地 圾 址 均 坎 坐 坡 坤 坦 坪 垂 垃 型 埃 城 埔 域 執 培 基 堂 堅 堆 堡 堪 報 場 塊 塔 塗 塞 填 塵 境 增 墨 墮 壁 壇 壓 壘 壞 壢 士 壬 壯 壽 夏 夕 外 多 夜 夠 夢 夥 大 天-夫 央 失 夷 夸 夾 奇-奉 奎 奏 契 奔 套 奧 奪 奮 女 奴 奶 她 好 如 妙 妝 妥 妨 妮 妳 妹 妻 姆 姊 始 姐 姑 姓 委 姿 威 娃 娘 娛 婁 婆 婚 婦 媒 媽 嫌 嫩 子 孔 字 存 孝 孟 季 孤 孩 孫 學 它 宅 宇-安 宋 完 宏 宗-宜 客-室 宮 害 家 容 宿 寂 寄-密 富 寒 寞 察 寢 實-審 寫 寬 寮 寵 寶 封 射 將 專 尊 尋 對-小 少 尖 尚 尤 就 尺 尼 尾 局 屁 居 屆 屋 屏 展 屠 層 屬 山 岡 岩 岸 峰 島 峽 崇 崙 崴 嵐 嶺 川 州 巡 工-巨 巫 差 己-巴 巷 市 布 希 帕 帖 帛 帝 帥 師 席 帳 帶 常 帽 幅 幕 幣 幫 干-年 幸 幹 幻-幾 庇 床 序 底 店 庚 府 度 座 庫 庭 康 庸 廉 廖 廠 廢 廣 廳 延 廷 建 弄 式 引 弗 弘 弟 弦 弱 張 強 彈 彊 彌 彎 彝 彞 形 彥 彩 彬 彭 彰 影 役 彼 往 征 待 很 律 後 徐-徒 得 從 復 微 徵 德 徹 心 必 忌 忍 志-忙 忠 快 念 忽 怎 怒 怕 怖 思 怡 急 性 怨 怪 恆 恐 恢 恥 恨 恩 恭 息 恰 悅 悉 悔 悟 悠 您 悲 悶 情 惑 惜 惠 惡 惱 想 惹 愁 愈 愉 意 愚 愛 感 慈 態 慕 慘 慢 慣 慧 慮 慰 慶 慾 憂 憐 憑 憲 憶 憾 懂 應 懶 懷 懼 戀 戈 戊 戌 成-戒 或 截 戰 戲 戴 戶 房-扁 扇 手 才 扎 打 托 扣 扥 扭 扯 批 找-技 抄 把 抓 投 抗 折 披 抬 抱 抵 抹 抽 拆 拉 拋 拍 拏 拒 拔 拖 招 拜 括 拳 拼 拾 拿 持 指 按 挑 挖 挪 振 挺 捐 捕 捨 捲 捷 掃 授 掉 掌 排 掛 採 探 接 控 推 措 描 提 插 揚 換 握 揮 援 損 搖 搜 搞 搬 搭 搶 摘 摩 摸 撐 撒 撞 撣 撥 播 撾 撿 擁 擇 擊 擋 操 擎 擔 據 擠 擦 擬 擴 擺 擾 攝 支 收 改 攻 放 政 故 效 敍 敏 救 敗-教 敝 敢 散 敦 敬 整 敵 數 文 斐 斗 料 斯 新 斷 方 於 施 旁 旅 旋 族 旗 既 日 旦 早 旭 旺 昂 昆 昇 昌 明 昏 易 星 映 春 昨 昭 是 時 晉 晒 晚 晨 普 景 晴 晶 智 暑 暖 暗 暫 暴 曆 曉 曰 曲 更 書 曼 曾-最 會 月 有 朋 服 朗 望 朝 期 木 未-札 朱 朵 杉 李 材 村 杜 束 杯-東 松 板 析 林 果 枝 架 柏 某 染 柔 查 柬 柯 柳 柴 校 核 根 格 桃 案 桌 桑 梁 梅 條 梨 梯 械 梵 棄 棉 棋 棒 棚 森 椅 植 椰 楊 楓 楚 業 極 概 榜 榮 構 槍 樂 樓 標 樞 模 樣 樹 橋 機 橫 檀 檔 檢 欄 權 次 欣 欲 欺 欽 款 歉 歌 歐 歡-武 歲 歷 歸 死 殊 殘 段 殺 殼 毀 毅 母 每 毒 比 毛 毫 氏 民 氣 水 永 求 汗 汝 江-污 汪 汶 決 汽 沃 沈 沉 沒 沖 沙 河 油 治 沿 況 泉 泊 法 泡 波 泥 注 泰 泳 洋 洗 洛 洞 洩 洪 洲 活 洽 派 流 浦 浩 浪 浮 海 涇-涉 涯 液 涵 涼 淑 淚 淡 淨 深 混 淺 清 減 渡 測 港 游 湖 湯 源 準 溝 溪 溫 滄 滅 滋 滑 滴 滾 滿 漂 漏 演 漠 漢 漫 漲 漸 潔 潘 潛 潮 澤 澳 激 濃 濟 濤 濫 濱 瀏 灌 灣 火 灰 災 炎 炮 炸 為 烈 烏 烤 無 焦 然 煙 煞 照 煩 熊 熟 熱 燃 燈 燒 營 爆 爐 爛 爪 爬 爭 爵 父 爸 爺 爽 爾 牆-版 牌 牙 牛 牠 牧 物 牲 特 牽 犧 犯 狀 狂 狐 狗 狠 狼 猛 猜 猴 猶 獄 獅 獎 獨 獲 獸 獻 玄 率 玉 王 玩 玫 玲 玻 珊 珍 珠 珥 班 現 球 理 琉 琪 琴 瑙 瑜 瑞 瑟 瑤 瑪 瑰 環 瓜 瓦 瓶 甘 甚 甜 生 產 用 田-申 男 甸 界 留 畢 略 番 畫 異 當 疆 疏 疑 疼 病 痕 痛 痴 瘋 療 癡 癸 登-百 的 皆 皇 皮 盃 益 盛 盜 盟 盡 監 盤 盧 目 盲 直 相 盼 盾 省 眉 看 真 眠 眼 眾 睛 睡 督 瞧 瞭 矛 矣 知 短 石 砂 砍 研 砲 破 硬 碎 碗 碟 碧 碩 碰 確 碼 磁 磨 磯 礎 礙 示 社 祕 祖 祚 祛 祝 神 祥 票 祿 禁 禍-福 禪 禮 秀 私 秋 科 秒 秘 租 秤 秦 移 稅 程 稍 種 稱 稿 穆 穌 積 穩 究 穹 空 穿 突 窗 窩 窮 窶 立 站 竟 章 童 端 競 竹 笑 笛 符 笨 第 筆 等 筋 答 策 简 算 管 箭 箱 節 範 篇 築 簡 簫 簽 簿 籃 籌 籍 籤 米 粉 粗 粵 精 糊 糕 糟 系 糾 紀 約 紅 納 紐 純 紙-紛 素 索 紫 累 細 紹 終 組 結 絕 絡 給 統 絲 經 綜 綠 維 綱 網 緊 緒 線 緣 編 緩 緬 緯 練 縛 縣 縮 縱 總 績 繁 繆 織 繞 繪 繳 繼 續 缸 缺 罕 罪 置 罰 署 罵 罷 羅 羊 美 羞 群 義 羽 翁 習 翔 翰 翹 翻 翼 耀 老 考 者 而 耍 耐 耗 耳 耶 聊 聖 聚 聞 聯 聰 聲 職 聽 肉 肚 股 肥 肩 肯 育 背 胎 胖 胞 胡 胸 能 脆 脫 腓 腔 腦 腰 腳 腿 膽 臉 臘 臣 臥 臨 自 臭 至 致 臺 與-舊 舌 舍 舒 舞 舟 航 般 船 艦 良 色 艾 芝 芬 花 芳 若 苦 英 茅 茫 茲 茶 草 荒 荷 荼 莉 莊 莎 莫 菜 菩 華 菲 萄 萊 萬 落 葉 著 葛 葡 蒂 蒙 蒲 蒼 蓋 蓮 蔕 蔡 蔣 蕭 薄 薦 薩 薪 藉 藍 藏 藝 藤 藥 蘆 蘇 蘭 虎 處 虛 號 虧 蛇 蛋 蛙 蜂 蜜 蝶 融 螢 蟲 蟹 蠍 蠻 血 行 術 街 衛 衝 衡 衣 表 袋 被 裁 裂 裕 補 裝 裡 製 複 褲 西 要 覆 見 規 視 親 覺 覽 觀 角 解 觸 言 訂 計 訊 討 訓 託 記 訥 訪 設 許 訴 註 証 評 詞 詢 試 詩 話-詳 誇 誌 認 誓 誕 語 誠 誤 說 誰 課 誼 調 談 請 諒 論 諸 諺 諾 謀 謂 講 謝 證 識 譜 警 譯 議 護 譽 讀 變 讓 讚 谷 豆 豈 豐 象 豪 豬 貌 貓 貝 貞 負-貢 貨 貪-責 貴 買 費 貼 賀 資 賈 賓 賜 賞 賢-賤 賦 質 賭 賴 賺 購 賽 贈 贊 贏 赤 赫 走 起 超 越 趕 趙 趣 趨 足 跌 跎 跑 距 跟 跡 路 跳 踏 踢 蹟 蹤 躍 身 躲 車 軌 軍 軒 軟 較 載 輔 輕 輛 輝 輩 輪 輯 輸 轉 轟 辛 辦 辨 辭 辯-農 迅 迎 近 返 迦 迪 迫 述 迴 迷 追 退 送 逃 逆 透 逐 途 這-逛 逝 速 造 逢 連 週 進 逸 逼 遇 遊 運 遍 過 道-違 遙 遜 遠 適 遭 遮 遲 遷 選 遺 避-邁 還 邊 邏 那 邦 邪 邱 郎 部 郭 郵 都 鄂 鄉 鄭 鄰 酉 配 酒 酷 酸 醉 醒 醜 醫 采 釋-量 金 針 釣 鈴 鉢 銀 銅 銖 銘 銳 銷 鋒 鋼 錄 錢 錦 錫 錯 鍋 鍵 鍾 鎊 鎖 鎮 鏡 鐘 鐵 鑑 長 門 閃 閉 開 閏 閒 間 閣 閱 闆 闊 闍 闐 關 闡 防 阻 阿 陀 附 降 限 院-除 陪 陰 陳 陵-陸 陽 隆 隊 階 隔 際 障 隨 險 隱 隻 雄-集 雉 雖 雙 雜 雞 離 難 雨 雪 雲 零 雷 電 需 震 霍 霧 露 霸 霹 靂 靈 青 靖 靜 非 靠 面 革 靼 鞋 韃 韋 韓 音 韻 響 頁 頂 項 順 須 預 頑 頓 頗 領 頞 頭 頻 顆 題 額 顏 願 類 顧 顯 風 飄 飛 食 飯 飲 飽 飾 餅 養 餐 餘 館 首 香 馬 駐 駕 駛 騎 騙 騷 驅 驗 驚 骨 體 高 髮 鬆 鬥 鬧 鬱 鬼 魁 魂 魅 魔 魚 魯 鮮 鳥 鳳 鳴 鴻 鵝 鷹 鹿 麗 麥 麵 麻 麼 黃 黎 黑 默 點 黨 鼓 鼠 鼻 齊 齋 齒 齡 龍 龜"
   auxiliary: "乍 乳 仂 伏 佐 侶 俏 倉 偽 傅 傘 僳 兆 兌 兹 凋 凍 凸 划 刨 别 刮 券 剃 勳 勾 匕 匙 匣 匯 卑 卞 占 卹 叉 叶 吻 哺 唇 唵 啤 喪 喲 嘟 噁 噓 噘 嚏 坑 堤 墅 墎 墓 墟 墳 壤 壩 壺 奥 妖 嬰 孕 孜 孵 寺 尿 屍 屑 峇 嶼 巽 巾 帆 帚 幟 廁 廈 廚 廟 弋 弓 忡 憊 懨 懸 戟 扮 扳 捂 捏 捧 掠 掰 揹 搏 摀 摔 撕 撲 攀 攤 敞 斑 斜 斧 暈 暮 曇 曬 曳 朔 杖 枯 栓 栗 栽 框 桶 桿 棍 棕 棺 椒 楔 槌 橄 橇 橘 橙 檬 檸 櫃 櫚 櫻 欖 欠 残 殭 汁 沫 沮 泣 浣 浴 涅 涎 涮 淇 淋 渾 湘 溜 漿 澎 澡 濕 灘 烘 烹 焊 焙 焰 煎 煮 燕 燙 燦 燭 爍 牡 犀 犬 狄 狡 狸 猩 猾 猿 獺 獾 琳 瑚 瓢 甕 甫 疊 疲 疾 瘦 瘧 皂 皺 皿 盆 盈 盒 盔 盥 眨 眩 睏 瞇 瞌 瞪 碑 磚 礁 礫 祈 禱 禿 稻 穀 窄 竿 筒 筷 箏 箔 篷 簍 籠 糖 糰 紉 紋 紗 紮 紳 綽 綿 縫 繃 繡 繩 纏 纖 纜 罈 罐 罩 羯 聳 聾 肌 肖 肺 脈 脖 腐 腹 膚 膠 臂 臟 艇 芒 芙 芭 芽 苗 苣 茄 茨 茵 茸 莓 莖 菇 菌 菱 萎 萵 葵 蒜 蒸 蓄 蓉 蓬 蔔 蔥 蔬 蕉 蕾 薑 薯 蘋 蘑 蘿 虹 蚊 蚓 蚩 蚯 蛛 蜀 蜘 蜥 蜴 蝙 蝟 蝠 蝦 蝴 蝸 螂 螃 螞 螺 蟀 蟄 蟋 蟑 蟳 蟻 蠅 蠕 蠟 蠣 衫 袍 裏 裘 裙 裱 裹 褐 襪 襯 訝 診 謎 謬 豎 豔 豚 豹 贛 跆 跨 跪 踩 躬 軸 轎 辜 辣 遞 鄙 酋 酪 醬 釘 鈔 鈕 鉅 鉛 鉤 鋁 錨 錶 鍊 鎚 鎬 鏈 鏢 鐺 鑰 鑽 鑿 閩 阱 隴 雀 雌 霄 霜 静 靴 鞠 鞭 頌 頸 顛 颱 飆 飪 餃 餌 餚 餵 餾 駝 駱 驕 骰 骷 髏 鬍 魷 鮑 鯉 鯊 鯨 鱷 鳩 鳶 鴨 鵡 鶴 鸚 鹽 黛 鼬 龐"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9 〇 一 七 三 九 二 五 八 六 四"
-  punctuation: "‾ ﹉﹊﹋﹌ _ ＿ ﹍﹎﹏ ︳︴ - － ﹣ ‐ ‑ – ︲ — ﹘ ︱ , ， ﹐ 、 ﹑ ; ； ﹔ : ： ﹕ ! ！ ﹗ ? ？ ﹖ . ． ﹒ ‥ ︰ … 。 · ＇ ‘ ’ \" ＂ “ ” 〝 〞 ( （ ﹙ ︵ ) ） ﹚ ︶ [ ［ ] ］ { ｛ ﹛ ︷ } ｝ ﹜ ︸ 〈 ︿ 〉 ﹀ 《 ︽ 》 ︾ 「 ﹁ 」 ﹂ 『 ﹃ 』 ﹄ 【 ︻ 】 ︼ 〔 ﹝ ︹ 〕 ﹞ ︺ § @ ＠ ﹫ * ＊ ﹡ / ／ \\ ＼ ﹨ & ＆ ﹠ # ＃ ﹟ % ％ ﹪ ‰ † ‡ ‧ ′ ″ ‵ 〃 ※"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9 〇 一 七 三 九 二 五 八 六 四"
+  punctuation: "‾ ﹉﹊﹋﹌ _ ＿ ﹍﹎﹏ ︳︴ - － ﹣ – ︲ — ﹘ ︱ , ， ﹐ 、 ﹑ ; ； ﹔ : ： ﹕ ! ！ ﹗ ? ？ ﹖ . ． ﹒ ‥ ︰ … 。 · ＇ ‘ ’ \" ＂ “ ” 〝 〞 ( （ ﹙ ︵ ) ） ﹚ ︶ [ ［ ] ］ { ｛ ﹛ ︷ } ｝ ﹜ ︸ 〈 ︿ 〉 ﹀ 《 ︽ 》 ︾ 「 ﹁ 」 ﹂ 『 ﹃ 』 ﹄ 【 ︻ 】 ︼ 〔 ﹝ ︹ 〕 ﹞ ︺ @ ＠ ﹫ * ＊ ﹡ / ／ \\ ＼ ﹨ & ＆ ﹠ # ＃ ﹟ % ％ ﹪ ‧‵ 〃 ※"
   index: "一 丁 丈 不 且 丞 並 串 乘 乾 亂 亭 傀 僎 僵 儐 償 儳 儷 儻 叢 嚴 囌 囑 廳"
 }
 sample_text {
   masthead_full: "人生而自"
   masthead_partial: "由在"
   styles: "鑑於對人類家庭所有成員的固有尊嚴及其平等的和不移的權利的承認，乃是世界自由、正義與和平的基礎"
   tester: "鑑於對人權的無視和侮蔑已發展為野蠻暴行，這些暴行沾污了人類的良心，而一個人人享有言論和信仰自由並免予恐懼和匱乏的世界的來臨，已被宣布為普通人民的最高願望"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zh_Hebr.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zh_Hebr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zlm_Arab.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zlm_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zlm_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zlm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zro_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/ztu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/ztu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zu_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zu_Latn.textproto`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 region: "MW"
 region: "MZ"
 region: "SZ"
 region: "ZA"
 exemplar_chars {
   base: "a b {bh} c {ch} d {dl} {dy} e f g {gc} {gq} {gx} h {hh} {hl} i j k {kh} {kl} {kp} l m n {nc} {ngc} {ngq} {ngx} {nhl} {nk} {nkc} {nkq} {nkx} {nq} {ntsh} {nx} {ny} o p {ph} q {qh} r {rh} s {sh} t {th} {tl} {ts} {tsh} u v w x {xh} y z"
   auxiliary: "á à ă â å ä ã ā æ ç é è ĕ ê ë ē í ì ĭ î ï ī ñ ó ò ŏ ô ö ø ō œ ú ù ŭ û ü ū ÿ"
-  numerals: "- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9"
-  punctuation: "- ‑ , ; : ! ? . ( ) [ ] { }"
+  numerals: "- , . % + 0 1 2 3 4 5 6 7 8 9"
+  punctuation: "- , ; : ! ? . ( ) [ ] { }"
   index: "A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
 }
 sample_text {
   masthead_full: "BbOo"
   masthead_partial: "Nn"
   styles: "Ngokunjalo ukwamukelwa ngokuzuzwa kwesithunzi"
   tester: "Ngokunjalo ukunganakwa nokwedelelwa kwamalungelo esintu kube"
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages/data/languages/zza_Latn.textproto` & `gflanguages-5.0.4/Lib/gflanguages/data/languages/zza_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/languages_public.proto` & `gflanguages-5.0.4/Lib/gflanguages/languages_public.proto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages/languages_public_pb2.py` & `gflanguages-5.0.4/Lib/gflanguages/languages_public_pb2.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/Lib/gflanguages.egg-info/PKG-INFO` & `gflanguages-5.0.4/Lib/gflanguages.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gflanguages
-Version: 0.8.9
+Version: 5.0.4
 Summary: A python API for evaluating language support in the Google Fonts collection.
 Home-page: https://github.com/googlefonts/lang/
 Author: Dave Crossland, Felipe Sanches, Marc Foley, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `gflanguages-0.8.9/Lib/gflanguages.egg-info/SOURCES.txt` & `gflanguages-5.0.4/Lib/gflanguages.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1191,57 +1191,45 @@
 Lib/gflanguages/data/languages/rug_Latn.textproto
 Lib/gflanguages/data/languages/rup_Latn.textproto
 Lib/gflanguages/data/languages/rw_Latn.textproto
 Lib/gflanguages/data/languages/rwk_Latn.textproto
 Lib/gflanguages/data/languages/ryu_Jpan.textproto
 Lib/gflanguages/data/languages/ryu_Kana.textproto
 Lib/gflanguages/data/languages/sa_Ahom.textproto
-Lib/gflanguages/data/languages/sa_Avst.textproto
 Lib/gflanguages/data/languages/sa_Bali.textproto
-Lib/gflanguages/data/languages/sa_Batk.textproto
 Lib/gflanguages/data/languages/sa_Bhks.textproto
 Lib/gflanguages/data/languages/sa_Brah.textproto
 Lib/gflanguages/data/languages/sa_Bugi.textproto
-Lib/gflanguages/data/languages/sa_Buhd.textproto
 Lib/gflanguages/data/languages/sa_Cham.textproto
 Lib/gflanguages/data/languages/sa_Deva.textproto
-Lib/gflanguages/data/languages/sa_Dogr.textproto
 Lib/gflanguages/data/languages/sa_Gonm.textproto
 Lib/gflanguages/data/languages/sa_Gran.textproto
-Lib/gflanguages/data/languages/sa_Hano.textproto
 Lib/gflanguages/data/languages/sa_Khar.textproto
-Lib/gflanguages/data/languages/sa_Khoj.textproto
-Lib/gflanguages/data/languages/sa_Kthi.textproto
-Lib/gflanguages/data/languages/sa_Lepc.textproto
 Lib/gflanguages/data/languages/sa_Limb.textproto
-Lib/gflanguages/data/languages/sa_Mahj.textproto
 Lib/gflanguages/data/languages/sa_Marc.textproto
 Lib/gflanguages/data/languages/sa_Modi.textproto
 Lib/gflanguages/data/languages/sa_Mong.textproto
 Lib/gflanguages/data/languages/sa_Mroo.textproto
 Lib/gflanguages/data/languages/sa_Mtei.textproto
 Lib/gflanguages/data/languages/sa_Mult.textproto
 Lib/gflanguages/data/languages/sa_Nand.textproto
 Lib/gflanguages/data/languages/sa_Newa.textproto
-Lib/gflanguages/data/languages/sa_Olck.textproto
 Lib/gflanguages/data/languages/sa_Orya.textproto
 Lib/gflanguages/data/languages/sa_Phag.textproto
 Lib/gflanguages/data/languages/sa_Ranj.textproto
 Lib/gflanguages/data/languages/sa_Rjng.textproto
-Lib/gflanguages/data/languages/sa_Saur.textproto
 Lib/gflanguages/data/languages/sa_Shrd.textproto
 Lib/gflanguages/data/languages/sa_Sidd.textproto
 Lib/gflanguages/data/languages/sa_Sind.textproto
 Lib/gflanguages/data/languages/sa_Sinh.textproto
 Lib/gflanguages/data/languages/sa_Sora.textproto
 Lib/gflanguages/data/languages/sa_Soyo.textproto
 Lib/gflanguages/data/languages/sa_Sund.textproto
 Lib/gflanguages/data/languages/sa_Sylo.textproto
 Lib/gflanguages/data/languages/sa_Tagb.textproto
-Lib/gflanguages/data/languages/sa_Takr.textproto
 Lib/gflanguages/data/languages/sa_Tirh.textproto
 Lib/gflanguages/data/languages/sa_Wara.textproto
 Lib/gflanguages/data/languages/sa_Wcho.textproto
 Lib/gflanguages/data/languages/sa_Xpeo.textproto
 Lib/gflanguages/data/languages/sa_Zanb.textproto
 Lib/gflanguages/data/languages/sad_Latn.textproto
 Lib/gflanguages/data/languages/saf_Latn.textproto
@@ -1263,15 +1251,15 @@
 Lib/gflanguages/data/languages/sck_Deva.textproto
 Lib/gflanguages/data/languages/scn_Latn.textproto
 Lib/gflanguages/data/languages/sco_Latn.textproto
 Lib/gflanguages/data/languages/scs_Latn.textproto
 Lib/gflanguages/data/languages/sd_Arab.textproto
 Lib/gflanguages/data/languages/sd_Deva.textproto
 Lib/gflanguages/data/languages/sd_Khoj.textproto
-Lib/gflanguages/data/languages/sd_Sind.textproto
+Lib/gflanguages/data/languages/sd_Khud.textproto
 Lib/gflanguages/data/languages/sdc_Latn.textproto
 Lib/gflanguages/data/languages/sdh_Arab.textproto
 Lib/gflanguages/data/languages/se_Cyrl.textproto
 Lib/gflanguages/data/languages/se_Latn.textproto
 Lib/gflanguages/data/languages/see_Latn.textproto
 Lib/gflanguages/data/languages/sef_Latn.textproto
 Lib/gflanguages/data/languages/seh_Latn.textproto
@@ -1323,14 +1311,15 @@
 Lib/gflanguages/data/languages/sog_Sogo.textproto
 Lib/gflanguages/data/languages/sok_Latn.textproto
 Lib/gflanguages/data/languages/sou_Thai.textproto
 Lib/gflanguages/data/languages/soy_Latn.textproto
 Lib/gflanguages/data/languages/spp_Latn.textproto
 Lib/gflanguages/data/languages/sq_Elba.textproto
 Lib/gflanguages/data/languages/sq_Latn.textproto
+Lib/gflanguages/data/languages/sq_Vith.textproto
 Lib/gflanguages/data/languages/sr_Cyrl.textproto
 Lib/gflanguages/data/languages/sr_Latn.textproto
 Lib/gflanguages/data/languages/srb_Latn.textproto
 Lib/gflanguages/data/languages/srb_Sora.textproto
 Lib/gflanguages/data/languages/srn_Latn.textproto
 Lib/gflanguages/data/languages/srr_Latn.textproto
 Lib/gflanguages/data/languages/srx_Deva.textproto
@@ -2016,14 +2005,15 @@
 Lib/gflanguages/data/scripts/Thai.textproto
 Lib/gflanguages/data/scripts/Tibt.textproto
 Lib/gflanguages/data/scripts/Tirh.textproto
 Lib/gflanguages/data/scripts/Tnsa.textproto
 Lib/gflanguages/data/scripts/Toto.textproto
 Lib/gflanguages/data/scripts/Ugar.textproto
 Lib/gflanguages/data/scripts/Vaii.textproto
+Lib/gflanguages/data/scripts/Vith.textproto
 Lib/gflanguages/data/scripts/Wara.textproto
 Lib/gflanguages/data/scripts/Wcho.textproto
 Lib/gflanguages/data/scripts/Xpeo.textproto
 Lib/gflanguages/data/scripts/Xsux.textproto
 Lib/gflanguages/data/scripts/Yezi.textproto
 Lib/gflanguages/data/scripts/Yiii.textproto
 Lib/gflanguages/data/scripts/Zanb.textproto
```

### Comparing `gflanguages-0.8.9/PKG-INFO` & `gflanguages-5.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gflanguages
-Version: 0.8.9
+Version: 5.0.4
 Summary: A python API for evaluating language support in the Google Fonts collection.
 Home-page: https://github.com/googlefonts/lang/
 Author: Dave Crossland, Felipe Sanches, Marc Foley, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `gflanguages-0.8.9/README.md` & `gflanguages-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/data/test/nunito/Nunito-Regular.ttf` & `gflanguages-5.0.4/data/test/nunito/Nunito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/data/test/nunito/OFL.txt` & `gflanguages-5.0.4/data/test/nunito/OFL.txt`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/setup.py` & `gflanguages-5.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/snippets/fix-exemplars-duplicates.py` & `gflanguages-5.0.4/snippets/fix-exemplars-duplicates.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
                         continue
                     else:
                         value_set.add(value)
                         clean_values.append(value)
 
                 if clean_values != values:
                     if {len(set(values))} != {len(set(clean_values))}:
-                        print("before: " + " ".join(values))
-                        print("after: " + " ".join(clean_values))
+                        print("before: "+ " ".join(values))
+                        print("after: "+ " ".join(clean_values))
                         sys.exit("Failed fixing exemplar.")
                     setattr(language.exemplar_chars, attr, " ".join(clean_values))
                     changed = True
                     exemplar_values[attr] = {
                         "before": values,
                         "after": clean_values
                     }
```

### Comparing `gflanguages-0.8.9/snippets/supported_languages.py` & `gflanguages-5.0.4/snippets/supported_languages.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/tests/test_data_languages.py` & `gflanguages-5.0.4/tests/test_data_languages.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/tests/test_dottedcircle.py` & `gflanguages-5.0.4/tests/test_dottedcircle.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.8.9/tests/test_gflanguages_api.py` & `gflanguages-5.0.4/tests/test_gflanguages_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 def test_LoadLanguages():
     for langs in [LoadLanguages(),
                   LoadLanguages(None),
                   LoadLanguages(DATA_DIR)]:
         numerals = langs["yi_Hebr"].exemplar_chars.numerals
-        assert numerals == '- ‑ , . % ‰ + 0 1 2 3 4 5 6 7 8 9'
+        assert numerals == '- , . % + 0 1 2 3 4 5 6 7 8 9'
 
 
 def test_LoadScripts():
     for scripts in [LoadScripts(),
                     LoadScripts(None),
                     LoadScripts(DATA_DIR)]:
         scripts = LoadScripts()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gflanguages-0.8.9/tests/test_parsable.py` & `gflanguages-5.0.4/tests/test_parsable.py`

 * *Files identical despite different names*

