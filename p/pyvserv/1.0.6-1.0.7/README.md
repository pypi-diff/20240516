# Comparing `tmp/pyvserv-1.0.6.tar.gz` & `tmp/pyvserv-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvserv-1.0.6.tar", last modified: Sat May  4 15:30:18 2024, max compression
+gzip compressed data, was "pyvserv-1.0.7.tar", last modified: Sat May  4 17:33:51 2024, max compression
```

## Comparing `pyvserv-1.0.6.tar` & `pyvserv-1.0.7.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.155934 pyvserv-1.0.6/
--rw-rw-r--   0 peterglen  (1000) users      (100)     1097 2024-03-15 11:18:08.000000 pyvserv-1.0.6/LICENSE
--rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-05-04 15:30:18.155934 pyvserv-1.0.6/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)    17156 2024-04-10 00:53:07.000000 pyvserv-1.0.6/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.131934 pyvserv-1.0.6/pyvclient/
--rw-rw-r--   0 peterglen  (1000) users      (100)       14 2024-04-15 07:22:33.000000 pyvserv-1.0.6/pyvclient/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.139934 pyvserv-1.0.6/pyvclient/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)    13937 2024-04-15 06:50:03.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_acc.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12079 2024-04-15 06:49:27.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_akey.html
--rw-r--r--   0 peterglen  (1000) users      (100)    13072 2024-04-15 06:49:28.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_bigget.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14945 2024-04-15 06:49:29.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_cd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    24511 2024-04-15 06:49:30.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_cli.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11941 2024-04-15 06:49:31.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_fdel.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11688 2024-04-15 06:49:31.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_fget.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12082 2024-04-15 06:49:32.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_file.html
--rw-r--r--   0 peterglen  (1000) users      (100)    18815 2024-04-15 06:49:33.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_fman.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11794 2024-04-15 06:49:34.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_fput.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12743 2024-04-15 06:49:35.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_gethelp.html
--rw-r--r--   0 peterglen  (1000) users      (100)    13095 2024-04-15 06:49:36.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_hello.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10536 2024-04-10 00:54:07.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_id.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14864 2024-04-15 06:49:38.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_ihost.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12497 2024-04-15 06:49:39.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_login.html
--rw-r--r--   0 peterglen  (1000) users      (100)    13464 2024-04-15 06:49:41.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_ls.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12238 2024-04-15 06:49:40.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_lsd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:42.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_mkdir.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12205 2024-04-15 06:49:42.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_pass.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10253 2024-04-15 06:49:43.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_ping.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14879 2024-04-15 06:49:44.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_qr.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16745 2024-04-15 06:49:45.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rabs.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16354 2024-04-15 06:49:46.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rcheck.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14273 2024-04-15 06:49:47.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rcount.html
--rw-r--r--   0 peterglen  (1000) users      (100)    32879 2024-04-15 06:57:46.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_replic.html
--rw-r--r--   0 peterglen  (1000) users      (100)    17860 2024-04-15 06:49:49.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rget.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16101 2024-04-15 06:49:50.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rlist.html
--rw-r--r--   0 peterglen  (1000) users      (100)    24463 2024-04-15 06:49:51.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rman.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:52.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rmdir.html
--rw-r--r--   0 peterglen  (1000) users      (100)    18495 2024-04-15 06:49:53.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rput.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14769 2024-04-15 06:49:54.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_sess.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16015 2024-04-15 06:50:05.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_sess_tout.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11681 2024-04-15 06:49:55.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_throt.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10607 2024-04-15 06:50:04.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_tout.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11574 2024-04-15 06:49:56.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uadd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14358 2024-04-15 06:49:57.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uchpass.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11365 2024-04-15 06:49:58.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_udel.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12115 2024-04-15 06:49:59.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uena.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16680 2024-04-15 06:50:00.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uini.html
--rw-r--r--   0 peterglen  (1000) users      (100)    20642 2024-04-15 06:50:01.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uman.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12963 2024-04-15 06:50:02.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_ver.html
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1208 2024-02-05 14:55:18.000000 pyvserv-1.0.6/pyvclient/loadtest.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3848 2024-04-06 08:48:29.000000 pyvserv-1.0.6/pyvclient/pyvcli_akey.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4743 2024-04-09 14:23:35.000000 pyvserv-1.0.6/pyvclient/pyvcli_bigget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5567 2024-04-06 08:47:43.000000 pyvserv-1.0.6/pyvclient/pyvcli_cd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     9985 2024-04-11 22:53:59.000000 pyvserv-1.0.6/pyvclient/pyvcli_cli.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3784 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_fdel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3503 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_fget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3976 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_file.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6078 2024-04-10 01:59:10.000000 pyvserv-1.0.6/pyvclient/pyvcli_fman.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3639 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_fput.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3156 2024-04-09 05:49:52.000000 pyvserv-1.0.6/pyvclient/pyvcli_gethelp.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3409 2024-04-09 05:40:35.000000 pyvserv-1.0.6/pyvclient/pyvcli_hello.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2432 2024-04-05 22:02:34.000000 pyvserv-1.0.6/pyvclient/pyvcli_id.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6166 2024-04-12 22:44:34.000000 pyvserv-1.0.6/pyvclient/pyvcli_ihost.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3988 2024-04-06 08:49:18.000000 pyvserv-1.0.6/pyvclient/pyvcli_login.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4960 2024-04-06 08:50:29.000000 pyvserv-1.0.6/pyvclient/pyvcli_ls.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4076 2024-04-06 08:50:00.000000 pyvserv-1.0.6/pyvclient/pyvcli_lsd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_mkdir.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3776 2024-04-06 08:50:51.000000 pyvserv-1.0.6/pyvclient/pyvcli_pass.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2351 2024-02-25 16:08:36.000000 pyvserv-1.0.6/pyvclient/pyvcli_ping.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4099 2024-04-09 05:32:53.000000 pyvserv-1.0.6/pyvclient/pyvcli_qr.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4992 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rabs.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4816 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rcheck.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3850 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rcount.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    13786 2024-04-15 11:47:19.000000 pyvserv-1.0.6/pyvclient/pyvcli_replic.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5462 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4659 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rlist.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     8530 2024-04-10 01:58:55.000000 pyvserv-1.0.6/pyvclient/pyvcli_rman.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rmdir.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5788 2024-04-12 12:45:56.000000 pyvserv-1.0.6/pyvclient/pyvcli_rput.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6137 2024-04-05 13:27:04.000000 pyvserv-1.0.6/pyvclient/pyvcli_sess.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3548 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_throt.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3353 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_uadd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5689 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_uchpass.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3192 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_udel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3867 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_uena.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4818 2024-04-14 07:07:11.000000 pyvserv-1.0.6/pyvclient/pyvcli_uini.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6972 2024-04-10 01:56:40.000000 pyvserv-1.0.6/pyvclient/pyvcli_uman.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3171 2024-04-09 05:24:42.000000 pyvserv-1.0.6/pyvclient/pyvcli_ver.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.143934 pyvserv-1.0.6/pyvcommon/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:55.000000 pyvserv-1.0.6/pyvcommon/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    12254 2024-04-15 07:57:44.000000 pyvserv-1.0.6/pyvcommon/comline.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4270 2021-02-05 17:39:14.000000 pyvserv-1.0.6/pyvcommon/crysupp.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      608 2024-03-09 10:44:12.000000 pyvserv-1.0.6/pyvcommon/genstrerr.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    17642 2024-04-08 08:14:28.000000 pyvserv-1.0.6/pyvcommon/pyclisup.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5322 2021-02-05 17:39:14.000000 pyvserv-1.0.6/pyvcommon/pycrypt.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6778 2024-04-11 23:55:27.000000 pyvserv-1.0.6/pyvcommon/pydata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    29729 2024-05-04 15:30:03.000000 pyvserv-1.0.6/pyvcommon/pyservsup.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3479 2024-03-10 14:51:33.000000 pyvserv-1.0.6/pyvcommon/pysyslog.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      571 2024-03-01 12:52:57.000000 pyvserv-1.0.6/pyvcommon/pyv2fa.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10878 2024-04-22 16:13:09.000000 pyvserv-1.0.6/pyvcommon/pyvhash.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4762 2024-03-03 14:03:00.000000 pyvserv-1.0.6/pyvcommon/pywrap.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9529 2024-04-15 10:48:15.000000 pyvserv-1.0.6/pyvcommon/support.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.143934 pyvserv-1.0.6/pyvgui/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:37.000000 pyvserv-1.0.6/pyvgui/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.143934 pyvserv-1.0.6/pyvgui/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)    11912 2024-05-03 10:03:11.000000 pyvserv-1.0.6/pyvgui/docs/pyvcpanel.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11223 2024-05-03 10:03:07.000000 pyvserv-1.0.6/pyvgui/docs/pyvservui.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11883 2024-05-03 10:03:10.000000 pyvserv-1.0.6/pyvgui/docs/pyvtally.html
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.147934 pyvserv-1.0.6/pyvgui/guilib/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:46.000000 pyvserv-1.0.6/pyvgui/guilib/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    19985 2024-05-03 08:59:03.000000 pyvserv-1.0.6/pyvgui/guilib/config.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1718 2024-05-01 16:45:09.000000 pyvserv-1.0.6/pyvgui/guilib/entry_color.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    32884 2024-05-03 08:34:42.000000 pyvserv-1.0.6/pyvgui/guilib/mainballot.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14685 2024-05-03 09:05:10.000000 pyvserv-1.0.6/pyvgui/guilib/mainwin.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    28844 2024-05-03 08:21:52.000000 pyvserv-1.0.6/pyvgui/guilib/mainwinpeople.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5928 2024-04-03 06:14:02.000000 pyvserv-1.0.6/pyvgui/guilib/mainwinserv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    13140 2024-05-02 17:09:41.000000 pyvserv-1.0.6/pyvgui/guilib/mainwintally.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    33945 2024-05-03 08:44:59.000000 pyvserv-1.0.6/pyvgui/guilib/mainwinvote.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    12769 2024-05-01 11:17:04.000000 pyvserv-1.0.6/pyvgui/guilib/passdlg.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10836 2024-04-29 14:32:40.000000 pyvserv-1.0.6/pyvgui/guilib/pgcal.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3214 2024-03-11 03:29:27.000000 pyvserv-1.0.6/pyvgui/guilib/pgui.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    11922 2021-02-03 22:50:23.000000 pyvserv-1.0.6/pyvgui/guilib/pymenu.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    30364 2024-05-03 07:01:14.000000 pyvserv-1.0.6/pyvgui/guilib/recsel.py
--rw-r--r--   0 peterglen  (1000) users      (100)     6002 2024-05-01 10:13:15.000000 pyvserv-1.0.6/pyvgui/pyvballot.png
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4314 2024-04-30 13:08:04.000000 pyvserv-1.0.6/pyvgui/pyvballot.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3108 2024-05-03 09:01:56.000000 pyvserv-1.0.6/pyvgui/pyvcpanel.py
--rw-r--r--   0 peterglen  (1000) users      (100)    14408 2024-05-01 09:57:52.000000 pyvserv-1.0.6/pyvgui/pyvpeople.png
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4320 2024-05-01 07:37:40.000000 pyvserv-1.0.6/pyvgui/pyvpeople.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2687 2024-05-03 09:28:18.000000 pyvserv-1.0.6/pyvgui/pyvservui.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3093 2024-05-02 17:03:45.000000 pyvserv-1.0.6/pyvgui/pyvtally.py
--rw-r--r--   0 peterglen  (1000) users      (100)     9831 2024-04-26 07:01:28.000000 pyvserv-1.0.6/pyvgui/pyvvote.png
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4316 2024-04-30 06:47:34.000000 pyvserv-1.0.6/pyvgui/pyvvote.py
--rw-r--r--   0 peterglen  (1000) users      (100)     8794 2024-04-26 07:12:36.000000 pyvserv-1.0.6/pyvgui/pyvvote_sub.png
--rw-r--r--   0 peterglen  (1000) users      (100)    80291 2024-04-17 01:51:25.000000 pyvserv-1.0.6/pyvgui/vote.png
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.155934 pyvserv-1.0.6/pyvserv.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)     3855 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)      732 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       48 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/requires.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       46 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/top_level.txt
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.151934 pyvserv-1.0.6/pyvserver/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:41.000000 pyvserv-1.0.6/pyvserver/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.151934 pyvserv-1.0.6/pyvserver/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)   171300 2024-04-15 06:32:07.000000 pyvserv-1.0.6/pyvserver/docs/pyvfunc.html
--rw-r--r--   0 peterglen  (1000) users      (100)    76482 2024-04-15 06:32:05.000000 pyvserv-1.0.6/pyvserver/docs/pyvreplic.html
--rw-r--r--   0 peterglen  (1000) users      (100)    68036 2024-04-15 06:32:04.000000 pyvserv-1.0.6/pyvserver/docs/pyvserv.html
--rw-r--r--   0 peterglen  (1000) users      (100)    35380 2024-04-15 06:32:06.000000 pyvserv-1.0.6/pyvserver/docs/pyvstate.html
--rw-rw-r--   0 peterglen  (1000) users      (100)    67566 2024-04-15 10:22:32.000000 pyvserv-1.0.6/pyvserver/pyvfunc.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    23259 2024-04-15 06:31:36.000000 pyvserv-1.0.6/pyvserver/pyvreplic.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    22417 2024-04-15 05:56:51.000000 pyvserv-1.0.6/pyvserver/pyvserv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14128 2024-04-15 10:48:53.000000 pyvserv-1.0.6/pyvserver/pyvstate.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.155934 pyvserv-1.0.6/pyvtools/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:20.000000 pyvserv-1.0.6/pyvtools/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.155934 pyvserv-1.0.6/pyvtools/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)    16315 2024-05-03 10:03:06.000000 pyvserv-1.0.6/pyvtools/docs/pyvgenkey.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10283 2024-05-03 10:03:05.000000 pyvserv-1.0.6/pyvtools/docs/pyvgenkeys.html
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4542 2024-04-04 05:48:31.000000 pyvserv-1.0.6/pyvtools/pyvgenkey.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2508 2024-04-09 08:30:16.000000 pyvserv-1.0.6/pyvtools/pyvgenkeys.py
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-04 15:30:18.155934 pyvserv-1.0.6/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     5787 2024-05-04 15:28:16.000000 pyvserv-1.0.6/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.677723 pyvserv-1.0.7/
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1097 2024-03-15 11:18:08.000000 pyvserv-1.0.7/LICENSE
+-rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-05-04 17:33:51.677723 pyvserv-1.0.7/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)    17156 2024-04-10 00:53:07.000000 pyvserv-1.0.7/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.649722 pyvserv-1.0.7/pyvclient/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       14 2024-04-15 07:22:33.000000 pyvserv-1.0.7/pyvclient/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.661723 pyvserv-1.0.7/pyvclient/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    13937 2024-04-15 06:50:03.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_acc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12079 2024-04-15 06:49:27.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_akey.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13072 2024-04-15 06:49:28.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_bigget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14945 2024-04-15 06:49:29.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_cd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24511 2024-04-15 06:49:30.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_cli.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11941 2024-04-15 06:49:31.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_fdel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11688 2024-04-15 06:49:31.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_fget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12082 2024-04-15 06:49:32.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_file.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    18815 2024-04-15 06:49:33.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_fman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11794 2024-04-15 06:49:34.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_fput.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12743 2024-04-15 06:49:35.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_gethelp.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13095 2024-04-15 06:49:36.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_hello.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10536 2024-04-10 00:54:07.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_id.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14864 2024-04-15 06:49:38.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_ihost.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12497 2024-04-15 06:49:39.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_login.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13464 2024-04-15 06:49:41.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_ls.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12238 2024-04-15 06:49:40.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_lsd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:42.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_mkdir.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12205 2024-04-15 06:49:42.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_pass.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10253 2024-04-15 06:49:43.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_ping.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14879 2024-04-15 06:49:44.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_qr.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16745 2024-04-15 06:49:45.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_rabs.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16354 2024-04-15 06:49:46.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_rcheck.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14273 2024-04-15 06:49:47.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_rcount.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    32879 2024-04-15 06:57:46.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_replic.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    17860 2024-04-15 06:49:49.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_rget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16101 2024-04-15 06:49:50.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_rlist.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24463 2024-04-15 06:49:51.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_rman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:52.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_rmdir.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    18495 2024-04-15 06:49:53.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_rput.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14769 2024-04-15 06:49:54.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_sess.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16015 2024-04-15 06:50:05.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_sess_tout.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11681 2024-04-15 06:49:55.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_throt.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10607 2024-04-15 06:50:04.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_tout.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11574 2024-04-15 06:49:56.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_uadd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14358 2024-04-15 06:49:57.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_uchpass.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11365 2024-04-15 06:49:58.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_udel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12115 2024-04-15 06:49:59.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_uena.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16680 2024-04-15 06:50:00.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_uini.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    20642 2024-04-15 06:50:01.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_uman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12963 2024-04-15 06:50:02.000000 pyvserv-1.0.7/pyvclient/docs/pyvcli_ver.html
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1208 2024-02-05 14:55:18.000000 pyvserv-1.0.7/pyvclient/loadtest.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3848 2024-04-06 08:48:29.000000 pyvserv-1.0.7/pyvclient/pyvcli_akey.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4743 2024-04-09 14:23:35.000000 pyvserv-1.0.7/pyvclient/pyvcli_bigget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5567 2024-04-06 08:47:43.000000 pyvserv-1.0.7/pyvclient/pyvcli_cd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     9985 2024-04-11 22:53:59.000000 pyvserv-1.0.7/pyvclient/pyvcli_cli.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3784 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_fdel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3503 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_fget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3976 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_file.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6078 2024-04-10 01:59:10.000000 pyvserv-1.0.7/pyvclient/pyvcli_fman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3639 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_fput.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3156 2024-04-09 05:49:52.000000 pyvserv-1.0.7/pyvclient/pyvcli_gethelp.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3409 2024-04-09 05:40:35.000000 pyvserv-1.0.7/pyvclient/pyvcli_hello.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2432 2024-04-05 22:02:34.000000 pyvserv-1.0.7/pyvclient/pyvcli_id.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6166 2024-04-12 22:44:34.000000 pyvserv-1.0.7/pyvclient/pyvcli_ihost.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3988 2024-04-06 08:49:18.000000 pyvserv-1.0.7/pyvclient/pyvcli_login.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4960 2024-04-06 08:50:29.000000 pyvserv-1.0.7/pyvclient/pyvcli_ls.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4076 2024-04-06 08:50:00.000000 pyvserv-1.0.7/pyvclient/pyvcli_lsd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_mkdir.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3776 2024-04-06 08:50:51.000000 pyvserv-1.0.7/pyvclient/pyvcli_pass.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2351 2024-02-25 16:08:36.000000 pyvserv-1.0.7/pyvclient/pyvcli_ping.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4099 2024-04-09 05:32:53.000000 pyvserv-1.0.7/pyvclient/pyvcli_qr.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4992 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_rabs.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4816 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_rcheck.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3850 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_rcount.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    13786 2024-04-15 11:47:19.000000 pyvserv-1.0.7/pyvclient/pyvcli_replic.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5462 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_rget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4659 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_rlist.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     8530 2024-04-10 01:58:55.000000 pyvserv-1.0.7/pyvclient/pyvcli_rman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_rmdir.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5788 2024-04-12 12:45:56.000000 pyvserv-1.0.7/pyvclient/pyvcli_rput.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6137 2024-04-05 13:27:04.000000 pyvserv-1.0.7/pyvclient/pyvcli_sess.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3548 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_throt.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3353 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_uadd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5689 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_uchpass.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3192 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_udel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3867 2024-04-09 05:45:08.000000 pyvserv-1.0.7/pyvclient/pyvcli_uena.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4818 2024-04-14 07:07:11.000000 pyvserv-1.0.7/pyvclient/pyvcli_uini.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6972 2024-04-10 01:56:40.000000 pyvserv-1.0.7/pyvclient/pyvcli_uman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3171 2024-04-09 05:24:42.000000 pyvserv-1.0.7/pyvclient/pyvcli_ver.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.665722 pyvserv-1.0.7/pyvcommon/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:55.000000 pyvserv-1.0.7/pyvcommon/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    12254 2024-04-15 07:57:44.000000 pyvserv-1.0.7/pyvcommon/comline.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4270 2021-02-05 17:39:14.000000 pyvserv-1.0.7/pyvcommon/crysupp.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)      608 2024-03-09 10:44:12.000000 pyvserv-1.0.7/pyvcommon/genstrerr.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    17642 2024-04-08 08:14:28.000000 pyvserv-1.0.7/pyvcommon/pyclisup.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5322 2021-02-05 17:39:14.000000 pyvserv-1.0.7/pyvcommon/pycrypt.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6778 2024-04-11 23:55:27.000000 pyvserv-1.0.7/pyvcommon/pydata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    29729 2024-05-04 17:31:01.000000 pyvserv-1.0.7/pyvcommon/pyservsup.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3479 2024-03-10 14:51:33.000000 pyvserv-1.0.7/pyvcommon/pysyslog.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)      571 2024-03-01 12:52:57.000000 pyvserv-1.0.7/pyvcommon/pyv2fa.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10878 2024-04-22 16:13:09.000000 pyvserv-1.0.7/pyvcommon/pyvhash.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4762 2024-03-03 14:03:00.000000 pyvserv-1.0.7/pyvcommon/pywrap.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     9529 2024-04-15 10:48:15.000000 pyvserv-1.0.7/pyvcommon/support.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.665722 pyvserv-1.0.7/pyvgui/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:37.000000 pyvserv-1.0.7/pyvgui/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.669723 pyvserv-1.0.7/pyvgui/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    11912 2024-05-03 10:03:11.000000 pyvserv-1.0.7/pyvgui/docs/pyvcpanel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11223 2024-05-03 10:03:07.000000 pyvserv-1.0.7/pyvgui/docs/pyvservui.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11883 2024-05-03 10:03:10.000000 pyvserv-1.0.7/pyvgui/docs/pyvtally.html
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.669723 pyvserv-1.0.7/pyvgui/guilib/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:46.000000 pyvserv-1.0.7/pyvgui/guilib/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    19985 2024-05-03 08:59:03.000000 pyvserv-1.0.7/pyvgui/guilib/config.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1718 2024-05-01 16:45:09.000000 pyvserv-1.0.7/pyvgui/guilib/entry_color.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    32884 2024-05-03 08:34:42.000000 pyvserv-1.0.7/pyvgui/guilib/mainballot.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14685 2024-05-03 09:05:10.000000 pyvserv-1.0.7/pyvgui/guilib/mainwin.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    28844 2024-05-03 08:21:52.000000 pyvserv-1.0.7/pyvgui/guilib/mainwinpeople.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5928 2024-04-03 06:14:02.000000 pyvserv-1.0.7/pyvgui/guilib/mainwinserv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13140 2024-05-02 17:09:41.000000 pyvserv-1.0.7/pyvgui/guilib/mainwintally.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    33946 2024-05-04 15:43:47.000000 pyvserv-1.0.7/pyvgui/guilib/mainwinvote.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    12769 2024-05-01 11:17:04.000000 pyvserv-1.0.7/pyvgui/guilib/passdlg.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10836 2024-04-29 14:32:40.000000 pyvserv-1.0.7/pyvgui/guilib/pgcal.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3214 2024-03-11 03:29:27.000000 pyvserv-1.0.7/pyvgui/guilib/pgui.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    11922 2021-02-03 22:50:23.000000 pyvserv-1.0.7/pyvgui/guilib/pymenu.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    30364 2024-05-03 07:01:14.000000 pyvserv-1.0.7/pyvgui/guilib/recsel.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     6002 2024-05-01 10:13:15.000000 pyvserv-1.0.7/pyvgui/pyvballot.png
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4314 2024-04-30 13:08:04.000000 pyvserv-1.0.7/pyvgui/pyvballot.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3108 2024-05-03 09:01:56.000000 pyvserv-1.0.7/pyvgui/pyvcpanel.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    14408 2024-05-01 09:57:52.000000 pyvserv-1.0.7/pyvgui/pyvpeople.png
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4320 2024-05-01 07:37:40.000000 pyvserv-1.0.7/pyvgui/pyvpeople.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2687 2024-05-03 09:28:18.000000 pyvserv-1.0.7/pyvgui/pyvservui.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3093 2024-05-02 17:03:45.000000 pyvserv-1.0.7/pyvgui/pyvtally.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     9831 2024-04-26 07:01:28.000000 pyvserv-1.0.7/pyvgui/pyvvote.png
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4316 2024-04-30 06:47:34.000000 pyvserv-1.0.7/pyvgui/pyvvote.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     8794 2024-04-26 07:12:36.000000 pyvserv-1.0.7/pyvgui/pyvvote_sub.png
+-rw-r--r--   0 peterglen  (1000) users      (100)    80291 2024-04-17 01:51:25.000000 pyvserv-1.0.7/pyvgui/vote.png
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.677723 pyvserv-1.0.7/pyvserv.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-05-04 17:33:51.000000 pyvserv-1.0.7/pyvserv.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)     3855 2024-05-04 17:33:51.000000 pyvserv-1.0.7/pyvserv.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-05-04 17:33:51.000000 pyvserv-1.0.7/pyvserv.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)      732 2024-05-04 17:33:51.000000 pyvserv-1.0.7/pyvserv.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       48 2024-05-04 17:33:51.000000 pyvserv-1.0.7/pyvserv.egg-info/requires.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       46 2024-05-04 17:33:51.000000 pyvserv-1.0.7/pyvserv.egg-info/top_level.txt
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.677723 pyvserv-1.0.7/pyvserver/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:41.000000 pyvserv-1.0.7/pyvserver/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.677723 pyvserv-1.0.7/pyvserver/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)   171300 2024-04-15 06:32:07.000000 pyvserv-1.0.7/pyvserver/docs/pyvfunc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    76482 2024-04-15 06:32:05.000000 pyvserv-1.0.7/pyvserver/docs/pyvreplic.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    68036 2024-04-15 06:32:04.000000 pyvserv-1.0.7/pyvserver/docs/pyvserv.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    35380 2024-04-15 06:32:06.000000 pyvserv-1.0.7/pyvserver/docs/pyvstate.html
+-rw-rw-r--   0 peterglen  (1000) users      (100)    67610 2024-05-04 17:05:19.000000 pyvserv-1.0.7/pyvserver/pyvfunc.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    23259 2024-04-15 06:31:36.000000 pyvserv-1.0.7/pyvserver/pyvreplic.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    22493 2024-05-04 16:32:54.000000 pyvserv-1.0.7/pyvserver/pyvserv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14128 2024-04-15 10:48:53.000000 pyvserv-1.0.7/pyvserver/pyvstate.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.677723 pyvserv-1.0.7/pyvtools/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:20.000000 pyvserv-1.0.7/pyvtools/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 17:33:51.677723 pyvserv-1.0.7/pyvtools/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    16315 2024-05-03 10:03:06.000000 pyvserv-1.0.7/pyvtools/docs/pyvgenkey.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10283 2024-05-03 10:03:05.000000 pyvserv-1.0.7/pyvtools/docs/pyvgenkeys.html
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4542 2024-04-04 05:48:31.000000 pyvserv-1.0.7/pyvtools/pyvgenkey.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2508 2024-04-09 08:30:16.000000 pyvserv-1.0.7/pyvtools/pyvgenkeys.py
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-04 17:33:51.681723 pyvserv-1.0.7/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5787 2024-05-04 15:28:16.000000 pyvserv-1.0.7/setup.py
```

### Comparing `pyvserv-1.0.6/LICENSE` & `pyvserv-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/PKG-INFO` & `pyvserv-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvserv
-Version: 1.0.6
+Version: 1.0.7
 Summary: High power secure server with blockchain backend.
 Home-page: https://github.com/pglen/pyvserv
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvserv-1.0.6/README.md` & `pyvserv-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_acc.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_acc.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_akey.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_akey.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_bigget.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_bigget.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_cd.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_cd.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_cli.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_cli.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_fdel.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_fdel.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_fget.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_fget.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_file.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_file.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_fman.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_fman.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_fput.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_fput.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_gethelp.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_gethelp.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_hello.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_hello.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_id.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_id.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_ihost.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_ihost.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_login.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_login.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_ls.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_ls.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_lsd.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_lsd.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_mkdir.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_mkdir.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_pass.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_pass.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_ping.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_ping.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_qr.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_qr.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_rabs.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_rabs.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_rcheck.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_rcheck.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_rcount.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_rcount.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_replic.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_replic.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_rget.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_rget.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_rlist.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_rlist.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_rman.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_rman.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_rmdir.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_rmdir.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_rput.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_rput.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_sess.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_sess.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_sess_tout.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_sess_tout.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_throt.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_throt.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_tout.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_tout.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_uadd.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_uadd.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_uchpass.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_uchpass.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_udel.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_udel.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_uena.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_uena.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_uini.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_uini.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_uman.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_uman.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/docs/pyvcli_ver.html` & `pyvserv-1.0.7/pyvclient/docs/pyvcli_ver.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/loadtest.py` & `pyvserv-1.0.7/pyvclient/loadtest.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_akey.py` & `pyvserv-1.0.7/pyvclient/pyvcli_akey.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_bigget.py` & `pyvserv-1.0.7/pyvclient/pyvcli_bigget.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_cd.py` & `pyvserv-1.0.7/pyvclient/pyvcli_cd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_cli.py` & `pyvserv-1.0.7/pyvclient/pyvcli_cli.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_fdel.py` & `pyvserv-1.0.7/pyvclient/pyvcli_fdel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_fget.py` & `pyvserv-1.0.7/pyvclient/pyvcli_fget.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_file.py` & `pyvserv-1.0.7/pyvclient/pyvcli_file.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_fman.py` & `pyvserv-1.0.7/pyvclient/pyvcli_fman.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_fput.py` & `pyvserv-1.0.7/pyvclient/pyvcli_fput.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_gethelp.py` & `pyvserv-1.0.7/pyvclient/pyvcli_gethelp.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_hello.py` & `pyvserv-1.0.7/pyvclient/pyvcli_hello.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_id.py` & `pyvserv-1.0.7/pyvclient/pyvcli_id.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_ihost.py` & `pyvserv-1.0.7/pyvclient/pyvcli_ihost.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_login.py` & `pyvserv-1.0.7/pyvclient/pyvcli_login.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_ls.py` & `pyvserv-1.0.7/pyvclient/pyvcli_ls.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_lsd.py` & `pyvserv-1.0.7/pyvclient/pyvcli_lsd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_mkdir.py` & `pyvserv-1.0.7/pyvclient/pyvcli_mkdir.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_pass.py` & `pyvserv-1.0.7/pyvclient/pyvcli_pass.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_ping.py` & `pyvserv-1.0.7/pyvclient/pyvcli_ping.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_qr.py` & `pyvserv-1.0.7/pyvclient/pyvcli_qr.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_rabs.py` & `pyvserv-1.0.7/pyvclient/pyvcli_rabs.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_rcheck.py` & `pyvserv-1.0.7/pyvclient/pyvcli_rcheck.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_rcount.py` & `pyvserv-1.0.7/pyvclient/pyvcli_rcount.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_replic.py` & `pyvserv-1.0.7/pyvclient/pyvcli_replic.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_rget.py` & `pyvserv-1.0.7/pyvclient/pyvcli_rget.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_rlist.py` & `pyvserv-1.0.7/pyvclient/pyvcli_rlist.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_rman.py` & `pyvserv-1.0.7/pyvclient/pyvcli_rman.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_rmdir.py` & `pyvserv-1.0.7/pyvclient/pyvcli_rmdir.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_rput.py` & `pyvserv-1.0.7/pyvclient/pyvcli_rput.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_sess.py` & `pyvserv-1.0.7/pyvclient/pyvcli_sess.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_throt.py` & `pyvserv-1.0.7/pyvclient/pyvcli_throt.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_uadd.py` & `pyvserv-1.0.7/pyvclient/pyvcli_uadd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_uchpass.py` & `pyvserv-1.0.7/pyvclient/pyvcli_uchpass.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_udel.py` & `pyvserv-1.0.7/pyvclient/pyvcli_udel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_uena.py` & `pyvserv-1.0.7/pyvclient/pyvcli_uena.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_uini.py` & `pyvserv-1.0.7/pyvclient/pyvcli_uini.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_uman.py` & `pyvserv-1.0.7/pyvclient/pyvcli_uman.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvclient/pyvcli_ver.py` & `pyvserv-1.0.7/pyvclient/pyvcli_ver.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/comline.py` & `pyvserv-1.0.7/pyvcommon/comline.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/crysupp.py` & `pyvserv-1.0.7/pyvcommon/crysupp.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/genstrerr.py` & `pyvserv-1.0.7/pyvcommon/genstrerr.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/pyclisup.py` & `pyvserv-1.0.7/pyvcommon/pyclisup.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/pycrypt.py` & `pyvserv-1.0.7/pyvcommon/pycrypt.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/pydata.py` & `pyvserv-1.0.7/pyvcommon/pydata.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/pyservsup.py` & `pyvserv-1.0.7/pyvcommon/pyservsup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #from Crypto.Hash import SHA512
 from Crypto.Hash import SHA256
 from Crypto import Random
 
 # Globals and configurables
 
 # Update it here from setup
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 
 # Actions
 USER_AUTH  = 0;  USER_ADD = 1;   USER_DEL = 2;   USER_CHPASS = 3;
 USER_CHMOD = 4;
 
 # Permissions
 PERM_NONE = 0;  PERM_INI = 1;   PERM_ADMIN = 2;   PERM_DIS = 4;
