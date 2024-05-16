# Comparing `tmp/buildz-0.5.4.tar.gz` & `tmp/buildz-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.5.4.tar", last modified: Wed May  8 03:06:37 2024, max compression
+gzip compressed data, was "buildz-0.5.5.tar", last modified: Wed May 15 18:21:32 2024, max compression
```

## Comparing `buildz-0.5.4.tar` & `buildz-0.5.5.tar`

### file list

```diff
@@ -1,161 +1,163 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.033407 buildz-0.5.4/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.4/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2823 2024-05-08 03:06:37.033407 buildz-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.924044 buildz-0.5.4/buildz/
--rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.4/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.4/buildz/__main__.py
--rw-rw-rw-   0        0        0     2944 2024-05-07 11:40:11.000000 buildz-0.5.4/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.4/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.4/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.4/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.4/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.4/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.4/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.4/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.4/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.4/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.4/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.4/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.4/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.4/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.4/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.4/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.4/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.4/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.4/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.4/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.4/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/fz/
--rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.5.4/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.4/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      629 2024-05-03 05:05:00.000000 buildz-0.5.4/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.4/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.4/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-25 13:59:49.000000 buildz-0.5.4/buildz/ioc/base.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.4/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.970921 buildz-0.5.4/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     2390 2024-04-25 13:41:08.000000 buildz-0.5.4/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.4/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.4/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.986537 buildz-0.5.4/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.4/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1243 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.002166 buildz-0.5.4/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/deal_lists.js
--rw-rw-rw-   0        0        0     2197 2024-04-23 19:17:12.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/xfile_defaults.js
--rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.4/buildz/ioc/ioc_deal/conf/xfile_lists.js
--rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/deal.py
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.4/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0     1038 2024-05-06 14:06:01.000000 buildz-0.5.4/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      954 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0      932 2024-05-07 08:29:26.000000 buildz-0.5.4/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1090 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1021 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     6134 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1087 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.5.4/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.4/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.4/buildz/ioc/ioc_deal/xfile.py
--rw-rw-rw-   0        0        0     1958 2024-04-23 08:58:52.000000 buildz-0.5.4/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.002166 buildz-0.5.4/buildz/tz/
--rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.4/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.4/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.002166 buildz-0.5.4/buildz/xf/
--rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.4/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.4/buildz/xf/__main__.py
--rw-rw-rw-   0        0        0      960 2024-05-03 05:07:16.000000 buildz-0.5.4/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.017784 buildz-0.5.4/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.4/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.4/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.017784 buildz-0.5.4/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.4/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.4/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.4/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.4/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.4/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.4/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.4/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.4/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.4/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.4/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.4/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.4/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.4/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.4/buildz/xf/loader/pos.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.017784 buildz-0.5.4/buildz/xf/loaderz/
--rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.4/buildz/xf/loaderz/base.py
--rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.4/buildz/xf/loaderz/buffer.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.033407 buildz-0.5.4/buildz/xf/loaderz/deal/
--rw-rw-rw-   0        0        0      963 2024-04-26 07:40:02.000000 buildz-0.5.4/buildz/xf/loaderz/deal/listz.py
--rw-rw-rw-   0        0        0     2056 2024-05-07 13:50:27.000000 buildz-0.5.4/buildz/xf/loaderz/deal/lr.py
--rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.4/buildz/xf/loaderz/deal/lrval.py
--rw-rw-rw-   0        0        0     1143 2024-04-26 07:39:58.000000 buildz-0.5.4/buildz/xf/loaderz/deal/mapz.py
--rw-rw-rw-   0        0        0      740 2024-04-26 07:40:46.000000 buildz-0.5.4/buildz/xf/loaderz/deal/nextz.py
--rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.4/buildz/xf/loaderz/deal/reval.py
--rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.4/buildz/xf/loaderz/deal/setz.py
--rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.4/buildz/xf/loaderz/deal/spc.py
--rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.4/buildz/xf/loaderz/deal/spt.py
--rw-rw-rw-   0        0        0     3313 2024-05-07 12:00:45.000000 buildz-0.5.4/buildz/xf/loaderz/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.4/buildz/xf/loaderz/exp.py
--rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.4/buildz/xf/loaderz/item.py
--rw-rw-rw-   0        0        0     3515 2024-04-26 08:09:20.000000 buildz-0.5.4/buildz/xf/loaderz/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.4/buildz/xf/loaderz/pos.py
--rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.4/buildz/xf/loaderz/test.py
--rw-rw-rw-   0        0        0       97 2024-04-26 07:42:38.000000 buildz-0.5.4/buildz/xf/loaderz/test1.py
--rw-rw-rw-   0        0        0     2600 2024-05-06 14:14:08.000000 buildz-0.5.4/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.4/buildz/xf/read.py
--rw-rw-rw-   0        0        0     2746 2024-05-07 11:58:30.000000 buildz-0.5.4/buildz/xf/readz.py
--rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.4/buildz/xf/stack.py
--rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.4/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.033407 buildz-0.5.4/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.4/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.4/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:37.033407 buildz-0.5.4/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.4/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.4/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.4/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.4/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.4/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.4/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.4/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.4/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:36.955298 buildz-0.5.4/buildz.egg-info/
--rw-rw-rw-   0        0        0     2823 2024-05-08 03:06:36.000000 buildz-0.5.4/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3751 2024-05-08 03:06:36.000000 buildz-0.5.4/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:06:36.000000 buildz-0.5.4/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 03:06:36.000000 buildz-0.5.4/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 03:06:37.033407 buildz-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0      836 2024-05-08 03:04:03.000000 buildz-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.778694 buildz-0.5.5/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2823 2024-05-15 18:21:32.778694 buildz-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.211562 buildz-0.5.5/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.5/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.5/buildz/__main__.py
+-rw-rw-rw-   0        0        0     2944 2024-05-07 11:40:11.000000 buildz-0.5.5/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.227181 buildz-0.5.5/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.233766 buildz-0.5.5/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.5/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.5/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.247717 buildz-0.5.5/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.5/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.5/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.251663 buildz-0.5.5/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.291259 buildz-0.5.5/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.5/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.5/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.5/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.5/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.5/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.338042 buildz-0.5.5/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.5/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.5/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.5/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.5/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.5/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.5/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.353664 buildz-0.5.5/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.5/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.5/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.5/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.370150 buildz-0.5.5/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.5/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.5/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.385664 buildz-0.5.5/buildz/fz/
+-rw-rw-rw-   0        0        0      243 2024-05-11 09:00:08.000000 buildz-0.5.5/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.5/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      795 2024-05-11 08:59:27.000000 buildz-0.5.5/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.5/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.401307 buildz-0.5.5/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.5/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-25 13:59:49.000000 buildz-0.5.5/buildz/ioc/base.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.5/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.406162 buildz-0.5.5/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     2390 2024-04-25 13:41:08.000000 buildz-0.5.5/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.5/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.5/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.449205 buildz-0.5.5/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.5/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1243 2024-04-25 13:54:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.464959 buildz-0.5.5/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/deal_lists.js
+-rw-rw-rw-   0        0        0     2341 2024-05-08 19:55:33.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      421 2024-05-08 19:53:08.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/iocf_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      615 2024-05-13 09:04:25.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/xfile_defaults.js
+-rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.5/buildz/ioc/ioc_deal/conf/xfile_lists.js
+-rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/deal.py
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.5/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0     1038 2024-05-06 14:06:01.000000 buildz-0.5.5/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      954 2024-04-25 13:54:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0     1798 2024-05-09 01:32:23.000000 buildz-0.5.5/buildz/ioc/ioc_deal/iocf.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 08:29:26.000000 buildz-0.5.5/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1090 2024-04-25 13:54:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1022 2024-05-13 09:26:45.000000 buildz-0.5.5/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     6322 2024-05-15 08:22:26.000000 buildz-0.5.5/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1255 2024-05-14 03:17:05.000000 buildz-0.5.5/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      702 2024-05-13 09:30:29.000000 buildz-0.5.5/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.5/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.5/buildz/ioc/ioc_deal/xfile.py
+-rw-rw-rw-   0        0        0     2295 2024-05-13 02:27:31.000000 buildz-0.5.5/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.496221 buildz-0.5.5/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.5/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.5/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.527454 buildz-0.5.5/buildz/xf/
+-rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.5/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.5/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0     1082 2024-05-13 07:36:04.000000 buildz-0.5.5/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.558711 buildz-0.5.5/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.5/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.5/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.605969 buildz-0.5.5/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.5/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.5/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.5/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.5/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.5/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.5/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.5/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.5/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.5/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.5/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.5/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.5/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.5/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.5/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.637025 buildz-0.5.5/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.5/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.5/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.731814 buildz-0.5.5/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      963 2024-04-26 07:40:02.000000 buildz-0.5.5/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     2056 2024-05-07 13:50:27.000000 buildz-0.5.5/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.5/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0     1143 2024-04-26 07:39:58.000000 buildz-0.5.5/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      740 2024-04-26 07:40:46.000000 buildz-0.5.5/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.5/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.5/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.5/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.5/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     3295 2024-05-14 07:15:35.000000 buildz-0.5.5/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.5/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.5/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     3517 2024-05-14 07:12:19.000000 buildz-0.5.5/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.5/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.5/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0       97 2024-04-26 07:42:38.000000 buildz-0.5.5/buildz/xf/loaderz/test1.py
+-rw-rw-rw-   0        0        0     2940 2024-05-15 09:18:22.000000 buildz-0.5.5/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.5/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2746 2024-05-07 11:58:30.000000 buildz-0.5.5/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.5/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.5/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.747447 buildz-0.5.5/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.5/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.5/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.778694 buildz-0.5.5/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.5/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.5/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.5/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.5/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.5/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.5/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.5/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.5/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:21:32.211562 buildz-0.5.5/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2823 2024-05-15 18:21:32.000000 buildz-0.5.5/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3818 2024-05-15 18:21:32.000000 buildz-0.5.5/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:21:32.000000 buildz-0.5.5/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 18:21:32.000000 buildz-0.5.5/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 18:21:32.778694 buildz-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-05-15 18:20:54.000000 buildz-0.5.5/setup.py
```

### Comparing `buildz-0.5.4/LICENSE` & `buildz-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/PKG-INFO` & `buildz-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.4
+Version: 0.5.5
 Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.4/README.md` & `buildz-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/argx.py` & `buildz-0.5.5/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/ioc/deal.py` & `buildz-0.5.5/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/ioc/help.py` & `buildz-0.5.5/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/myers/deal.py` & `buildz-0.5.5/buildz/demo/myers/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/res/conf/main.js` & `buildz-0.5.5/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/res/help/ioc.js` & `buildz-0.5.5/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/res/help/myers.js` & `buildz-0.5.5/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/res/help/search.js` & `buildz-0.5.5/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/res/help/xf.js` & `buildz-0.5.5/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/res/test.js` & `buildz-0.5.5/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/search/deal.py` & `buildz-0.5.5/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/demo/test.py` & `buildz-0.5.5/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/fz/dirz.py` & `buildz-0.5.5/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/fz/fio.py` & `buildz-0.5.5/buildz/fz/fio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #coding=utf-8