```

### Comparing `pyvserv-1.0.6/pyvcommon/pysyslog.py` & `pyvserv-1.0.7/pyvcommon/pysyslog.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/pyv2fa.py` & `pyvserv-1.0.7/pyvcommon/pyv2fa.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/pyvhash.py` & `pyvserv-1.0.7/pyvcommon/pyvhash.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/pywrap.py` & `pyvserv-1.0.7/pyvcommon/pywrap.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvcommon/support.py` & `pyvserv-1.0.7/pyvcommon/support.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/docs/pyvcpanel.html` & `pyvserv-1.0.7/pyvgui/docs/pyvcpanel.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/docs/pyvservui.html` & `pyvserv-1.0.7/pyvgui/docs/pyvservui.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/docs/pyvtally.html` & `pyvserv-1.0.7/pyvgui/docs/pyvtally.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/config.py` & `pyvserv-1.0.7/pyvgui/guilib/config.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/entry_color.py` & `pyvserv-1.0.7/pyvgui/guilib/entry_color.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/mainballot.py` & `pyvserv-1.0.7/pyvgui/guilib/mainballot.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/mainwin.py` & `pyvserv-1.0.7/pyvgui/guilib/mainwin.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/mainwinpeople.py` & `pyvserv-1.0.7/pyvgui/guilib/mainwinpeople.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/mainwinserv.py` & `pyvserv-1.0.7/pyvgui/guilib/mainwinserv.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/mainwintally.py` & `pyvserv-1.0.7/pyvgui/guilib/mainwintally.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/mainwinvote.py` & `pyvserv-1.0.7/pyvgui/guilib/mainwinvote.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
             return
         #print("dat:", dat)
         try:
             dec = self.packer.decode_data(dat[0][1])[0]
         except:
             dec = {}
             pass
-        print("dec:", dec)
+        #print("dec:", dec)
         # Assign to form
         self.dat_dict['buuid'].set_text(dec['uuid'])
         self.dat_dict['bname'].set_text(dec['name'])
         self.dat_dict['bdate'].set_text(dec['dob'])
 
         for aa in range(8):
             idx = "can%d" % (aa+1)
```

### Comparing `pyvserv-1.0.6/pyvgui/guilib/passdlg.py` & `pyvserv-1.0.7/pyvgui/guilib/passdlg.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/pgcal.py` & `pyvserv-1.0.7/pyvgui/guilib/pgcal.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/pgui.py` & `pyvserv-1.0.7/pyvgui/guilib/pgui.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/pymenu.py` & `pyvserv-1.0.7/pyvgui/guilib/pymenu.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/guilib/recsel.py` & `pyvserv-1.0.7/pyvgui/guilib/recsel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvballot.png` & `pyvserv-1.0.7/pyvgui/pyvballot.png`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvballot.py` & `pyvserv-1.0.7/pyvgui/pyvballot.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvcpanel.py` & `pyvserv-1.0.7/pyvgui/pyvcpanel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvpeople.png` & `pyvserv-1.0.7/pyvgui/pyvpeople.png`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvpeople.py` & `pyvserv-1.0.7/pyvgui/pyvpeople.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvservui.py` & `pyvserv-1.0.7/pyvgui/pyvservui.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvtally.py` & `pyvserv-1.0.7/pyvgui/pyvtally.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvvote.png` & `pyvserv-1.0.7/pyvgui/pyvvote.png`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvvote.py` & `pyvserv-1.0.7/pyvgui/pyvvote.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/pyvvote_sub.png` & `pyvserv-1.0.7/pyvgui/pyvvote_sub.png`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvgui/vote.png` & `pyvserv-1.0.7/pyvgui/vote.png`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvserv.egg-info/PKG-INFO` & `pyvserv-1.0.7/pyvserv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvserv
-Version: 1.0.6
+Version: 1.0.7
 Summary: High power secure server with blockchain backend.
 Home-page: https://github.com/pglen/pyvserv
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvserv-1.0.6/pyvserv.egg-info/SOURCES.txt` & `pyvserv-1.0.7/pyvserv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvserv.egg-info/entry_points.txt` & `pyvserv-1.0.7/pyvserv.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvserver/docs/pyvfunc.html` & `pyvserv-1.0.7/pyvserver/docs/pyvfunc.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvserver/docs/pyvreplic.html` & `pyvserv-1.0.7/pyvserver/docs/pyvreplic.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvserver/docs/pyvserv.html` & `pyvserv-1.0.7/pyvserver/docs/pyvserv.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvserver/docs/pyvstate.html` & `pyvserv-1.0.7/pyvserver/docs/pyvstate.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvserver/pyvfunc.py` & `pyvserv-1.0.7/pyvserver/pyvfunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1314,15 +1314,15 @@
 # ------------------------------------------------------------------------
 
 def get_ver_func(self, strx):
 
     if pyservsup.globals.conf.pgdebug > 1:
         print( "get_ver_func()", strx)
 
-    res = [OK, "%s" % pyservsup.version,
+    res = [OK, "%s" % pyservsup.VERSION,
                         "%s" % pyservsup.globals.siteid, self.name]
 
     if pyservsup.globals.conf.pgdebug > 4:
         print( "get_ver_func->output", res)
 
     self.resp.datahandler.putencode(res, self.resp.ekey)
 
@@ -1384,24 +1384,25 @@
 
     if not self.resp.user:
         response = [ERR, "Not logged in.", strx[0], ]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     if pyservsup.globals.conf.pglog > 0:
-        stry = "Logout", _wr(resp.user), \
+        stry = "Logout", _wr(self.resp.user), \
                 str(self.resp.client_address)
         pysyslog.syslog(*stry)
 
     if self.pgdebug > 3:
         print("logout", self.resp.user)
 
-    if resp.user:
-        pyservsup.SHARED_LOGINS.deldat(resp.user)
+    if self.resp.user:
+        pyservsup.SHARED_LOGINS.deldat(self.resp.user)
 
+    olduser = self.resp.user
     self.resp.user = ""
 
     response = [OK, "Logged out.", olduser, ]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 #@support.timeit
 def get_user_func(self, strx):
```