-
+import os
 """
 读写文件再简化
 """
 def fread(fp, mode='rb'):
     with open(fp, mode) as f:
         return f.read()
 
@@ -28,8 +28,18 @@
 write = fwrite
 def fwrites(cts, fp, mode = 'wb'):
     with open(fp, mode) as f:
         for ct in cts:
             f.write(ct)
 
 pass
-writes = fwrites
+writes = fwrites
+
+def makefdir(fp):
+    fp = os.path.abspath(fp)
+    dp = os.path.dirname(fp)
+    if os.path.isdir(dp):
+        return
+    os.makedirs(dp)
+
+pass
+
```

### Comparing `buildz-0.5.4/buildz/fz/lsf.py` & `buildz-0.5.5/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc/base.py` & `buildz-0.5.5/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc/conf.py` & `buildz-0.5.5/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc/confs.py` & `buildz-0.5.5/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/base.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/call.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/calls.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.5.5/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -58,9 +58,13 @@
         note: xf配置文件读取,
         build: buildz.ioc.ioc_deal.xfile.XfileDeal,
         aliases: [xf]
     }, {
         type: deal,
         note: 扩展的自定义deal方法,
         build: buildz.ioc.ioc_deal.deal.DealDeal
+    }, {
+        type: iocf,
+        note: 加配置文件,
+        build: buildz.ioc.ioc_deal.iocf.IOCFObjectDeal
     }]
 }
```

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.5.5/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/deal.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/env.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/join.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/list.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/map.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/map.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,11 +25,11 @@
     def init(self, fp_lists=None, fp_defaults=None):
         super().init("MapDeal", fp_lists, fp_defaults, join(dp, "conf", "map_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         conf = edata.conf
         data = self.fill(data)
         maps = xf.g(data, data={})
-        rst = {k:self.get_obj(map[k], conf, edata.src, edata.info) for k in maps}
+        rst = {k:self.get_obj(maps[k], conf, edata.src, edata.info) for k in maps}
         return rst
 
 pass
```

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/obj.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/obj.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,24 +98,26 @@
         single = xf.g(data, single=None)
         if id is None:
             single = 0
         if single is None:
             single = 1
         ids = None
         if single or cid is not None:
-            if single:
-                ids = [sid, id]
+            if cid is not None:
+                ids = [sid, 'local_id', id, cid]
             else:
-                ids = [sid, id, cid]
+                ids = [sid, 'single', id]
         if ids is not None:
             obj = xf.gets(self.singles, ids)
             if obj is not None:
                 #raise IOCError(f"null for {ids}")
                 return obj
         source = xf.g(data, source=0)
+        if source == 0:
+            raise Exception(f"define object without 'source' key, {data}")
         fc = xf.get(self.sources, source, None)
         if fc is None:
             fc = pyz.load(source)
             self.sources[source]=fc
         cst = xf.g(data, construct = None)
         if cst is None:
             _args = xf.g(data, args = [])
@@ -127,14 +129,15 @@
         args = [self.get_obj(v, conf) for v in args]
         maps = {k:self.get_obj(maps[k], conf) for k in maps}
         obj = fc(*args, **maps)
         if ids is not None:
             xf.sets(self.singles, ids, obj)
         prev_call = xf.g(data, prev_call=None)
         if prev_call is not None:
+            # TODO: 这边info透传好像会有问题
             self.get_obj(prev_call, conf, obj, edata.info)
         sets = xf.g(data, sets=[])
         for kv in sets:
             kv = self.fmt_set(kv)
             k = kv['key']
             v = kv['data']
             v = self.get_obj(v, conf, obj, edata.info)
```

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/ref.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/ref.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,12 +24,14 @@
     def init(self, fp_lists=None, fp_defaults=None):
         super().init("RefDeal", fp_lists, fp_defaults, join(dp, "conf", "ref_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         data = self.fill(data)
         key = data['key']
         info = xf.g(data, info=None)
-        if info is not None:
-            info = self.get_obj(info, src = edata.src)
+        if info is not None and type(info)==dict:
+            #info = {k:self.get_obj(info, edata.conf, src = edata.src) for k in info}
+            info = {'type':'map', 'data':info}
+            info = self.get_obj(info, edata.conf, src = edata.src)
         return edata.conf.get_obj(key, info = info, src = edata.src)
 
 pass
```

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/val.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/var.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/ioc/ioc_deal/xfile.py` & `buildz-0.5.5/buildz/ioc/ioc_deal/xfile.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/pyz.py` & `buildz-0.5.5/buildz/pyz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 
 import sys
 import os