### Comparing `pyvserv-1.0.6/pyvserver/pyvreplic.py` & `pyvserv-1.0.7/pyvserver/pyvreplic.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvserver/pyvserv.py` & `pyvserv-1.0.7/pyvserver/pyvserv.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import time
 import subprocess
 import platform
 import socket
 import threading
 import tracemalloc
 import datetime
-import distro
+#import distro
 
 if sys.version_info[0] < 3:
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
 try:
     import fcntl
@@ -166,15 +166,15 @@
         self.datahandler.par        = self
 
         self.request.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
 
         if conf.pglog > 0:
             pysyslog.syslog("Connected " + " " + str(self.client_address))
 
-        response =  ["OK", "pyvserv %s ready" % pyservsup.version, self.name]
+        response =  ["OK", "pyvserv %s ready" % pyservsup.VERSION, self.name]
 
         # Connected, acknowledge it
         self.datahandler.putencode(response, "")
 
     def handle_error(self, request, client_address):
 
         ''' Placeholder '''
@@ -430,15 +430,15 @@
         self.datahandler.par = self
 
         self.client.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
 
         if conf.pglog > 0:
             pysyslog.syslog("Connected ", str(self.client_address))
 
-        response =  ["OK", "pyvserv %s ready" % pyservsup.version]
+        response =  ["OK", "pyvserv %s ready" % pyservsup.VERSION]
         # Connected, acknowledge it
         self.datahandler.putencode(response, "")
 
         try:
             while 1:
                 ret = self.datahandler.handle_one(self)
                 if not ret:
@@ -590,25 +590,29 @@
             #print("Try again later.")
             #terminate(None, None)
             sys.exit(1)
 
 def signon_message():
 
     ''' message for the terminal '''
+
     if not conf.quiet:
         if not pyservsup.globals.conf.pmode:
             print("Warning! Devmode ON. Use -P to allow 2FA auth")
-        try:
-            strx = distro.name()
-        except:
-            strx = "Win or Unkn."
+
+        # Sat 04.May.2024 Dropped the distro, so can be installed on pipx
+        #try:
+        #    strx = distro.name()
+        #except:
+        #    strx = "Win or Unkn."
+
         print("MainSiteID:      ", pyservsup.globals.siteid)
         print("Server running: ", "'"+conf.host+"'", "Port:", conf.port)
         #pyver = support.list2str(sys.version_info) #[0:3], ".")
-        print("Running python", platform.python_version(), "on", platform.system(), strx)
+        print("Running python", platform.python_version(), "on", platform.system())
 
 def set_sigs():
 
     '''  set up signal handlers '''
     # Set termination handlers, so lock will be deleted
     signal.signal(signal.SIGTERM, terminate)
     signal.signal(signal.SIGINT, soft_terminate)
```

### Comparing `pyvserv-1.0.6/pyvserver/pyvstate.py` & `pyvserv-1.0.7/pyvserver/pyvstate.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvtools/docs/pyvgenkey.html` & `pyvserv-1.0.7/pyvtools/docs/pyvgenkey.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvtools/docs/pyvgenkeys.html` & `pyvserv-1.0.7/pyvtools/docs/pyvgenkeys.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvtools/pyvgenkey.py` & `pyvserv-1.0.7/pyvtools/pyvgenkey.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/pyvtools/pyvgenkeys.py` & `pyvserv-1.0.7/pyvtools/pyvgenkeys.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.6/setup.py` & `pyvserv-1.0.7/setup.py`

 * *Files identical despite different names*