+def test_current(fp, up = 1):
+    """
+        将当前目录的上{up}层目录加入sys.path，这样可以在同层写测试代码，但是import还是要当在上{up}层做import
+    """
+    dp = os.path.dirname(os.path.abspath(fp))
+    for i in range(up):
+        dp = os.path.dirname(dp)
+    sys.path.insert(0, dp)
+
+pass
 def load(md, fc = None):
     """
         import object(whether module or others) from md(or md.fc)
         exp:
             load("buildz.xf") = package xf
             load("buildz.xf", "loads") = function loads from package buildz.xf
             load("buildz.xf.loads") = function loads from package buildz.xf
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `buildz-0.5.4/buildz/tz/myers_diff.py` & `buildz-0.5.5/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/file.py` & `buildz-0.5.5/buildz/xf/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #coding=utf-8
-
+import os
 coding="utf-8"
 def bread(filepath):
+    if type(filepath) not in [str, bytes, os.PathLike]:
+        raise Exception(f"error filepath: {filepath}")
     with open(filepath, 'rb') as file:
         s = file.read()
     return s
 
 pass
 def decode(s, coding = 'utf-8'):
     coding = coding.lower()
```

### Comparing `buildz-0.5.4/buildz/xf/loader/base.py` & `buildz-0.5.5/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/buffer.py` & `buildz-0.5.5/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/listz.py` & `buildz-0.5.5/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/lr.py` & `buildz-0.5.5/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/lrval.py` & `buildz-0.5.5/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/mapz.py` & `buildz-0.5.5/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/nextz.py` & `buildz-0.5.5/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/reval.py` & `buildz-0.5.5/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/setz.py` & `buildz-0.5.5/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/spt.py` & `buildz-0.5.5/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/deal/strz.py` & `buildz-0.5.5/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/item.py` & `buildz-0.5.5/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/mg.py` & `buildz-0.5.5/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loader/pos.py` & `buildz-0.5.5/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/base.py` & `buildz-0.5.5/buildz/xf/loaderz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/buffer.py` & `buildz-0.5.5/buildz/xf/loaderz/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/deal/listz.py` & `buildz-0.5.5/buildz/xf/loaderz/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/deal/lr.py` & `buildz-0.5.5/buildz/xf/loaderz/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/deal/lrval.py` & `buildz-0.5.5/buildz/xf/loaderz/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/deal/mapz.py` & `buildz-0.5.5/buildz/xf/loaderz/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/deal/nextz.py` & `buildz-0.5.5/buildz/xf/loaderz/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/deal/reval.py` & `buildz-0.5.5/buildz/xf/loaderz/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/deal/spt.py` & `buildz-0.5.5/buildz/xf/loaderz/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/deal/strz.py` & `buildz-0.5.5/buildz/xf/loaderz/deal/strz.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         return outs
     def deal(self, buffer, rst, mg):
         cl = buffer.read(self.ll)
         if cl != self.left:
             return False
         rm = buffer.full().strip()
         buffer.clean2read(self.ll)
-        if len(rm)>0 and not self.note:
+        if len(rm)>0:
             if not self.note:
                 print("left:", self.left, rm)
                 print(f"rst: [{rst}]")
                 raise Exception(f"unexcept char before string: {rm}")
             else:
                 rst.append(item.Item(rm, type = "", is_val = 0))
         tmp = cl[:0]
```

### Comparing `buildz-0.5.4/buildz/xf/loaderz/item.py` & `buildz-0.5.5/buildz/xf/loaderz/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/mg.py` & `buildz-0.5.5/buildz/xf/loaderz/mg.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,107 +114,107 @@
 00000710: 0a20 2020 2020 2020 2020 2020 2072 7374  .            rst
 00000720: 203d 2064 6561 6c2e 6275 696c 6428 6f62   = deal.build(ob
 00000730: 6a29 0d0a 2020 2020 2020 2020 2020 2020  j)..            
 00000740: 6966 2072 7374 2069 7320 6e6f 7420 4e6f  if rst is not No
 00000750: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
 00000760: 2020 2020 2072 6574 7572 6e20 7273 740d       return rst.
 00000770: 0a20 2020 2020 2020 2072 6169 7365 2045  .        raise E
-00000780: 7863 6570 7469 6f6e 2822 756e 7370 7420  xception("unspt 
-00000790: 6465 616c 2074 7970 653a 222b 5f74 7970  deal type:"+_typ
-000007a0: 6529 0d0a 2020 2020 6465 6620 6465 616c  e)..    def deal
-000007b0: 2873 656c 662c 2062 7566 6665 722c 2061  (self, buffer, a
-000007c0: 7272 293a 0d0a 2020 2020 2020 2020 6320  rr):..        c 
-000007d0: 3d20 6275 6666 6572 2e72 6561 6428 290d  = buffer.read().
-000007e0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-000007f0: 6329 3d3d 3020 616e 6420 6275 6666 6572  c)==0 and buffer
-00000800: 2e73 697a 6528 293d 3d30 3a0d 0a20 2020  .size()==0:..   
-00000810: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000820: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
-00000830: 6561 6c73 203d 2073 656c 662e 6765 745f  eals = self.get_
-00000840: 6465 616c 7328 6329 0d0a 2020 2020 2020  deals(c)..      
-00000850: 2020 6669 6e64 203d 2046 616c 7365 0d0a    find = False..
-00000860: 2020 2020 2020 2020 666f 7220 6465 616c          for deal
-00000870: 2069 6e20 6465 616c 733a 0d0a 2020 2020   in deals:..    
-00000880: 2020 2020 2020 2020 6966 2064 6561 6c2e          if deal.
-00000890: 6465 616c 2862 7566 6665 722c 2061 7272  deal(buffer, arr
-000008a0: 2c20 7365 6c66 293a 0d0a 2020 2020 2020  , self):..      
-000008b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000008c0: 2054 7275 650d 0a20 2020 2020 2020 2064   True..        d
-000008d0: 6561 6c73 203d 2073 656c 662e 6465 6661  eals = self.defa
-000008e0: 756c 745f 6465 616c 7328 290d 0a20 2020  ult_deals()..   
-000008f0: 2020 2020 2066 6f72 2064 6561 6c20 696e       for deal in
-00000900: 2064 6561 6c73 3a0d 0a20 2020 2020 2020   deals:..       
-00000910: 2020 2020 2069 6620 6465 616c 2e64 6561       if deal.dea
-00000920: 6c28 6275 6666 6572 2c20 6172 722c 2073  l(buffer, arr, s
-00000930: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-00000940: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00000950: 7565 0d0a 2020 2020 2020 2020 7265 7475  ue..        retu
-00000960: 726e 2046 616c 7365 0d0a 2020 2020 6465  rn False..    de
-00000970: 6620 6275 696c 645f 6172 7228 7365 6c66  f build_arr(self
-00000980: 2c20 5f61 7272 293a 0d0a 2020 2020 2020  , _arr):..      
-00000990: 2020 6474 7320 3d20 5b5d 0d0a 2020 2020    dts = []..    
-000009a0: 2020 2020 666f 7220 6b20 696e 205f 6172      for k in _ar
-000009b0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-000009c0: 5f6b 203d 2073 656c 662e 6275 696c 6428  _k = self.build(
-000009d0: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
-000009e0: 6966 2069 7465 6d2e 6973 5f6e 756c 6c28  if item.is_null(
-000009f0: 5f6b 293a 0d0a 2020 2020 2020 2020 2020  _k):..          
-00000a00: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00000a10: 2020 2020 2020 2020 2020 2020 6474 732e              dts.
-00000a20: 6170 7065 6e64 285f 6b29 0d0a 2020 2020  append(_k)..    
-00000a30: 2020 2020 7265 7475 726e 2064 7473 0d0a      return dts..
-00000a40: 2020 2020 6465 6620 6c6f 6164 2873 656c      def load(sel
-00000a50: 662c 2062 7566 6665 7229 3a0d 0a20 2020  f, buffer):..   
-00000a60: 2020 2020 2061 7272 203d 205b 5d0d 0a20       arr = [].. 
-00000a70: 2020 2020 2020 2077 6869 6c65 2073 656c         while sel
-00000a80: 662e 6465 616c 2862 7566 6665 722c 2061  f.deal(buffer, a
-00000a90: 7272 293a 0d0a 2020 2020 2020 2020 2020  rr):..          
-00000aa0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-00000ab0: 2361 7272 203d 205b 6b2e 7661 6c20 666f  #arr = [k.val fo
-00000ac0: 7220 6b20 696e 2061 7272 5d0d 0a20 2020  r k in arr]..   
-00000ad0: 2020 2020 2023 7273 7420 3d20 5b5d 0d0a       #rst = []..
-00000ae0: 2020 2020 2020 2020 2320 666f 7220 6b20          # for k 
-00000af0: 696e 2061 7272 3a0d 0a20 2020 2020 2020  in arr:..       
-00000b00: 2023 2020 2020 2069 6620 7479 7065 286b   #     if type(k
-00000b10: 2920 3d3d 2073 656c 662e 7479 7065 3a0d  ) == self.type:.
-00000b20: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-00000b30: 2020 2069 6620 6c65 6e28 6b2e 7374 7269     if len(k.stri
-00000b40: 7028 2929 3d3d 303a 0d0a 2020 2020 2020  p())==0:..      
-00000b50: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-00000b60: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
-00000b70: 2020 2320 2020 2020 7273 742e 6170 7065    #     rst.appe
-00000b80: 6e64 286b 290d 0a20 2020 2020 2020 2061  nd(k)..        a
-00000b90: 7272 203d 2073 656c 662e 6275 696c 645f  rr = self.build_
-00000ba0: 6172 7228 6172 7229 0d0a 2020 2020 2020  arr(arr)..      
-00000bb0: 2020 6f62 6a20 3d20 6974 656d 2e49 7465    obj = item.Ite
-00000bc0: 6d28 6172 722c 2074 7970 6520 3d20 2222  m(arr, type = ""
-00000bd0: 2c20 6973 5f76 616c 203d 2030 290d 0a20  , is_val = 0).. 
-00000be0: 2020 2020 2020 206f 626a 203d 2073 656c         obj = sel
-00000bf0: 662e 6275 696c 6428 6f62 6a29 0d0a 2020  f.build(obj)..  
-00000c00: 2020 2020 2020 2361 7272 203d 2072 7374        #arr = rst
-00000c10: 0d0a 2020 2020 2020 2020 2369 6620 6c65  ..        #if le
-00000c20: 6e28 6172 7229 3d3d 313a 0d0a 2020 2020  n(arr)==1:..    
-00000c30: 2020 2020 2320 2020 2061 7272 203d 2061      #    arr = a
-00000c40: 7272 5b30 5d0d 0a20 2020 2020 2020 2076  rr[0]..        v
-00000c50: 616c 203d 206f 626a 2e76 616c 0d0a 2020  al = obj.val..  
-00000c60: 2020 2020 2020 6966 2074 7970 6528 7661        if type(va
-00000c70: 6c29 3d3d 6c69 7374 2061 6e64 206c 656e  l)==list and len
-00000c80: 2876 616c 293d 3d31 3a0d 0a20 2020 2020  (val)==1:..     
-00000c90: 2020 2020 2020 2076 616c 203d 2076 616c         val = val
-00000ca0: 5b30 5d0d 0a20 2020 2020 2020 2072 6574  [0]..        ret
-00000cb0: 7572 6e20 7661 6c0d 0a20 2020 2064 6566  urn val..    def
-00000cc0: 206c 6f61 6473 2873 656c 662c 2072 6561   loads(self, rea
-00000cd0: 6465 7229 3a0d 0a20 2020 2020 2020 2069  der):..        i
-00000ce0: 6620 7479 7065 2872 6561 6465 7229 203d  f type(reader) =
-00000cf0: 3d20 7365 6c66 2e74 7970 653a 0d0a 2020  = self.type:..  
-00000d00: 2020 2020 2020 2020 2020 2370 7269 6e74            #print
-00000d10: 2866 2274 7279 2073 7472 2c20 7b6c 656e  (f"try str, {len
-00000d20: 2872 6561 6465 7229 7d22 290d 0a20 2020  (reader)}")..   
-00000d30: 2020 2020 2020 2020 2062 7566 6620 3d20           buff = 
-00000d40: 6275 6666 6572 2e53 7472 4275 6666 6572  buffer.StrBuffer
-00000d50: 2872 6561 6465 7229 0d0a 2020 2020 2020  (reader)..      
-00000d60: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00000d70: 2020 2020 2062 7566 6620 3d20 6275 6666       buff = buff
-00000d80: 6572 2e42 7566 6665 7228 7265 6164 6572  er.Buffer(reader
-00000d90: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00000da0: 6e20 7365 6c66 2e6c 6f61 6428 6275 6666  n self.load(buff
-00000db0: 290d 0a0d 0a70 6173 730d 0a              )....pass..
+00000780: 7863 6570 7469 6f6e 2866 2275 6e73 7074  xception(f"unspt
+00000790: 2064 6561 6c20 7479 7065 3a5b 7b6f 626a   deal type:[{obj
+000007a0: 7d5d 2229 0d0a 2020 2020 6465 6620 6465  }]")..    def de
+000007b0: 616c 2873 656c 662c 2062 7566 6665 722c  al(self, buffer,
+000007c0: 2061 7272 293a 0d0a 2020 2020 2020 2020   arr):..        
+000007d0: 6320 3d20 6275 6666 6572 2e72 6561 6428  c = buffer.read(
+000007e0: 290d 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
+000007f0: 6e28 6329 3d3d 3020 616e 6420 6275 6666  n(c)==0 and buff
+00000800: 6572 2e73 697a 6528 293d 3d30 3a0d 0a20  er.size()==0:.. 
+00000810: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000820: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
+00000830: 2064 6561 6c73 203d 2073 656c 662e 6765   deals = self.ge
+00000840: 745f 6465 616c 7328 6329 0d0a 2020 2020  t_deals(c)..    
+00000850: 2020 2020 6669 6e64 203d 2046 616c 7365      find = False
+00000860: 0d0a 2020 2020 2020 2020 666f 7220 6465  ..        for de
+00000870: 616c 2069 6e20 6465 616c 733a 0d0a 2020  al in deals:..  
+00000880: 2020 2020 2020 2020 2020 6966 2064 6561            if dea
+00000890: 6c2e 6465 616c 2862 7566 6665 722c 2061  l.deal(buffer, a
+000008a0: 7272 2c20 7365 6c66 293a 0d0a 2020 2020  rr, self):..    
+000008b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000008c0: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
+000008d0: 2064 6561 6c73 203d 2073 656c 662e 6465   deals = self.de
+000008e0: 6661 756c 745f 6465 616c 7328 290d 0a20  fault_deals().. 
+000008f0: 2020 2020 2020 2066 6f72 2064 6561 6c20         for deal 
+00000900: 696e 2064 6561 6c73 3a0d 0a20 2020 2020  in deals:..     
+00000910: 2020 2020 2020 2069 6620 6465 616c 2e64         if deal.d
+00000920: 6561 6c28 6275 6666 6572 2c20 6172 722c  eal(buffer, arr,
+00000930: 2073 656c 6629 3a0d 0a20 2020 2020 2020   self):..       
+00000940: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000950: 5472 7565 0d0a 2020 2020 2020 2020 7265  True..        re
+00000960: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
+00000970: 6465 6620 6275 696c 645f 6172 7228 7365  def build_arr(se
+00000980: 6c66 2c20 5f61 7272 293a 0d0a 2020 2020  lf, _arr):..    
+00000990: 2020 2020 6474 7320 3d20 5b5d 0d0a 2020      dts = []..  
+000009a0: 2020 2020 2020 666f 7220 6b20 696e 205f        for k in _
+000009b0: 6172 723a 0d0a 2020 2020 2020 2020 2020  arr:..          
+000009c0: 2020 5f6b 203d 2073 656c 662e 6275 696c    _k = self.buil
+000009d0: 6428 6b29 0d0a 2020 2020 2020 2020 2020  d(k)..          
+000009e0: 2020 6966 2069 7465 6d2e 6973 5f6e 756c    if item.is_nul
+000009f0: 6c28 5f6b 293a 0d0a 2020 2020 2020 2020  l(_k):..        
+00000a00: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00000a10: 0d0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
+00000a20: 732e 6170 7065 6e64 285f 6b29 0d0a 2020  s.append(_k)..  
+00000a30: 2020 2020 2020 7265 7475 726e 2064 7473        return dts
+00000a40: 0d0a 2020 2020 6465 6620 6c6f 6164 2873  ..    def load(s
+00000a50: 656c 662c 2062 7566 6665 7229 3a0d 0a20  elf, buffer):.. 
+00000a60: 2020 2020 2020 2061 7272 203d 205b 5d0d         arr = [].
+00000a70: 0a20 2020 2020 2020 2077 6869 6c65 2073  .        while s
+00000a80: 656c 662e 6465 616c 2862 7566 6665 722c  elf.deal(buffer,
+00000a90: 2061 7272 293a 0d0a 2020 2020 2020 2020   arr):..        
+00000aa0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
+00000ab0: 2020 2361 7272 203d 205b 6b2e 7661 6c20    #arr = [k.val 
+00000ac0: 666f 7220 6b20 696e 2061 7272 5d0d 0a20  for k in arr].. 
+00000ad0: 2020 2020 2020 2023 7273 7420 3d20 5b5d         #rst = []
+00000ae0: 0d0a 2020 2020 2020 2020 2320 666f 7220  ..        # for 
+00000af0: 6b20 696e 2061 7272 3a0d 0a20 2020 2020  k in arr:..     
+00000b00: 2020 2023 2020 2020 2069 6620 7479 7065     #     if type
+00000b10: 286b 2920 3d3d 2073 656c 662e 7479 7065  (k) == self.type
+00000b20: 3a0d 0a20 2020 2020 2020 2023 2020 2020  :..        #    
+00000b30: 2020 2020 2069 6620 6c65 6e28 6b2e 7374       if len(k.st
+00000b40: 7269 7028 2929 3d3d 303a 0d0a 2020 2020  rip())==0:..    
+00000b50: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+00000b60: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
+00000b70: 2020 2020 2320 2020 2020 7273 742e 6170      #     rst.ap
+00000b80: 7065 6e64 286b 290d 0a20 2020 2020 2020  pend(k)..       
+00000b90: 2061 7272 203d 2073 656c 662e 6275 696c   arr = self.buil
+00000ba0: 645f 6172 7228 6172 7229 0d0a 2020 2020  d_arr(arr)..    
+00000bb0: 2020 2020 6f62 6a20 3d20 6974 656d 2e49      obj = item.I
+00000bc0: 7465 6d28 6172 722c 2074 7970 6520 3d20  tem(arr, type = 
+00000bd0: 2222 2c20 6973 5f76 616c 203d 2030 290d  "", is_val = 0).
+00000be0: 0a20 2020 2020 2020 206f 626a 203d 2073  .        obj = s
+00000bf0: 656c 662e 6275 696c 6428 6f62 6a29 0d0a  elf.build(obj)..
+00000c00: 2020 2020 2020 2020 2361 7272 203d 2072          #arr = r
+00000c10: 7374 0d0a 2020 2020 2020 2020 2369 6620  st..        #if 
+00000c20: 6c65 6e28 6172 7229 3d3d 313a 0d0a 2020  len(arr)==1:..  
+00000c30: 2020 2020 2020 2320 2020 2061 7272 203d        #    arr =
+00000c40: 2061 7272 5b30 5d0d 0a20 2020 2020 2020   arr[0]..       
+00000c50: 2076 616c 203d 206f 626a 2e76 616c 0d0a   val = obj.val..
+00000c60: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00000c70: 7661 6c29 3d3d 6c69 7374 2061 6e64 206c  val)==list and l
+00000c80: 656e 2876 616c 293d 3d31 3a0d 0a20 2020  en(val)==1:..   
+00000c90: 2020 2020 2020 2020 2076 616c 203d 2076           val = v
+00000ca0: 616c 5b30 5d0d 0a20 2020 2020 2020 2072  al[0]..        r
+00000cb0: 6574 7572 6e20 7661 6c0d 0a20 2020 2064  eturn val..    d
+00000cc0: 6566 206c 6f61 6473 2873 656c 662c 2072  ef loads(self, r
+00000cd0: 6561 6465 7229 3a0d 0a20 2020 2020 2020  eader):..       
+00000ce0: 2069 6620 7479 7065 2872 6561 6465 7229   if type(reader)
+00000cf0: 203d 3d20 7365 6c66 2e74 7970 653a 0d0a   == self.type:..
+00000d00: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
+00000d10: 6e74 2866 2274 7279 2073 7472 2c20 7b6c  nt(f"try str, {l
+00000d20: 656e 2872 6561 6465 7229 7d22 290d 0a20  en(reader)}").. 
+00000d30: 2020 2020 2020 2020 2020 2062 7566 6620             buff 
+00000d40: 3d20 6275 6666 6572 2e53 7472 4275 6666  = buffer.StrBuff
+00000d50: 6572 2872 6561 6465 7229 0d0a 2020 2020  er(reader)..    
+00000d60: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000d70: 2020 2020 2020 2062 7566 6620 3d20 6275         buff = bu
+00000d80: 6666 6572 2e42 7566 6665 7228 7265 6164  ffer.Buffer(read
+00000d90: 6572 290d 0a20 2020 2020 2020 2072 6574  er)..        ret
+00000da0: 7572 6e20 7365 6c66 2e6c 6f61 6428 6275  urn self.load(bu
+00000db0: 6666 290d 0a0d 0a70 6173 730d 0a         ff)....pass..
```

### Comparing `buildz-0.5.4/buildz/xf/loaderz/pos.py` & `buildz-0.5.5/buildz/xf/loaderz/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/loaderz/test.py` & `buildz-0.5.5/buildz/xf/loaderz/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/mapz.py` & `buildz-0.5.5/buildz/xf/mapz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,163 +1,184 @@
 00000000: 0d0a 6465 6620 6765 7428 6f62 6a2c 206b  ..def get(obj, k
 00000010: 6579 2c20 6465 6661 756c 743d 4e6f 6e65  ey, default=None
-00000020: 293a 0d0a 2020 2020 6966 206b 6579 206e  ):..    if key n
-00000030: 6f74 2069 6e20 6f62 6a3a 0d0a 2020 2020  ot in obj:..    
-00000040: 2020 2020 7265 7475 726e 2064 6566 6175      return defau
-00000050: 6c74 0d0a 2020 2020 7265 7475 726e 206f  lt..    return o
-00000060: 626a 5b6b 6579 5d0d 0a0d 0a70 6173 730d  bj[key]....pass.
-00000070: 0a64 6566 2067 6574 6628 6f62 6a2c 206b  .def getf(obj, k
-00000080: 6579 2c20 6663 293a 0d0a 2020 2020 6966  ey, fc):..    if
-00000090: 206b 6579 206e 6f74 2069 6e20 6f62 6a3a   key not in obj:
-000000a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000000b0: 2066 6328 290d 0a20 2020 2072 6574 7572   fc()..    retur
-000000c0: 6e20 6f62 6a5b 6b65 795d 0d0a 0d0a 7061  n obj[key]....pa
-000000d0: 7373 0d0a 6465 6620 6766 6e28 6f62 6a2c  ss..def gfn(obj,
-000000e0: 202a 2a6d 6170 7329 3a0d 0a20 2020 2072   **maps):..    r
-000000f0: 7374 203d 205b 5d0d 0a20 2020 2066 6f72  st = []..    for
-00000100: 206b 2069 6e20 6d61 7073 3a0d 0a20 2020   k in maps:..   
-00000110: 2020 2020 2069 6620 6b20 696e 206f 626a       if k in obj
-00000120: 2061 6e64 206f 626a 5b6b 5d20 6973 206e   and obj[k] is n
-00000130: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00000140: 2020 2020 2020 7620 3d20 6f62 6a5b 6b5d        v = obj[k]
-00000150: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00000160: 0a20 2020 2020 2020 2020 2020 2076 203d  .            v =
-00000170: 206d 6170 735b 6b5d 2829 0d0a 2020 2020   maps[k]()..    
-00000180: 2020 2020 7273 742e 6170 7065 6e64 2876      rst.append(v
-00000190: 290d 0a20 2020 2069 6620 6c65 6e28 7273  )..    if len(rs
-000001a0: 7429 3d3d 313a 0d0a 2020 2020 2020 2020  t)==1:..        
-000001b0: 7273 7420 3d20 7273 745b 305d 0d0a 2020  rst = rst[0]..  
-000001c0: 2020 7265 7475 726e 2072 7374 0d0a 0d0a    return rst....
-000001d0: 7061 7373 0d0a 6465 6620 6766 286f 626a  pass..def gf(obj
-000001e0: 2c20 2a2a 6d61 7073 293a 0d0a 2020 2020  , **maps):..    
-000001f0: 7273 7420 3d20 5b5d 0d0a 2020 2020 666f  rst = []..    fo
-00000200: 7220 6b20 696e 206d 6170 733a 0d0a 2020  r k in maps:..  
-00000210: 2020 2020 2020 6966 206b 2069 6e20 6f62        if k in ob
-00000220: 6a3a 0d0a 2020 2020 2020 2020 2020 2020  j:..            
-00000230: 7620 3d20 6f62 6a5b 6b5d 0d0a 2020 2020  v = obj[k]..    
-00000240: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000250: 2020 2020 2020 2076 203d 206d 6170 735b         v = maps[
-00000260: 6b5d 2829 0d0a 2020 2020 2020 2020 7273  k]()..        rs
-00000270: 742e 6170 7065 6e64 2876 290d 0a20 2020  t.append(v)..   
-00000280: 2069 6620 6c65 6e28 7273 7429 3d3d 313a   if len(rst)==1:
-00000290: 0d0a 2020 2020 2020 2020 7273 7420 3d20  ..        rst = 
-000002a0: 7273 745b 305d 0d0a 2020 2020 7265 7475  rst[0]..    retu
-000002b0: 726e 2072 7374 0d0a 0d0a 7061 7373 0d0a  rn rst....pass..
-000002c0: 6465 6620 6728 6f62 6a2c 202a 2a6d 6170  def g(obj, **map
-000002d0: 7329 3a0d 0a20 2020 2072 7374 203d 205b  s):..    rst = [
-000002e0: 5d0d 0a20 2020 2066 6f72 206b 2069 6e20  ]..    for k in 
-000002f0: 6d61 7073 3a0d 0a20 2020 2020 2020 2076  maps:..        v
-00000300: 203d 206d 6170 735b 6b5d 0d0a 2020 2020   = maps[k]..    
-00000310: 2020 2020 6966 206b 2069 6e20 6f62 6a3a      if k in obj:
-00000320: 0d0a 2020 2020 2020 2020 2020 2020 7620  ..            v 
-00000330: 3d20 6f62 6a5b 6b5d 0d0a 2020 2020 2020  = obj[k]..      
-00000340: 2020 7273 742e 6170 7065 6e64 2876 290d    rst.append(v).
-00000350: 0a20 2020 2069 6620 6c65 6e28 7273 7429  .    if len(rst)
-00000360: 3d3d 313a 0d0a 2020 2020 2020 2020 7273  ==1:..        rs
-00000370: 7420 3d20 7273 745b 305d 0d0a 2020 2020  t = rst[0]..    
-00000380: 7265 7475 726e 2072 7374 0d0a 0d0a 7061  return rst....pa
-00000390: 7373 0d0a 6465 6620 7328 6f62 6a2c 202a  ss..def s(obj, *
-000003a0: 2a6d 6170 7329 3a0d 0a20 2020 2066 6f72  *maps):..    for
-000003b0: 206b 2069 6e20 6d61 7073 3a0d 0a20 2020   k in maps:..   
-000003c0: 2020 2020 2076 203d 206d 6170 735b 6b5d       v = maps[k]
-000003d0: 0d0a 2020 2020 2020 2020 6f62 6a5b 6b5d  ..        obj[k]
-000003e0: 203d 2076 0d0a 0d0a 7061 7373 0d0a 6465   = v....pass..de
-000003f0: 6620 7365 7473 286d 6170 732c 206b 6579  f sets(maps, key
-00000400: 732c 2076 616c 293a 0d0a 2020 2020 6966  s, val):..    if
-00000410: 2074 7970 6528 6b65 7973 2920 213d 206c   type(keys) != l
-00000420: 6973 743a 0d0a 2020 2020 2020 2020 6b65  ist:..        ke
-00000430: 7973 203d 205b 6b65 7973 5d0d 0a20 2020  ys = [keys]..   
-00000440: 2066 6f72 206b 6579 2069 6e20 6b65 7973   for key in keys
-00000450: 5b3a 2d31 5d3a 0d0a 2020 2020 2020 2020  [:-1]:..        
-00000460: 6966 206b 6579 206e 6f74 2069 6e20 6d61  if key not in ma
-00000470: 7073 3a0d 0a20 2020 2020 2020 2020 2020  ps:..           
-00000480: 206d 6170 735b 6b65 795d 203d 207b 7d0d   maps[key] = {}.
-00000490: 0a20 2020 2020 2020 206d 6170 7320 3d20  .        maps = 
-000004a0: 6d61 7073 5b6b 6579 5d0d 0a20 2020 206d  maps[key]..    m
-000004b0: 6170 735b 6b65 7973 5b2d 315d 5d20 3d20  aps[keys[-1]] = 
-000004c0: 7661 6c0d 0a0d 0a70 6173 730d 0a64 6566  val....pass..def
-000004d0: 2067 6574 7328 6d61 7073 2c20 6b65 7973   gets(maps, keys
-000004e0: 2c20 6465 6661 756c 7420 3d20 4e6f 6e65  , default = None
-000004f0: 293a 0d0a 2020 2020 6966 2074 7970 6528  ):..    if type(
-00000500: 6b65 7973 2920 213d 206c 6973 743a 0d0a  keys) != list:..
-00000510: 2020 2020 2020 2020 6b65 7973 203d 205b          keys = [
-00000520: 6b65 7973 5d0d 0a20 2020 2066 6f72 206b  keys]..    for k
-00000530: 6579 2069 6e20 6b65 7973 3a0d 0a20 2020  ey in keys:..   
-00000540: 2020 2020 2069 6620 6b65 7920 6e6f 7420       if key not 
-00000550: 696e 206d 6170 733a 0d0a 2020 2020 2020  in maps:..      
-00000560: 2020 2020 2020 7265 7475 726e 2064 6566        return def
-00000570: 6175 6c74 0d0a 2020 2020 2020 2020 6d61  ault..        ma
-00000580: 7073 203d 206d 6170 735b 6b65 795d 0d0a  ps = maps[key]..
-00000590: 2020 2020 7265 7475 726e 206d 6170 730d      return maps.
-000005a0: 0a0d 0a70 6173 730d 0a64 6566 2072 656d  ...pass..def rem
-000005b0: 6f76 6573 286d 6170 732c 206b 6579 7329  oves(maps, keys)
-000005c0: 3a0d 0a20 2020 2069 6620 7479 7065 286b  :..    if type(k
-000005d0: 6579 7329 2021 3d20 6c69 7374 3a0d 0a20  eys) != list:.. 
-000005e0: 2020 2020 2020 206b 6579 7320 3d20 5b6b         keys = [k
-000005f0: 6579 735d 0d0a 2020 2020 6172 7220 3d20  eys]..    arr = 
-00000600: 5b5d 0d0a 2020 2020 666f 7220 6b65 7920  []..    for key 
-00000610: 696e 206b 6579 733a 0d0a 2020 2020 2020  in keys:..      
-00000620: 2020 6966 206b 6579 206e 6f74 2069 6e20    if key not in 
-00000630: 6d61 7073 3a0d 0a20 2020 2020 2020 2020  maps:..         
-00000640: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
-00000650: 2020 6172 722e 6170 7065 6e64 285b 6d61    arr.append([ma
-00000660: 7073 2c20 6b65 795d 290d 0a20 2020 2020  ps, key])..     
-00000670: 2020 206d 6170 7320 3d20 6d61 7073 5b6b     maps = maps[k
-00000680: 6579 5d0d 0a20 2020 2061 7272 2e72 6576  ey]..    arr.rev
-00000690: 6572 7365 2829 0d0a 2020 2020 6669 7273  erse()..    firs
-000006a0: 743d 310d 0a20 2020 2066 6f72 206d 6170  t=1..    for map
-000006b0: 732c 6b65 7920 696e 2061 7272 3a0d 0a20  s,key in arr:.. 
-000006c0: 2020 2020 2020 2069 6620 6669 7273 7420         if first 
-000006d0: 6f72 206c 656e 286d 6170 735b 6b65 795d  or len(maps[key]
-000006e0: 293d 3d30 3a0d 0a20 2020 2020 2020 2020  )==0:..         
-000006f0: 2020 2064 656c 206d 6170 735b 6b65 795d     del maps[key]
-00000700: 0d0a 2020 2020 2020 2020 6669 7273 743d  ..        first=
-00000710: 300d 0a20 2020 2072 6574 7572 6e20 4e6f  0..    return No
-00000720: 6e65 0d0a 0d0a 7061 7373 0d0a 6465 6620  ne....pass..def 
-00000730: 6c32 6d28 6172 722c 202a 2a6d 6170 7329  l2m(arr, **maps)
-00000740: 3a0d 0a20 2020 2072 7374 203d 207b 7d0d  :..    rst = {}.
-00000750: 0a20 2020 2069 203d 2030 0d0a 2020 2020  .    i = 0..    
-00000760: 666f 7220 6b20 696e 206d 6170 733a 0d0a  for k in maps:..
-00000770: 2020 2020 2020 2020 6966 2069 3c6c 656e          if i<len
-00000780: 2861 7272 293a 0d0a 2020 2020 2020 2020  (arr):..        
-00000790: 2020 2020 7661 6c20 3d20 6172 725b 695d      val = arr[i]
-000007a0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-000007b0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-000007c0: 203d 206d 6170 735b 6b5d 0d0a 2020 2020   = maps[k]..    
-000007d0: 2020 2020 7273 745b 6b5d 203d 2076 616c      rst[k] = val
-000007e0: 0d0a 2020 2020 2020 2020 692b 3d31 0d0a  ..        i+=1..
-000007f0: 2020 2020 7265 7475 726e 2072 7374 0d0a      return rst..
-00000800: 0d0a 7061 7373 0d0a 0d0a 6465 6620 6465  ..pass....def de
-00000810: 6570 5f75 7064 6174 6528 7461 7267 6574  ep_update(target
-00000820: 2c20 7372 632c 2072 6570 6c61 6365 3d31  , src, replace=1
-00000830: 293a 0d0a 2020 2020 2222 220d 0a20 2020  ):..    """..   
-00000840: 2020 2020 2064 6963 74e6 b7b1 e5b1 82e6       dict.......
-00000850: 9bb4 e696 b0ef bc8c 7372 635b 6b65 795d  ........src[key]
-00000860: e698 af64 6963 74e5 b0b1 e6b7 b1e5 85a5  ...dict.........
-00000870: e69b b4e6 96b0 efbc 8ce5 90a6 e588 993a  ...............:
-00000880: 0d0a 2020 2020 2020 2020 2020 2020 7372  ..            sr
-00000890: 63e6 9c89 e880 8c6d 6170 73e6 b2a1 e69c  c......maps.....
-000008a0: 89e5 b0b1 e69b bfe6 8da2 efbc 8ce5 90a6  ................
-000008b0: e588 99ef bc9a 0d0a 2020 2020 2020 2020  ........        
-000008c0: 2020 2020 2020 2020 7265 706c 6163 653d          replace=
-000008d0: 31e5 b0b1 e69b bfe6 8da2 0d0a 2020 2020  1...........    
-000008e0: 2222 220d 0a20 2020 2066 6f72 206b 2069  """..    for k i
-000008f0: 6e20 7372 633a 0d0a 2020 2020 2020 2020  n src:..        
-00000900: 7661 6c20 3d20 7372 635b 6b5d 0d0a 2020  val = src[k]..  
-00000910: 2020 2020 2020 6966 206b 206e 6f74 2069        if k not i
-00000920: 6e20 7461 7267 6574 3a0d 0a20 2020 2020  n target:..     
-00000930: 2020 2020 2020 2074 6172 6765 745b 6b5d         target[k]
-00000940: 203d 2076 616c 0d0a 2020 2020 2020 2020   = val..        
-00000950: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
-00000960: 2020 2020 2020 6d76 616c 203d 2074 6172        mval = tar
-00000970: 6765 745b 6b5d 0d0a 2020 2020 2020 2020  get[k]..        
-00000980: 6966 2074 7970 6528 6d76 616c 2920 3d3d  if type(mval) ==
-00000990: 2064 6963 7420 616e 6420 7479 7065 2876   dict and type(v
-000009a0: 616c 293d 3d64 6963 743a 0d0a 2020 2020  al)==dict:..    
-000009b0: 2020 2020 2020 2020 6465 6570 5f75 7064          deep_upd
-000009c0: 6174 6528 6d76 616c 2c20 7661 6c2c 2072  ate(mval, val, r
-000009d0: 6570 6c61 6365 290d 0a20 2020 2020 2020  eplace)..       
-000009e0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000009f0: 2020 2020 6966 2072 6570 6c61 6365 3a0d      if replace:.
-00000a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a10: 2074 6172 6765 745b 6b5d 203d 2076 616c   target[k] = val
-00000a20: 0d0a 0d0a 7061 7373                      ....pass
+00000020: 2c20 7365 7420 3d20 4661 6c73 6529 3a0d  , set = False):.
+00000030: 0a20 2020 2069 6620 6b65 7920 6e6f 7420  .    if key not 
+00000040: 696e 206f 626a 3a0d 0a20 2020 2020 2020  in obj:..       
+00000050: 2069 6620 7365 743a 0d0a 2020 2020 2020   if set:..      
+00000060: 2020 2020 2020 6f62 6a5b 6b65 795d 203d        obj[key] =
+00000070: 2064 6566 6175 6c74 0d0a 2020 2020 2020   default..      
+00000080: 2020 7265 7475 726e 2064 6566 6175 6c74    return default
+00000090: 0d0a 2020 2020 7265 7475 726e 206f 626a  ..    return obj
+000000a0: 5b6b 6579 5d0d 0a0d 0a70 6173 730d 0a64  [key]....pass..d
+000000b0: 6566 2067 6574 6628 6f62 6a2c 206b 6579  ef getf(obj, key
+000000c0: 2c20 6663 293a 0d0a 2020 2020 6966 206b  , fc):..    if k
+000000d0: 6579 206e 6f74 2069 6e20 6f62 6a3a 0d0a  ey not in obj:..
+000000e0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000000f0: 6328 290d 0a20 2020 2072 6574 7572 6e20  c()..    return 
+00000100: 6f62 6a5b 6b65 795d 0d0a 0d0a 7061 7373  obj[key]....pass
+00000110: 0d0a 6465 6620 6766 6e28 6f62 6a2c 202a  ..def gfn(obj, *
+00000120: 2a6d 6170 7329 3a0d 0a20 2020 2072 7374  *maps):..    rst
+00000130: 203d 205b 5d0d 0a20 2020 2066 6f72 206b   = []..    for k
+00000140: 2069 6e20 6d61 7073 3a0d 0a20 2020 2020   in maps:..     
+00000150: 2020 2069 6620 6b20 696e 206f 626a 2061     if k in obj a
+00000160: 6e64 206f 626a 5b6b 5d20 6973 206e 6f74  nd obj[k] is not
+00000170: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00000180: 2020 2020 7620 3d20 6f62 6a5b 6b5d 0d0a      v = obj[k]..
+00000190: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000001a0: 2020 2020 2020 2020 2020 2076 203d 206d             v = m
+000001b0: 6170 735b 6b5d 2829 0d0a 2020 2020 2020  aps[k]()..      
+000001c0: 2020 7273 742e 6170 7065 6e64 2876 290d    rst.append(v).
+000001d0: 0a20 2020 2069 6620 6c65 6e28 7273 7429  .    if len(rst)
+000001e0: 3d3d 313a 0d0a 2020 2020 2020 2020 7273  ==1:..        rs
+000001f0: 7420 3d20 7273 745b 305d 0d0a 2020 2020  t = rst[0]..    
+00000200: 7265 7475 726e 2072 7374 0d0a 0d0a 7061  return rst....pa
+00000210: 7373 0d0a 6465 6620 6766 286f 626a 2c20  ss..def gf(obj, 
+00000220: 2a2a 6d61 7073 293a 0d0a 2020 2020 7273  **maps):..    rs
+00000230: 7420 3d20 5b5d 0d0a 2020 2020 666f 7220  t = []..    for 
+00000240: 6b20 696e 206d 6170 733a 0d0a 2020 2020  k in maps:..    
+00000250: 2020 2020 6966 206b 2069 6e20 6f62 6a3a      if k in obj:
+00000260: 0d0a 2020 2020 2020 2020 2020 2020 7620  ..            v 
+00000270: 3d20 6f62 6a5b 6b5d 0d0a 2020 2020 2020  = obj[k]..      
+00000280: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00000290: 2020 2020 2076 203d 206d 6170 735b 6b5d       v = maps[k]
+000002a0: 2829 0d0a 2020 2020 2020 2020 7273 742e  ()..        rst.
+000002b0: 6170 7065 6e64 2876 290d 0a20 2020 2069  append(v)..    i
+000002c0: 6620 6c65 6e28 7273 7429 3d3d 313a 0d0a  f len(rst)==1:..
+000002d0: 2020 2020 2020 2020 7273 7420 3d20 7273          rst = rs
+000002e0: 745b 305d 0d0a 2020 2020 7265 7475 726e  t[0]..    return
+000002f0: 2072 7374 0d0a 0d0a 7061 7373 0d0a 6465   rst....pass..de
+00000300: 6620 6728 6f62 6a2c 202a 2a6d 6170 7329  f g(obj, **maps)
+00000310: 3a0d 0a20 2020 2072 7374 203d 205b 5d0d  :..    rst = [].
+00000320: 0a20 2020 2066 6f72 206b 2069 6e20 6d61  .    for k in ma
+00000330: 7073 3a0d 0a20 2020 2020 2020 2076 203d  ps:..        v =
+00000340: 206d 6170 735b 6b5d 0d0a 2020 2020 2020   maps[k]..      
+00000350: 2020 6966 206b 2069 6e20 6f62 6a3a 0d0a    if k in obj:..
+00000360: 2020 2020 2020 2020 2020 2020 7620 3d20              v = 
+00000370: 6f62 6a5b 6b5d 0d0a 2020 2020 2020 2020  obj[k]..        
+00000380: 7273 742e 6170 7065 6e64 2876 290d 0a20  rst.append(v).. 
+00000390: 2020 2069 6620 6c65 6e28 7273 7429 3d3d     if len(rst)==
+000003a0: 313a 0d0a 2020 2020 2020 2020 7273 7420  1:..        rst 
+000003b0: 3d20 7273 745b 305d 0d0a 2020 2020 7265  = rst[0]..    re
+000003c0: 7475 726e 2072 7374 0d0a 0d0a 7061 7373  turn rst....pass
+000003d0: 0d0a 6465 6620 6773 286f 626a 2c20 2a2a  ..def gs(obj, **
+000003e0: 6d61 7073 293a 0d0a 2020 2020 7273 7420  maps):..    rst 
+000003f0: 3d20 5b5d 0d0a 2020 2020 666f 7220 6b20  = []..    for k 
+00000400: 696e 206d 6170 733a 0d0a 2020 2020 2020  in maps:..      
+00000410: 2020 7620 3d20 6d61 7073 5b6b 5d0d 0a20    v = maps[k].. 
+00000420: 2020 2020 2020 2069 6620 6b20 696e 206f         if k in o
+00000430: 626a 3a0d 0a20 2020 2020 2020 2020 2020  bj:..           
+00000440: 2076 203d 206f 626a 5b6b 5d0d 0a20 2020   v = obj[k]..   
+00000450: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00000460: 2020 2020 2020 2020 6f62 6a5b 6b5d 203d          obj[k] =
+00000470: 2076 0d0a 2020 2020 2020 2020 7273 742e   v..        rst.
+00000480: 6170 7065 6e64 2876 290d 0a20 2020 2069  append(v)..    i
+00000490: 6620 6c65 6e28 7273 7429 3d3d 313a 0d0a  f len(rst)==1:..
+000004a0: 2020 2020 2020 2020 7273 7420 3d20 7273          rst = rs
+000004b0: 745b 305d 0d0a 2020 2020 7265 7475 726e  t[0]..    return
+000004c0: 2072 7374 0d0a 0d0a 7061 7373 0d0a 6465   rst....pass..de
+000004d0: 6620 7328 6f62 6a2c 202a 2a6d 6170 7329  f s(obj, **maps)
+000004e0: 3a0d 0a20 2020 2066 6f72 206b 2069 6e20  :..    for k in 
+000004f0: 6d61 7073 3a0d 0a20 2020 2020 2020 2076  maps:..        v
+00000500: 203d 206d 6170 735b 6b5d 0d0a 2020 2020   = maps[k]..    
+00000510: 2020 2020 6f62 6a5b 6b5d 203d 2076 0d0a      obj[k] = v..
+00000520: 0d0a 7061 7373 0d0a 6465 6620 7365 7473  ..pass..def sets
+00000530: 286d 6170 732c 206b 6579 732c 2076 616c  (maps, keys, val
+00000540: 293a 0d0a 2020 2020 6966 2074 7970 6528  ):..    if type(
+00000550: 6b65 7973 2920 213d 206c 6973 743a 0d0a  keys) != list:..
+00000560: 2020 2020 2020 2020 6b65 7973 203d 205b          keys = [
+00000570: 6b65 7973 5d0d 0a20 2020 2066 6f72 206b  keys]..    for k
+00000580: 6579 2069 6e20 6b65 7973 5b3a 2d31 5d3a  ey in keys[:-1]:
+00000590: 0d0a 2020 2020 2020 2020 6966 206b 6579  ..        if key
+000005a0: 206e 6f74 2069 6e20 6d61 7073 3a0d 0a20   not in maps:.. 
+000005b0: 2020 2020 2020 2020 2020 206d 6170 735b             maps[
+000005c0: 6b65 795d 203d 207b 7d0d 0a20 2020 2020  key] = {}..     
+000005d0: 2020 206d 6170 7320 3d20 6d61 7073 5b6b     maps = maps[k
+000005e0: 6579 5d0d 0a20 2020 206d 6170 735b 6b65  ey]..    maps[ke
+000005f0: 7973 5b2d 315d 5d20 3d20 7661 6c0d 0a0d  ys[-1]] = val...
+00000600: 0a70 6173 730d 0a64 6566 2067 6574 7328  .pass..def gets(
+00000610: 6d61 7073 2c20 6b65 7973 2c20 6465 6661  maps, keys, defa
+00000620: 756c 7420 3d20 4e6f 6e65 293a 0d0a 2020  ult = None):..  
+00000630: 2020 6966 2074 7970 6528 6b65 7973 2920    if type(keys) 
+00000640: 213d 206c 6973 743a 0d0a 2020 2020 2020  != list:..      
+00000650: 2020 6b65 7973 203d 205b 6b65 7973 5d0d    keys = [keys].
+00000660: 0a20 2020 2066 6f72 206b 6579 2069 6e20  .    for key in 
+00000670: 6b65 7973 3a0d 0a20 2020 2020 2020 2069  keys:..        i
+00000680: 6620 6b65 7920 6e6f 7420 696e 206d 6170  f key not in map
+00000690: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000006a0: 7265 7475 726e 2064 6566 6175 6c74 0d0a  return default..
+000006b0: 2020 2020 2020 2020 6d61 7073 203d 206d          maps = m
+000006c0: 6170 735b 6b65 795d 0d0a 2020 2020 7265  aps[key]..    re
+000006d0: 7475 726e 206d 6170 730d 0a0d 0a70 6173  turn maps....pas
+000006e0: 730d 0a64 6566 2072 656d 6f76 6573 286d  s..def removes(m
+000006f0: 6170 732c 206b 6579 7329 3a0d 0a20 2020  aps, keys):..   
+00000700: 2069 6620 7479 7065 286b 6579 7329 2021   if type(keys) !
+00000710: 3d20 6c69 7374 3a0d 0a20 2020 2020 2020  = list:..       
+00000720: 206b 6579 7320 3d20 5b6b 6579 735d 0d0a   keys = [keys]..
+00000730: 2020 2020 6172 7220 3d20 5b5d 0d0a 2020      arr = []..  
+00000740: 2020 666f 7220 6b65 7920 696e 206b 6579    for key in key
+00000750: 733a 0d0a 2020 2020 2020 2020 6966 206b  s:..        if k
+00000760: 6579 206e 6f74 2069 6e20 6d61 7073 3a0d  ey not in maps:.
+00000770: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
+00000780: 616b 0d0a 2020 2020 2020 2020 6172 722e  ak..        arr.
+00000790: 6170 7065 6e64 285b 6d61 7073 2c20 6b65  append([maps, ke
+000007a0: 795d 290d 0a20 2020 2020 2020 206d 6170  y])..        map
+000007b0: 7320 3d20 6d61 7073 5b6b 6579 5d0d 0a20  s = maps[key].. 
+000007c0: 2020 2061 7272 2e72 6576 6572 7365 2829     arr.reverse()
+000007d0: 0d0a 2020 2020 6669 7273 743d 310d 0a20  ..    first=1.. 
+000007e0: 2020 2066 6f72 206d 6170 732c 6b65 7920     for maps,key 
+000007f0: 696e 2061 7272 3a0d 0a20 2020 2020 2020  in arr:..       
+00000800: 2069 6620 6669 7273 7420 6f72 206c 656e   if first or len
+00000810: 286d 6170 735b 6b65 795d 293d 3d30 3a0d  (maps[key])==0:.
+00000820: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+00000830: 206d 6170 735b 6b65 795d 0d0a 2020 2020   maps[key]..    
+00000840: 2020 2020 6669 7273 743d 300d 0a20 2020      first=0..   
+00000850: 2072 6574 7572 6e20 4e6f 6e65 0d0a 0d0a   return None....
+00000860: 7061 7373 0d0a 6465 6620 6c32 6d28 6172  pass..def l2m(ar
+00000870: 722c 202a 2a6d 6170 7329 3a0d 0a20 2020  r, **maps):..   
+00000880: 2072 7374 203d 207b 7d0d 0a20 2020 2069   rst = {}..    i
+00000890: 203d 2030 0d0a 2020 2020 666f 7220 6b20   = 0..    for k 
+000008a0: 696e 206d 6170 733a 0d0a 2020 2020 2020  in maps:..      
+000008b0: 2020 6966 2069 3c6c 656e 2861 7272 293a    if i<len(arr):
+000008c0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+000008d0: 6c20 3d20 6172 725b 695d 0d0a 2020 2020  l = arr[i]..    
+000008e0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000008f0: 2020 2020 2020 2076 616c 203d 206d 6170         val = map
+00000900: 735b 6b5d 0d0a 2020 2020 2020 2020 7273  s[k]..        rs
+00000910: 745b 6b5d 203d 2076 616c 0d0a 2020 2020  t[k] = val..    
+00000920: 2020 2020 692b 3d31 0d0a 2020 2020 7265      i+=1..    re
+00000930: 7475 726e 2072 7374 0d0a 0d0a 7061 7373  turn rst....pass
+00000940: 0d0a 0d0a 6465 6620 6465 6570 5f75 7064  ....def deep_upd
+00000950: 6174 6528 7461 7267 6574 2c20 7372 632c  ate(target, src,
+00000960: 2072 6570 6c61 6365 3d31 293a 0d0a 2020   replace=1):..  
+00000970: 2020 2222 220d 0a20 2020 2020 2020 2064    """..        d
+00000980: 6963 74e6 b7b1 e5b1 82e6 9bb4 e696 b0ef  ict.............
+00000990: bc8c 7372 635b 6b65 795d e698 af64 6963  ..src[key]...dic
+000009a0: 74e5 b0b1 e6b7 b1e5 85a5 e69b b4e6 96b0  t...............
+000009b0: efbc 8ce5 90a6 e588 993a 0d0a 2020 2020  .........:..    
+000009c0: 2020 2020 2020 2020 7372 63e6 9c89 e880          src.....
+000009d0: 8c74 6172 6765 74e6 b2a1 e69c 89e5 b0b1  .target.........
+000009e0: e69b bfe6 8da2 efbc 8ce5 90a6 e588 99ef  ................
+000009f0: bc9a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00000a00: 2020 2020 7265 706c 6163 653d 31e5 b0b1      replace=1...
+00000a10: e69b bfe6 8da2 0d0a 2020 2020 2222 220d  ........    """.
+00000a20: 0a20 2020 2066 6f72 206b 2069 6e20 7372  .    for k in sr
+00000a30: 633a 0d0a 2020 2020 2020 2020 7661 6c20  c:..        val 
+00000a40: 3d20 7372 635b 6b5d 0d0a 2020 2020 2020  = src[k]..      
+00000a50: 2020 6966 206b 206e 6f74 2069 6e20 7461    if k not in ta
+00000a60: 7267 6574 3a0d 0a20 2020 2020 2020 2020  rget:..         
+00000a70: 2020 2074 6172 6765 745b 6b5d 203d 2076     target[k] = v
+00000a80: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+00000a90: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00000aa0: 2020 6d76 616c 203d 2074 6172 6765 745b    mval = target[
+00000ab0: 6b5d 0d0a 2020 2020 2020 2020 6966 2074  k]..        if t
+00000ac0: 7970 6528 6d76 616c 2920 3d3d 2064 6963  ype(mval) == dic
+00000ad0: 7420 616e 6420 7479 7065 2876 616c 293d  t and type(val)=
+00000ae0: 3d64 6963 743a 0d0a 2020 2020 2020 2020  =dict:..        
+00000af0: 2020 2020 6465 6570 5f75 7064 6174 6528      deep_update(
+00000b00: 6d76 616c 2c20 7661 6c2c 2072 6570 6c61  mval, val, repla
+00000b10: 6365 290d 0a20 2020 2020 2020 2065 6c73  ce)..        els
+00000b20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000b30: 6966 2072 6570 6c61 6365 3a0d 0a20 2020  if replace:..   
+00000b40: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00000b50: 6765 745b 6b5d 203d 2076 616c 0d0a 0d0a  get[k] = val....
+00000b60: 7061 7373 0d0a 7570 6461 7465 203d 2064  pass..update = d
+00000b70: 6565 705f 7570 6461 7465 0d0a            eep_update..
```

### Comparing `buildz-0.5.4/buildz/xf/read.py` & `buildz-0.5.5/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/readz.py` & `buildz-0.5.5/buildz/xf/readz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/stack.py` & `buildz-0.5.5/buildz/xf/stack.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/write.py` & `buildz-0.5.5/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/writer/base.py` & `buildz-0.5.5/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/writer/conf.py` & `buildz-0.5.5/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/writer/deal/listz.py` & `buildz-0.5.5/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/writer/deal/mapz.py` & `buildz-0.5.5/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/writer/deal/strz.py` & `buildz-0.5.5/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/writer/itemz.py` & `buildz-0.5.5/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/writer/mg.py` & `buildz-0.5.5/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz/xf/xargs.py` & `buildz-0.5.5/buildz/xf/xargs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.4/buildz.egg-info/PKG-INFO` & `buildz-0.5.5/buildz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.4
+Version: 0.5.5
 Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.4/buildz.egg-info/SOURCES.txt` & `buildz-0.5.5/buildz.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 buildz/ioc/ioc_deal/base.py
 buildz/ioc/ioc_deal/call.py
 buildz/ioc/ioc_deal/calls.py
 buildz/ioc/ioc_deal/deal.py
 buildz/ioc/ioc_deal/demo.py
 buildz/ioc/ioc_deal/env.py
 buildz/ioc/ioc_deal/ioc.py
+buildz/ioc/ioc_deal/iocf.py
 buildz/ioc/ioc_deal/join.py
 buildz/ioc/ioc_deal/list.py
 buildz/ioc/ioc_deal/map.py
 buildz/ioc/ioc_deal/mcall.py
 buildz/ioc/ioc_deal/obj.py
 buildz/ioc/ioc_deal/ovar.py
 buildz/ioc/ioc_deal/ref.py
@@ -61,14 +62,15 @@
 buildz/ioc/ioc_deal/conf/call_lists.js
 buildz/ioc/ioc_deal/conf/calls_defaults.js
 buildz/ioc/ioc_deal/conf/calls_lists.js
 buildz/ioc/ioc_deal/conf/deal_lists.js
 buildz/ioc/ioc_deal/conf/deals.js
 buildz/ioc/ioc_deal/conf/env_lists.js
 buildz/ioc/ioc_deal/conf/ioc_lists.js
+buildz/ioc/ioc_deal/conf/iocf_lists.js
 buildz/ioc/ioc_deal/conf/join_lists.js
 buildz/ioc/ioc_deal/conf/list_lists.js
 buildz/ioc/ioc_deal/conf/map_lists.js
 buildz/ioc/ioc_deal/conf/mcall_defaults.js
 buildz/ioc/ioc_deal/conf/mcall_lists.js
 buildz/ioc/ioc_deal/conf/obj_cst_lists.js
 buildz/ioc/ioc_deal/conf/obj_defaults.js
```

### Comparing `buildz-0.5.4/setup.py` & `buildz-0.5.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.5.4',
+    version = '0.5.5',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

