# Comparing `tmp/notebook-7.2.0rc0.tar.gz` & `tmp/notebook-7.2.0rc1.tar.gz`

## Comparing `notebook-7.2.0rc0.tar` & `notebook-7.2.0rc1.tar`

### file list

```diff
@@ -1,443 +1,443 @@
--rw-r--r--   0        0        0   201096 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/CHANGELOG.md
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/CONTRIBUTING.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/RELEASE.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/jupyter-notebook.desktop
--rw-r--r--   0        0        0    14487 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook.svg
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/package.json
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/tsconfig.eslint.json
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/tsconfigbase.json
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/tsconfigbase.test.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/jupyter-config/jupyter_server_config.d/notebook.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/node_modules/@jupyterlab/ui-components/style/icons/filetype/notebook.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/__main__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/_version.py
--rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/app.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/custom/custom.css
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/package.json
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/interface-switcher.json
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/launch-tree.json
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/package.json.orig
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/static/546.f643d3e7381a2d9b834f.js
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/static/568.c842f59b09a70d32fbf5.js
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/static/928.0be57dd4ecbedec78b46.js
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/static/93.eae3497dd223d842d198.js
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/static/remoteEntry.dbe55a308c2bef40bd5e.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/static/style.js
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/menus.json
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/package.json.orig
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/pages.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/shell.json
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/title.json
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/top.json
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/zen.json
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/documentsearch-extension/package.json.orig
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/help-extension/open.json
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/help-extension/package.json.orig
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/notebook-extension/checkpoints.json
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/notebook-extension/kernel-logo.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/notebook-extension/package.json.orig
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/notebook-extension/scroll-output.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/tree-extension/file-actions.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/tree-extension/package.json.orig
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/tree-extension/widget.json
--rw-r--r--   0        0        0    40298 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1053.bundle.js
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1088.bundle.js
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1091.bundle.js
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1122.bundle.js
--rw-r--r--   0        0        0    25832 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/113.bundle.js
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/114.bundle.js
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1169.bundle.js
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1198.bundle.js
--rw-r--r--   0        0        0    45520 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1261.bundle.js
--rw-r--r--   0        0        0   120311 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/131.bundle.js
--rw-r--r--   0        0        0   751525 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1326.bundle.js
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1326.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/134.bundle.js
--rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1388.bundle.js
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1408.bundle.js
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1418.bundle.js
--rw-r--r--   0        0        0   456718 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1495.bundle.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1495.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0    16688 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1496.bundle.js
--rw-r--r--   0        0        0   133211 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1542.bundle.js
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1542.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1558.bundle.js
--rw-r--r--   0        0        0    40776 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1584.bundle.js
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1618.bundle.js
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1647.bundle.js
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1650.bundle.js
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1684.bundle.js
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1696.bundle.js
--rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/170.bundle.js
--rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1809.bundle.js
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1827.bundle.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1828.bundle.js
--rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1833.bundle.js
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1837.bundle.js
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1846.bundle.js
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1869.bundle.js
--rw-r--r--   0        0        0   123638 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1884.bundle.js
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1941.bundle.js
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1958.bundle.js
--rw-r--r--   0        0        0    60657 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1962.bundle.js
--rw-r--r--   0        0        0    34160 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/1cb1c39ea642f26a4dfe.woff
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2007.bundle.js
--rw-r--r--   0        0        0   119944 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2065.bundle.js
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2088.bundle.js
--rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2089.bundle.js
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2122.bundle.js
--rw-r--r--   0        0        0    20897 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/214.bundle.js
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2167.bundle.js
--rw-r--r--   0        0        0    16587 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2184.bundle.js
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2188.bundle.js
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/221.bundle.js
--rw-r--r--   0        0        0    82023 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2241.bundle.js
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2311.bundle.js
--rw-r--r--   0        0        0    48217 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2323.bundle.js
--rw-r--r--   0        0        0  1481171 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2324.bundle.js
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2343.bundle.js
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2386.bundle.js
--rw-r--r--   0        0        0    29011 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2401.bundle.js
--rw-r--r--   0        0        0    45221 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2479.bundle.js
--rw-r--r--   0        0        0    33689 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2489.bundle.js
--rw-r--r--   0        0        0    29106 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2520.bundle.js
--rw-r--r--   0        0        0    54893 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2552.bundle.js
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2607.bundle.js
--rw-r--r--   0        0        0    37924 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/261.bundle.js
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2615.bundle.js
--rw-r--r--   0        0        0    18310 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2636.bundle.js
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2666.bundle.js
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/26683bf201fb258a2237.woff
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2682.bundle.js
--rw-r--r--   0        0        0    29991 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2692.bundle.js
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/270.bundle.js
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2702.bundle.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2756.bundle.js
--rw-r--r--   0        0        0    55533 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/28.bundle.js
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2813.bundle.js
--rw-r--r--   0        0        0    25782 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2866.bundle.js
--rw-r--r--   0        0        0     6665 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2871.bundle.js
--rw-r--r--   0        0        0   128623 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2913.bundle.js
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2913.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2924.bundle.js
--rw-r--r--   0        0        0    50041 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2944.bundle.js
--rw-r--r--   0        0        0   182907 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/2955.bundle.js
--rw-r--r--   0        0        0    35771 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3079.bundle.js
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/30e889b58cbc51adfbb0.woff
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/311.bundle.js
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3111.bundle.js
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3129.bundle.js
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3146.bundle.js
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3154.bundle.js
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3187.bundle.js
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3211.bundle.js
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3213.bundle.js
--rw-r--r--   0        0        0     6786 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3230.bundle.js
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/32792104b5ef69eded90.woff
--rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3301.bundle.js
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3322.bundle.js
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3325.bundle.js
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3336.bundle.js
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3340.bundle.js
--rw-r--r--   0        0        0    29122 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3360.bundle.js
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3370.bundle.js
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3420.bundle.js
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3449.bundle.js
--rw-r--r--   0        0        0    96169 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3462.bundle.js
--rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3466.bundle.js
--rw-r--r--   0        0        0    39408 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3488.bundle.js
--rw-r--r--   0        0        0    22195 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/35.bundle.js
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3501.bundle.js
--rw-r--r--   0        0        0   105135 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3512.bundle.js
--rw-r--r--   0        0        0    20832 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/355254db9ca10a09a3b5.woff
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3562.bundle.js
--rw-r--r--   0        0        0    94250 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3676.bundle.js
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3680.bundle.js
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/36e0d72d8a7afc696a3e.woff
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3700.bundle.js
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3733.bundle.js
--rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/373c04fd2418f5c77eea.eot
--rw-r--r--   0        0        0   125530 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/374.bundle.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3752.bundle.js
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3768.bundle.js
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/377.bundle.js
--rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3797.bundle.js
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3863.bundle.js
--rw-r--r--   0        0        0    21299 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3881.bundle.js
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3bc6ecaae7ecf6f8d7f8.woff
--rw-r--r--   0        0        0    40808 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3de784d07b9fa8f104c1.woff
--rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/3f6d3488cf65374f6f67.woff
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4002.bundle.js
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/403.bundle.js
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4030.bundle.js
--rw-r--r--   0        0        0    22183 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4035.bundle.js
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4038.bundle.js
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4039.bundle.js
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4042.bundle.js
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4058.bundle.js
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/409.bundle.js
--rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4105.bundle.js
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4148.bundle.js
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4212.bundle.js
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4271.bundle.js
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4291.bundle.js
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/431.bundle.js
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4382.bundle.js
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4387.bundle.js
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4430.bundle.js
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4498.bundle.js
--rw-r--r--   0        0        0    73759 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4499.bundle.js
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4521.bundle.js
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4526.bundle.js
--rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4588.bundle.js
--rw-r--r--   0        0        0   232362 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4630.bundle.js
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4630.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4645.bundle.js
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4670.bundle.js
--rw-r--r--   0        0        0   290991 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4708.bundle.js
--rw-r--r--   0        0        0    58945 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4780.bundle.js
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4810.bundle.js
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4811.bundle.js
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/481e39042508ae313a60.woff
--rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4825.bundle.js
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4837.bundle.js
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4843.bundle.js
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4965.bundle.js
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/4971.bundle.js
--rw-r--r--   0        0        0    27083 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5019.bundle.js
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5061.bundle.js
--rw-r--r--   0        0        0    39906 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5099.bundle.js
--rw-r--r--   0        0        0    55004 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5115.bundle.js
--rw-r--r--   0        0        0    12382 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5135.bundle.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5166.bundle.js
--rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5234.bundle.js
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5249.bundle.js
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5254.bundle.js
--rw-r--r--   0        0        0    22266 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5261.bundle.js
--rw-r--r--   0        0        0   142567 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5263.bundle.js
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5297.bundle.js
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5299.bundle.js
--rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5313.bundle.js
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5325.bundle.js
--rw-r--r--   0        0        0    25694 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5343.bundle.js
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5346.bundle.js
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5425.bundle.js
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5426.bundle.js
--rw-r--r--   0        0        0    15287 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/545.bundle.js
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5451.bundle.js
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5494.bundle.js
--rw-r--r--   0        0        0     8326 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5573.bundle.js
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5601.bundle.js
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5614.bundle.js
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/563.bundle.js
--rw-r--r--   0        0        0   154121 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5649.bundle.js
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5698.bundle.js
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5733.bundle.js
--rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5765.bundle.js
--rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5777.bundle.js
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5822.bundle.js
--rw-r--r--   0        0        0    26675 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5828.bundle.js
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5834.bundle.js
--rw-r--r--   0        0        0    79105 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5850.bundle.js
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5912.bundle.js
--rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5921.bundle.js
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5972.bundle.js
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5996.bundle.js
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/5cda41563a095bd70c78.woff
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6017.bundle.js
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6061.bundle.js
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6139.bundle.js
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/62.bundle.js
--rw-r--r--   0        0        0    43105 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6271.bundle.js
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6281.bundle.js
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/632.bundle.js
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6345.bundle.js
--rw-r--r--   0        0        0    10635 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6417.bundle.js
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/647.bundle.js
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6521.bundle.js
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6604.bundle.js
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/661.bundle.js
--rw-r--r--   0        0        0    69446 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6621.bundle.js
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6627.bundle.js
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6640.bundle.js
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6667.bundle.js
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/67.bundle.js
--rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6731.bundle.js
--rw-r--r--   0        0        0    25925 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6739.bundle.js
--rw-r--r--   0        0        0    14245 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6748.bundle.js
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/677.bundle.js
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6788.bundle.js
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6815.bundle.js
--rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6853.bundle.js
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6893.bundle.js
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/69.bundle.js
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/690.bundle.js
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6942.bundle.js
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6962.bundle.js
--rw-r--r--   0        0        0    71127 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6972.bundle.js
--rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/6999.bundle.js
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7005.bundle.js
--rw-r--r--   0        0        0    37240 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7010.bundle.js
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7022.bundle.js
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7054.bundle.js
--rw-r--r--   0        0        0    24130 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7097.bundle.js
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7153.bundle.js
--rw-r--r--   0        0        0    79037 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7154.bundle.js
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7170.bundle.js
--rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7179.bundle.js
--rw-r--r--   0        0        0    22340 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/721921bab0d001ebff02.woff
--rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7226.bundle.js
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7252.bundle.js
--rw-r--r--   0        0        0    50957 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7259.bundle.js
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7264.bundle.js
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/72bc573386dd1d48c5bb.woff
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7302.bundle.js
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7360.bundle.js
--rw-r--r--   0        0        0   210656 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7369.bundle.js
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7378.bundle.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7378.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7386.bundle.js
--rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7391.bundle.js
--rw-r--r--   0        0        0    67961 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7427.bundle.js
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/745.bundle.js
--rw-r--r--   0        0        0    27539 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7450.bundle.js
--rw-r--r--   0        0        0    38950 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7471.bundle.js
--rw-r--r--   0        0        0   249944 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7506.bundle.js
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7506.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7534.bundle.js
--rw-r--r--   0        0        0    23183 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7543.bundle.js
--rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/755.bundle.js
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7582.bundle.js
--rw-r--r--   0        0        0    27079 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7603.bundle.js
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7639.bundle.js
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7655.bundle.js
--rw-r--r--   0        0        0   101788 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7674.bundle.js
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7679.bundle.js
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7684.bundle.js
--rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7796.bundle.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7796.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7803.bundle.js
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7811.bundle.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7811.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7812.bundle.js
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7817.bundle.js
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7819.bundle.js
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7821.bundle.js
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7854.bundle.js
--rw-r--r--   0        0        0    28770 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7866.bundle.js
--rw-r--r--   0        0        0   102421 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7884.bundle.js
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7900.bundle.js
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7906.bundle.js
--rw-r--r--   0        0        0    14397 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/792.bundle.js
--rw-r--r--   0        0        0    88000 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7957.bundle.js
--rw-r--r--   0        0        0    60153 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7969.bundle.js
--rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7995.bundle.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7995.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/7997.bundle.js
--rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/79d088064beb3826054f.eot
--rw-r--r--   0        0        0    95138 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8010.bundle.js
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8032.bundle.js
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8060.bundle.js
--rw-r--r--   0        0        0    15277 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8285.bundle.js
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8378.bundle.js
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8381.bundle.js
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8433.bundle.js
--rw-r--r--   0        0        0    31497 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8443.bundle.js
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8446.bundle.js
--rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8471.bundle.js
--rw-r--r--   0        0        0    37190 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8479.bundle.js
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/85.bundle.js
--rw-r--r--   0        0        0    13993 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8579.bundle.js
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8633.bundle.js
--rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/870673df72e70f87c91a.woff
--rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8768.bundle.js
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8771.bundle.js
--rw-r--r--   0        0        0    32886 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8781.bundle.js
--rw-r--r--   0        0        0    17597 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8801.bundle.js
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/883.bundle.js
--rw-r--r--   0        0        0   197078 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8845.bundle.js
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8845.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8875.bundle.js
--rw-r--r--   0        0        0    34464 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/88b98cad3688915e50da.woff
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8907.bundle.js
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8928.bundle.js
--rw-r--r--   0        0        0   122744 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8929.bundle.js
--rw-r--r--   0        0        0    20114 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/893.bundle.js
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8937.bundle.js
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8979.bundle.js
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8983.bundle.js
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/899.bundle.js
--rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8ea8791754915a898a31.woff2
--rw-r--r--   0        0        0    19776 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/8ea8dbb1b02e6f730f55.woff
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/901.bundle.js
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9022.bundle.js
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9037.bundle.js
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/906.bundle.js
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9060.bundle.js
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9068.bundle.js
--rw-r--r--   0        0        0   145674 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/911.bundle.js
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9116.bundle.js
--rw-r--r--   0        0        0   512648 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9136.bundle.js
--rw-r--r--   0        0        0    63709 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9151.bundle.js
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9161.bundle.js
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9222.bundle.js
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9233.bundle.js
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9234.bundle.js
--rw-r--r--   0        0        0    22448 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9239.bundle.js
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9250.bundle.js
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9268.bundle.js
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9331.bundle.js
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9335.bundle.js
--rw-r--r--   0        0        0    55528 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9341.bundle.js
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9380.bundle.js
--rw-r--r--   0        0        0    22234 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9425.bundle.js
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9558.bundle.js
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9604.bundle.js
--rw-r--r--   0        0        0   278958 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9605.bundle.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9605.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9638.bundle.js
--rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9674eb1bd55047179038.svg
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9676.bundle.js
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9680.bundle.js
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9685.bundle.js
--rw-r--r--   0        0        0    87653 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9752.bundle.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9752.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0    40964 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9799.bundle.js
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9821.bundle.js
--rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9834b82ad26e2a37583d.woff2
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9852.bundle.js
--rw-r--r--   0        0        0    35474 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/9866.bundle.js
--rw-r--r--   0        0        0    19360 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/a009bea404f7a500ded4.woff
--rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/a3b9817780214caf01e8.svg
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/af04542b29eaac04550a.woff
--rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/af6397503fcefbd61397.ttf
--rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/af96f67d7accf5fd2a4a.woff
--rw-r--r--   0        0        0    12660 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/b418136e3b384baaadec.woff
--rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/be0a084962d8066884f7.svg
--rw-r--r--   0        0        0    54559 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/bundle.js
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/c49810b53ecc0d87d802.woff
--rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/c56da8d69f1a0208b8e0.woff
--rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/cb9e9e693192413cde2b.woff
--rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/cda59d6efffa685830fd.ttf
--rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/e4299464e7b012968eed.eot
--rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/e42a88444448ac3d6054.woff2
--rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/e8711bbb871afd8e9dea.ttf
--rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/f9217f66874b0c01cd8c.woff
--rw-r--r--   0        0        0    14628 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/fc6ddf5df402b263cfb1.woff
--rw-r--r--   0        0        0   407631 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/static/third-party-licenses.json
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/templates/consoles.html
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/templates/edit.html
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/templates/error.html
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/templates/notebooks.html
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/templates/terminals.html
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/notebook/templates/tree.html
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/tests/conftest.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/tests/test_app.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/LICENSE
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/README.md
--rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/pyproject.toml
--rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 notebook-7.2.0rc0/PKG-INFO
+-rw-r--r--   0        0        0   202699 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/RELEASE.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/jupyter-notebook.desktop
+-rw-r--r--   0        0        0    14487 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook.svg
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/package.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/tsconfigbase.json
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/tsconfigbase.test.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/jupyter-config/jupyter_server_config.d/notebook.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/node_modules/@jupyterlab/ui-components/style/icons/filetype/notebook.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/__main__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/_version.py
+-rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/app.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/custom/custom.css
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/package.json
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/interface-switcher.json
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/launch-tree.json
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/package.json.orig
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/static/302.8a8d0af0376cb309e580.js
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/static/568.1176453d31b84477bbd4.js
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/static/928.76f40c4b4ee1c8583ca3.js
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/static/93.eae3497dd223d842d198.js
+-rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/static/remoteEntry.a5e570ba118d1d45c877.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/static/style.js
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/menus.json
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/package.json.orig
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/pages.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/shell.json
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/title.json
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/top.json
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/zen.json
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/documentsearch-extension/package.json.orig
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/help-extension/open.json
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/help-extension/package.json.orig
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/notebook-extension/checkpoints.json
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/notebook-extension/kernel-logo.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/notebook-extension/package.json.orig
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/notebook-extension/scroll-output.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/tree-extension/file-actions.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/tree-extension/package.json.orig
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/tree-extension/widget.json
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1088.bundle.js
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1091.bundle.js
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1122.bundle.js
+-rw-r--r--   0        0        0    25832 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/113.bundle.js
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/114.bundle.js
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1169.bundle.js
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1198.bundle.js
+-rw-r--r--   0        0        0    45520 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1261.bundle.js
+-rw-r--r--   0        0        0   120311 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/131.bundle.js
+-rw-r--r--   0        0        0   751525 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1326.bundle.js
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1326.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/134.bundle.js
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1388.bundle.js
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1408.bundle.js
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1418.bundle.js
+-rw-r--r--   0        0        0   456718 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1495.bundle.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1495.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0    16690 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1496.bundle.js
+-rw-r--r--   0        0        0   133211 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1542.bundle.js
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1542.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1558.bundle.js
+-rw-r--r--   0        0        0    40776 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1584.bundle.js
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1618.bundle.js
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1647.bundle.js
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1650.bundle.js
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1684.bundle.js
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1696.bundle.js
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/170.bundle.js
+-rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1809.bundle.js
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1827.bundle.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1828.bundle.js
+-rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1833.bundle.js
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1837.bundle.js
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1846.bundle.js
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1869.bundle.js
+-rw-r--r--   0        0        0   123638 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1884.bundle.js
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1941.bundle.js
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1958.bundle.js
+-rw-r--r--   0        0        0    60684 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1962.bundle.js
+-rw-r--r--   0        0        0    34160 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/1cb1c39ea642f26a4dfe.woff
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2007.bundle.js
+-rw-r--r--   0        0        0   119944 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2065.bundle.js
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2088.bundle.js
+-rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2089.bundle.js
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2122.bundle.js
+-rw-r--r--   0        0        0    20897 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/214.bundle.js
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2167.bundle.js
+-rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2184.bundle.js
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2188.bundle.js
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/221.bundle.js
+-rw-r--r--   0        0        0    82023 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2241.bundle.js
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2311.bundle.js
+-rw-r--r--   0        0        0    48217 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2323.bundle.js
+-rw-r--r--   0        0        0  1481171 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2324.bundle.js
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2343.bundle.js
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2386.bundle.js
+-rw-r--r--   0        0        0    29013 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2401.bundle.js
+-rw-r--r--   0        0        0    45222 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2479.bundle.js
+-rw-r--r--   0        0        0    33690 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2489.bundle.js
+-rw-r--r--   0        0        0    29106 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2520.bundle.js
+-rw-r--r--   0        0        0    54893 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2552.bundle.js
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2607.bundle.js
+-rw-r--r--   0        0        0    37924 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/261.bundle.js
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2615.bundle.js
+-rw-r--r--   0        0        0    18311 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2636.bundle.js
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2666.bundle.js
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/26683bf201fb258a2237.woff
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2682.bundle.js
+-rw-r--r--   0        0        0    29991 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2692.bundle.js
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/270.bundle.js
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2702.bundle.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2756.bundle.js
+-rw-r--r--   0        0        0    55533 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/28.bundle.js
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2813.bundle.js
+-rw-r--r--   0        0        0    25782 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2866.bundle.js
+-rw-r--r--   0        0        0     6665 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2871.bundle.js
+-rw-r--r--   0        0        0   128623 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2913.bundle.js
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2913.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2924.bundle.js
+-rw-r--r--   0        0        0    50042 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2944.bundle.js
+-rw-r--r--   0        0        0   182907 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/2955.bundle.js
+-rw-r--r--   0        0        0    35771 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3079.bundle.js
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/30e889b58cbc51adfbb0.woff
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/311.bundle.js
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3111.bundle.js
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3129.bundle.js
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3146.bundle.js
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3154.bundle.js
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3187.bundle.js
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3211.bundle.js
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3213.bundle.js
+-rw-r--r--   0        0        0     6786 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3230.bundle.js
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/32792104b5ef69eded90.woff
+-rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3301.bundle.js
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3322.bundle.js
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3325.bundle.js
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3336.bundle.js
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3340.bundle.js
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3360.bundle.js
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3370.bundle.js
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3420.bundle.js
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3449.bundle.js
+-rw-r--r--   0        0        0    96169 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3462.bundle.js
+-rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3466.bundle.js
+-rw-r--r--   0        0        0    39408 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3488.bundle.js
+-rw-r--r--   0        0        0    22195 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/35.bundle.js
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3501.bundle.js
+-rw-r--r--   0        0        0   105136 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3512.bundle.js
+-rw-r--r--   0        0        0    20832 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/355254db9ca10a09a3b5.woff
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3562.bundle.js
+-rw-r--r--   0        0        0    94265 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3676.bundle.js
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3680.bundle.js
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/36e0d72d8a7afc696a3e.woff
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3700.bundle.js
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3733.bundle.js
+-rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/373c04fd2418f5c77eea.eot
+-rw-r--r--   0        0        0   125908 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/374.bundle.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3752.bundle.js
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3768.bundle.js
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/377.bundle.js
+-rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3797.bundle.js
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3863.bundle.js
+-rw-r--r--   0        0        0    21301 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3881.bundle.js
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3bc6ecaae7ecf6f8d7f8.woff
+-rw-r--r--   0        0        0    40808 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3de784d07b9fa8f104c1.woff
+-rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/3f6d3488cf65374f6f67.woff
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4002.bundle.js
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/403.bundle.js
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4030.bundle.js
+-rw-r--r--   0        0        0    22183 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4035.bundle.js
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4038.bundle.js
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4039.bundle.js
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4042.bundle.js
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4058.bundle.js
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/409.bundle.js
+-rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4105.bundle.js
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4148.bundle.js
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4212.bundle.js
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4271.bundle.js
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4291.bundle.js
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/431.bundle.js
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4382.bundle.js
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4387.bundle.js
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4430.bundle.js
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4498.bundle.js
+-rw-r--r--   0        0        0    73759 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4499.bundle.js
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4521.bundle.js
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4526.bundle.js
+-rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4588.bundle.js
+-rw-r--r--   0        0        0   232362 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4630.bundle.js
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4630.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4645.bundle.js
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4670.bundle.js
+-rw-r--r--   0        0        0   290991 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4708.bundle.js
+-rw-r--r--   0        0        0    58945 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4780.bundle.js
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4810.bundle.js
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4811.bundle.js
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/481e39042508ae313a60.woff
+-rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4825.bundle.js
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4837.bundle.js
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4843.bundle.js
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4965.bundle.js
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/4971.bundle.js
+-rw-r--r--   0        0        0    27083 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5019.bundle.js
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5061.bundle.js
+-rw-r--r--   0        0        0    39908 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5099.bundle.js
+-rw-r--r--   0        0        0    55004 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5115.bundle.js
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5135.bundle.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5166.bundle.js
+-rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5234.bundle.js
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5249.bundle.js
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5254.bundle.js
+-rw-r--r--   0        0        0    22266 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5261.bundle.js
+-rw-r--r--   0        0        0   142637 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5263.bundle.js
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5297.bundle.js
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5299.bundle.js
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5313.bundle.js
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5325.bundle.js
+-rw-r--r--   0        0        0    25694 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5343.bundle.js
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5346.bundle.js
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5425.bundle.js
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5426.bundle.js
+-rw-r--r--   0        0        0    15288 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/545.bundle.js
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5451.bundle.js
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5494.bundle.js
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5573.bundle.js
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5601.bundle.js
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5614.bundle.js
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/563.bundle.js
+-rw-r--r--   0        0        0   154121 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5649.bundle.js
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5698.bundle.js
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5733.bundle.js
+-rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5765.bundle.js
+-rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5777.bundle.js
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5822.bundle.js
+-rw-r--r--   0        0        0    26675 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5828.bundle.js
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5834.bundle.js
+-rw-r--r--   0        0        0    79105 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5850.bundle.js
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5912.bundle.js
+-rw-r--r--   0        0        0    10859 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5921.bundle.js
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5972.bundle.js
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5996.bundle.js
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/5cda41563a095bd70c78.woff
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6017.bundle.js
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6061.bundle.js
+-rw-r--r--   0        0        0    40298 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6078.bundle.js
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6139.bundle.js
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/62.bundle.js
+-rw-r--r--   0        0        0    43105 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6271.bundle.js
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6281.bundle.js
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/632.bundle.js
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6345.bundle.js
+-rw-r--r--   0        0        0    10635 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6417.bundle.js
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/647.bundle.js
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6521.bundle.js
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6604.bundle.js
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/661.bundle.js
+-rw-r--r--   0        0        0    69447 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6621.bundle.js
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6627.bundle.js
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6640.bundle.js
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6667.bundle.js
+-rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/67.bundle.js
+-rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6731.bundle.js
+-rw-r--r--   0        0        0    25925 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6739.bundle.js
+-rw-r--r--   0        0        0    14246 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6748.bundle.js
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/677.bundle.js
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6788.bundle.js
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6815.bundle.js
+-rw-r--r--   0        0        0    38124 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6853.bundle.js
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6893.bundle.js
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/69.bundle.js
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/690.bundle.js
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6942.bundle.js
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6962.bundle.js
+-rw-r--r--   0        0        0    71127 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6972.bundle.js
+-rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/6999.bundle.js
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7005.bundle.js
+-rw-r--r--   0        0        0    37240 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7010.bundle.js
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7022.bundle.js
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7054.bundle.js
+-rw-r--r--   0        0        0    24130 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7097.bundle.js
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7153.bundle.js
+-rw-r--r--   0        0        0    79037 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7154.bundle.js
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7170.bundle.js
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7179.bundle.js
+-rw-r--r--   0        0        0    22340 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/721921bab0d001ebff02.woff
+-rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7226.bundle.js
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7252.bundle.js
+-rw-r--r--   0        0        0    50957 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7259.bundle.js
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7264.bundle.js
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/72bc573386dd1d48c5bb.woff
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7302.bundle.js
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7360.bundle.js
+-rw-r--r--   0        0        0   210656 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7369.bundle.js
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7378.bundle.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7378.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7386.bundle.js
+-rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7391.bundle.js
+-rw-r--r--   0        0        0    67961 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7427.bundle.js
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/745.bundle.js
+-rw-r--r--   0        0        0    27539 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7450.bundle.js
+-rw-r--r--   0        0        0    38950 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7471.bundle.js
+-rw-r--r--   0        0        0   249964 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7506.bundle.js
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7506.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7534.bundle.js
+-rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7543.bundle.js
+-rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/755.bundle.js
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7582.bundle.js
+-rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7603.bundle.js
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7639.bundle.js
+-rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7655.bundle.js
+-rw-r--r--   0        0        0   101788 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7674.bundle.js
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7679.bundle.js
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7684.bundle.js
+-rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7796.bundle.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7796.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7803.bundle.js
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7811.bundle.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7811.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7812.bundle.js
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7817.bundle.js
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7819.bundle.js
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7821.bundle.js
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7854.bundle.js
+-rw-r--r--   0        0        0    28770 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7866.bundle.js
+-rw-r--r--   0        0        0   102421 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7884.bundle.js
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7900.bundle.js
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7906.bundle.js
+-rw-r--r--   0        0        0    14397 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/792.bundle.js
+-rw-r--r--   0        0        0    88000 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7957.bundle.js
+-rw-r--r--   0        0        0    60153 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7969.bundle.js
+-rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7995.bundle.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7995.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/7997.bundle.js
+-rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/79d088064beb3826054f.eot
+-rw-r--r--   0        0        0    95138 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8010.bundle.js
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8032.bundle.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8060.bundle.js
+-rw-r--r--   0        0        0    15277 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8285.bundle.js
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8378.bundle.js
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8381.bundle.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8433.bundle.js
+-rw-r--r--   0        0        0    31497 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8443.bundle.js
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8446.bundle.js
+-rw-r--r--   0        0        0    18683 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8471.bundle.js
+-rw-r--r--   0        0        0    37190 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8479.bundle.js
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/85.bundle.js
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8579.bundle.js
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8633.bundle.js
+-rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/870673df72e70f87c91a.woff
+-rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8768.bundle.js
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8771.bundle.js
+-rw-r--r--   0        0        0    32578 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8781.bundle.js
+-rw-r--r--   0        0        0    17597 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8801.bundle.js
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/883.bundle.js
+-rw-r--r--   0        0        0   197078 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8845.bundle.js
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8845.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8875.bundle.js
+-rw-r--r--   0        0        0    34464 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/88b98cad3688915e50da.woff
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8907.bundle.js
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8928.bundle.js
+-rw-r--r--   0        0        0   122744 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8929.bundle.js
+-rw-r--r--   0        0        0    20115 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/893.bundle.js
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8937.bundle.js
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8979.bundle.js
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8983.bundle.js
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/899.bundle.js
+-rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8ea8791754915a898a31.woff2
+-rw-r--r--   0        0        0    19776 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/8ea8dbb1b02e6f730f55.woff
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/901.bundle.js
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9022.bundle.js
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9037.bundle.js
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/906.bundle.js
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9060.bundle.js
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9068.bundle.js
+-rw-r--r--   0        0        0   145674 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/911.bundle.js
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9116.bundle.js
+-rw-r--r--   0        0        0   512648 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9136.bundle.js
+-rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9151.bundle.js
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9161.bundle.js
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9222.bundle.js
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9233.bundle.js
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9234.bundle.js
+-rw-r--r--   0        0        0    22448 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9239.bundle.js
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9250.bundle.js
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9268.bundle.js
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9331.bundle.js
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9335.bundle.js
+-rw-r--r--   0        0        0    55528 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9341.bundle.js
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9380.bundle.js
+-rw-r--r--   0        0        0    22234 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9425.bundle.js
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9558.bundle.js
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9604.bundle.js
+-rw-r--r--   0        0        0   278959 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9605.bundle.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9605.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9638.bundle.js
+-rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9674eb1bd55047179038.svg
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9676.bundle.js
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9680.bundle.js
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9685.bundle.js
+-rw-r--r--   0        0        0    87653 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9752.bundle.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9752.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0    40964 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9799.bundle.js
+-rw-r--r--   0        0        0    10072 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9821.bundle.js
+-rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9834b82ad26e2a37583d.woff2
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9852.bundle.js
+-rw-r--r--   0        0        0    35474 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/9866.bundle.js
+-rw-r--r--   0        0        0    19360 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/a009bea404f7a500ded4.woff
+-rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/a3b9817780214caf01e8.svg
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/af04542b29eaac04550a.woff
+-rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/af6397503fcefbd61397.ttf
+-rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/af96f67d7accf5fd2a4a.woff
+-rw-r--r--   0        0        0    12660 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/b418136e3b384baaadec.woff
+-rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/be0a084962d8066884f7.svg
+-rw-r--r--   0        0        0    53489 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/bundle.js
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/c49810b53ecc0d87d802.woff
+-rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/c56da8d69f1a0208b8e0.woff
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/cb9e9e693192413cde2b.woff
+-rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/cda59d6efffa685830fd.ttf
+-rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/e4299464e7b012968eed.eot
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/e42a88444448ac3d6054.woff2
+-rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/e8711bbb871afd8e9dea.ttf
+-rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/f9217f66874b0c01cd8c.woff
+-rw-r--r--   0        0        0    14628 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/fc6ddf5df402b263cfb1.woff
+-rw-r--r--   0        0        0   407181 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/templates/consoles.html
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/templates/edit.html
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/templates/error.html
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/templates/notebooks.html
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/templates/terminals.html
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/notebook/templates/tree.html
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/tests/test_app.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/README.md
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 notebook-7.2.0rc1/PKG-INFO
```

### Comparing `notebook-7.2.0rc0/CHANGELOG.md` & `notebook-7.2.0rc1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,39 @@
 - The current theme (dark/light) can now be synced with the browser/system preference (Settings menu → Theme → Synchronise with System Settings)
 - A blue "read-only" status indicator is now  displayed in the toolbar of documents which cannot be saved because their model is read-only.
 - Native support for viewing jsonl/ndjson files was added
 - Collapsing of breadcrumbs in the File Browser can be disabled in File Browser settings
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 7.2.0rc1
+
+([Full Changelog](https://github.com/jupyter/notebook/compare/v7.2.0rc0...f5d8aea3bdc3eea25213792f9d101738f2a1f627))
+
+### Enhancements made
+
+- Update to JupyterLab 4.2.0 [#7357](https://github.com/jupyter/notebook/pull/7357) ([@jtpio](https://github.com/jtpio))
+
+### Bugs fixed
+
+- Add the `@jupyterlab/notebook-extension:copy-output` plugin [#7353](https://github.com/jupyter/notebook/pull/7353) ([@jtpio](https://github.com/jtpio))
+- Default to the `full` windowing mode [#7321](https://github.com/jupyter/notebook/pull/7321) ([@jtpio](https://github.com/jtpio))
+
+### Documentation improvements
+
+- update RISE extension installation instructions [#7299](https://github.com/jupyter/notebook/pull/7299) ([@afeld](https://github.com/afeld))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/notebook/graphs/contributors?from=2024-05-01&to=2024-05-13&type=c))
+
+[@afeld](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Aafeld+updated%3A2024-05-01..2024-05-13&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Agithub-actions+updated%3A2024-05-01..2024-05-13&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Ajtpio+updated%3A2024-05-01..2024-05-13&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Akrassowski+updated%3A2024-05-01..2024-05-13&type=Issues) | [@takluyver](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Atakluyver+updated%3A2024-05-01..2024-05-13&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 7.2.0rc0
 
 ([Full Changelog](https://github.com/jupyter/notebook/compare/v7.2.0b1...49ddd0fe1e4d4bfa24f74042f2232c5b91d1c36e))
 
 ### Enhancements made
 
 - Update to JupyterLab 4.2.0rc0 [#7333](https://github.com/jupyter/notebook/pull/7333) ([@jtpio](https://github.com/jtpio))
@@ -126,16 +151,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/notebook/graphs/contributors?from=2024-04-19&to=2024-05-01&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Agithub-actions+updated%3A2024-04-19..2024-05-01&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Ajtpio+updated%3A2024-04-19..2024-05-01&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Akrassowski+updated%3A2024-04-19..2024-05-01&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 7.2.0b1
 
 ([Full Changelog](https://github.com/jupyter/notebook/compare/@jupyter-notebook/application-extension@7.2.0-beta.0...b45d666d5ee1ee053b55ac9cb6e9aecde5d53945))
 
 ### Enhancements made
 
 - Add `@jupyterlab/theme-dark-high-contrast-extension` [#7331](https://github.com/jupyter/notebook/pull/7331) ([@jtpio](https://github.com/jtpio))
```

### Comparing `notebook-7.2.0rc0/CONTRIBUTING.md` & `notebook-7.2.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/RELEASE.md` & `notebook-7.2.0rc1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook.svg` & `notebook-7.2.0rc1/notebook.svg`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/package.json` & `notebook-7.2.0rc1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985207100591715%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/buildutils': '~4.2.0'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "devDependencies": {
-        "@jupyterlab/buildutils": "~4.2.0-rc.0",
+        "@jupyterlab/buildutils": "~4.2.0",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
         "eslint-plugin-jest": "^27.2.1",
         "eslint-plugin-prettier": "^4.2.1",
         "eslint-plugin-react": "^7.32.2",
```

### Comparing `notebook-7.2.0rc0/notebook/__init__.py` & `notebook-7.2.0rc1/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/_version.py` & `notebook-7.2.0rc1/notebook/_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version info for notebook."""
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 import re
 from collections import namedtuple
 
 # Use "hatch version xx.yy.zz" to handle version changes
-__version__ = "7.2.0rc0"
+__version__ = "7.2.0rc1"
 
 # PEP440 version parser
 _version_regex = re.compile(
     r"""
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `notebook-7.2.0rc0/notebook/app.py` & `notebook-7.2.0rc1/notebook/app.py`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/labextension/package.json` & `notebook-7.2.0rc1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/package.json.orig`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9567460317460318%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-rc.1', '@jupyterlab/application': "*

 * *                   "'~4.2.0', '@jupyterlab/apputils': '~4.3.0', '@jupyterlab/coreutils': '~6.2.0', "*

 * *                   "'@jupyterlab/docregistry': '~4.2.0', '@jupyterlab/notebook': '~4.2.0', "*

 * *                   "'@jupyterlab/translation': '~4.2.0', '@jupyterlab/ui-components': '~4.2.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '~4.2.0'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'7.2.0- […]*

```diff
@@ -1,27 +1,27 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-rc.0",
-        "@jupyterlab/application": "~4.2.0-rc.0",
-        "@jupyterlab/apputils": "~4.3.0-rc.0",
-        "@jupyterlab/coreutils": "~6.2.0-rc.0",
-        "@jupyterlab/docregistry": "~4.2.0-rc.0",
-        "@jupyterlab/notebook": "~4.2.0-rc.0",
-        "@jupyterlab/translation": "~4.2.0-rc.0",
-        "@jupyterlab/ui-components": "~4.2.0-rc.0",
+        "@jupyter-notebook/application": "^7.2.0-rc.1",
+        "@jupyterlab/application": "~4.2.0",
+        "@jupyterlab/apputils": "~4.3.0",
+        "@jupyterlab/coreutils": "~6.2.0",
+        "@jupyterlab/docregistry": "~4.2.0",
+        "@jupyterlab/notebook": "~4.2.0",
+        "@jupyterlab/translation": "~4.2.0",
+        "@jupyterlab/ui-components": "~4.2.0",
         "@lumino/commands": "^2.3.0",
         "@lumino/disposable": "^2.1.2"
     },
     "description": "Jupyter Notebook - Lab Extension",
     "devDependencies": {
-        "@jupyterlab/builder": "~4.2.0-rc.0",
+        "@jupyterlab/builder": "~4.2.0",
         "rimraf": "^3.0.2",
         "typescript": "~5.0.2"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
@@ -29,19 +29,14 @@
         "lib/*.js.map",
         "lib/*.js",
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyter/notebook",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.dbe55a308c2bef40bd5e.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../../notebook/labextension",
         "schemaDir": "schema"
     },
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@jupyter-notebook/lab-extension",
@@ -101,9 +96,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-rc.0"
+    "version": "7.2.0-rc.1"
 }
```

### Comparing `notebook-7.2.0rc0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/interface-switcher.json` & `notebook-7.2.0rc1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/interface-switcher.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/package.json.orig` & `notebook-7.2.0rc1/notebook/labextension/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9567460317460318%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-rc.1', '@jupyterlab/application': "*

 * *                   "'~4.2.0', '@jupyterlab/apputils': '~4.3.0', '@jupyterlab/coreutils': '~6.2.0', "*

 * *                   "'@jupyterlab/docregistry': '~4.2.0', '@jupyterlab/notebook': '~4.2.0', "*

 * *                   "'@jupyterlab/translation': '~4.2.0', '@jupyterlab/ui-components': '~4.2.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '~4.2.0'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remo […]*

```diff
@@ -1,27 +1,27 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-rc.0",
-        "@jupyterlab/application": "~4.2.0-rc.0",
-        "@jupyterlab/apputils": "~4.3.0-rc.0",
-        "@jupyterlab/coreutils": "~6.2.0-rc.0",
-        "@jupyterlab/docregistry": "~4.2.0-rc.0",
-        "@jupyterlab/notebook": "~4.2.0-rc.0",
-        "@jupyterlab/translation": "~4.2.0-rc.0",
-        "@jupyterlab/ui-components": "~4.2.0-rc.0",
+        "@jupyter-notebook/application": "^7.2.0-rc.1",
+        "@jupyterlab/application": "~4.2.0",
+        "@jupyterlab/apputils": "~4.3.0",
+        "@jupyterlab/coreutils": "~6.2.0",
+        "@jupyterlab/docregistry": "~4.2.0",
+        "@jupyterlab/notebook": "~4.2.0",
+        "@jupyterlab/translation": "~4.2.0",
+        "@jupyterlab/ui-components": "~4.2.0",
         "@lumino/commands": "^2.3.0",
         "@lumino/disposable": "^2.1.2"
     },
     "description": "Jupyter Notebook - Lab Extension",
     "devDependencies": {
-        "@jupyterlab/builder": "~4.2.0-rc.0",
+        "@jupyterlab/builder": "~4.2.0",
         "rimraf": "^3.0.2",
         "typescript": "~5.0.2"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
@@ -29,14 +29,19 @@
         "lib/*.js.map",
         "lib/*.js",
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyter/notebook",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.a5e570ba118d1d45c877.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "../../notebook/labextension",
         "schemaDir": "schema"
     },
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@jupyter-notebook/lab-extension",
@@ -96,9 +101,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-rc.0"
+    "version": "7.2.0-rc.1"
 }
```

### Comparing `notebook-7.2.0rc0/notebook/labextension/static/546.f643d3e7381a2d9b834f.js` & `notebook-7.2.0rc1/notebook/labextension/static/302.8a8d0af0376cb309e580.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,34 @@
 "use strict";
 (self.webpackChunk_jupyter_notebook_lab_extension = self.webpackChunk_jupyter_notebook_lab_extension || []).push([
-    [546], {
+    [302], {
         30: (e, t, i) => {
             i.r(t), i.d(t, {
                 INotebookPathOpener: () => C,
                 INotebookShell: () => y,
                 NotebookApp: () => H,
                 NotebookShell: () => k,
                 PanelHandler: () => f,
                 Private: () => v,
                 SidePanelHandler: () => w,
                 SidePanelPalette: () => W,
                 defaultNotebookPathOpener: () => P
             });
-            var s, n = i(666),
-                r = i(957),
+            var s, n = i(898),
+                r = i(517),
                 a = i(950),
                 o = i(448),
-                d = i(268),
+                d = i(363),
                 l = i(797),
-                h = i(545),
+                h = i(715),
                 p = i(697),
                 g = i(930),
                 u = i(901),
                 c = i(882),
-                _ = i(454),
+                _ = i(944),
                 m = i(633);
             class f {
                 constructor() {
                     this._panelChildHook = (e, t) => {
                         if ("child-removed" === t.type) {
                             const e = t.child;
                             p.ArrayExt.removeFirstWhere(this._items, (t => t.widget === e))
```

### Comparing `notebook-7.2.0rc0/notebook/labextension/static/568.c842f59b09a70d32fbf5.js` & `notebook-7.2.0rc1/notebook/labextension/static/568.1176453d31b84477bbd4.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_jupyter_notebook_lab_extension = self.webpackChunk_jupyter_notebook_lab_extension || []).push([
     [568], {
         568: (e, o, t) => {
             t.r(o), t.d(o, {
                 default: () => m
             });
-            var n, a = t(666),
-                r = t(834),
-                c = t(268),
-                l = t(73),
-                i = t(545),
+            var n, a = t(898),
+                r = t(712),
+                c = t(363),
+                l = t(793),
+                i = t(715),
                 s = t(882),
-                b = t(758),
-                d = t(454);
+                b = t(616),
+                d = t(944);
             ! function(e) {
                 e.launchNotebookTree = "jupyter-notebook:launch-tree", e.openNotebook = "jupyter-notebook:open-notebook", e.openLab = "jupyter-notebook:open-lab", e.openNbClassic = "jupyter-notebook:open-nbclassic"
             }(n || (n = {}));
             const u = {
                     id: "@jupyter-notebook/lab-extension:interface-switcher",
                     description: "A plugin to add custom toolbar items to the notebook page.",
                     autoStart: !0,
```

### Comparing `notebook-7.2.0rc0/notebook/labextension/static/928.0be57dd4ecbedec78b46.js` & `notebook-7.2.0rc1/notebook/labextension/static/928.76f40c4b4ee1c8583ca3.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_jupyter_notebook_lab_extension = self.webpackChunk_jupyter_notebook_lab_extension || []).push([
     [928], {
         950: (t, e, r) => {
             r.d(e, {
                 as: () => p
             });
-            var n = r(834),
-                i = r(957),
-                a = r(515),
-                o = r(545),
-                s = r(454),
+            var n = r(712),
+                i = r(517),
+                a = r(505),
+                o = r(715),
+                s = r(944),
                 c = r(930),
                 d = r(4);
             const u = new c.Token("@jupyterlab/application:ILayoutRestorer", "A service providing application layout restoration functionality. Use this to have your activities restored across page loads.");
             var y;
             ! function(t) {
                 function e(r) {
                     return r && r.type ? "tab-area" === r.type ? {
```

### Comparing `notebook-7.2.0rc0/notebook/labextension/static/93.eae3497dd223d842d198.js` & `notebook-7.2.0rc1/notebook/labextension/static/93.eae3497dd223d842d198.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/labextension/static/remoteEntry.dbe55a308c2bef40bd5e.js` & `notebook-7.2.0rc1/notebook/labextension/static/remoteEntry.a5e570ba118d1d45c877.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, n, a, i, l, u, s, d, f, c, p, h, b, v, m, g, y, j, w, k, S = {
+    var e, r, t, o, n, a, i, l, u, s, f, d, p, c, b, h, v, m, g, y, j, w, k, S = {
             215: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(141), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(141), t.e(568)]).then((() => () => t(568))),
+                        "./index": () => Promise.all([t.e(728), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(728), t.e(568)]).then((() => () => t(568))),
                         "./style": () => t.e(93).then((() => () => t(93)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -44,54 +44,54 @@
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
         93: "eae3497dd223d842d198",
-        141: "e94382aef4ebc132d608",
-        546: "f643d3e7381a2d9b834f",
-        568: "c842f59b09a70d32fbf5",
-        928: "0be57dd4ecbedec78b46"
+        302: "8a8d0af0376cb309e580",
+        568: "1176453d31b84477bbd4",
+        728: "98e8303b92484079cb9f",
+        928: "76f40c4b4ee1c8583ca3"
     } [e] + ".js?v=" + {
         93: "eae3497dd223d842d198",
-        141: "e94382aef4ebc132d608",
-        546: "f643d3e7381a2d9b834f",
-        568: "c842f59b09a70d32fbf5",
-        928: "0be57dd4ecbedec78b46"
+        302: "8a8d0af0376cb309e580",
+        568: "1176453d31b84477bbd4",
+        728: "98e8303b92484079cb9f",
+        928: "76f40c4b4ee1c8583ca3"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter-notebook/lab-extension:", x.l = (t, o, n, a) => {
         if (e[t]) e[t].push(o);
         else {
             var i, l;
             if (void 0 !== n)
                 for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var d = u[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                    var f = u[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
-            var f = (r, o) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+            var d = (r, o) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(o))), r) return r(o)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!o != !l.eager ? o : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter-notebook/application", "7.2.0-rc.0", (() => Promise.all([x.e(928), x.e(546), x.e(141)]).then((() => () => x(30))))), l("@jupyter-notebook/lab-extension", "7.2.0-rc.0", (() => Promise.all([x.e(141), x.e(568)]).then((() => () => x(568)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter-notebook/application", "7.2.0-rc.1", (() => Promise.all([x.e(928), x.e(302), x.e(728)]).then((() => () => x(30))))), l("@jupyter-notebook/lab-extension", "7.2.0-rc.1", (() => Promise.all([x.e(728), x.e(568)]).then((() => () => x(568)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -171,93 +171,93 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
                 n = o < 0;
             n && (o = -o - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, d, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !u || ("u" == f ? l > o && !n : "" == f != n);
-                if ("u" == d) {
-                    if (!u || "u" != f) return !1
+                var s, f, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == d ? l > o && !n : "" == d != n);
+                if ("u" == f) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (f == d)
+                    if (d == f)
                         if (l <= o) {
                             if (s != e[l]) return !1
                         } else {
                             if (n ? s > e[l] : s < e[l]) return !1;
                             s != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (n || l <= o) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= o || d < f != n) return !1;
+                    if (l <= o || f < d != n) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
-            var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            var b = e[i];
+            p.push(1 == b ? c() | c() : 2 == b ? c() & c() : b ? a(b, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || o(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, s = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", d = (e, r, t, o) => {
+    }, s = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", f = (e, r, t, o) => {
         var n = u(e, t);
-        return a(o, n) || p(s(e, t, n, o)), b(e[t][n])
-    }, f = (e, r, t) => {
+        return a(o, n) || c(s(e, t, n, o)), h(e[t][n])
+    }, d = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !a(t, r) || e && !o(e, r) ? e : r), 0)) && n[r]
-    }, c = (e, r, t, o) => {
+    }, p = (e, r, t, o) => {
         var a = e[t];
         return "No satisfying version (" + n(o) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
-    }, p = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, h = (e, r, t, o) => {
-        p(c(e, r, t, o))
-    }, b = e => (e.loaded = 1, e.get()), m = (v = e => function(r, t, o, n) {
+    }, b = (e, r, t, o) => {
+        c(p(e, r, t, o))
+    }, h = e => (e.loaded = 1, e.get()), m = (v = e => function(r, t, o, n) {
         var a = x.I(r);
         return a && a.then ? a.then(e.bind(e, r, x.S[r], t, o, n)) : e(r, x.S[r], t, o, n)
-    })(((e, r, t, o) => (i(e, t), b(f(r, t, o) || h(r, e, t, o) || l(r, t))))), g = v(((e, r, t, o) => (i(e, t), d(r, 0, t, o)))), y = v(((e, r, t, o, n) => {
-        var a = r && x.o(r, t) && f(r, t, o);
-        return a ? b(a) : n()
+    })(((e, r, t, o) => (i(e, t), h(d(r, t, o) || b(r, e, t, o) || l(r, t))))), g = v(((e, r, t, o) => (i(e, t), f(r, 0, t, o)))), y = v(((e, r, t, o, n) => {
+        var a = r && x.o(r, t) && d(r, t, o);
+        return a ? h(a) : n()
     })), j = {}, w = {
-        268: () => g("default", "@jupyterlab/coreutils", [1, 6, 2, 0, , "rc", 0]),
-        454: () => g("default", "@jupyterlab/ui-components", [1, 4, 2, 0, , "rc", 0]),
-        545: () => g("default", "@jupyterlab/translation", [1, 4, 2, 0, , "rc", 0]),
-        666: () => g("default", "@jupyterlab/application", [1, 4, 2, 0, , "rc", 0]),
-        834: () => g("default", "@jupyterlab/apputils", [1, 4, 3, 0, , "rc", 0]),
+        363: () => g("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
+        712: () => g("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
+        715: () => g("default", "@jupyterlab/translation", [1, 4, 2, 0]),
         882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        73: () => g("default", "@jupyterlab/notebook", [1, 4, 2, 0, , "rc", 0]),
-        758: () => y("default", "@jupyter-notebook/application", [1, 7, 2, 0, , "rc", 0], (() => Promise.all([x.e(928), x.e(546)]).then((() => () => x(30))))),
+        898: () => g("default", "@jupyterlab/application", [1, 4, 2, 0]),
+        944: () => g("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
+        616: () => y("default", "@jupyter-notebook/application", [1, 7, 2, 0, , "rc", 1], (() => Promise.all([x.e(928), x.e(302)]).then((() => () => x(30))))),
+        793: () => g("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
         4: () => g("default", "@lumino/properties", [1, 2, 0, 0]),
-        515: () => g("default", "@jupyterlab/rendermime", [1, 4, 2, 0, , "rc", 0]),
+        505: () => g("default", "@jupyterlab/rendermime", [1, 4, 2, 0]),
+        517: () => m("default", "@jupyterlab/docregistry", [1, 4, 2, 0]),
         633: () => g("default", "@lumino/messaging", [1, 2, 0, 0]),
         697: () => g("default", "@lumino/algorithm", [1, 2, 0, 0]),
         717: () => g("default", "@lumino/disposable", [1, 2, 0, 0]),
         797: () => g("default", "@lumino/polling", [1, 2, 0, 0]),
         901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        957: () => m("default", "@jupyterlab/docregistry", [1, 4, 2, 0, , "rc", 0])
+        930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0])
     }, k = {
-        141: [268, 454, 545, 666, 834, 882],
-        546: [4, 515, 633, 697, 717, 797, 901, 930, 957],
-        568: [73, 758]
+        302: [4, 505, 517, 633, 697, 717, 797, 901, 930],
+        568: [616, 793],
+        728: [363, 712, 715, 882, 898, 944]
     }, x.f.consumes = (e, r) => {
         x.o(k, e) && k[e].forEach((e => {
             if (x.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, x.m[e] = t => {
                         delete x.c[e], t.exports = r()
                     }
@@ -278,15 +278,15 @@
         var e = {
             572: 0
         };
         x.f.j = (r, t) => {
             var o = x.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
-                else if (141 != r) {
+                else if (728 != r) {
                 var n = new Promise(((t, n) => o = e[r] = [t, n]));
                 t.push(o[2] = n);
                 var a = x.p + x.u(r),
                     i = new Error;
                 x.l(a, (t => {
                     if (x.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
```

### Comparing `notebook-7.2.0rc0/notebook/labextension/static/third-party-licenses.json` & `notebook-7.2.0rc1/notebook/labextension/static/third-party-licenses.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '7.2.0-rc.1'}, 1: {'versionInfo': '4.2.0'}}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/application",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/application",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.8.1"
         },
```

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/menus.json` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/menus.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/package.json.orig` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/package.json.orig`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96484375%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-rc.1', "*

 * *                   "'@jupyter-notebook/ui-components': '^7.2.0-rc.1', '@jupyterlab/application': "*

 * *                   "'~4.2.0', '@jupyterlab/apputils': '~4.3.0', '@jupyterlab/codeeditor': "*

 * *                   "'~4.2.0', '@jupyterlab/console': '~4.2.0', '@jupyterlab/coreutils': '~6.2.0', "*

 * *                   "'@jupyterlab/docmanager': '~4.2.0', '@jupyterlab/docregistry': '~4.2.0', "*

 * *                   "'@jupyterlab/mainmenu': '~4.2.0', ' […]*

```diff
@@ -1,26 +1,26 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-rc.0",
-        "@jupyter-notebook/ui-components": "^7.2.0-rc.0",
-        "@jupyterlab/application": "~4.2.0-rc.0",
-        "@jupyterlab/apputils": "~4.3.0-rc.0",
-        "@jupyterlab/codeeditor": "~4.2.0-rc.0",
-        "@jupyterlab/console": "~4.2.0-rc.0",
-        "@jupyterlab/coreutils": "~6.2.0-rc.0",
-        "@jupyterlab/docmanager": "~4.2.0-rc.0",
-        "@jupyterlab/docregistry": "~4.2.0-rc.0",
-        "@jupyterlab/mainmenu": "~4.2.0-rc.0",
-        "@jupyterlab/rendermime": "~4.2.0-rc.0",
-        "@jupyterlab/settingregistry": "~4.2.0-rc.0",
-        "@jupyterlab/translation": "~4.2.0-rc.0",
+        "@jupyter-notebook/application": "^7.2.0-rc.1",
+        "@jupyter-notebook/ui-components": "^7.2.0-rc.1",
+        "@jupyterlab/application": "~4.2.0",
+        "@jupyterlab/apputils": "~4.3.0",
+        "@jupyterlab/codeeditor": "~4.2.0",
+        "@jupyterlab/console": "~4.2.0",
+        "@jupyterlab/coreutils": "~6.2.0",
+        "@jupyterlab/docmanager": "~4.2.0",
+        "@jupyterlab/docregistry": "~4.2.0",
+        "@jupyterlab/mainmenu": "~4.2.0",
+        "@jupyterlab/rendermime": "~4.2.0",
+        "@jupyterlab/settingregistry": "~4.2.0",
+        "@jupyterlab/translation": "~4.2.0",
         "@lumino/coreutils": "^2.1.2",
         "@lumino/disposable": "^2.1.2",
         "@lumino/widgets": "^2.3.2"
     },
     "description": "Jupyter Notebook - Application Extension",
     "devDependencies": {
         "rimraf": "^3.0.2",
@@ -62,9 +62,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-rc.0"
+    "version": "7.2.0-rc.1"
 }
```

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/shell.json` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/shell.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/application-extension/top.json` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/application-extension/top.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/documentsearch-extension/package.json.orig` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/documentsearch-extension/package.json.orig`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.965625%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-rc.1', '@jupyterlab/application': "*

 * *                   "'~4.2.0', '@jupyterlab/documentsearch': '~4.2.0'}",*

 * * "'version'": "'7.2.0-rc.1'"}*

```diff
@@ -1,16 +1,16 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-rc.0",
-        "@jupyterlab/application": "~4.2.0-rc.0",
-        "@jupyterlab/documentsearch": "~4.2.0-rc.0",
+        "@jupyter-notebook/application": "^7.2.0-rc.1",
+        "@jupyterlab/application": "~4.2.0",
+        "@jupyterlab/documentsearch": "~4.2.0",
         "@lumino/widgets": "^2.3.2"
     },
     "description": "Jupyter Notebook - Document Search Extension",
     "devDependencies": {
         "rimraf": "^3.0.2",
         "typescript": "~5.0.2"
     },
@@ -50,9 +50,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-rc.0"
+    "version": "7.2.0-rc.1"
 }
```

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/help-extension/package.json.orig` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/help-extension/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9660714285714285%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/ui-components': '^7.2.0-rc.1', '@jupyterlab/application': "*

 * *                   "'~4.2.0', '@jupyterlab/apputils': '~4.3.0', '@jupyterlab/mainmenu': '~4.2.0', "*

 * *                   "'@jupyterlab/translation': '~4.2.0'}",*

 * * "'version'": "'7.2.0-rc.1'"}*

```diff
@@ -1,18 +1,18 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/ui-components": "^7.2.0-rc.0",
-        "@jupyterlab/application": "~4.2.0-rc.0",
-        "@jupyterlab/apputils": "~4.3.0-rc.0",
-        "@jupyterlab/mainmenu": "~4.2.0-rc.0",
-        "@jupyterlab/translation": "~4.2.0-rc.0",
+        "@jupyter-notebook/ui-components": "^7.2.0-rc.1",
+        "@jupyterlab/application": "~4.2.0",
+        "@jupyterlab/apputils": "~4.3.0",
+        "@jupyterlab/mainmenu": "~4.2.0",
+        "@jupyterlab/translation": "~4.2.0",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
     "description": "Jupyter Notebook - Help Extension",
     "devDependencies": {
         "rimraf": "^3.0.2",
         "typescript": "~5.0.2"
@@ -53,9 +53,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-rc.0"
+    "version": "7.2.0-rc.1"
 }
```

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/notebook-extension/package.json.orig` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/notebook-extension/package.json.orig`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666668%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-rc.1', '@jupyterlab/application': "*

 * *                   "'~4.2.0', '@jupyterlab/apputils': '~4.3.0', '@jupyterlab/cells': '~4.2.0', "*

 * *                   "'@jupyterlab/docmanager': '~4.2.0', '@jupyterlab/notebook': '~4.2.0', "*

 * *                   "'@jupyterlab/settingregistry': '~4.2.0', '@jupyterlab/translation': '~4.2.0'}",*

 * * "'version'": "'7.2.0-rc.1'"}*

```diff
@@ -1,21 +1,21 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-rc.0",
-        "@jupyterlab/application": "~4.2.0-rc.0",
-        "@jupyterlab/apputils": "~4.3.0-rc.0",
-        "@jupyterlab/cells": "~4.2.0-rc.0",
-        "@jupyterlab/docmanager": "~4.2.0-rc.0",
-        "@jupyterlab/notebook": "~4.2.0-rc.0",
-        "@jupyterlab/settingregistry": "~4.2.0-rc.0",
-        "@jupyterlab/translation": "~4.2.0-rc.0",
+        "@jupyter-notebook/application": "^7.2.0-rc.1",
+        "@jupyterlab/application": "~4.2.0",
+        "@jupyterlab/apputils": "~4.3.0",
+        "@jupyterlab/cells": "~4.2.0",
+        "@jupyterlab/docmanager": "~4.2.0",
+        "@jupyterlab/notebook": "~4.2.0",
+        "@jupyterlab/settingregistry": "~4.2.0",
+        "@jupyterlab/translation": "~4.2.0",
         "@lumino/polling": "^2.1.2",
         "@lumino/widgets": "^2.3.2",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
     "description": "Jupyter Notebook - Notebook Extension",
     "devDependencies": {
@@ -58,9 +58,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-rc.0"
+    "version": "7.2.0-rc.1"
 }
```

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/notebook-extension/scroll-output.json` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/notebook-extension/scroll-output.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/tree-extension/file-actions.json` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/tree-extension/file-actions.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/tree-extension/package.json.orig` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/tree-extension/package.json.orig`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9647058823529413%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-rc.1', '@jupyter-notebook/tree': "*

 * *                   "'^7.2.0-rc.1', '@jupyterlab/application': '~4.2.0', '@jupyterlab/apputils': "*

 * *                   "'~4.3.0', '@jupyterlab/coreutils': '~6.2.0', '@jupyterlab/docmanager': "*

 * *                   "'~4.2.0', '@jupyterlab/filebrowser': '~4.2.0', '@jupyterlab/mainmenu': "*

 * *                   "'~4.2.0', '@jupyterlab/services': '~7.2.0', '@jupyterlab/settingeditor': "*

 * *                   "'~4.2.0', '@jupy […]*

```diff
@@ -1,27 +1,27 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-rc.0",
-        "@jupyter-notebook/tree": "^7.2.0-rc.0",
-        "@jupyterlab/application": "~4.2.0-rc.0",
-        "@jupyterlab/apputils": "~4.3.0-rc.0",
-        "@jupyterlab/coreutils": "~6.2.0-rc.0",
-        "@jupyterlab/docmanager": "~4.2.0-rc.0",
-        "@jupyterlab/filebrowser": "~4.2.0-rc.0",
-        "@jupyterlab/mainmenu": "~4.2.0-rc.0",
-        "@jupyterlab/services": "~7.2.0-rc.0",
-        "@jupyterlab/settingeditor": "~4.2.0-rc.0",
-        "@jupyterlab/settingregistry": "~4.2.0-rc.0",
-        "@jupyterlab/statedb": "~4.2.0-rc.0",
-        "@jupyterlab/translation": "~4.2.0-rc.0",
-        "@jupyterlab/ui-components": "~4.2.0-rc.0",
+        "@jupyter-notebook/application": "^7.2.0-rc.1",
+        "@jupyter-notebook/tree": "^7.2.0-rc.1",
+        "@jupyterlab/application": "~4.2.0",
+        "@jupyterlab/apputils": "~4.3.0",
+        "@jupyterlab/coreutils": "~6.2.0",
+        "@jupyterlab/docmanager": "~4.2.0",
+        "@jupyterlab/filebrowser": "~4.2.0",
+        "@jupyterlab/mainmenu": "~4.2.0",
+        "@jupyterlab/services": "~7.2.0",
+        "@jupyterlab/settingeditor": "~4.2.0",
+        "@jupyterlab/settingregistry": "~4.2.0",
+        "@jupyterlab/statedb": "~4.2.0",
+        "@jupyterlab/translation": "~4.2.0",
+        "@jupyterlab/ui-components": "~4.2.0",
         "@lumino/algorithm": "^2.0.1",
         "@lumino/commands": "^2.3.0",
         "@lumino/widgets": "^2.3.2"
     },
     "description": "Jupyter Notebook - Tree Extension",
     "devDependencies": {
         "rimraf": "^3.0.2",
@@ -63,9 +63,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-rc.0"
+    "version": "7.2.0-rc.1"
 }
```

### Comparing `notebook-7.2.0rc0/notebook/schemas/@jupyter-notebook/tree-extension/widget.json` & `notebook-7.2.0rc1/notebook/schemas/@jupyter-notebook/tree-extension/widget.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1053.bundle.js` & `notebook-7.2.0rc1/notebook/static/6078.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [1053], {
-        41053: (O, Q, P) => {
+    [6078], {
+        76078: (O, Q, P) => {
             P.r(Q), P.d(Q, {
                 java: () => S,
                 javaLanguage: () => X
             });
             var $ = P(49906),
                 a = P(92209);
             const i = (0, a.styleTags)({
```

### Comparing `notebook-7.2.0rc0/notebook/static/1088.bundle.js` & `notebook-7.2.0rc1/notebook/static/1088.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1091.bundle.js` & `notebook-7.2.0rc1/notebook/static/1091.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1122.bundle.js` & `notebook-7.2.0rc1/notebook/static/1122.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/113.bundle.js` & `notebook-7.2.0rc1/notebook/static/113.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [113], {
         113: (t, e, s) => {
             s.r(e), s.d(e, {
                 default: () => K
             });
-            var i, n = s(24554),
-                r = s(37267),
-                o = s(22620),
+            var i, n = s(23295),
+                r = s(12030),
+                o = s(35613),
                 l = s(16934),
                 a = s(20998),
                 c = s(2549),
                 h = s(18395);
             ! function(t) {
                 t.editBinding = "shortcuts:edit-keybinding", t.addBinding = "shortcuts:add-keybinding", t.deleteBinding = "shortcuts:delete-keybinding", t.toggleSelectors = "shortcuts:toggle-selectors", t.resetAll = "shortcuts:reset-all"
             }(i || (i = {}));
```

### Comparing `notebook-7.2.0rc0/notebook/static/114.bundle.js` & `notebook-7.2.0rc1/notebook/static/114.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1169.bundle.js` & `notebook-7.2.0rc1/notebook/static/1169.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1198.bundle.js` & `notebook-7.2.0rc1/notebook/static/1198.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,16 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [1198, 8907], {
         41198: (t, e, s) => {
             s.r(e), s.d(e, {
                 IPropertyInspectorProvider: () => c,
                 SideBarPropertyInspectorProvider: () => a
             });
-            var n = s(37267),
-                r = s(22620),
+            var n = s(12030),
+                r = s(35613),
                 o = s(81997),
                 i = s(63485);
             const c = new(s(20998).Token)("@jupyterlab/property-inspector:IPropertyInspectorProvider", "A service to registry new widget in the property inspector side panel.");
             class h extends i.Widget {
                 constructor() {
                     super(), this._tracker = new i.FocusTracker, this._inspectors = new Map, this.addClass("jp-PropertyInspector"), this._tracker = new i.FocusTracker, this._tracker.currentChanged.connect(this._onCurrentChanged, this)
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/1261.bundle.js` & `notebook-7.2.0rc1/notebook/static/1261.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/131.bundle.js` & `notebook-7.2.0rc1/notebook/static/131.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1326.bundle.js` & `notebook-7.2.0rc1/notebook/static/1326.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/134.bundle.js` & `notebook-7.2.0rc1/notebook/static/134.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,16 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [134, 4042], {
         44042: (t, e, s) => {
             s.r(e), s.d(e, {
                 AttachmentsModel: () => r,
                 AttachmentsResolver: () => h
             });
-            var a = s(58959),
-                n = s(13408),
+            var a = s(31231),
+                n = s(81221),
                 i = s(81997);
             class r {
                 constructor(t) {
                     var e;
                     if (this._map = new a.ObservableMap, this._isDisposed = !1, this._stateChanged = new i.Signal(this), this._changed = new i.Signal(this), this._serialized = null, this._changeGuard = !1, this.contentFactory = null !== (e = t.contentFactory) && void 0 !== e ? e : r.defaultContentFactory, t.values)
                         for (const e of Object.keys(t.values)) void 0 !== t.values[e] && this.set(e, t.values[e]);
                     this._map.changed.connect(this._onMapChanged, this)
```

### Comparing `notebook-7.2.0rc0/notebook/static/1388.bundle.js` & `notebook-7.2.0rc1/notebook/static/1388.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         91388: (t, e, a) => {
             a.d(e, {
                 diagram: () => f
             });
             var r = a(17010),
                 i = a(23617),
                 n = a(7259),
-                d = a(29197),
+                d = a(67406),
                 o = a(24028);
             a(27693), a(7608), a(31699);
             let s = 0;
             const l = function(t, e, a, r) {
                     const {
                         displayText: i,
                         cssStyle: n
```

### Comparing `notebook-7.2.0rc0/notebook/static/1408.bundle.js` & `notebook-7.2.0rc1/notebook/static/1408.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     [1408], {
         11408: (e, t, a) => {
             a.r(t), a.d(t, {
                 MathJaxTypesetter: () => o,
                 default: () => r
             });
             var n, i = a(20998),
-                s = a(13408);
+                s = a(81221);
             ! function(e) {
                 e.copy = "mathjax:clipboard", e.scale = "mathjax:scale"
             }(n || (n = {}));
             class o {
                 constructor() {
                     this._initialized = !1
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/1418.bundle.js` & `notebook-7.2.0rc1/notebook/static/1418.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1495.bundle.js` & `notebook-7.2.0rc1/notebook/static/1495.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1496.bundle.js` & `notebook-7.2.0rc1/notebook/static/1496.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [1496], {
         91496: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => f
             });
-            var a = n(2922),
-                s = n(96049),
-                r = n(1167),
-                l = n(50845),
-                o = n(37267),
-                i = n(22620),
+            var a = n(44604),
+                s = n(53312),
+                r = n(68722),
+                l = n(29879),
+                o = n(12030),
+                i = n(35613),
                 c = n(78156),
-                d = n(70611),
+                d = n(87408),
                 u = n(20998),
                 m = n(81997),
                 h = n(24475),
                 p = n(63485);
             const g = "jp-Licenses-Filters-title";
             class _ extends p.SplitPanel {
                 constructor(e) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/1542.bundle.js` & `notebook-7.2.0rc1/notebook/static/1542.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1558.bundle.js` & `notebook-7.2.0rc1/notebook/static/1558.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1584.bundle.js` & `notebook-7.2.0rc1/notebook/static/1584.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1618.bundle.js` & `notebook-7.2.0rc1/notebook/static/1618.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1647.bundle.js` & `notebook-7.2.0rc1/notebook/static/1647.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,16 +3,16 @@
     [1647, 2167], {
         51647: (t, e, o) => {
             o.r(e), o.d(e, {
                 ITooltipManager: () => s,
                 Tooltip: () => a
             });
             const s = new(o(20998).Token)("@jupyterlab/tooltip:ITooltipManager", "A service for the tooltip manager for the application. Use this to allow your extension to invoke a tooltip.");
-            var i = o(22620),
-                n = o(13408),
+            var i = o(35613),
+                n = o(81221),
                 r = o(63485);
             const d = "jp-mod-tooltip",
                 h = !0;
             class a extends r.Widget {
                 constructor(t) {
                     super(), this._content = null;
                     const e = this.layout = new r.PanelLayout,
```

### Comparing `notebook-7.2.0rc0/notebook/static/1650.bundle.js` & `notebook-7.2.0rc1/notebook/static/1650.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [1650, 8875], {
         71650: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => s
             });
-            var n = o(1167),
-                a = o(91942),
-                i = o(46807),
+            var n = o(68722),
+                a = o(5094),
+                i = o(59625),
                 d = o(81997);
             const s = [{
                 id: "@jupyter-notebook/docmanager-extension:opener",
                 autoStart: !0,
                 optional: [i.INotebookPathOpener, i.INotebookShell],
                 provides: a.IDocumentWidgetOpener,
                 description: "Open documents in a new browser tab",
```

### Comparing `notebook-7.2.0rc0/notebook/static/1684.bundle.js` & `notebook-7.2.0rc1/notebook/static/5601.bundle.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [1684, 5601], {
+    [5601, 1684], {
         95601: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => l
             });
-            var a = n(2922),
-                o = n(1167),
-                i = n(69200),
-                r = n(46807),
+            var a = n(44604),
+                o = n(68722),
+                i = n(5333),
+                r = n(59625),
                 s = n(33625);
             const c = {
                     id: "@jupyter-notebook/terminal-extension:opener",
                     description: "A plugin to open terminals in a new tab.",
                     requires: [a.IRouter, i.ITerminalTracker],
                     autoStart: !0,
                     activate: (e, t, n) => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/1696.bundle.js` & `notebook-7.2.0rc1/notebook/static/1696.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/170.bundle.js` & `notebook-7.2.0rc1/notebook/static/170.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1809.bundle.js` & `notebook-7.2.0rc1/notebook/static/1809.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,17 +6,17 @@
                 IRunningSessionManagers: () => C,
                 IRunningSessionSidebar: () => y,
                 RunningSessionManagers: () => I,
                 RunningSessions: () => L,
                 SearchableSessions: () => D,
                 SearchableSessionsList: () => B
             });
-            var n = s(96049),
-                i = s(37267),
-                a = s(22620),
+            var n = s(53312),
+                i = s(12030),
+                a = s(35613),
                 o = s(20998),
                 l = s(2549),
                 r = s(18395),
                 d = s(81997),
                 h = s(63485),
                 c = s(78156),
                 u = s.n(c);
```

### Comparing `notebook-7.2.0rc0/notebook/static/1827.bundle.js` & `notebook-7.2.0rc1/notebook/static/1827.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [1827], {
         41827: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => y
             });
-            var r = n(2922),
-                i = n(96049),
+            var r = n(44604),
+                i = n(53312),
                 o = n(21058),
                 a = n(40930),
-                s = n(26862),
-                d = n(50845),
-                l = n(24554),
-                c = n(37267);
+                s = n(95183),
+                d = n(29879),
+                l = n(23295),
+                c = n(12030);
             const h = "CSVTable",
                 u = "TSVTable";
             var g;
             ! function(e) {
                 e.CSVGoToLine = "csv:go-to-line", e.TSVGoToLine = "tsv:go-to-line"
             }(g || (g = {}));
             const _ = {
@@ -210,16 +210,16 @@
                 }
             }(w || (w = {}))
         },
         40930: (e, t, n) => {
             n.d(t, {
                 p: () => s
             });
-            var r, i = n(37267),
-                o = n(22620),
+            var r, i = n(12030),
+                o = n(35613),
                 a = n(63485);
             class s extends a.Widget {
                 constructor(e) {
                     super({
                         node: r.createNode(e.widget.delimiter, e.translator)
                     }), this._widget = e.widget, this.addClass("jp-CSVDelimiter")
                 }
@@ -264,16 +264,16 @@
                 A9: () => u,
                 B0: () => c,
                 JZ: () => h,
                 LT: () => _,
                 _d: () => m,
                 kw: () => g
             });
-            var r, i = n(1167),
-                o = n(10979),
+            var r, i = n(68722),
+                o = n(65903),
                 a = n(20998),
                 s = n(81997),
                 d = n(63485),
                 l = n(40930);
             class c {}
             class h {
                 constructor(e) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/1828.bundle.js` & `notebook-7.2.0rc1/notebook/static/1828.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1833.bundle.js` & `notebook-7.2.0rc1/notebook/static/1833.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,16 +15,16 @@
                 LaTeXTableOfContentsModel: () => A,
                 MarkdownTableOfContentsFactory: () => k,
                 MarkdownTableOfContentsModel: () => O,
                 PythonTableOfContentsFactory: () => I,
                 PythonTableOfContentsModel: () => D,
                 TabSpaceStatus: () => w
             });
-            var n = i(52839),
-                o = i(52138),
+            var n = i(51429),
+                o = i(61907),
                 s = i(20998);
             class r extends o.WidgetLSPAdapter {
                 constructor(e, t) {
                     const {
                         docRegistry: i,
                         ...n
                     } = t;
@@ -99,18 +99,18 @@
                 getEditorWrapper(e) {
                     return this.wrapperElement
                 }
                 async initOnceReady() {
                     this.initVirtual(), await this.connectDocument(this.virtualDocument, !1), this.editor.model.mimeTypeChanged.connect(this.reloadConnection, this)
                 }
             }
-            var a = i(96049),
-                d = i(49269),
-                l = i(10979),
-                c = i(22620),
+            var a = i(53312),
+                d = i(30525),
+                l = i(65903),
+                c = i(35613),
                 h = i(63485);
             class u extends h.Widget {
                 constructor(e) {
                     super(), this._ready = new s.PromiseDelegate, this.addClass("jp-FileEditor");
                     const t = this._context = e.context;
                     this._mimeTypeService = e.mimeTypeService;
                     const i = this._editorWidget = new n.CodeEditorWrapper({
@@ -229,16 +229,16 @@
                     return e instanceof a.MainAreaWidget && e.content instanceof u && e.content.editor instanceof d.CodeMirrorEditor
                 }
                 getInitialQuery() {
                     const e = this.editor;
                     return e.state.sliceDoc(e.state.selection.main.from, e.state.selection.main.to)
                 }
             }
-            var y = i(27829),
-                v = i(37267),
+            var y = i(71098),
+                v = i(12030),
                 _ = i(78156),
                 f = i.n(_);
 
             function C(e) {
                 return f().createElement(y.TextItem, {
                     source: e.language,
                     onClick: e.handleClick
@@ -360,15 +360,15 @@
                     }
                     set indentUnit(e) {
                         e !== this._indentUnit && (this._indentUnit = e, this.stateChanged.emit())
                     }
                 }
                 e.Model = t
             }(w || (w = {}));
-            var E = i(87017);
+            var E = i(79426);
             class b extends E.TableOfContentsFactory {
                 createNew(e, t) {
                     const i = super.createNew(e, t),
                         n = (t, i) => {
                             i && e.content.editor.setCursorPosition({
                                 line: i.line,
                                 column: 0
```

### Comparing `notebook-7.2.0rc0/notebook/static/1837.bundle.js` & `notebook-7.2.0rc1/notebook/static/1837.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1846.bundle.js` & `notebook-7.2.0rc1/notebook/static/1846.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [1846], {
-        11846: (e, t, l) => {
+        72647: (e, t, l) => {
             l.d(t, {
                 diagram: () => f
             });
             var n = l(17010),
                 a = l(23617),
-                o = l(29197),
+                o = l(67406),
                 i = l(24028),
                 s = l(86281);
             l(27693), l(7608), l(31699), l(7259), l(81779);
             const d = e => i.e.sanitizeText(e, (0, i.c)());
             let r = {
                 dividerMargin: 10,
                 padding: 5,
```

### Comparing `notebook-7.2.0rc0/notebook/static/1869.bundle.js` & `notebook-7.2.0rc1/notebook/static/1869.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1884.bundle.js` & `notebook-7.2.0rc1/notebook/static/1884.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1941.bundle.js` & `notebook-7.2.0rc1/notebook/static/1941.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/1958.bundle.js` & `notebook-7.2.0rc1/notebook/static/1958.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             a.r(t), a.d(t, {
                 Grid: () => i,
                 GridModel: () => c
             });
             var o, r = a(59072),
                 s = a(81997),
                 n = a(63485),
-                l = a(37267),
+                l = a(12030),
                 d = a(78947);
             class i extends n.Panel {
                 constructor(e) {
                     super();
                     const {
                         commands: t,
                         model: a,
```

### Comparing `notebook-7.2.0rc0/notebook/static/1962.bundle.js` & `notebook-7.2.0rc1/notebook/static/1962.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,54 +5,54 @@
             o.r(t), o.d(t, {
                 commandEditItem: () => G,
                 default: () => me,
                 executionIndicator: () => X,
                 exportPlugin: () => Q,
                 notebookTrustItem: () => Z
             });
-            var n = o(2922),
-                l = o(96049),
-                a = o(67406),
-                r = o(52839),
-                d = o(1167),
-                i = o(49269),
-                s = o(89144),
-                c = o(91942),
-                u = o(18602),
-                b = o(26862),
-                m = o(42751),
-                p = o(65651),
-                g = o(52138),
-                C = o(50845),
-                k = o(40465),
-                v = o(17894),
-                h = o(66724),
-                f = o(13408),
-                w = o(24554),
-                x = o(96692),
-                _ = o(27829),
-                A = o(87017),
-                y = o(37267),
-                S = o(22620),
+            var n = o(44604),
+                l = o(53312),
+                a = o(73166),
+                r = o(51429),
+                d = o(68722),
+                i = o(30525),
+                s = o(81002),
+                c = o(5094),
+                u = o(97708),
+                b = o(95183),
+                m = o(71427),
+                p = o(86810),
+                g = o(61907),
+                C = o(29879),
+                k = o(12077),
+                v = o(25460),
+                h = o(77872),
+                f = o(81221),
+                w = o(23295),
+                x = o(41053),
+                _ = o(71098),
+                A = o(79426),
+                y = o(12030),
+                S = o(35613),
                 E = o(33625),
                 N = o(20998),
                 I = o(2549),
                 M = o(49503),
                 T = o(63485);
             const R = {
                 id: "@jupyterlab/notebook-extension:cell-executor",
                 description: "Provides the notebook cell executor.",
                 autoStart: !0,
                 provides: v.INotebookCellExecutor,
                 activate: () => Object.freeze({
                     runCell: v.runCell
                 })
             };
-            var O = o(98603),
-                B = o(70611);
+            var O = o(44182),
+                B = o(87408);
             const P = {
                 activate: function(e, t, o) {
                     function n(e) {
                         function t(t, n, l) {
                             if (B.KernelMessage.isDisplayDataMsg(t) || B.KernelMessage.isStreamMsg(t) || B.KernelMessage.isErrorMsg(t) || B.KernelMessage.isExecuteResultMsg(t)) {
                                 const a = o.getLogger(e.context.path);
                                 a.rendermime = e.content.rendermime;
@@ -106,15 +106,15 @@
                         ref: e => null == e ? void 0 : e.appendChild(this.node)
                     })
                 }
                 async refresh() {
                     await this._refreshDebouncer.invoke()
                 }
             }
-            var W, K = o(58959);
+            var W, K = o(31231);
             class F extends v.NotebookTools.MetadataEditorTool {
                 constructor(e) {
                     super(e), this._tracker = e.tracker, this.editor.editorHostNode.addEventListener("blur", this.editor, !0), this.editor.editorHostNode.addEventListener("click", this.editor, !0), this.editor.headerNode.addEventListener("click", this.editor)
                 }
                 _onSourceChanged() {
                     var e;
                     this.editor.source && (null === (e = this._tracker.activeCell) || void 0 === e || e.model.sharedModel.setMetadata(this.editor.source.toJSON()))
@@ -2060,15 +2060,15 @@
                     isVisible: e => {
                         var t;
                         return (!!e.toolbar || d()) && null !== (t = "full" === (null == r ? void 0 : r.composite.windowingMode)) && void 0 !== t && t
                     }
                 });
                 const m = [W.createNew, W.createOutputView],
                     p = () => {
-                        Object.values(W).filter((e => !m.includes(e))).forEach((t => e.commands.notifyCommandChanged(t)))
+                        Object.values(W).filter((t => !m.includes(t) && e.commands.hasCommand(t))).forEach((t => e.commands.notifyCommandChanged(t)))
                     };
                 t.currentChanged.connect(p), null === (i = u.currentChanged) || void 0 === i || i.connect(p)
             }
             var Ce;
             ! function(e) {
                 e.createConsole = function(e, t, o) {
                     const n = {
```

### Comparing `notebook-7.2.0rc0/notebook/static/1cb1c39ea642f26a4dfe.woff` & `notebook-7.2.0rc1/notebook/static/1cb1c39ea642f26a4dfe.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2007.bundle.js` & `notebook-7.2.0rc1/notebook/static/2007.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -10,18 +10,18 @@
                 KernelMenu: () => c,
                 MainMenu: () => p,
                 RunMenu: () => l,
                 SettingsMenu: () => M,
                 TabsMenu: () => h,
                 ViewMenu: () => _
             });
-            var t, r = s(22620),
+            var t, r = s(35613),
                 i = s(33625),
                 a = s(63485),
-                u = s(96049);
+                u = s(53312);
             class d extends r.RankedMenu {
                 constructor(e) {
                     super(e), this.undoers = {
                         redo: new u.SemanticCommand,
                         undo: new u.SemanticCommand
                     }, this.clearers = {
                         clearAll: new u.SemanticCommand,
```

### Comparing `notebook-7.2.0rc0/notebook/static/2065.bundle.js` & `notebook-7.2.0rc1/notebook/static/2065.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2088.bundle.js` & `notebook-7.2.0rc1/notebook/static/2088.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [2088, 6604], {
         6604: (e, o, t) => {
             t.r(o), t.d(o, {
                 default: () => b
             });
-            var n, i = t(80106),
-                r = t(1167),
-                l = t(42703),
-                s = t(17894),
-                a = t(13408),
-                d = t(15327),
-                c = t(37267),
+            var n, i = t(67260),
+                r = t(68722),
+                l = t(34663),
+                s = t(25460),
+                a = t(81221),
+                d = t(27865),
+                c = t(12030),
                 u = t(33625),
                 p = t(63485);
             ! function(e) {
                 e.dismiss = "tooltip:dismiss", e.launchConsole = "tooltip:launch-console", e.launchNotebook = "tooltip:launch-notebook", e.launchFile = "tooltip:launch-file"
             }(n || (n = {}));
             const m = {
                     id: "@jupyterlab/tooltip-extension:manager",
```

### Comparing `notebook-7.2.0rc0/notebook/static/2089.bundle.js` & `notebook-7.2.0rc1/notebook/static/2089.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,16 +7,16 @@
                 LogConsolePanel: () => w,
                 LogOutputModel: () => a,
                 Logger: () => u,
                 LoggerOutputAreaModel: () => l,
                 LoggerRegistry: () => g,
                 ScrollingWidget: () => v
             });
-            var i, r = s(36726),
-                n = s(13408),
+            var i, r = s(44946),
+                n = s(81221),
                 o = s(81997);
             class a extends n.OutputModel {
                 constructor(e) {
                     super(e), this.timestamp = new Date(e.value.timestamp), this.level = e.value.level
                 }
             }
             class h extends r.OutputAreaModel.ContentFactory {
@@ -203,15 +203,15 @@
                     return this._isDisposed
                 }
                 dispose() {
                     this.isDisposed || (this._isDisposed = !0, this._loggers.forEach((e => e.dispose())), o.Signal.clearData(this))
                 }
             }
             const d = new(s(20998).Token)("@jupyterlab/logconsole:ILoggerRegistry", "A service providing a logger infrastructure.");
-            var c = s(37267),
+            var c = s(12030),
                 _ = s(63485);
             class p extends _.Widget {
                 constructor() {
                     super(), this._timestampNode = document.createElement("div"), this.node.append(this._timestampNode)
                 }
                 set timestamp(e) {
                     this._timestamp = e, this._timestampNode.innerHTML = this._timestamp.toLocaleTimeString(), this.update()
```

### Comparing `notebook-7.2.0rc0/notebook/static/2122.bundle.js` & `notebook-7.2.0rc1/notebook/static/2122.bundle.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [2122], {
         92122: (t, e, o) => {
             o.r(e), o.d(e, {
                 default: () => i
             });
-            var a = o(24554),
-                l = o(5510),
-                n = o(96049),
-                r = o(37267);
+            var a = o(23295),
+                l = o(82426),
+                n = o(53312),
+                r = o(12030);
             const s = {
                     id: "@jupyterlab/cell-toolbar-extension:plugin",
                     description: "Add the cells toolbar.",
                     autoStart: !0,
                     activate: async (t, e, o, a) => {
                         const i = e && o ? (0, n.createToolbarFactory)(o, e, l.CellBarExtension.FACTORY_NAME, s.id, null != a ? a : r.nullTranslator) : void 0;
                         t.docRegistry.addWidgetExtension("Notebook", new l.CellBarExtension(t.commands, i))
```

### Comparing `notebook-7.2.0rc0/notebook/static/214.bundle.js` & `notebook-7.2.0rc1/notebook/static/214.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2167.bundle.js` & `notebook-7.2.0rc1/notebook/static/2167.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,16 +3,16 @@
     [2167, 1647], {
         51647: (t, e, o) => {
             o.r(e), o.d(e, {
                 ITooltipManager: () => s,
                 Tooltip: () => a
             });
             const s = new(o(20998).Token)("@jupyterlab/tooltip:ITooltipManager", "A service for the tooltip manager for the application. Use this to allow your extension to invoke a tooltip.");
-            var i = o(22620),
-                n = o(13408),
+            var i = o(35613),
+                n = o(81221),
                 r = o(63485);
             const d = "jp-mod-tooltip",
                 h = !0;
             class a extends r.Widget {
                 constructor(t) {
                     super(), this._content = null;
                     const e = this.layout = new r.PanelLayout,
```

### Comparing `notebook-7.2.0rc0/notebook/static/2184.bundle.js` & `notebook-7.2.0rc1/notebook/static/2184.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [2184], {
         42184: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => E
             });
-            var a = n(2922),
-                o = n(96049),
-                i = n(67406),
-                r = n(52839),
-                s = n(80106),
-                l = n(1167),
-                d = n(49713),
-                c = n(10979),
-                u = n(42703),
-                g = n(98603),
-                b = n(17894),
-                p = n(13408),
-                v = n(24554),
-                m = n(37267);
+            var a = n(44604),
+                o = n(53312),
+                i = n(73166),
+                r = n(51429),
+                s = n(67260),
+                l = n(68722),
+                d = n(63050),
+                c = n(65903),
+                u = n(34663),
+                g = n(44182),
+                b = n(25460),
+                p = n(81221),
+                v = n(23295),
+                m = n(12030);
 
             function h(e) {
                 Object.values(d.Debugger.CommandIDs).forEach((t => {
                     e.commands.hasCommand(t) && e.commands.notifyCommandChanged(t)
                 }))
             }
             const I = {
```

### Comparing `notebook-7.2.0rc0/notebook/static/2188.bundle.js` & `notebook-7.2.0rc1/notebook/static/2188.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/221.bundle.js` & `notebook-7.2.0rc1/notebook/static/221.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2241.bundle.js` & `notebook-7.2.0rc1/notebook/static/2241.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2311.bundle.js` & `notebook-7.2.0rc1/notebook/static/2311.bundle.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [2311], {
         22311: (e, n, t) => {
             t.r(n), t.d(n, {
                 default: () => m
             });
-            var a = t(2922),
-                i = t(96049),
-                o = t(49922),
-                s = t(24554),
-                l = t(37267),
-                d = t(22620);
+            var a = t(44604),
+                i = t(53312),
+                o = t(95411),
+                s = t(23295),
+                l = t(12030),
+                d = t(35613);
             const r = "@jupyterlab/extensionmanager-extension:plugin";
             var c;
             ! function(e) {
                 e.showPanel = "extensionmanager:show-panel", e.toggle = "extensionmanager:toggle"
             }(c || (c = {}));
             const g = {
                     id: r,
```

### Comparing `notebook-7.2.0rc0/notebook/static/2323.bundle.js` & `notebook-7.2.0rc1/notebook/static/2323.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2324.bundle.js` & `notebook-7.2.0rc1/notebook/static/2324.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2343.bundle.js` & `notebook-7.2.0rc1/notebook/static/2343.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2386.bundle.js` & `notebook-7.2.0rc1/notebook/static/2386.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2401.bundle.js` & `notebook-7.2.0rc1/notebook/static/2401.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [2401], {
         43967: (e, t, n) => {
             "use strict";
             n.d(t, {
                 g: () => o
             });
-            var r, s = n(58959),
+            var r, s = n(31231),
                 a = n(20998),
                 i = n(81997);
             class o {
                 constructor(e) {
                     this.trusted = !1, this._changed = new i.Signal(this), this._raw = {};
                     const t = r.getData(e.value);
                     this._data = new s.ObservableJSON({
@@ -172,15 +172,15 @@
                 renderSVG: () => h.KB,
                 renderText: () => h.IY,
                 replaceMath: () => o.b,
                 standardRendererFactories: () => i.Nf,
                 svgRendererFactory: () => i.F,
                 textRendererFactory: () => i.BJ
             });
-            var r = n(41070),
+            var r = n(22425),
                 s = {};
             for (const e in r) "default" !== e && (s[e] = () => r[e]);
             n.d(t, s);
             var a = n(43967),
                 i = n(15862),
                 o = n(69837),
                 l = n(32021),
@@ -255,16 +255,16 @@
             }(s || (s = {}))
         },
         4800: (e, t, n) => {
             "use strict";
             n.d(t, {
                 M: () => l
             });
-            var r, s = n(81692),
-                a = n(58959),
+            var r, s = n(81139),
+                a = n(31231),
                 i = n(20998),
                 o = n(81997);
             class l {
                 constructor(e) {
                     this._changed = new o.Signal(this), this._raw = {};
                     const {
                         data: t,
@@ -367,17 +367,17 @@
             }(r || (r = {}))
         },
         32549: (e, t, n) => {
             "use strict";
             n.d(t, {
                 D: () => l
             });
-            var r, s = n(96049),
-                a = n(1167),
-                i = n(37267),
+            var r, s = n(53312),
+                a = n(68722),
+                i = n(12030),
                 o = n(32021);
             class l {
                 constructor(e = {}) {
                     var t, n, r, a, o, l;
                     if (this._id = 0, this._ranks = {}, this._types = null, this._factories = {}, this.translator = null !== (t = e.translator) && void 0 !== t ? t : i.nullTranslator, this.resolver = null !== (n = e.resolver) && void 0 !== n ? n : null, this.linkHandler = null !== (r = e.linkHandler) && void 0 !== r ? r : null, this.latexTypesetter = null !== (a = e.latexTypesetter) && void 0 !== a ? a : null, this.markdownParser = null !== (o = e.markdownParser) && void 0 !== o ? o : null, this.sanitizer = null !== (l = e.sanitizer) && void 0 !== l ? l : new s.Sanitizer, e.initialFactories)
                         for (const t of e.initialFactories) this.addFactory(t)
                 }
@@ -518,16 +518,16 @@
                 K3: () => u,
                 KB: () => f,
                 NN: () => d,
                 Op: () => T,
                 ap: () => p,
                 co: () => h
             });
-            var r, s, a = n(1167),
-                i = n(37267),
+            var r, s, a = n(68722),
+                i = n(12030),
                 o = n(8872),
                 l = n.n(o),
                 c = n(69837);
 
             function d(e) {
                 let {
                     host: t,
@@ -1062,15 +1062,15 @@
                 UH: () => d,
                 cw: () => h,
                 lH: () => p,
                 oI: () => l,
                 pY: () => i,
                 zt: () => u
             });
-            var r = n(37267),
+            var r = n(12030),
                 s = n(63485),
                 a = n(3328);
             class i extends s.Widget {
                 constructor(e) {
                     var t, n;
                     super(), this.mimeType = e.mimeType, this.sanitizer = e.sanitizer, this.resolver = e.resolver, this.linkHandler = e.linkHandler, this.translator = null !== (t = e.translator) && void 0 !== t ? t : r.nullTranslator, this.latexTypesetter = e.latexTypesetter, this.markdownParser = null !== (n = e.markdownParser) && void 0 !== n ? n : null, this.node.dataset.mimeType = this.mimeType
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/2479.bundle.js` & `notebook-7.2.0rc1/notebook/static/2479.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -97,15 +97,15 @@
                     }, i.h.span({
                         className: a
                     }), i.h.span({
                         className: r
                     }, h))))
                 }
             }(l || (l = {}));
-            var h = s(22620),
+            var h = s(35613),
                 u = s(18395),
                 c = s(78156);
             class p extends h.ReactWidget {
                 constructor() {
                     super(), this.addClass("jp-Collapser")
                 }
                 get collapsed() {
@@ -159,15 +159,15 @@
                 }
             }
             class v extends C.Widget {
                 constructor() {
                     super(), this.addClass("jp-CellFooter")
                 }
             }
-            var y = s(52839);
+            var y = s(51429);
             class w extends C.Widget {
                 constructor(e) {
                     super(), this.addClass("jp-InputArea");
                     const {
                         contentFactory: t,
                         editorOptions: s,
                         model: i
@@ -230,16 +230,16 @@
                     return this._executionCount
                 }
                 set executionCount(e) {
                     this._executionCount = e, this.node.textContent = null === e ? " " : `[${e||" "}]:`
                 }
             }
             var x = s(81997),
-                M = s(98289),
-                O = s(36726),
+                M = s(42193),
+                O = s(44946),
                 P = s(57508);
             const S = (0, P.createMutex)();
 
             function E(e) {
                 return "code" === e.type
             }
 
@@ -472,15 +472,15 @@
                 class t {
                     createOutputArea(e) {
                         return new O.OutputAreaModel(e)
                     }
                 }
                 e.ContentFactory = t, e.defaultContentFactory = new t
             }(k || (k = {}));
-            var N = s(37267);
+            var N = s(12030);
             class F extends C.Widget {
                 constructor(e) {
                     var t, s, i;
                     const n = document.createElement("div");
                     super({
                         node: n
                     });
@@ -521,17 +521,17 @@
                 constructor(e) {
                     super({
                         ...e,
                         promptClass: "jp-Placeholder-prompt jp-OutputPrompt"
                     }), this.addClass("jp-OutputPlaceholder")
                 }
             }
-            var T = s(49269),
-                R = s(1167),
-                V = s(26862);
+            var T = s(30525),
+                R = s(68722),
+                V = s(95183);
             const z = "jp-mod-selected";
             class B extends T.EditorSearchProvider {
                 constructor(e) {
                     super(), this.cell = e, this.cell.inViewport || this.cell.editor || (0, R.signalToPromise)(e.inViewportChanged).then((([, e]) => {
                         e && this.cmHandler.setEditor(this.editor)
                     }))
                 }
@@ -680,17 +680,17 @@
                     case "markdown":
                         return new $(e);
                     default:
                         return new B(e)
                 }
             }
             var Q = s(3546),
-                q = s(96049),
-                G = s(13408),
-                X = s(87017),
+                q = s(53312),
+                G = s(81221),
+                X = s(79426),
                 Y = s(20998),
                 K = s(33625),
                 Z = s(49503),
                 ee = s(97934);
             const te = "jp-mod-resizedCell";
             class se extends C.Widget {
                 constructor(e) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/2489.bundle.js` & `notebook-7.2.0rc1/notebook/static/2489.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -11,18 +11,18 @@
                 DocumentWidget: () => w,
                 MimeContent: () => b,
                 MimeDocument: () => C,
                 MimeDocumentFactory: () => D,
                 TextModelFactory: () => y,
                 createReadonlyLabel: () => g
             });
-            var s, a = i(96049),
-                n = i(1167),
-                o = i(13408),
-                r = i(37267),
+            var s, a = i(53312),
+                n = i(68722),
+                o = i(81221),
+                r = i(12030),
                 l = i(20998),
                 h = i(2549),
                 d = i(81997),
                 c = i(63485);
             class _ {
                 constructor(e) {
                     var t, i;
@@ -427,15 +427,15 @@
                 }
 
                 function i(e) {
                     const t = document.createElement("input");
                     return t.value = e, t
                 }
             }(s || (s = {}));
-            var m = i(52839),
+            var m = i(51429),
                 u = i(78156);
 
             function g(e, t) {
                 var i;
                 let s = (null != t ? t : r.nullTranslator).load("jupyterlab");
                 return a.ReactWidget.create(u.createElement("div", null, u.createElement("span", {
                     className: "jp-ToolbarLabelComponent",
@@ -755,15 +755,15 @@
                 e.createRegistryOptions = function(e) {
                     return {
                         ...e,
                         readOnly: !0
                     }
                 }
             }(x || (x = {}));
-            var S, M = i(22620),
+            var S, M = i(35613),
                 O = i(33625);
             class E {
                 constructor(e = {}) {
                     this._modelFactories = Object.create(null), this._widgetFactories = Object.create(null), this._defaultWidgetFactory = "", this._defaultWidgetFactoryOverrides = Object.create(null), this._defaultWidgetFactories = Object.create(null), this._defaultRenderedWidgetFactories = Object.create(null), this._widgetFactoriesForFileType = Object.create(null), this._fileTypes = [], this._extenders = Object.create(null), this._changed = new d.Signal(this), this._isDisposed = !1;
                     const t = e.textModelFactory;
                     if (this.translator = e.translator || r.nullTranslator, t && "text" !== t.name) throw new Error("Text model factory must have the name `text`");
                     this._modelFactories.text = t || new y(!0), (e.initialFileTypes || E.getDefaultFileTypes(this.translator)).forEach((e => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/2520.bundle.js` & `notebook-7.2.0rc1/notebook/static/2520.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2552.bundle.js` & `notebook-7.2.0rc1/notebook/static/2552.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2607.bundle.js` & `notebook-7.2.0rc1/notebook/static/2607.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -10,18 +10,18 @@
                 KernelMenu: () => c,
                 MainMenu: () => p,
                 RunMenu: () => l,
                 SettingsMenu: () => M,
                 TabsMenu: () => h,
                 ViewMenu: () => _
             });
-            var t, r = s(22620),
+            var t, r = s(35613),
                 i = s(33625),
                 a = s(63485),
-                u = s(96049);
+                u = s(53312);
             class d extends r.RankedMenu {
                 constructor(e) {
                     super(e), this.undoers = {
                         redo: new u.SemanticCommand,
                         undo: new u.SemanticCommand
                     }, this.clearers = {
                         clearAll: new u.SemanticCommand,
```

### Comparing `notebook-7.2.0rc0/notebook/static/261.bundle.js` & `notebook-7.2.0rc1/notebook/static/261.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2615.bundle.js` & `notebook-7.2.0rc1/notebook/static/2615.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -16,15 +16,15 @@
                 MermaidMarkdown: () => _,
                 RenderedMermaid: () => w,
                 SUMMARY_CLASS: () => g,
                 WARNING_CLASS: () => o,
                 rendererFactory: () => T
             });
             var r = a(20998),
-                n = a(1167);
+                n = a(68722);
             const i = "text/vnd.mermaid",
                 s = [".mmd", ".mermaid"],
                 d = "default",
                 m = "dark",
                 l = "jp-RenderedMermaid",
                 c = "mermaid",
                 o = "jp-mod-warning",
```

### Comparing `notebook-7.2.0rc0/notebook/static/2636.bundle.js` & `notebook-7.2.0rc1/notebook/static/2636.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
                 ConsoleHistory: () => a,
                 ConsolePanel: () => S,
                 ForeignHandler: () => r,
                 IConsoleCellExecutor: () => E,
                 IConsoleTracker: () => F,
                 runCell: () => n
             });
-            var o = s(67406);
+            var o = s(73166);
             async function n({
                 cell: e,
                 onCellExecuted: t,
                 sessionContext: s
             }) {
                 return o.CodeCell.execute(e, s).then((s => {
                     if (s && "ok" === s.content.status) {
@@ -208,25 +208,25 @@
                 e.initialRequest = {
                     output: !1,
                     raw: !0,
                     hist_access_type: "tail",
                     n: 500
                 }
             }(i || (i = {}));
-            var c = s(96049),
-                h = s(1167),
-                d = s(13408),
-                u = s(37267),
-                p = s(22620),
+            var c = s(53312),
+                h = s(68722),
+                d = s(81221),
+                u = s(12030),
+                p = s(35613),
                 _ = s(20998),
                 C = s(63485),
                 m = s(89843),
                 g = s(3546),
                 y = s(57508),
-                f = s(58959),
+                f = s(31231),
                 v = s(99615);
             const x = "jp-Console-cell",
                 w = "jp-CodeConsole-promptCell";
             class D extends C.Widget {
                 constructor(e) {
                     var t, s, o;
                     super(), this.editorConfig = D.defaultEditorConfig, this._banner = null, this._executed = new l.Signal(this), this._mimetype = "text/x-ipython", this._msgIds = new Map, this._msgIdCells = new Map, this._promptCellCreated = new l.Signal(this), this._dragData = null, this._drag = null, this._focusedCell = null, this._translator = null !== (t = e.translator) && void 0 !== t ? t : u.nullTranslator, this._executor = null !== (s = e.executor) && void 0 !== s ? s : Object.freeze({
```

### Comparing `notebook-7.2.0rc0/notebook/static/2666.bundle.js` & `notebook-7.2.0rc1/notebook/static/2666.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/26683bf201fb258a2237.woff` & `notebook-7.2.0rc1/notebook/static/26683bf201fb258a2237.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2682.bundle.js` & `notebook-7.2.0rc1/notebook/static/2682.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2692.bundle.js` & `notebook-7.2.0rc1/notebook/static/2692.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [2692], {
         22692: (t, e, r) => {
             r.d(e, {
                 diagram: () => M
             });
             var i = r(24028),
-                a = r(29197),
+                a = r(67406),
                 n = r(23617),
                 s = r(7259);
             const o = [];
             for (let t = 0; t < 256; ++t) o.push((t + 256).toString(16).slice(1));
             const c = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i,
                 l = function(t) {
                     if (! function(t) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/270.bundle.js` & `notebook-7.2.0rc1/notebook/static/270.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2702.bundle.js` & `notebook-7.2.0rc1/notebook/static/2702.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2756.bundle.js` & `notebook-7.2.0rc1/notebook/static/2756.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/28.bundle.js` & `notebook-7.2.0rc1/notebook/static/28.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2813.bundle.js` & `notebook-7.2.0rc1/notebook/static/2813.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2866.bundle.js` & `notebook-7.2.0rc1/notebook/static/2866.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2871.bundle.js` & `notebook-7.2.0rc1/notebook/static/2871.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2913.bundle.js` & `notebook-7.2.0rc1/notebook/static/2913.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2913.bundle.js.LICENSE.txt` & `notebook-7.2.0rc1/notebook/static/2913.bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/2924.bundle.js` & `notebook-7.2.0rc1/notebook/static/2924.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,16 +4,16 @@
         22924: (t, e, o) => {
             o.r(e), o.d(e, {
                 FormWidget: () => r,
                 IMetadataFormProvider: () => g,
                 MetadataFormProvider: () => v,
                 MetadataFormWidget: () => _
             });
-            var a = o(96049),
-                i = o(22620),
+            var a = o(53312),
+                i = o(35613),
                 s = o(27478),
                 l = o.n(s),
                 d = o(78156),
                 n = o.n(d);
             class r extends a.ReactWidget {
                 constructor(t) {
                     super(), this.addClass("jp-FormWidget"), this._props = t
@@ -36,17 +36,17 @@
                         },
                         compact: !0,
                         showModifiedFromDefault: this._props.showModified,
                         translator: this._props.translator
                     })
                 }
             }
-            var h, m = o(17894),
-                p = o(24554),
-                c = o(37267),
+            var h, m = o(25460),
+                p = o(23295),
+                c = o(12030),
                 u = o(20998),
                 f = o(63485);
             class _ extends m.NotebookTools.Tool {
                 constructor(t) {
                     super(), this.updateMetadata = (t, e) => {
                         var o, a, i, s, l, d, n, r;
                         if (null == this.notebookTools) return;
```

### Comparing `notebook-7.2.0rc0/notebook/static/2944.bundle.js` & `notebook-7.2.0rc1/notebook/static/2944.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -17,16 +17,16 @@
                 InlineCompletionTriggerKind: () => n,
                 KERNEL_PROVIDER_ID: () => L,
                 KernelCompleterProvider: () => H,
                 ProviderReconciliator: () => M,
                 completerWidgetIcon: () => K,
                 inlineCompleterIcon: () => U
             });
-            var s, n, o = i(52839),
-                r = i(1167),
+            var s, n, o = i(51429),
+                r = i(68722),
                 l = i(49503),
                 a = i(81997),
                 h = i(20998);
             ! function(e) {
                 e[e.Invoked = 1] = "Invoked", e[e.TriggerCharacter = 2] = "TriggerCharacter", e[e.TriggerForIncompleteCompletions = 3] = "TriggerForIncompleteCompletions"
             }(s || (s = {})),
             function(e) {
@@ -431,17 +431,17 @@
                     const s = Array.from(i);
                     return s.sort(((e, t) => e.localeCompare(t))), t.concat(s)
                 }, e.findOrderedTypes = function(e) {
                     const s = Object.keys(e).map((t => e[t])).filter((e => !!e && !(e in i))).sort(((e, t) => e.localeCompare(t)));
                     return t.concat(s)
                 }
             }(m || (m = {}));
-            var v = i(96049),
-                f = i(13408),
-                C = i(22620),
+            var v = i(53312),
+                f = i(81221),
+                C = i(35613),
                 y = i(18395),
                 w = i(63485);
             const x = "jp-Completer-item",
                 P = "jp-mod-active",
                 I = "jp-Completer-list",
                 S = !0;
             class b extends w.Widget {
@@ -1720,15 +1720,15 @@
                     name: "completer:inline",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n  <path class="jp-icon4" fill="#bbbbbb" d="M17 15H3v2h14v-2Zm0-8h-6v2h6V7ZM3 13h18v-2H3v2Zm0 8h18v-2H3v2Z"/>\n  <path class="jp-icon1" fill="#616161" d="M3 3v2h18V3H3ZM3 7v2h8V7H3Z"/>\n</svg>\n'
                 }),
                 K = new C.LabIcon({
                     name: "completer:widget",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 24 24">\n<g fill="#616161" class="jp-icon2 jp-icon-selectable">\n  <path d="M6 8h16v14.3H6z" style="fill:#eee;stroke:#444;stroke-linejoin:round"/>\n  <path d="M3 3v2h10V3H3Z" transform="matrix(.8 0 0 1 .5 0)"/>\n</g>\n<g class="jp-icon3 jp-icon-selectable">\n  <path fill="#616161" d="M18 14.1H8v2h11v-2ZM8 12.1H20V10.1H8v2Zm0 8H20v-2H8v3Z"/>\n</g>\n</svg>\n'
                 });
-            var Z = i(37267);
+            var Z = i(12030);
             class $ {
                 constructor(e) {
                     this.options = e, this.identifier = "@jupyterlab/inline-completer:history", this._maxSuggestions = 100;
                     const t = e.translator || Z.nullTranslator;
                     this._trans = t.load("jupyterlab")
                 }
                 get name() {
```

### Comparing `notebook-7.2.0rc0/notebook/static/2955.bundle.js` & `notebook-7.2.0rc1/notebook/static/2955.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3079.bundle.js` & `notebook-7.2.0rc1/notebook/static/3079.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/30e889b58cbc51adfbb0.woff` & `notebook-7.2.0rc1/notebook/static/30e889b58cbc51adfbb0.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/311.bundle.js` & `notebook-7.2.0rc1/notebook/static/311.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3111.bundle.js` & `notebook-7.2.0rc1/notebook/static/3111.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3129.bundle.js` & `notebook-7.2.0rc1/notebook/static/3129.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -3,18 +3,18 @@
     [3129, 9268], {
         79268: (e, n, r) => {
             r.r(n), r.d(n, {
                 createMarkdownParser: () => l,
                 default: () => u
             });
             var t = r(20998),
-                a = r(1167),
-                i = r(49269),
-                o = r(13408),
-                s = r(83149);
+                a = r(68722),
+                i = r(30525),
+                o = r(81221),
+                s = r(8337);
             const c = "```~~~";
 
             function l(e, n) {
                 return {
                     render: r => d.render(r, e, n)
                 }
             }
```

### Comparing `notebook-7.2.0rc0/notebook/static/3154.bundle.js` & `notebook-7.2.0rc1/notebook/static/3154.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [3154], {
         43154: (e, t, s) => {
             s.d(t, {
                 diagram: () => _
             });
             var o = s(75343),
-                i = s(29197),
+                i = s(67406),
                 a = s(23617),
                 r = s(24028),
                 n = s(86281);
             s(27693), s(7608), s(31699), s(7259), s(81779);
             const d = "rect",
                 l = "rectWithTitle",
                 c = "statediagram",
```

### Comparing `notebook-7.2.0rc0/notebook/static/3187.bundle.js` & `notebook-7.2.0rc1/notebook/static/3187.bundle.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [3187], {
         53187: (e, n, a) => {
             a.r(n), a.d(n, {
                 default: () => d
             });
-            var l, r = a(2922),
-                t = a(96049),
-                i = a(37267),
-                o = a(22620),
-                s = a(57355);
+            var l, r = a(44604),
+                t = a(53312),
+                i = a(12030),
+                o = a(35613),
+                s = a(9033);
             ! function(e) {
                 e.open = "pluginmanager:open", e.refreshPlugins = "pluginmanager:refresh"
             }(l || (l = {}));
             const u = "@jupyterlab/pluginmanager-extension:plugin",
                 d = [{
                     id: u,
                     description: "Enable or disable individual plugins.",
```

### Comparing `notebook-7.2.0rc0/notebook/static/3211.bundle.js` & `notebook-7.2.0rc1/notebook/static/3211.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3213.bundle.js` & `notebook-7.2.0rc1/notebook/static/3213.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -23,15 +23,15 @@
                     initialCommand: "",
                     screenReaderMode: !1,
                     pasteWithCtrlV: !0,
                     autoFit: !0,
                     macOptionIsMeta: !1
                 }
             }(o || (o = {}));
-            var r, a = s(37267),
+            var r, a = s(12030),
                 h = s(18395),
                 c = s(49503),
                 d = s(63485);
             class l extends d.Widget {
                     constructor(e, t = {}, s) {
                         super(), this._needsResize = !0, this._offsetWidth = -1, this._offsetHeight = -1, this._isReady = !1, this._ready = new i.PromiseDelegate, this._termOpened = !1, s = s || a.nullTranslator, this._trans = s.load("jupyterlab"), this.session = e, this._options = {
                             ...o.defaultOptions,
```

### Comparing `notebook-7.2.0rc0/notebook/static/3230.bundle.js` & `notebook-7.2.0rc1/notebook/static/3230.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/32792104b5ef69eded90.woff` & `notebook-7.2.0rc1/notebook/static/32792104b5ef69eded90.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3301.bundle.js` & `notebook-7.2.0rc1/notebook/static/3301.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3322.bundle.js` & `notebook-7.2.0rc1/notebook/static/3322.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3325.bundle.js` & `notebook-7.2.0rc1/notebook/static/3325.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3336.bundle.js` & `notebook-7.2.0rc1/notebook/static/3336.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3340.bundle.js` & `notebook-7.2.0rc1/notebook/static/3340.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [3340], {
         33340: (e, n, t) => {
             t.r(n), t.d(n, {
                 default: () => y
             });
-            var o = t(22620),
-                i = t(89144),
-                r = t(24554),
-                l = t(37267),
+            var o = t(35613),
+                i = t(81002),
+                r = t(23295),
+                l = t(12030),
                 a = t(16934),
                 c = t(78156),
                 s = t.n(c);
             const d = "availableProviders";
 
             function m(e) {
                 const {
```

### Comparing `notebook-7.2.0rc0/notebook/static/3360.bundle.js` & `notebook-7.2.0rc1/notebook/static/3360.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,17 +4,17 @@
         63360: (t, e, s) => {
             s.r(e), s.d(e, {
                 IJSONSettingEditorTracker: () => W.g,
                 ISettingEditorTracker: () => W.O,
                 JsonSettingEditor: () => O,
                 SettingsEditor: () => S
             });
-            var i = s(96049),
-                r = s(37267),
-                n = s(22620),
+            var i = s(53312),
+                r = s(12030),
+                n = s(35613),
                 a = s(81997),
                 o = s(63485),
                 l = s(78156),
                 d = s.n(l),
                 h = s(33625);
             class c extends i.ReactWidget {
                 constructor(t) {
@@ -422,15 +422,15 @@
                         title: e.__("Warning"),
                         body: e.__("Some changes have not been saved. Continue without saving?")
                     }).then((e => {
                         e.button.accept && (this.dispose(), super.onCloseRequest(t))
                     })) : (this.dispose(), super.onCloseRequest(t))
                 }
             }
-            var y = s(52839);
+            var y = s(51429);
             const E = "jp-Inspector-content";
             class w extends o.Panel {
                 constructor(t = {}) {
                     super(), this._source = null, this.translator = t.translator || r.nullTranslator, this._trans = this.translator.load("jupyterlab"), t.initialContent instanceof o.Widget ? this._content = t.initialContent : "string" == typeof t.initialContent ? this._content = w._generateContentWidget(`<p>${t.initialContent}</p>`) : this._content = w._generateContentWidget("<p>" + this._trans.__("Click on a function to see documentation.") + "</p>"), this.addClass("jp-Inspector"), this.layout.addWidget(this._content)
                 } [i.Printing.symbol]() {
                     return () => i.Printing.printWidget(this)
                 }
@@ -453,16 +453,16 @@
                     this.source = null
                 }
                 static _generateContentWidget(t) {
                     const e = new o.Widget;
                     return e.node.innerHTML = t, e.addClass(E), e.addClass("jp-Inspector-default-content"), e
                 }
             }
-            var b = s(1167),
-                C = s(13408);
+            var b = s(68722),
+                C = s(81221);
             class j {
                 constructor(t) {
                     this._cleared = new a.Signal(this), this._disposed = new a.Signal(this), this._editor = null, this._inspected = new a.Signal(this), this._isDisposed = !1, this._pending = 0, this._standby = !0, this._lastInspectedReply = null, this._connector = t.connector, this._rendermime = t.rendermime, this._debouncer = new p.Debouncer(this.onEditorChange.bind(this), 250)
                 }
                 get cleared() {
                     return this._cleared
                 }
@@ -526,15 +526,15 @@
                         this._lastInspectedReply = null, this._inspected.emit(n)
                     }))
                 }
                 _onChange() {
                     this._debouncer.invoke()
                 }
             }
-            var D = s(96692);
+            var D = s(41053);
             class P extends D.DataConnector {
                 constructor(t, e) {
                     super(), this._current = 0, this._editor = t, this._trans = (null != e ? e : r.nullTranslator).load("jupyterlab")
                 }
                 fetch(t) {
                     return new Promise((e => {
                         const s = this._current = window.setTimeout((() => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/3370.bundle.js` & `notebook-7.2.0rc1/notebook/static/3370.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3420.bundle.js` & `notebook-7.2.0rc1/notebook/static/3420.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3449.bundle.js` & `notebook-7.2.0rc1/notebook/static/3449.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3462.bundle.js` & `notebook-7.2.0rc1/notebook/static/3462.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3466.bundle.js` & `notebook-7.2.0rc1/notebook/static/3466.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,25 +2,25 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [3466], {
         83466: (e, t, r) => {
             r.r(t), r.d(t, {
                 RunningLanguageServer: () => _,
                 default: () => k
             });
-            var n = r(52138),
-                a = r(15729),
-                s = r(24554),
-                o = r(37267),
-                i = r(22620),
+            var n = r(61907),
+                a = r(9235),
+                s = r(23295),
+                o = r(12030),
+                i = r(35613),
                 c = r(81997),
                 l = r(20998),
                 u = r(97934),
                 m = r(78156),
                 d = r.n(m),
-                p = r(96049);
+                p = r(53312);
             const g = "languageServers",
                 h = "configuration";
 
             function v(e) {
                 const {
                     [h]: t, ...r
                 } = e.schema, {
```

### Comparing `notebook-7.2.0rc0/notebook/static/3488.bundle.js` & `notebook-7.2.0rc1/notebook/static/3488.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/35.bundle.js` & `notebook-7.2.0rc1/notebook/static/35.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3501.bundle.js` & `notebook-7.2.0rc1/notebook/static/3501.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3512.bundle.js` & `notebook-7.2.0rc1/notebook/static/3512.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -30,16 +30,16 @@
                 offsetAtPosition: () => J,
                 positionAtOffset: () => H,
                 sleep: () => C,
                 untilReady: () => S
             });
             var i = n(95282),
                 r = n.n(i),
-                s = n(96049),
-                o = n(37267),
+                s = n(53312),
+                o = n(12030),
                 a = n(81997);
             class c {
                 constructor(e) {
                     this._widgetAdapter = e.widgetAdapter, this._extensions = e.extensions, e.editor.ready().then((t => {
                         this._injectExtensions(e.editor)
                     }))
                 }
@@ -282,15 +282,15 @@
                     if (!this._virtualDocument) return;
                     const {
                         model: e
                     } = this.widget.context;
                     this._shouldUpdateVirtualDocument() ? e.contentChanged.connect(this._onContentChanged, this) : e.contentChanged.disconnect(this._onContentChanged, this)
                 }
             }
-            var h = n(10979);
+            var h = n(65903);
             class f {
                 constructor(e) {
                     this._isDisposed = !1, this._current = null, this._adapters = new Set, this._adapterAdded = new a.Signal(this), this._adapterUpdated = new a.Signal(this), this._currentChanged = new a.Signal(this), (this._shell = e.shell).currentChanged.connect(((e, t) => {
                         let n = t.newValue;
                         if (!(n && n instanceof h.DocumentWidget)) return;
                         const i = this.find((e => e.widget === n));
                         i && (this._current = i, this._currentChanged.emit(i))
@@ -346,15 +346,15 @@
                         e(n) && t.push(n)
                     })), t
                 }
                 has(e) {
                     return this._adapters.has(e)
                 }
             }
-            var g, p = n(1167),
+            var g, p = n(68722),
                 m = n(20998);
             ! function(e) {
                 e.URL_NS = "lsp"
             }(g || (g = {}));
             const v = new m.Token("@jupyterlab/lsp:ILSPDocumentConnectionManager", "Provides the virtual documents and language server connections service."),
                 _ = new m.Token("@jupyterlab/lsp:ILSPFeatureManager", "Provides the language server feature manager. This token is required to register new client capabilities."),
                 y = new m.Token("@jupyterlab/lsp:ILSPCodeExtractorsManager", "Provides the code extractor manager. This token is required in your extension to register code extractor allowing the creation of multiple virtual document from an opened document."),
@@ -1149,15 +1149,15 @@
                 }
                 extensionFactories() {
                     const e = [];
                     for (const t of this.features) t.extensionFactory && e.push(t.extensionFactory);
                     return e
                 }
             }
-            var K = n(70611);
+            var K = n(87408);
             class Z {
                 constructor(e) {
                     this._sessions = new Map, this._specs = new Map, this._warningsEmitted = new Set, this._ready = new m.PromiseDelegate, this._sessionsChanged = new a.Signal(this), this._isDisposed = !1, this._enabled = !0, this._settings = e.settings || K.ServerConnection.makeSettings(), this._baseUrl = e.baseUrl || p.PageConfig.getBaseUrl(), this._retries = e.retries || 2, this._retriesInterval = e.retriesInterval || 1e4, this._statusCode = -1, this._configuration = {}, this.fetchSessions().catch((e => console.log(e)))
                 }
                 get isEnabled() {
                     return this._enabled
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/355254db9ca10a09a3b5.woff` & `notebook-7.2.0rc1/notebook/static/355254db9ca10a09a3b5.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3562.bundle.js` & `notebook-7.2.0rc1/notebook/static/3562.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3676.bundle.js` & `notebook-7.2.0rc1/notebook/static/3676.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
             }
         },
         76418: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.BuildManager = void 0;
-            const n = s(1167),
+            const n = s(68722),
                 i = s(43851);
             t.BuildManager = class {
                 constructor(e = {}) {
                     var t;
                     this._url = "", this.serverSettings = null !== (t = e.serverSettings) && void 0 !== t ? t : i.ServerConnection.makeSettings();
                     const {
                         baseUrl: s,
@@ -92,15 +92,15 @@
             }
         },
         34027: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.ConfigWithDefaults = t.ConfigSection = void 0;
-            const n = s(1167),
+            const n = s(68722),
                 i = s(83676);
             var r;
             ! function(e) {
                 e.create = function(e) {
                     const t = new o(e);
                     return t.load().then((() => t))
                 }
@@ -185,15 +185,15 @@
                     if (null != e)
                         for (var s in e) "default" !== s && Object.prototype.hasOwnProperty.call(e, s) && n(t, e, s);
                     return i(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Drive = t.ContentsManager = t.Contents = void 0;
-            const o = s(1167),
+            const o = s(68722),
                 a = s(81997),
                 l = s(83676),
                 c = r(s(36556));
             var h, u;
             ! function(e) {
                 e.validateContentsModel = function(e) {
                     c.validateContentsModel(e)
@@ -558,15 +558,15 @@
             }
         },
         95348: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.EventManager = void 0;
-            const n = s(1167),
+            const n = s(68722),
                 i = s(97934),
                 r = s(81997),
                 o = s(43851),
                 a = "api/events";
             t.EventManager = class {
                 constructor(e = {}) {
                     var t;
@@ -784,15 +784,15 @@
                     if (null != e)
                         for (var s in e) "default" !== s && Object.prototype.hasOwnProperty.call(e, s) && n(t, e, s);
                     return i(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.KernelConnection = void 0;
-            const o = s(1167),
+            const o = s(68722),
                 a = s(20998),
                 l = s(81997),
                 c = s(83676),
                 h = s(35139),
                 u = r(s(70552)),
                 d = s(60682),
                 p = r(s(92917)),
@@ -1725,15 +1725,15 @@
         },
         33505: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.getKernelModel = t.shutdownKernel = t.interruptKernel = t.restartKernel = t.startNew = t.listRunning = t.KERNEL_SERVICE_URL = void 0;
             const n = s(43851),
-                i = s(1167),
+                i = s(68722),
                 r = s(92917);
             t.KERNEL_SERVICE_URL = "api/kernels", t.listRunning = async function(e = n.ServerConnection.makeSettings()) {
                 const s = i.URLExt.join(e.baseUrl, t.KERNEL_SERVICE_URL),
                     o = await n.ServerConnection.makeRequest(s, {}, e);
                 if (200 !== o.status) throw await n.ServerConnection.ResponseError.create(o);
                 const a = await o.json();
                 return (0, r.validateModels)(a), a
@@ -2131,15 +2131,15 @@
         29723: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.getSpecs = void 0;
             const n = s(43851),
                 i = s(4891),
-                r = s(1167);
+                r = s(68722);
             t.getSpecs = async function(e = n.ServerConnection.makeSettings()) {
                 const t = r.URLExt.join(e.baseUrl, "api/kernelspecs"),
                     s = await n.ServerConnection.makeRequest(t, {}, e);
                 if (200 !== s.status) throw await n.ServerConnection.ResponseError.create(s);
                 const o = await s.json();
                 return (0, i.validateSpecModels)(o)
             }
@@ -2247,15 +2247,15 @@
             }
         },
         8178: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.NbConvertManager = void 0;
-            const n = s(1167),
+            const n = s(68722),
                 i = s(43851),
                 r = s(20998);
             t.NbConvertManager = class {
                 constructor(e = {}) {
                     var t;
                     this._exportFormats = null, this.serverSettings = null !== (t = e.serverSettings) && void 0 !== t ? t : i.ServerConnection.makeSettings()
                 }
@@ -2284,15 +2284,15 @@
         },
         43851: (e, t, s) => {
             "use strict";
             var n = s(27061);
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.ServerConnection = void 0;
-            const i = s(1167),
+            const i = s(68722),
                 r = s(81259);
             let o;
             var a, l;
             o = "undefined" == typeof window ? s(67277) : WebSocket,
                 function(e) {
                     e.makeSettings = function(e) {
                         return l.makeSettings(e)
@@ -2743,15 +2743,15 @@
         },
         79: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.updateSession = t.startSession = t.getSessionModel = t.shutdownSession = t.getSessionUrl = t.listRunning = t.SESSION_SERVICE_URL = void 0;
             const n = s(43851),
-                i = s(1167),
+                i = s(68722),
                 r = s(11180);
 
             function o(e, s) {
                 const n = i.URLExt.join(e, t.SESSION_SERVICE_URL),
                     r = i.URLExt.join(n, s);
                 if (!r.startsWith(n)) throw new Error("Can only be used for services requests");
                 return r
@@ -2831,16 +2831,16 @@
             }
         },
         69494: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.SettingManager = void 0;
-            const n = s(1167),
-                i = s(96692),
+            const n = s(68722),
+                i = s(41053),
                 r = s(43851);
             class o extends i.DataConnector {
                 constructor(e = {}) {
                     var t;
                     super(), this.serverSettings = null !== (t = e.serverSettings) && void 0 !== t ? t : r.ServerConnection.makeSettings()
                 }
                 async fetch(e) {
@@ -2919,15 +2919,15 @@
             }), t.default = WebSocket
         },
         49253: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.TerminalConnection = void 0;
-            const n = s(1167),
+            const n = s(68722),
                 i = s(20998),
                 r = s(81997),
                 o = s(83676),
                 a = s(11887);
             class l {
                 constructor(e) {
                     var t;
@@ -3205,15 +3205,15 @@
                 }(c || (t.TerminalManager = c = {}))
         },
         11887: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.shutdownTerminal = t.listRunning = t.startNew = t.isAvailable = t.TERMINAL_SERVICE_URL = void 0;
-            const n = s(1167),
+            const n = s(68722),
                 i = s(43851);
 
             function r() {
                 return "true" === String(n.PageConfig.getOption("terminalsAvailable")).toLowerCase()
             }
             var o;
             t.TERMINAL_SERVICE_URL = "api/terminals", t.isAvailable = r, t.startNew = async function(e = i.ServerConnection.makeSettings(), s, r) {
@@ -3271,15 +3271,15 @@
             })
         },
         78162: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UserManager = void 0;
-            const n = s(1167),
+            const n = s(68722),
                 i = s(20998),
                 r = s(97934),
                 o = s(81997),
                 a = s(43851),
                 l = s(78037),
                 c = "@jupyterlab/services:UserManager#user";
             class h extends l.BaseManager {
@@ -3395,16 +3395,16 @@
             }
         },
         53265: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.WorkspaceManager = void 0;
-            const n = s(1167),
-                i = s(96692),
+            const n = s(68722),
+                i = s(41053),
                 r = s(43851);
             class o extends i.DataConnector {
                 constructor(e = {}) {
                     var t;
                     super(), this.serverSettings = null !== (t = e.serverSettings) && void 0 !== t ? t : r.ServerConnection.makeSettings()
                 }
                 async fetch(e) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/3680.bundle.js` & `notebook-7.2.0rc1/notebook/static/3680.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -35,15 +35,15 @@
                     }
                 }, e) : i.createElement("div", {
                     style: {
                         margin: `0px ${t}px`
                     }
                 }, e))))
             }
-            var n = s(22620),
+            var n = s(35613),
                 o = s(63485);
 
             function d(e) {
                 const t = new h(e);
                 return e.startHidden || t.launch(), t
             }
             class h extends o.Widget {
```

### Comparing `notebook-7.2.0rc0/notebook/static/36e0d72d8a7afc696a3e.woff` & `notebook-7.2.0rc1/notebook/static/36e0d72d8a7afc696a3e.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3700.bundle.js` & `notebook-7.2.0rc1/notebook/static/3700.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3733.bundle.js` & `notebook-7.2.0rc1/notebook/static/3733.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/373c04fd2418f5c77eea.eot` & `notebook-7.2.0rc1/notebook/static/373c04fd2418f5c77eea.eot`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/374.bundle.js` & `notebook-7.2.0rc1/notebook/static/374.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -32,18 +32,18 @@
                 RunningStatus: () => pe,
                 StaticNotebook: () => ge,
                 ToolbarItems: () => f,
                 getIdForHeading: () => be,
                 runCell: () => u,
                 setCellExecutor: () => v
             });
-            var o = n(96049),
-                i = n(67406),
-                s = n(1167),
-                l = n(37267),
+            var o = n(53312),
+                i = n(73166),
+                s = n(68722),
+                l = n(12030),
                 a = n(33625),
                 d = n(20998),
                 r = n(81997),
                 c = n(78156),
                 h = n.n(c);
             async function u({
                 cell: e,
@@ -1007,15 +1007,15 @@
                             newValues: [],
                             oldIndex: o,
                             oldValues: new Array(e.delete).fill(void 0)
                         }) : null != e.retain && (o += e.retain)
                     })), i.forEach((e => this._changed.emit(e)))
                 }
             }
-            var f, w = n(22620);
+            var f, w = n(35613);
             ! function(e) {
                 function t(e, t) {
                     const n = (t || l.nullTranslator).load("jupyterlab");
 
                     function i() {
                         if (e.context.model.readOnly) return (0, o.showDialog)({
                             title: n.__("Cannot Save"),
@@ -1177,16 +1177,16 @@
                     }, this._trans.__("Code")), c.createElement("option", {
                         value: "markdown"
                     }, this._trans.__("Markdown")), c.createElement("option", {
                         value: "raw"
                     }, this._trans.__("Raw")))
                 }
             }
-            var b = n(27829),
-                k = n(70611);
+            var b = n(71098),
+                k = n(87408);
 
             function S(e) {
                 const t = e.translator || l.nullTranslator,
                     n = (0, o.translateKernelStatuses)(t),
                     i = t.load("jupyterlab"),
                     s = e.state,
                     a = e.displayOption.showOnToolBar,
@@ -1494,15 +1494,15 @@
                     this._filtered.length = 0;
                     let t = "",
                         n = "";
                     for (let o = 0; o < this._history.length; o++) n = this._history[o][2], n !== t && e !== n && this._filtered.push(t = n);
                     this._filtered.push(e)
                 }
             }
-            var I = n(81692),
+            var I = n(81139),
                 E = n(57508);
             class A {
                 constructor(e = {}) {
                     var t, n;
                     this.standaloneModel = !1, this._dirty = !1, this._readOnly = !1, this._contentChanged = new r.Signal(this), this._stateChanged = new r.Signal(this), this._isDisposed = !1, this._metadataChanged = new r.Signal(this), this.standaloneModel = void 0 === e.sharedModel, e.sharedModel ? this.sharedModel = e.sharedModel : this.sharedModel = E.YNotebook.create({
                         disableDocumentWideUndoRedo: null === (t = e.disableDocumentWideUndoRedo) || void 0 === t || t,
                         data: {
@@ -1704,29 +1704,29 @@
                     })
                 }
                 preferredLanguage(e) {
                     return ""
                 }
             }
 
-            function N(e) {
+            function P(e) {
                 const t = (e.translator || l.nullTranslator).load("jupyterlab");
                 return c.createElement(b.TextItem, {
                     source: t.__("Mode: %1", e.modeNames[e.notebookMode])
                 })
             }
             class H extends w.VDomRenderer {
                 constructor(e) {
                     super(new H.Model), this.translator = e || l.nullTranslator, this._trans = this.translator.load("jupyterlab"), this._modeNames = {
                         command: this._trans.__("Command"),
                         edit: this._trans.__("Edit")
                     }
                 }
                 render() {
-                    return this.model ? (this.node.title = this._trans.__("Notebook is in %1 mode", this._modeNames[this.model.notebookMode]), c.createElement(N, {
+                    return this.model ? (this.node.title = this._trans.__("Notebook is in %1 mode", this._modeNames[this.model.notebookMode]), c.createElement(P, {
                         notebookMode: this.model.notebookMode,
                         translator: this.translator,
                         modeNames: this._modeNames
                     })) : null
                 }
             }! function(e) {
                 class t extends w.VDomModel {
@@ -1747,29 +1747,29 @@
                     }
                     _triggerChange(e, t) {
                         e !== t && this.stateChanged.emit(void 0)
                     }
                 }
                 e.Model = t
             }(H || (H = {}));
-            var P = n(52839),
-                D = n(52138);
+            var N = n(51429),
+                D = n(61907);
             class L extends D.WidgetLSPAdapter {
                 constructor(e, t) {
                     super(e, t), this.editorWidget = e, this.options = t, this._type = "code", this._readyDelegate = new d.PromiseDelegate, this._editorToCell = new Map, this.editor = e.content, this._cellToEditor = new WeakMap, Promise.all([this.widget.context.sessionContext.ready, this.connectionManager.ready]).then((async () => {
                         await this.initOnceReady(), this._readyDelegate.resolve()
                     })).catch(console.error)
                 }
                 get documentPath() {
                     return this.widget.context.path
                 }
                 get mimeType() {
                     var e;
                     let t, n = this.language_info();
-                    return t = n && n.mimetype ? n.mimetype : this.widget.content.codeMimetype, Array.isArray(t) ? null !== (e = t[0]) && void 0 !== e ? e : P.IEditorMimeTypeService.defaultMimeType : t
+                    return t = n && n.mimetype ? n.mimetype : this.widget.content.codeMimetype, Array.isArray(t) ? null !== (e = t[0]) && void 0 !== e ? e : N.IEditorMimeTypeService.defaultMimeType : t
                 }
                 get languageFileExtension() {
                     let e = this.language_info();
                     if (e && e.file_extension) return e.file_extension.replace(".", "")
                 }
                 get wrapperElement() {
                     return this.widget.node
@@ -1885,15 +1885,15 @@
                         })), this._editorAdded.emit({
                             editor: t
                         })
                     }
                     return this._cellToEditor.get(e)
                 }
             }
-            var O, R = n(58959),
+            var O, R = n(31231),
                 B = n(49503),
                 F = n(63485);
             class W extends F.Widget {
                 constructor() {
                     super(), this._items = [], this.layout = new F.PanelLayout, this.addClass("jp-RankedPanel")
                 }
                 addWidget(e, t) {
@@ -2044,27 +2044,27 @@
                         get editor() {
                             return this._editor
                         }
                         onActiveNotebookPanelChanged(e) {
                             this.editor.dispose(), this.notebookTools.activeNotebookPanel && this.createEditor()
                         }
                         createEditor() {
-                            this._editor = new P.JSONEditor({
+                            this._editor = new N.JSONEditor({
                                 editorFactory: this._editorFactory
                             }), this.editor.title.label = this._editorLabel, this.layout.addWidget(this.editor)
                         }
                     }
                 }(V || (V = {})),
                 function(e) {
                     e.itemCmp = function(e, t) {
                         return e.rank - t.rank
                     }
                 }(O || (O = {}));
-            var j = n(10979),
-                U = n(87017),
+            var j = n(65903),
+                U = n(79426),
                 q = n(18395),
                 K = n(99615),
                 z = n(14421),
                 $ = n(24475);
             const J = "jp-mod-dropTarget",
                 Y = "jp-mod-dropSource";
             var G = n(97934);
@@ -2241,15 +2241,15 @@
                         model: new Q(d, {
                             overscanCount: null !== (i = null === (o = e.notebookConfig) || void 0 === o ? void 0 : o.overscanCount) && void 0 !== i ? i : ge.defaultNotebookConfig.overscanCount,
                             windowingActive: c
                         }),
                         layout: new X,
                         renderer: null !== (s = e.renderer) && void 0 !== s ? s : w.WindowedList.defaultRenderer,
                         scrollbar: !1
-                    }), this._cellCollapsed = new r.Signal(this), this._cellInViewportChanged = new r.Signal(this), this._renderingLayoutChanged = new r.Signal(this), this.addClass("jp-Notebook"), this.cellsArray = d, this._idleCallBack = null, this._editorConfig = ge.defaultEditorConfig, this._notebookConfig = ge.defaultNotebookConfig, this._mimetype = P.IEditorMimeTypeService.defaultMimeType, this._notebookModel = null, this._modelChanged = new r.Signal(this), this._modelContentChanged = new r.Signal(this), this.node.dataset.jpKernelUser = "true", this.node.dataset.jpUndoer = "true", this.node.dataset.jpCodeRunner = "true", this.rendermime = e.rendermime, this.translator = e.translator || l.nullTranslator, this.contentFactory = e.contentFactory, this.editorConfig = e.editorConfig || ge.defaultEditorConfig, this.notebookConfig = e.notebookConfig || ge.defaultNotebookConfig, this._updateNotebookConfig(), this._mimetypeService = e.mimeTypeService, this.renderingLayout = null === (a = e.notebookConfig) || void 0 === a ? void 0 : a.renderingLayout, this.kernelHistory = e.kernelHistory
+                    }), this._cellCollapsed = new r.Signal(this), this._cellInViewportChanged = new r.Signal(this), this._renderingLayoutChanged = new r.Signal(this), this.addClass("jp-Notebook"), this.cellsArray = d, this._idleCallBack = null, this._editorConfig = ge.defaultEditorConfig, this._notebookConfig = ge.defaultNotebookConfig, this._mimetype = N.IEditorMimeTypeService.defaultMimeType, this._notebookModel = null, this._modelChanged = new r.Signal(this), this._modelContentChanged = new r.Signal(this), this.node.dataset.jpKernelUser = "true", this.node.dataset.jpUndoer = "true", this.node.dataset.jpCodeRunner = "true", this.rendermime = e.rendermime, this.translator = e.translator || l.nullTranslator, this.contentFactory = e.contentFactory, this.editorConfig = e.editorConfig || ge.defaultEditorConfig, this.notebookConfig = e.notebookConfig || ge.defaultNotebookConfig, this._updateNotebookConfig(), this._mimetypeService = e.mimeTypeService, this.renderingLayout = null === (a = e.notebookConfig) || void 0 === a ? void 0 : a.renderingLayout, this.kernelHistory = e.kernelHistory
                 }
                 get cellCollapsed() {
                     return this._cellCollapsed
                 }
                 get cellInViewportChanged() {
                     return this._cellInViewportChanged
                 }
@@ -2351,15 +2351,15 @@
                 onUpdateRequest(e) {
                     "defer" === this.notebookConfig.windowingMode ? this._runOnIdleTime() : super.onUpdateRequest(e)
                 }
                 _onModelChanged(e, t) {
                     var n;
                     if (e)
                         for (e.contentChanged.disconnect(this.onModelContentChanged, this), e.metadataChanged.disconnect(this.onMetadataChanged, this), e.cells.changed.disconnect(this._onCellsChanged, this); this.cellsArray.length;) this._removeCell(0);
-                    if (!t) return void(this._mimetype = P.IEditorMimeTypeService.defaultMimeType);
+                    if (!t) return void(this._mimetype = N.IEditorMimeTypeService.defaultMimeType);
                     this._updateMimetype();
                     const o = t.cells;
                     null !== (n = t.collaborative) && void 0 !== n && n || o.length || t.sharedModel.insertCell(0, {
                         cell_type: this.notebookConfig.defaultCell,
                         metadata: "code" === this.notebookConfig.defaultCell ? {
                             trusted: !0
                         } : {}
@@ -3338,15 +3338,15 @@
                 class t extends Ce.ContentFactory {
                     createNotebook(e) {
                         return new Ce(e)
                     }
                 }
                 e.ContentFactory = t, e.IContentFactory = new d.Token("@jupyterlab/notebook:IContentFactory", "A factory object that creates new notebooks.\n    Use this if you want to create and host notebooks in your own UI elements.")
             }(ve || (ve = {}));
-            var pe, _e = n(26862);
+            var pe, _e = n(95183);
             class fe extends _e.SearchProvider {
                 constructor(e, t = l.nullTranslator) {
                     super(e), this.translator = t, this._textSelection = null, this._currentProviderIndex = null, this._delayedActiveCellChangeHandler = null, this._onSelection = !1, this._selectedCells = 1, this._selectedLines = 0, this._query = null, this._searchProviders = [], this._editorSelectionsObservable = null, this._selectionSearchMode = "cells", this._selectionLock = !1, this._searchActive = !1, this._handleHighlightsAfterActiveCellChange = this._handleHighlightsAfterActiveCellChange.bind(this), this.widget.model.cells.changed.connect(this._onCellsChanged, this), this.widget.content.activeCellChanged.connect(this._onActiveCellChanged, this), this.widget.content.selectionChanged.connect(this._onCellSelectionChanged, this), this.widget.content.stateChanged.connect(this._onNotebookStateChanged, this), this._observeActiveCell(), this._filtersChanged.connect(this._setEnginesSelectionSearchMode, this)
                 }
                 _onNotebookStateChanged(e, t) {
                     "mode" === t.name && window.setTimeout((() => {
                         var e;
@@ -3468,15 +3468,17 @@
                         var n;
                         const o = null === (n = this.widget) || void 0 === n ? void 0 : n.content.activeCell;
                         "markdown" === (null == o ? void 0 : o.model.type) && o.rendered && (o.rendered = !1, e && await this.highlightNext(t))
                     };
                     if (null !== this._currentProviderIndex) {
                         await i();
                         const s = this._searchProviders[this._currentProviderIndex];
-                        o = await s.replaceCurrentMatch(e, !1, n), null === s.currentMatchIndex && await this.highlightNext(t)
+                        o = await s.replaceCurrentMatch(e, !1, n), null === s.currentMatchIndex && await this.highlightNext(t, {
+                            from: "previous-match"
+                        })
                     }
                     return await i(!0), o
                 }
                 async replaceAllMatches(e, t) {
                     return (await Promise.all(this._searchProviders.map((n => n.replaceAllMatches(e, t))))).includes(!0)
                 }
                 async validateFilter(e, t) {
@@ -3527,39 +3529,42 @@
                             t.newValues.forEach(((e, n) => {
                                 this._addCellProvider(t.newIndex + n), this._removeCellProvider(t.newIndex + n + 1)
                             }))
                     }
                     this._stateChanged.emit()
                 }
                 async _stepNext(e = !1, t = !1, n) {
-                    const o = async e => {
+                    var o;
+                    const i = async e => {
                         var t;
                         if (null !== (t = null == n ? void 0 : n.scroll) && void 0 !== t && !t) return;
                         if (this._selectionLock = !0, this.widget.content.activeCellIndex !== this._currentProviderIndex && (this.widget.content.activeCellIndex = this._currentProviderIndex), -1 === this.widget.content.activeCellIndex) return console.warn("No active cell (no cells or no model), aborting search"), void(this._selectionLock = !1);
                         const o = this.widget.content.activeCell;
                         if (!o.inViewport) try {
                             await this.widget.content.scrollToItem(this._currentProviderIndex)
                         } catch (e) {}
                         if (o.inputHidden && (o.inputHidden = !1), !o.inViewport) return void(this._selectionLock = !1);
                         await o.ready;
                         const i = o.editor;
                         i.revealPosition(i.getPositionAt(e.position)), this._selectionLock = !1
                     };
                     null === this._currentProviderIndex && (this._currentProviderIndex = this.widget.content.activeCellIndex), e && "command" === this.widget.content.mode && (this._searchProviders[this._currentProviderIndex].getCurrentMatch() || (this._currentProviderIndex -= 1), t && (this._currentProviderIndex = (this._currentProviderIndex + this._searchProviders.length) % this._searchProviders.length));
-                    const i = this._currentProviderIndex;
+                    const s = "previous-match" === (null !== (o = null == n ? void 0 : n.from) && void 0 !== o ? o : "") && null === this._searchProviders[this._currentProviderIndex].currentMatchIndex,
+                        l = this._currentProviderIndex;
+                    s && this._searchProviders[this._currentProviderIndex].clearHighlight(), t && s && this._currentProviderIndex + 1 >= this._searchProviders.length ? this._currentProviderIndex = 0 : this._currentProviderIndex += s ? 1 : 0;
                     do {
-                        const i = this._searchProviders[this._currentProviderIndex],
-                            s = e ? await i.highlightPrevious(!1, n) : await i.highlightNext(!1, n);
-                        if (s) return await o(s), s;
+                        const o = this._searchProviders[this._currentProviderIndex],
+                            s = e ? await o.highlightPrevious(!1, n) : await o.highlightNext(!1, n);
+                        if (s) return await i(s), s;
                         this._currentProviderIndex = this._currentProviderIndex + (e ? -1 : 1), t && (this._currentProviderIndex = (this._currentProviderIndex + this._searchProviders.length) % this._searchProviders.length)
-                    } while (t ? this._currentProviderIndex !== i : 0 <= this._currentProviderIndex && this._currentProviderIndex < this._searchProviders.length);
+                    } while (t ? this._currentProviderIndex !== l : 0 <= this._currentProviderIndex && this._currentProviderIndex < this._searchProviders.length);
                     if (t) {
-                        const t = this._searchProviders[i],
-                            s = e ? await t.highlightPrevious(!1, n) : await t.highlightNext(!1, n);
-                        if (s) return await o(s), s
+                        const t = this._searchProviders[l],
+                            o = e ? await t.highlightPrevious(!1, n) : await t.highlightNext(!1, n);
+                        if (o) return await i(o), o
                     }
                     return this._currentProviderIndex = null, null
                 }
                 async _onActiveCellChanged() {
                     null !== this._delayedActiveCellChangeHandler && (clearTimeout(this._delayedActiveCellChangeHandler), this._delayedActiveCellChangeHandler = null), this.widget.content.activeCellIndex !== this._currentProviderIndex && (this._delayedActiveCellChangeHandler = window.setTimeout((() => {
                         this.delayedActiveCellChangeHandlerReady = this._handleHighlightsAfterActiveCellChange()
                     }), 0)), this._observeActiveCell()
```

### Comparing `notebook-7.2.0rc0/notebook/static/3768.bundle.js` & `notebook-7.2.0rc1/notebook/static/7302.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [3768, 7302], {
+    [7302, 3768], {
         83768: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => F
             });
-            var n = o(96049),
-                r = o(1167),
-                i = o(42751),
-                a = o(24554),
-                s = o(15729),
-                l = o(1131),
-                d = o(37267),
-                c = o(22620),
+            var n = o(53312),
+                r = o(68722),
+                i = o(71427),
+                a = o(23295),
+                s = o(9235),
+                l = o(74258),
+                d = o(12030),
+                c = o(35613),
                 g = o(81997),
                 u = o(63485),
-                w = o(42367),
+                w = o(64803),
                 h = o(78156),
                 b = o.n(h);
             class p {
                 constructor(e) {
                     this._onSelectionChanged = () => {
                         var e, t, o, n, r, i;
                         const a = Array.from(this._browser.selectedItems()),
```

### Comparing `notebook-7.2.0rc0/notebook/static/377.bundle.js` & `notebook-7.2.0rc1/notebook/static/377.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -5,18 +5,18 @@
             n.r(e), n.d(e, {
                 HTMLViewer: () => h,
                 HTMLViewerFactory: () => m,
                 IHTMLViewerTracker: () => r,
                 ToolbarItems: () => o
             });
             const r = new(n(20998).Token)("@jupyterlab/htmlviewer:IHTMLViewerTracker", "A widget tracker for rendered HTML documents.\n  Use this if you want to be able to iterate over and interact with HTML documents\n  viewed by the application.");
-            var o, a, s = n(1167),
-                i = n(10979),
-                l = n(37267),
-                u = n(22620),
+            var o, a, s = n(68722),
+                i = n(65903),
+                l = n(12030),
+                u = n(35613),
                 c = n(81997),
                 d = n(78156);
             class h extends i.DocumentWidget {
                 constructor(t) {
                     super({
                         ...t,
                         content: new u.IFrame({
```

### Comparing `notebook-7.2.0rc0/notebook/static/3797.bundle.js` & `notebook-7.2.0rc1/notebook/static/3797.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3863.bundle.js` & `notebook-7.2.0rc1/notebook/static/3863.bundle.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [3863], {
         73863: (e, r, t) => {
             t.r(r), t.d(r, {
                 default: () => i
             });
-            var n = t(22620);
+            var n = t(35613);
             const i = [{
                 id: "@jupyterlab/ui-components-extension:labicon-manager",
                 description: "Provides the icon manager.",
                 provides: n.ILabIconManager,
                 autoStart: !0,
                 activate: e => Object.create(null)
             }, {
```

### Comparing `notebook-7.2.0rc0/notebook/static/3881.bundle.js` & `notebook-7.2.0rc1/notebook/static/3881.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,23 +2,23 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [3881], {
         92871: (e, t, a) => {
             a.r(t), a.d(t, {
                 DEFAULT_CONTEXT_ITEM_RANK: () => f,
                 default: () => D
             });
-            var o = a(2922),
-                i = a(96049),
-                n = a(1167),
-                r = a(66724),
-                l = a(24554),
-                s = a(96692),
-                d = a(27829),
-                c = a(37267),
-                u = a(22620),
+            var o = a(44604),
+                i = a(53312),
+                n = a(68722),
+                r = a(77872),
+                l = a(23295),
+                s = a(41053),
+                d = a(71098),
+                c = a(12030),
+                u = a(35613),
                 p = a(33625),
                 g = a(20998),
                 m = a(16934),
                 b = a(2549),
                 h = a(63485),
                 v = a(78156);
             const y = {
```

### Comparing `notebook-7.2.0rc0/notebook/static/3bc6ecaae7ecf6f8d7f8.woff` & `notebook-7.2.0rc1/notebook/static/3bc6ecaae7ecf6f8d7f8.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3de784d07b9fa8f104c1.woff` & `notebook-7.2.0rc1/notebook/static/3de784d07b9fa8f104c1.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/3f6d3488cf65374f6f67.woff` & `notebook-7.2.0rc1/notebook/static/3f6d3488cf65374f6f67.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4002.bundle.js` & `notebook-7.2.0rc1/notebook/static/4002.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/403.bundle.js` & `notebook-7.2.0rc1/notebook/static/403.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4030.bundle.js` & `notebook-7.2.0rc1/notebook/static/4030.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4035.bundle.js` & `notebook-7.2.0rc1/notebook/static/4035.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4038.bundle.js` & `notebook-7.2.0rc1/notebook/static/4038.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4039.bundle.js` & `notebook-7.2.0rc1/notebook/static/4039.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4042.bundle.js` & `notebook-7.2.0rc1/notebook/static/4042.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,16 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [4042, 134], {
         44042: (t, e, s) => {
             s.r(e), s.d(e, {
                 AttachmentsModel: () => r,
                 AttachmentsResolver: () => h
             });
-            var a = s(58959),
-                n = s(13408),
+            var a = s(31231),
+                n = s(81221),
                 i = s(81997);
             class r {
                 constructor(t) {
                     var e;
                     if (this._map = new a.ObservableMap, this._isDisposed = !1, this._stateChanged = new i.Signal(this), this._changed = new i.Signal(this), this._serialized = null, this._changeGuard = !1, this.contentFactory = null !== (e = t.contentFactory) && void 0 !== e ? e : r.defaultContentFactory, t.values)
                         for (const e of Object.keys(t.values)) void 0 !== t.values[e] && this.set(e, t.values[e]);
                     this._map.changed.connect(this._onMapChanged, this)
```

### Comparing `notebook-7.2.0rc0/notebook/static/4058.bundle.js` & `notebook-7.2.0rc1/notebook/static/4058.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/409.bundle.js` & `notebook-7.2.0rc1/notebook/static/409.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4105.bundle.js` & `notebook-7.2.0rc1/notebook/static/4105.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4148.bundle.js` & `notebook-7.2.0rc1/notebook/static/4148.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4212.bundle.js` & `notebook-7.2.0rc1/notebook/static/4212.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [4212], {
         24212: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => v
             });
-            var i = n(2922),
-                c = n(96049),
-                s = n(26862),
-                a = n(24554),
-                d = n(37267),
+            var i = n(44604),
+                c = n(53312),
+                s = n(95183),
+                a = n(23295),
+                d = n(12030),
                 o = n(63485);
             const r = "jp-mod-searchable",
                 l = "jp-mod-search-active";
             var h;
             ! function(e) {
                 e.search = "documentsearch:start", e.searchAndReplace = "documentsearch:startWithReplace", e.findNext = "documentsearch:highlightNext", e.findPrevious = "documentsearch:highlightPrevious", e.end = "documentsearch:end", e.toggleSearchInSelection = "documentsearch:toggleSearchInSelection"
             }(h || (h = {}));
```

### Comparing `notebook-7.2.0rc0/notebook/static/4271.bundle.js` & `notebook-7.2.0rc1/notebook/static/4271.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4291.bundle.js` & `notebook-7.2.0rc1/notebook/static/4291.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/431.bundle.js` & `notebook-7.2.0rc1/notebook/static/431.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4382.bundle.js` & `notebook-7.2.0rc1/notebook/static/4382.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [4382, 7906], {
         54382: (e, t, r) => {
             r.r(t), r.d(t, {
                 default: () => a
             });
-            var n = r(26862),
-                o = r(46807);
+            var n = r(95183),
+                o = r(59625);
             const c = "jp-mod-searchable",
                 a = [{
                     id: "@jupyter-notebook/documentsearch-extension:notebookShellWidgetListener",
                     requires: [o.INotebookShell, n.ISearchProviderRegistry],
                     autoStart: !0,
                     description: "A plugin to add document search functionalities",
                     activate: (e, t, r) => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/4387.bundle.js` & `notebook-7.2.0rc1/notebook/static/4387.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4430.bundle.js` & `notebook-7.2.0rc1/notebook/static/4430.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4498.bundle.js` & `notebook-7.2.0rc1/notebook/static/4498.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4499.bundle.js` & `notebook-7.2.0rc1/notebook/static/4499.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4521.bundle.js` & `notebook-7.2.0rc1/notebook/static/4521.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4526.bundle.js` & `notebook-7.2.0rc1/notebook/static/4526.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4588.bundle.js` & `notebook-7.2.0rc1/notebook/static/4588.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4630.bundle.js` & `notebook-7.2.0rc1/notebook/static/4630.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6293,15 +6293,15 @@
                     detector: (t, e) => {
                         var i;
                         return !(!/^\s*classDiagram/.test(t) || "dagre-wrapper" !== (null == (i = null == e ? void 0 : e.class) ? void 0 : i.defaultRenderer)) || /^\s*classDiagram-v2/.test(t)
                     },
                     loader: async () => {
                         const {
                             diagram: t
-                        } = await Promise.all([i.e(7259), i.e(4780), i.e(8443), i.e(6281), i.e(7010), i.e(1846)]).then(i.bind(i, 11846));
+                        } = await Promise.all([i.e(7259), i.e(4780), i.e(8443), i.e(6281), i.e(7010), i.e(1846)]).then(i.bind(i, 72647));
                         return {
                             id: ii,
                             diagram: t
                         }
                     }
                 },
                 oi = "state",
```

### Comparing `notebook-7.2.0rc0/notebook/static/4645.bundle.js` & `notebook-7.2.0rc1/notebook/static/4645.bundle.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [4645, 6345], {
         94645: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => p
             });
-            var n = o(2922),
-                s = o(80106),
-                a = o(1167),
-                r = o(46807),
+            var n = o(44604),
+                s = o(67260),
+                a = o(68722),
+                r = o(59625),
                 c = o(33625);
             const i = {
                     id: "@jupyter-notebook/console-extension:opener",
                     requires: [n.IRouter],
                     autoStart: !0,
                     description: "A plugin to open consoles in a new tab",
                     activate: (e, t) => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/4670.bundle.js` & `notebook-7.2.0rc1/notebook/static/4670.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4708.bundle.js` & `notebook-7.2.0rc1/notebook/static/4708.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4780.bundle.js` & `notebook-7.2.0rc1/notebook/static/4780.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4810.bundle.js` & `notebook-7.2.0rc1/notebook/static/4810.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4811.bundle.js` & `notebook-7.2.0rc1/notebook/static/4811.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,17 +2,17 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [4811, 7386], {
         37386: (e, t, o) => {
             o.r(t), o.d(t, {
                 CellBarExtension: () => u,
                 CellToolbarTracker: () => c
             });
-            var l = o(96049),
-                n = o(58959),
-                a = o(22620),
+            var l = o(53312),
+                n = o(31231),
+                a = o(35613),
                 i = o(33625),
                 s = o(81997);
             const r = ["text/plain", "application/vnd.jupyter.stdout", "application/vnd.jupyter.stderr"],
                 d = "jp-toolbar-overlap";
             class c {
                 constructor(e, t, o) {
                     if (this._isDisposed = !1, this._toolbar = null, this._toolbarItems = null, this._toolbarFactory = null, this._panel = e, this._previousActiveCell = this._panel.content.activeCell, this._toolbarItems = null != t ? t : null, this._toolbarFactory = null != o ? o : null, null === this._toolbarItems && null === this._toolbarFactory) throw Error("You must provide the toolbarFactory or the toolbar items.");
```

### Comparing `notebook-7.2.0rc0/notebook/static/481e39042508ae313a60.woff` & `notebook-7.2.0rc1/notebook/static/481e39042508ae313a60.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4825.bundle.js` & `notebook-7.2.0rc1/notebook/static/4825.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4843.bundle.js` & `notebook-7.2.0rc1/notebook/static/4843.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4965.bundle.js` & `notebook-7.2.0rc1/notebook/static/4965.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/4971.bundle.js` & `notebook-7.2.0rc1/notebook/static/4971.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5019.bundle.js` & `notebook-7.2.0rc1/notebook/static/5019.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5061.bundle.js` & `notebook-7.2.0rc1/notebook/static/5061.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5099.bundle.js` & `notebook-7.2.0rc1/notebook/static/5099.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,25 +2,25 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5099], {
         25099: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => re,
                 toggleHeader: () => ae
             });
-            var n = a(2922),
-                o = a(96049),
-                s = a(1167),
-                i = a(24554),
-                r = a(96692),
-                l = a(37267),
-                c = a(22620),
+            var n = a(44604),
+                o = a(53312),
+                s = a(68722),
+                i = a(23295),
+                r = a(41053),
+                l = a(12030),
+                c = a(35613),
                 d = a(20998),
                 u = a(2549),
                 m = a(97934),
-                p = a(70611);
+                p = a(87408);
             const h = "help:open",
                 g = "https://jupyterlab.readthedocs.io/en/latest/privacy_policies.html";
             async function b(e, t = {}) {
                 const a = p.ServerConnection.makeSettings(),
                     n = s.URLExt.join(a.baseUrl, e);
                 let o;
                 try {
@@ -187,15 +187,15 @@
                                     }
                                 }
                             }
                         }
                     }))
                 }
             };
-            var y, v = a(27829),
+            var y, v = a(71098),
                 _ = a(63485),
                 w = a(78156),
                 k = a(37634);
 
             function C(e) {
                 const {
                     manager: t,
@@ -788,15 +788,15 @@
                         n.model.sessions = Array.from(e.serviceManager.sessions.running()).length, n.model.terminals = Array.from(e.serviceManager.terminals.running()).length, t.registerStatusItem(M.id, {
                             item: n,
                             align: "left",
                             rank: 0
                         })
                     }
                 };
-            var O, L = a(50845);
+            var O, L = a(29879);
             ! function(e) {
                 e.changeTheme = "apputils:change-theme", e.changePreferredLightTheme = "apputils:change-light-theme", e.changePreferredDarkTheme = "apputils:change-dark-theme", e.toggleAdaptiveTheme = "apputils:adaptive-theme", e.themeScrollbars = "apputils:theme-scrollbars", e.changeFont = "apputils:change-font", e.incrFontSize = "apputils:incr-font-size", e.decrFontSize = "apputils:decr-font-size"
             }(O || (O = {}));
             const z = {
                     id: "@jupyterlab/apputils-extension:themes",
                     description: "Provides the theme manager.",
                     requires: [i.ISettingRegistry, n.JupyterFrontEnd.IPaths, l.ITranslator],
@@ -1012,16 +1012,16 @@
                     description: "Provides toolbar items registry.",
                     autoStart: !0,
                     provides: o.IToolbarWidgetRegistry,
                     activate: e => new o.ToolbarWidgetRegistry({
                         defaultFactory: (0, o.createDefaultFactory)(e.commands)
                     })
                 };
-            var U = a(10979),
-                B = a(13892);
+            var U = a(65903),
+                B = a(72164);
             const H = "jupyterlab-workspace",
                 q = "." + H,
                 J = {
                     id: "@jupyterlab/apputils-extension:workspaces",
                     description: "Add workspace file type.",
                     autoStart: !0,
                     requires: [r.IStateDB, l.ITranslator, n.JupyterFrontEnd.IPaths],
```

### Comparing `notebook-7.2.0rc0/notebook/static/5115.bundle.js` & `notebook-7.2.0rc1/notebook/static/5115.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5135.bundle.js` & `notebook-7.2.0rc1/notebook/static/5135.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9,26 +9,26 @@
                 NotebookShell: () => k,
                 PanelHandler: () => f,
                 Private: () => v,
                 SidePanelHandler: () => w,
                 SidePanelPalette: () => W,
                 defaultNotebookPathOpener: () => b
             });
-            var s, n = i(2922),
-                r = i(10979),
+            var s, n = i(44604),
+                r = i(65903),
                 a = i(75677),
                 o = i(20389),
-                d = i(1167),
+                d = i(68722),
                 l = i(97934),
-                h = i(37267),
+                h = i(12030),
                 p = i(33625),
                 g = i(20998),
                 u = i(81997),
                 c = i(63485),
-                _ = i(22620),
+                _ = i(35613),
                 m = i(49503);
             class f {
                 constructor() {
                     this._panelChildHook = (e, t) => {
                         if ("child-removed" === t.type) {
                             const e = t.child;
                             p.ArrayExt.removeFirstWhere(this._items, (t => t.widget === e))
```

### Comparing `notebook-7.2.0rc0/notebook/static/5166.bundle.js` & `notebook-7.2.0rc1/notebook/static/5166.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5234.bundle.js` & `notebook-7.2.0rc1/notebook/static/5234.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5249.bundle.js` & `notebook-7.2.0rc1/notebook/static/5249.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5254.bundle.js` & `notebook-7.2.0rc1/notebook/static/5254.bundle.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5254], {
         95254: (e, a, t) => {
             t.r(a), t.d(a, {
                 default: () => i
             });
-            var r = t(96049),
-                s = t(37267);
+            var r = t(53312),
+                s = t(12030);
             const i = {
                 id: "@jupyterlab/theme-dark-high-contrast-extension:plugin",
                 description: "Adds a dark high contrast theme.",
                 requires: [r.IThemeManager, s.ITranslator],
                 activate: (e, a, t) => {
                     const r = t.load("jupyterlab");
                     a.register({
```

### Comparing `notebook-7.2.0rc0/notebook/static/5261.bundle.js` & `notebook-7.2.0rc1/notebook/static/5261.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5263.bundle.js` & `notebook-7.2.0rc1/notebook/static/5263.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -28,15 +28,15 @@
                 rulers: () => P,
                 ySync: () => I,
                 ySyncAnnotation: () => L,
                 ySyncFacet: () => A,
                 ybinding: () => R
             });
             var n = i(87797),
-                s = i(52839);
+                s = i(51429);
             const r = "[data-jp-code-runner]";
             var a;
             ! function(e) {
                 e.indentMoreOrInsertTab = function(e) {
                     var t;
                     if (null === (t = e.dom.parentElement) || void 0 === t ? void 0 : t.classList.contains(s.COMPLETER_ENABLED_CLASS)) return !1;
                     const i = {
@@ -80,15 +80,15 @@
             }(a || (a = {}));
             var o = i(17592),
                 l = i(89843),
                 c = i(3546),
                 h = i(20998),
                 u = i(81997),
                 d = i(56318),
-                m = i(37267);
+                m = i(12030);
             const p = l.Facet.define({
                 combine: e => (0, l.combineConfig)(e, {
                     fontFamily: null,
                     fontSize: null,
                     lineHeight: null
                 }, {
                     fontFamily: (e, t) => null != e ? e : t,
@@ -784,15 +784,15 @@
                             Diagnostics: u.__("Diagnostics"),
                             "No diagnostics": u.__("No diagnostics")
                         },
                         factory: () => s((e => l.EditorState.phrases.of(e)))
                     })), p
                 }
             }(q || (q = {}));
-            var B = i(1167),
+            var B = i(68722),
                 F = i(49906),
                 H = i(27061);
             class G {
                 constructor(e) {
                     this.start = e
                 }
             }
@@ -4302,15 +4302,15 @@
                         extensions: ["html", "htm", "handlebars", "hbs"],
                         load: async () => (await Promise.all([i.e(5850), i.e(9239), i.e(7866)]).then(i.bind(i, 77866))).html()
                     }, {
                         name: "Java",
                         displayName: s.__("Java"),
                         mime: "text/x-java",
                         extensions: ["java"],
-                        load: async () => (await i.e(1053).then(i.bind(i, 41053))).java()
+                        load: async () => (await i.e(6078).then(i.bind(i, 76078))).java()
                     }, {
                         name: "Javascript",
                         displayName: s.__("Javascript"),
                         alias: ["ecmascript", "js", "node"],
                         mime: ["text/javascript", "text/ecmascript", "application/javascript", "application/x-javascript", "application/ecmascript"],
                         extensions: ["js", "mjs", "cjs"],
                         load: async () => (await i.e(5850).then(i.bind(i, 65850))).javascript()
@@ -5017,15 +5017,15 @@
                         displayName: s.__("TiddlyWiki"),
                         mime: "text/x-tiddlywiki",
                         load: async () => t((await i.e(7054).then(i.bind(i, 27054))).tiddlyWiki)
                     }, {
                         name: "Tiki wiki",
                         displayName: s.__("Tiki wiki"),
                         mime: "text/tiki",
-                        load: async () => t((await i.e(5425).then(i.bind(i, 15425))).tiki)
+                        load: async () => t((await i.e(5425).then(i.bind(i, 43038))).tiki)
                     }, {
                         name: "TOML",
                         displayName: s.__("TOML"),
                         mime: "text/x-toml",
                         extensions: ["toml"],
                         load: async () => t((await i.e(2682).then(i.bind(i, 92682))).toml)
                     }, {
@@ -5351,15 +5351,15 @@
                         dispatch: this.editor.dispatch
                     })
                 }
                 execCommand(e) {
                     e(this.editor)
                 }
                 onConfigChanged(e, t) {
-                    e.reconfigureExtensions(this._editor, t)
+                    e.reconfigureExtensions(this._editor, t), t.customStyles && !t.fontSize && this.editor.setState(this.editor.state)
                 }
                 onKeydown(e) {
                     const t = this.state.selection.main.head;
                     return 0 === t && 38 === e.keyCode ? (e.shiftKey || this.edgeRequested.emit("top"), !1) : 1 === this.doc.lineAt(t).number && 38 === e.keyCode ? (e.shiftKey || this.edgeRequested.emit("topLine"), !1) : t === this.doc.length && 40 === e.keyCode && (e.shiftKey || this.edgeRequested.emit("bottom"), !1)
                 }
                 _onMimeTypeChanged() {
                     this._languages.getLanguage(this._model.mimeType).then((e => {
@@ -5489,15 +5489,15 @@
                     const i = B.PathExt.extname(e);
                     if (".ipy" === i) return "text/x-python";
                     if (".md" === i) return "text/x-ipythongfm";
                     const n = this.languages.findByFileName(e);
                     return n ? Array.isArray(n.mime) ? null !== (t = n.mime[0]) && void 0 !== t ? t : s.IEditorMimeTypeService.defaultMimeType : n.mime : s.IEditorMimeTypeService.defaultMimeType
                 }
             }
-            var zi, qi = i(26862);
+            var zi, qi = i(95183);
             class Bi {
                 constructor() {
                     this.currentIndex = null, this.query = null, this._isActive = !0, this._inSelection = null, this._isDisposed = !1, this._cmHandler = null, this.currentIndex = null, this._stateChanged = new u.Signal(this)
                 }
                 get cmHandler() {
                     return this._cmHandler || (this._cmHandler = new Fi(this.editor)), this._cmHandler
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/5299.bundle.js` & `notebook-7.2.0rc1/notebook/static/5299.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5313.bundle.js` & `notebook-7.2.0rc1/notebook/static/5313.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,16 +19,16 @@
                 n = i(40930),
                 o = i(21058)
         },
         40930: (e, t, i) => {
             i.d(t, {
                 p: () => a
             });
-            var r, s = i(37267),
-                n = i(22620),
+            var r, s = i(12030),
+                n = i(35613),
                 o = i(63485);
             class a extends o.Widget {
                 constructor(e) {
                     super({
                         node: r.createNode(e.widget.delimiter, e.translator)
                     }), this._widget = e.widget, this.addClass("jp-CSVDelimiter")
                 }
@@ -73,16 +73,16 @@
                 A9: () => u,
                 B0: () => h,
                 JZ: () => c,
                 LT: () => g,
                 _d: () => m,
                 kw: () => _
             });
-            var r, s = i(1167),
-                n = i(10979),
+            var r, s = i(68722),
+                n = i(65903),
                 o = i(20998),
                 a = i(81997),
                 d = i(63485),
                 l = i(40930);
             class h {}
             class c {
                 constructor(e) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/5325.bundle.js` & `notebook-7.2.0rc1/notebook/static/5325.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,18 +5,18 @@
             n.r(e), n.d(e, {
                 HTMLViewer: () => h,
                 HTMLViewerFactory: () => m,
                 IHTMLViewerTracker: () => r,
                 ToolbarItems: () => o
             });
             const r = new(n(20998).Token)("@jupyterlab/htmlviewer:IHTMLViewerTracker", "A widget tracker for rendered HTML documents.\n  Use this if you want to be able to iterate over and interact with HTML documents\n  viewed by the application.");
-            var o, a, s = n(1167),
-                i = n(10979),
-                l = n(37267),
-                u = n(22620),
+            var o, a, s = n(68722),
+                i = n(65903),
+                l = n(12030),
+                u = n(35613),
                 c = n(81997),
                 d = n(78156);
             class h extends i.DocumentWidget {
                 constructor(t) {
                     super({
                         ...t,
                         content: new u.IFrame({
```

### Comparing `notebook-7.2.0rc0/notebook/static/5343.bundle.js` & `notebook-7.2.0rc1/notebook/static/5343.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5346.bundle.js` & `notebook-7.2.0rc1/notebook/static/5346.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5346], {
         15346: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => m
             });
-            var n = a(17894),
+            var n = a(25460),
                 l = a(78156),
                 s = a.n(l),
-                d = a(22620),
+                d = a(35613),
                 i = a(33625),
-                r = a(37267);
+                r = a(12030);
             const o = "jp-CellTags-Tag",
                 c = "jp-CellTags-Unapplied",
                 g = "jp-CellTags-Holder",
                 p = "jp-CellTags-Add",
                 u = "jp-CellTags-Empty";
             class h {
                 constructor(e, t) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/5425.bundle.js` & `notebook-7.2.0rc1/notebook/static/5425.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5425], {
-        15425: (e, t, n) => {
+        43038: (e, t, n) => {
             function r(e, t, n) {
                 return function(r, i) {
                     for (; !r.eol();) {
                         if (r.match(t)) {
                             i.tokenize = a;
                             break
                         }
```

### Comparing `notebook-7.2.0rc0/notebook/static/5426.bundle.js` & `notebook-7.2.0rc1/notebook/static/5426.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5426], {
         45426: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => s
             });
-            var i = a(96049),
-                r = a(37267);
+            var i = a(53312),
+                r = a(12030);
             const s = {
                 id: "@jupyterlab/theme-light-extension:plugin",
                 description: "Adds a light theme.",
                 requires: [i.IThemeManager, r.ITranslator],
                 activate: (e, t, a) => {
                     const i = a.load("jupyterlab");
                     t.register({
```

### Comparing `notebook-7.2.0rc0/notebook/static/545.bundle.js` & `notebook-7.2.0rc1/notebook/static/545.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,27 +2,27 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [545], {
         60545: (e, n, t) => {
             t.r(n), t.d(n, {
                 CommandIDs: () => w,
                 default: () => f
             });
-            var a, o = t(2922),
-                l = t(96049),
-                r = t(1167),
-                s = t(50845),
-                d = t(70611),
-                i = t(24554),
-                c = t(37267),
-                u = t(22620),
+            var a, o = t(44604),
+                l = t(53312),
+                r = t(68722),
+                s = t(29879),
+                d = t(87408),
+                i = t(23295),
+                c = t(12030),
+                u = t(35613),
                 m = t(33625),
                 p = t(20998),
                 h = t(63485),
-                _ = t(91942),
-                g = t(42751);
+                _ = t(5094),
+                g = t(71427);
             ! function(e) {
                 e.openRecent = "recentmenu:open-recent", e.reopenLast = "recentmenu:reopen-last", e.clearRecents = "docmanager:clear-recents"
             }(a || (a = {}));
             class b extends h.Menu {
                 constructor(e) {
                     super(e), this._manager = e.manager, this._showDirectories = e.showDirectories, this.updateItems(), this._manager.changed.connect(this.updateItems, this)
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/5451.bundle.js` & `notebook-7.2.0rc1/notebook/static/5451.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5494.bundle.js` & `notebook-7.2.0rc1/notebook/static/5494.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5573.bundle.js` & `notebook-7.2.0rc1/notebook/static/5573.bundle.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5573], {
         5573: (e, o, t) => {
             t.r(o), t.d(o, {
-                default: () => W
+                default: () => A
             });
-            var n = t(96049),
-                a = t(1167),
-                s = t(91942),
-                r = t(50845),
-                i = t(17894),
-                c = t(24554),
-                d = t(37267),
-                l = t(46807),
+            var n = t(53312),
+                a = t(68722),
+                s = t(5094),
+                r = t(29879),
+                c = t(25460),
+                i = t(23295),
+                l = t(12030),
+                d = t(59625),
                 u = t(97934),
                 k = t(63485),
                 b = t(78156),
                 p = t.n(b);
             const g = e => {
                     const o = e.model;
                     if (!o) return !1;
@@ -42,15 +42,15 @@
                         className: "jp-NotebookTrustedStatus",
                         style: n ? {
                             cursor: "help"
                         } : {
                             cursor: "pointer"
                         },
                         onClick: () => !n && (async () => {
-                            await i.NotebookActions.trust(e, o), s()
+                            await c.NotebookActions.trust(e, o), s()
                         })(),
                         title: n ? t.__("JavaScript enabled for notebook display") : t.__("JavaScript disabled for notebook display")
                     }, n ? t.__("Trusted") : t.__("Not Trusted"))
                 };
             var m;
             ! function(e) {
                 e.create = ({
@@ -59,67 +59,67 @@
                 }) => n.ReactWidget.create(p().createElement(h, {
                     notebook: e,
                     translator: o
                 }))
             }(m || (m = {}));
             const C = "jp-NotebookKernelStatus-error",
                 f = "jp-NotebookKernelStatus-warn",
-                v = "jp-NotebookKernelStatus-info",
-                y = "jp-NotebookKernelStatus-fade";
-            var w;
+                y = "jp-NotebookKernelStatus-info",
+                v = "jp-NotebookKernelStatus-fade";
+            var N;
             ! function(e) {
                 e.openEditNotebookMetadata = "notebook:edit-metadata"
-            }(w || (w = {}));
-            const N = {
+            }(N || (N = {}));
+            const S = {
                     id: "@jupyter-notebook/notebook-extension:checkpoints",
                     description: "A plugin for the checkpoint indicator.",
                     autoStart: !0,
-                    requires: [s.IDocumentManager, d.ITranslator],
-                    optional: [l.INotebookShell, n.IToolbarWidgetRegistry],
+                    requires: [s.IDocumentManager, l.ITranslator],
+                    optional: [d.INotebookShell, n.IToolbarWidgetRegistry],
                     activate: (e, o, t, s, r) => {
                         const {
-                            shell: i
-                        } = e, c = t.load("notebook"), d = document.createElement("div");
+                            shell: c
+                        } = e, i = t.load("notebook"), l = document.createElement("div");
                         r && r.addFactory("TopBar", "checkpoint", (e => {
                             const o = new k.Widget({
-                                node: d
+                                node: l
                             });
                             return o.id = n.DOMUtils.createDomID(), o.addClass("jp-NotebookCheckpoint"), o
                         }));
-                        const l = async () => {
-                            const e = i.currentWidget;
+                        const d = async () => {
+                            const e = c.currentWidget;
                             if (!e) return;
                             const t = o.contextForWidget(e);
-                            null == t || t.fileChanged.disconnect(l), null == t || t.fileChanged.connect(l);
+                            null == t || t.fileChanged.disconnect(d), null == t || t.fileChanged.connect(d);
                             const n = await (null == t ? void 0 : t.listCheckpoints());
                             if (!n) return;
                             const s = n[n.length - 1];
-                            d.textContent = c.__("Last Checkpoint: %1", a.Time.formatHuman(new Date(s.last_modified)))
+                            l.textContent = i.__("Last Checkpoint: %1", a.Time.formatHuman(new Date(s.last_modified)))
                         };
-                        s && s.currentChanged.connect(l), new u.Poll({
+                        s && s.currentChanged.connect(d), new u.Poll({
                             auto: !0,
-                            factory: () => l(),
+                            factory: () => d(),
                             frequency: {
                                 interval: 2e3,
                                 backoff: !1
                             },
                             standby: "when-hidden"
                         })
                     }
                 },
-                S = {
+                w = {
                     id: "@jupyter-notebook/notebook-extension:close-tab",
                     description: 'Add a command to close the browser tab when clicking on "Close and Shut Down".',
                     autoStart: !0,
                     requires: [r.IMainMenu],
-                    optional: [d.ITranslator],
+                    optional: [l.ITranslator],
                     activate: (e, o, t) => {
                         const {
                             commands: n
-                        } = e, a = (t = null != t ? t : d.nullTranslator).load("notebook"), s = "notebook:close-and-halt";
+                        } = e, a = (t = null != t ? t : l.nullTranslator).load("notebook"), s = "notebook:close-and-halt";
                         n.addCommand(s, {
                             label: a.__("Close and Shut Down Notebook"),
                             execute: async () => {
                                 await n.execute("notebook:close-and-shutdown"), window.close()
                             }
                         }), o.fileMenu.closeAndCleaners.add({
                             id: s,
@@ -127,26 +127,26 @@
                         })
                     }
                 },
                 T = {
                     id: "@jupyter-notebook/notebook-extension:kernel-logo",
                     description: "The kernel logo plugin.",
                     autoStart: !0,
-                    requires: [l.INotebookShell],
+                    requires: [d.INotebookShell],
                     optional: [n.IToolbarWidgetRegistry],
                     activate: (e, o, t) => {
                         const {
                             serviceManager: n
                         } = e, a = document.createElement("div"), s = document.createElement("img"), r = async () => {
-                            var e, t, c, d, l;
+                            var e, t, i, l, d;
                             const u = o.currentWidget;
-                            if (!(u instanceof i.NotebookPanel)) return;
+                            if (!(u instanceof c.NotebookPanel)) return;
                             a.hasChildNodes() || a.appendChild(s), await u.sessionContext.ready, u.sessionContext.kernelChanged.disconnect(r), u.sessionContext.kernelChanged.connect(r);
-                            const k = null !== (c = null === (t = null === (e = u.sessionContext.session) || void 0 === e ? void 0 : e.kernel) || void 0 === t ? void 0 : t.name) && void 0 !== c ? c : "",
-                                b = null === (l = null === (d = n.kernelspecs) || void 0 === d ? void 0 : d.specs) || void 0 === l ? void 0 : l.kernelspecs[k];
+                            const k = null !== (i = null === (t = null === (e = u.sessionContext.session) || void 0 === e ? void 0 : e.kernel) || void 0 === t ? void 0 : t.name) && void 0 !== i ? i : "",
+                                b = null === (d = null === (l = n.kernelspecs) || void 0 === l ? void 0 : l.specs) || void 0 === d ? void 0 : d.kernelspecs[k];
                             if (!b) return void a.childNodes[0].remove();
                             const p = b.resources["logo-64x64"];
                             p ? (s.src = p, s.title = b.display_name) : a.childNodes[0].remove()
                         };
                         t && t.addFactory("TopBar", "kernelLogo", (e => {
                             const o = new k.Widget({
                                 node: a
@@ -157,53 +157,53 @@
                         }))
                     }
                 },
                 x = {
                     id: "@jupyter-notebook/notebook-extension:kernel-status",
                     description: "A plugin to display the kernel status.",
                     autoStart: !0,
-                    requires: [l.INotebookShell, d.ITranslator],
+                    requires: [d.INotebookShell, l.ITranslator],
                     activate: (e, o, t) => {
                         const n = t.load("notebook"),
                             s = new k.Widget;
                         s.addClass("jp-NotebookKernelStatus"), e.shell.add(s, "menu", {
                             rank: 10010
                         });
                         const r = e => {
                             const o = e.kernelDisplayStatus;
                             let t = `Kernel ${a.Text.titleCase(o)}`;
-                            switch (s.removeClass(C), s.removeClass(f), s.removeClass(v), s.removeClass(y), o) {
+                            switch (s.removeClass(C), s.removeClass(f), s.removeClass(y), s.removeClass(v), o) {
                                 case "busy":
                                 case "idle":
-                                    t = "", s.addClass(y);
+                                    t = "", s.addClass(v);
                                     break;
                                 case "dead":
                                 case "terminating":
                                     s.addClass(C);
                                     break;
                                 case "unknown":
                                     s.addClass(f);
                                     break;
                                 default:
-                                    s.addClass(v), s.addClass(y)
+                                    s.addClass(y), s.addClass(v)
                             }
                             s.node.textContent = n.__(t)
                         };
                         o.currentChanged.connect((async () => {
                             const e = o.currentWidget;
-                            e instanceof i.NotebookPanel && e.sessionContext.statusChanged.connect(r)
+                            e instanceof c.NotebookPanel && e.sessionContext.statusChanged.connect(r)
                         }))
                     }
                 },
                 _ = {
                     id: "@jupyter-notebook/notebook-extension:scroll-output",
                     description: "A plugin to enable scrolling for outputs by default.",
                     autoStart: !0,
-                    requires: [i.INotebookTracker],
-                    optional: [c.ISettingRegistry],
+                    requires: [c.INotebookTracker],
+                    optional: [i.ISettingRegistry],
                     activate: async (e, o, t) => {
                         let n = !0;
                         const a = e => {
                                 if (!n) return;
                                 const {
                                     outputArea: o
                                 } = e;
@@ -243,29 +243,29 @@
                         }
                     }
                 },
                 I = {
                     id: "@jupyter-notebook/notebook-extension:notebook-tools",
                     description: "A plugin to add the NotebookTools to the side panel.",
                     autoStart: !0,
-                    requires: [l.INotebookShell],
-                    optional: [i.INotebookTools],
+                    requires: [d.INotebookShell],
+                    optional: [c.INotebookTools],
                     activate: (e, o, t) => {
                         o.currentChanged.connect((async () => {
-                            o.currentWidget instanceof i.NotebookPanel && t && o.add(t, "right", {
+                            o.currentWidget instanceof c.NotebookPanel && t && o.add(t, "right", {
                                 type: "Property Inspector"
                             })
                         }))
                     }
                 },
                 E = {
                     id: "@jupyter-notebook/notebook-extension:tab-icon",
                     description: "A plugin to update the tab icon based on the kernel status.",
                     autoStart: !0,
-                    requires: [i.INotebookTracker],
+                    requires: [c.INotebookTracker],
                     activate: (e, o) => {
                         const t = a.PageConfig.getBaseUrl(),
                             n = a.URLExt.join(t, "static/favicons/favicon-notebook.ico"),
                             s = a.URLExt.join(t, "static/favicons/favicon-busy-1.ico");
                         o.currentChanged.connect((async () => {
                             const e = o.currentWidget,
                                 t = null == e ? void 0 : e.sessionContext;
@@ -284,70 +284,59 @@
                         }))
                     }
                 },
                 j = {
                     id: "@jupyter-notebook/notebook-extension:trusted",
                     description: "A plugin that adds a Trusted indicator to the menu area.",
                     autoStart: !0,
-                    requires: [l.INotebookShell, d.ITranslator],
+                    requires: [d.INotebookShell, l.ITranslator],
                     activate: (e, o, t) => {
                         o.currentChanged.connect((async () => {
                             const e = o.currentWidget;
-                            if (!(e instanceof i.NotebookPanel)) return;
+                            if (!(e instanceof c.NotebookPanel)) return;
                             const n = e.content;
                             await e.context.ready;
                             const a = m.create({
                                 notebook: n,
                                 translator: t
                             });
                             o.add(a, "menu", {
                                 rank: 11e3
                             })
                         }))
                     }
                 },
-                A = {
+                A = [S, w, {
                     id: "@jupyter-notebook/notebook-extension:edit-notebook-metadata",
                     description: 'Add a command to open right sidebar for Editing Notebook Metadata when clicking on "Edit Notebook Metadata" under Edit menu',
                     autoStart: !0,
-                    optional: [n.ICommandPalette, d.ITranslator, i.INotebookTools],
+                    optional: [n.ICommandPalette, l.ITranslator, c.INotebookTools],
                     activate: (e, o, t, n) => {
                         const {
                             commands: a,
                             shell: s
-                        } = e, r = (t = null != t ? t : d.nullTranslator).load("notebook");
-                        a.addCommand(w.openEditNotebookMetadata, {
+                        } = e, r = (t = null != t ? t : l.nullTranslator).load("notebook");
+                        a.addCommand(N.openEditNotebookMetadata, {
                             label: r.__("Edit Notebook Metadata"),
                             execute: async () => {
                                 const e = "application:toggle-panel",
                                     o = {
                                         side: "right",
                                         title: "Show Notebook Tools",
                                         id: "notebook-tools"
                                     };
                                 a.isToggled(e, o) || await a.execute(e, o).then((e => {
                                     n && (null == n ? void 0 : n.layout).widgets.forEach((e => {
                                         e.widget.title.label === r.__("Advanced Tools") && e.collapsed && e.toggle()
                                     }))
                                 }))
                             },
-                            isVisible: () => null !== s.currentWidget && s.currentWidget instanceof i.NotebookPanel
+                            isVisible: () => null !== s.currentWidget && s.currentWidget instanceof c.NotebookPanel
                         }), o && o.addItem({
-                            command: w.openEditNotebookMetadata,
+                            command: N.openEditNotebookMetadata,
                             category: "Notebook Operations"
                         })
                     }
-                },
-                M = {
-                    id: "@jupyter-notebook/notebook-extension:windowing",
-                    autoStart: !0,
-                    requires: [i.INotebookTracker],
-                    activate: (e, o) => {
-                        o.widgetAdded.connect(((e, o) => {
-                            o.content._viewModel.windowingActive = !1, o.content.notebookConfig.windowingMode = "defer"
-                        }))
-                    }
-                },
-                W = [N, S, A, T, x, I, _, E, j, M]
+                }, T, x, I, _, E, j]
         }
     }
 ]);
```

### Comparing `notebook-7.2.0rc0/notebook/static/5601.bundle.js` & `notebook-7.2.0rc1/notebook/static/1684.bundle.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [5601, 1684], {
+    [1684, 5601], {
         95601: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => l
             });
-            var a = n(2922),
-                o = n(1167),
-                i = n(69200),
-                r = n(46807),
+            var a = n(44604),
+                o = n(68722),
+                i = n(5333),
+                r = n(59625),
                 s = n(33625);
             const c = {
                     id: "@jupyter-notebook/terminal-extension:opener",
                     description: "A plugin to open terminals in a new tab.",
                     requires: [a.IRouter, i.ITerminalTracker],
                     autoStart: !0,
                     activate: (e, t, n) => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/5614.bundle.js` & `notebook-7.2.0rc1/notebook/static/5614.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/563.bundle.js` & `notebook-7.2.0rc1/notebook/static/563.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5649.bundle.js` & `notebook-7.2.0rc1/notebook/static/5649.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5698.bundle.js` & `notebook-7.2.0rc1/notebook/static/5698.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5733.bundle.js` & `notebook-7.2.0rc1/notebook/static/5733.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             __webpack_require__.r(__webpack_exports__), __webpack_require__.d(__webpack_exports__, {
                 APPLICATION_JAVASCRIPT_MIMETYPE: () => APPLICATION_JAVASCRIPT_MIMETYPE,
                 ExperimentalRenderedJavascript: () => ExperimentalRenderedJavascript,
                 TEXT_JAVASCRIPT_MIMETYPE: () => TEXT_JAVASCRIPT_MIMETYPE,
                 default: () => __WEBPACK_DEFAULT_EXPORT__,
                 rendererFactory: () => rendererFactory
             });
-            var _jupyterlab_rendermime__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(13408),
+            var _jupyterlab_rendermime__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(81221),
                 _jupyterlab_rendermime__WEBPACK_IMPORTED_MODULE_0___default = __webpack_require__.n(_jupyterlab_rendermime__WEBPACK_IMPORTED_MODULE_0__);
             const TEXT_JAVASCRIPT_MIMETYPE = "text/javascript",
                 APPLICATION_JAVASCRIPT_MIMETYPE = "application/javascript";
 
             function evalInContext(code, element, document, window) {
                 return eval(code)
             }
```

### Comparing `notebook-7.2.0rc0/notebook/static/5765.bundle.js` & `notebook-7.2.0rc1/notebook/static/5765.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5777.bundle.js` & `notebook-7.2.0rc1/notebook/static/5777.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5822.bundle.js` & `notebook-7.2.0rc1/notebook/static/5822.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5828.bundle.js` & `notebook-7.2.0rc1/notebook/static/5828.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5834.bundle.js` & `notebook-7.2.0rc1/notebook/static/5834.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5850.bundle.js` & `notebook-7.2.0rc1/notebook/static/5850.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5912.bundle.js` & `notebook-7.2.0rc1/notebook/static/5912.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [5912], {
         15912: (e, n, t) => {
             t.r(n), t.d(n, {
                 default: () => p
             });
-            var a, r = t(2922),
-                o = t(96049),
-                i = t(65651),
-                s = t(50845),
-                c = t(15729),
-                l = t(70611),
-                d = t(24554),
-                m = t(69200),
-                h = t(37267),
-                u = t(22620),
+            var a, r = t(44604),
+                o = t(53312),
+                i = t(86810),
+                s = t(29879),
+                c = t(9235),
+                l = t(87408),
+                d = t(23295),
+                m = t(5333),
+                h = t(12030),
+                u = t(35613),
                 g = t(63485);
             ! function(e) {
                 e.copy = "terminal:copy", e.createNew = "terminal:create-new", e.open = "terminal:open", e.refresh = "terminal:refresh", e.increaseFont = "terminal:increase-font", e.decreaseFont = "terminal:decrease-font", e.paste = "terminal:paste", e.setTheme = "terminal:set-theme", e.shutdown = "terminal:shut-down"
             }(a || (a = {}));
             const _ = {
                     activate: function(e, n, t, r, i, s, c, d, h) {
                         const p = t.load("jupyterlab"),
```

### Comparing `notebook-7.2.0rc0/notebook/static/5921.bundle.js` & `notebook-7.2.0rc1/notebook/static/5921.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -29,15 +29,15 @@
                 addPrefix: () => E,
                 clearNumbering: () => M,
                 filterHeadings: () => y,
                 getHTMLHeadings: () => k,
                 getPrefix: () => O,
                 isHTML: () => A
             });
-            var a = n(1167);
+            var a = n(68722);
             class l {
                 constructor(e) {
                     this.tracker = e
                 }
                 isApplicable(e) {
                     return !!this.tracker.has(e)
                 }
@@ -62,15 +62,15 @@
                     })).catch((e => {
                         console.error(`Failed to initiate headings for ${s.localPath}.`)
                     })), e.disposed.connect((() => {
                         l.activityStopped.disconnect(i), s.pathChanged.disconnect(r)
                     })), n
                 }
             }
-            var r = n(22620),
+            var r = n(35613),
                 o = n(20998),
                 c = n(81997);
             const h = new o.Token("@jupyterlab/toc:ITableOfContentsRegistry", "A service to register table of content factory."),
                 d = new o.Token("@jupyterlab/toc:ITableOfContentsTracker", "A widget tracker for table of contents.");
             var g;
             ! function(e) {
                 e.defaultConfig = {
@@ -425,16 +425,16 @@
             }
 
             function M(e) {
                 null == e || e.querySelectorAll(`span.${H}`).forEach((e => {
                     e.remove()
                 }))
             }
-            var j = n(96049),
-                R = n(13408);
+            var j = n(53312),
+                R = n(81221);
             async function N(e, t, n, s) {
                 try {
                     const i = document.createElement("div");
                     await (0, R.renderMarkdown)({
                         markdownParser: e,
                         host: i,
                         source: t,
```

### Comparing `notebook-7.2.0rc0/notebook/static/5972.bundle.js` & `notebook-7.2.0rc1/notebook/static/5972.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5996.bundle.js` & `notebook-7.2.0rc1/notebook/static/5996.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/5cda41563a095bd70c78.woff` & `notebook-7.2.0rc1/notebook/static/5cda41563a095bd70c78.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6017.bundle.js` & `notebook-7.2.0rc1/notebook/static/6017.bundle.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6017], {
         36017: (e, r, t) => {
             t.d(r, {
                 CSVSearchProvider: () => c
             });
-            var i = t(37544),
-                s = t(10979),
-                n = t(26862);
+            var i = t(16478),
+                s = t(65903),
+                n = t(95183);
             class c extends n.SearchProvider {
                 constructor() {
                     super(...arguments), this.isReadOnly = !0
                 }
                 static createNew(e, r) {
                     return new c(e)
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/6061.bundle.js` & `notebook-7.2.0rc1/notebook/static/6061.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6139.bundle.js` & `notebook-7.2.0rc1/notebook/static/6139.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6139], {
         56139: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => g
             });
-            var n, a = o(2922),
-                i = o(96049),
-                r = o(94889),
-                c = o(37267);
+            var n, a = o(44604),
+                i = o(53312),
+                r = o(43269),
+                c = o(12030);
             ! function(e) {
                 e.resetImage = "imageviewer:reset-image", e.zoomIn = "imageviewer:zoom-in", e.zoomOut = "imageviewer:zoom-out", e.flipHorizontal = "imageviewer:flip-horizontal", e.flipVertical = "imageviewer:flip-vertical", e.rotateClockwise = "imageviewer:rotate-clockwise", e.rotateCounterclockwise = "imageviewer:rotate-counterclockwise", e.invertColors = "imageviewer:invert-colors"
             }(n || (n = {}));
             const l = ["png", "gif", "jpeg", "bmp", "ico", "tiff"],
                 d = "Image",
                 s = "Image (Text)",
                 m = ["svg", "xbm"],
```

### Comparing `notebook-7.2.0rc0/notebook/static/62.bundle.js` & `notebook-7.2.0rc1/notebook/static/62.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [62], {
         40062: (e, o, n) => {
             n.r(o), n.d(o, {
                 default: () => c
             });
-            var t, l = n(2922),
-                a = n(24554),
-                d = n(87017),
-                i = n(37267),
-                s = n(22620);
+            var t, l = n(44604),
+                a = n(23295),
+                d = n(79426),
+                i = n(12030),
+                s = n(35613);
             ! function(e) {
                 e.displayNumbering = "toc:display-numbering", e.displayH1Numbering = "toc:display-h1-numbering", e.displayOutputNumbering = "toc:display-outputs-numbering", e.showPanel = "toc:show-panel", e.toggleCollapse = "toc:toggle-collapse"
             }(t || (t = {}));
             const r = {
                     id: "@jupyterlab/toc-extension:registry",
                     description: "Provides the table of contents registry.",
                     autoStart: !0,
```

### Comparing `notebook-7.2.0rc0/notebook/static/6271.bundle.js` & `notebook-7.2.0rc1/notebook/static/6271.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6281.bundle.js` & `notebook-7.2.0rc1/notebook/static/6281.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -52,15 +52,15 @@
             n.d(t, {
                 r: () => N
             });
             var r = n(7259),
                 i = n(81779),
                 a = n(98443),
                 d = n(24028),
-                l = n(29197),
+                l = n(67406),
                 o = n(14780),
                 s = n(23617);
             let c = {},
                 h = {},
                 g = {};
             const f = (e, t) => (d.l.trace("In isDecendant", t, " ", e, " = ", h[t].includes(e)), !!h[t].includes(e)),
                 u = (e, t, n, r) => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/632.bundle.js` & `notebook-7.2.0rc1/notebook/static/632.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6345.bundle.js` & `notebook-7.2.0rc1/notebook/static/6345.bundle.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6345, 4645], {
         94645: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => p
             });
-            var n = o(2922),
-                s = o(80106),
-                a = o(1167),
-                r = o(46807),
+            var n = o(44604),
+                s = o(67260),
+                a = o(68722),
+                r = o(59625),
                 c = o(33625);
             const i = {
                     id: "@jupyter-notebook/console-extension:opener",
                     requires: [n.IRouter],
                     autoStart: !0,
                     description: "A plugin to open consoles in a new tab",
                     activate: (e, t) => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/6417.bundle.js` & `notebook-7.2.0rc1/notebook/static/6417.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -71,15 +71,15 @@
             }
         },
         66417: (e, t, n) => {
             n.d(t, {
                 diagram: () => s
             });
             var r = n(31261),
-                l = (n(29197), n(23617));
+                l = (n(67406), n(23617));
             n(24028), n(36004), n(65479), n(21845), n(7259), n(51723), n(74193), n(12451), n(36735), n(87768), l.c_6;
             var o = n(3675);
             n(27693), n(7608), n(31699), n(81779);
             const a = {},
                 s = {
                     parser: r.p,
                     db: r.f,
@@ -95,15 +95,15 @@
                 }
         },
         3675: (e, t, n) => {
             n.d(t, {
                 a: () => h,
                 f: () => u
             });
-            var r = n(29197),
+            var r = n(67406),
                 l = n(23617),
                 o = n(24028),
                 a = n(86281),
                 s = n(74193),
                 i = n(90267),
                 c = n(42528);
             const d = (e, t) => i.Z.lang.round(c.Z.parse(e)[t]);
```

### Comparing `notebook-7.2.0rc0/notebook/static/647.bundle.js` & `notebook-7.2.0rc1/notebook/static/647.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6521.bundle.js` & `notebook-7.2.0rc1/notebook/static/6521.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6604.bundle.js` & `notebook-7.2.0rc1/notebook/static/6604.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6604, 2088], {
         6604: (e, o, t) => {
             t.r(o), t.d(o, {
                 default: () => b
             });
-            var n, i = t(80106),
-                r = t(1167),
-                l = t(42703),
-                s = t(17894),
-                a = t(13408),
-                d = t(15327),
-                c = t(37267),
+            var n, i = t(67260),
+                r = t(68722),
+                l = t(34663),
+                s = t(25460),
+                a = t(81221),
+                d = t(27865),
+                c = t(12030),
                 u = t(33625),
                 p = t(63485);
             ! function(e) {
                 e.dismiss = "tooltip:dismiss", e.launchConsole = "tooltip:launch-console", e.launchNotebook = "tooltip:launch-notebook", e.launchFile = "tooltip:launch-file"
             }(n || (n = {}));
             const m = {
                     id: "@jupyterlab/tooltip-extension:manager",
```

### Comparing `notebook-7.2.0rc0/notebook/static/661.bundle.js` & `notebook-7.2.0rc1/notebook/static/661.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6621.bundle.js` & `notebook-7.2.0rc1/notebook/static/6621.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6621], {
         78947: (e, t, s) => {
             s.d(t, {
                 q: () => He
             });
-            var i = s(22620);
+            var i = s(35613);
             const r = 1540483477,
                 n = new TextEncoder;
 
             function o(e, t) {
                 const s = n.encode(e);
                 let i = s.length,
                     o = t ^ i,
@@ -66,16 +66,16 @@
                         suffix: i
                     })
                 }
                 getTmpFileParams(e) {
                     return this._fileParams.get(e)
                 }
             }
-            var l, d = s(96049),
-                c = s(67406),
+            var l, d = s(53312),
+                c = s(73166),
                 h = s(63485);
             ! function(e) {
                 e.getCode = function(e) {
                     return new u({
                         ...e,
                         body: new p(e),
                         buttons: [d.Dialog.cancelButton({
@@ -118,15 +118,15 @@
                 getValue() {
                     return this._prompt.model.sharedModel.getSource()
                 }
                 onAfterAttach(e) {
                     super.onAfterAttach(e), this._prompt.activate()
                 }
             }
-            var g = s(52839);
+            var g = s(51429);
             class _ {
                 constructor(e) {
                     this._services = e.editorServices
                 }
                 createNewEditor(e) {
                     const {
                         content: t,
@@ -147,18 +147,18 @@
                         factory: r
                     });
                     return a.node.setAttribute("data-jp-debugger", "true"), a.disposed.connect((() => {
                         o.dispose()
                     })), a
                 }
             }
-            var m, v = s(37267),
-                b = s(58959),
+            var m, v = s(12030),
+                b = s(31231),
                 f = s(81997),
-                w = s(1167),
+                w = s(68722),
                 k = s(89843),
                 S = s(3546);
             class C {
                 constructor(e) {
                     var t, s, i, r;
                     this._src = e.src, this._id = null !== (i = null === (s = null === (t = e.debuggerService.session) || void 0 === t ? void 0 : t.connection) || void 0 === s ? void 0 : s.id) && void 0 !== i ? i : "", this._path = null !== (r = e.path) && void 0 !== r ? r : "", this._debuggerService = e.debuggerService, this._editor = e.getEditor, this._editorMonitor = new w.ActivityMonitor({
                         signal: this._src.changed,
@@ -804,15 +804,15 @@
                             dataModel: e
                         } = this._grid;
                         e.filter = this._filter, e.scope = this._scope, e.setData(null !== (t = this.model.scopes) && void 0 !== t ? t : [])
                     }
                     super.onUpdateRequest(e)
                 }
             }
-            var U = s(13408),
+            var U = s(81221),
                 J = s(20998);
             class Y extends d.MainAreaWidget {
                 constructor(e) {
                     const {
                         dataLoader: t,
                         rendermime: s,
                         translator: i
```

### Comparing `notebook-7.2.0rc0/notebook/static/6627.bundle.js` & `notebook-7.2.0rc1/notebook/static/6627.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6627], {
         6627: (e, a, r) => {
             r.r(a), r.d(a, {
                 default: () => d
             });
-            var t = r(96049),
-                s = r(37267);
+            var t = r(53312),
+                s = r(12030);
             const d = {
                 id: "@jupyterlab/theme-dark-extension:plugin",
                 description: "Adds a dark theme.",
                 requires: [t.IThemeManager, s.ITranslator],
                 activate: (e, a, r) => {
                     const t = r.load("jupyterlab");
                     a.register({
```

### Comparing `notebook-7.2.0rc0/notebook/static/6640.bundle.js` & `notebook-7.2.0rc1/notebook/static/6640.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         6640: (t, e, a) => {
             a.d(e, {
                 diagram: () => f
             });
             var i = a(75343),
                 n = a(23617),
                 d = a(7259),
-                r = a(29197),
+                r = a(67406),
                 s = a(24028);
             a(27693), a(7608), a(31699);
             const o = {},
                 c = (t, e, a) => {
                     const i = (0, s.c)().state.padding,
                         n = 2 * (0, s.c)().state.padding,
                         d = t.node().getBBox(),
```

### Comparing `notebook-7.2.0rc0/notebook/static/6667.bundle.js` & `notebook-7.2.0rc1/notebook/static/6667.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/67.bundle.js` & `notebook-7.2.0rc1/notebook/static/67.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6731.bundle.js` & `notebook-7.2.0rc1/notebook/static/6731.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6739.bundle.js` & `notebook-7.2.0rc1/notebook/static/6739.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6748.bundle.js` & `notebook-7.2.0rc1/notebook/static/6748.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6748], {
         86748: (e, n, o) => {
             o.r(n), o.d(n, {
                 default: () => P
             });
-            var t = o(2922),
-                r = o(96049),
-                l = o(52839),
-                s = o(89144),
-                a = o(80106),
-                c = o(42751),
-                i = o(65651),
-                d = o(50845),
-                u = o(13408),
-                p = o(24554),
-                m = o(37267),
-                C = o(22620),
+            var t = o(44604),
+                r = o(53312),
+                l = o(51429),
+                s = o(81002),
+                a = o(67260),
+                c = o(71427),
+                i = o(86810),
+                d = o(29879),
+                u = o(81221),
+                p = o(23295),
+                m = o(12030),
+                C = o(35613),
                 v = o(33625),
                 g = o(20998),
                 h = o(2549),
                 b = o(14421);
             const f = {
                     id: "@jupyterlab/console-extension:foreign",
                     description: "Add foreign handler of IOPub messages to the console.",
```

### Comparing `notebook-7.2.0rc0/notebook/static/677.bundle.js` & `notebook-7.2.0rc1/notebook/static/677.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6788.bundle.js` & `notebook-7.2.0rc1/notebook/static/6788.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6815.bundle.js` & `notebook-7.2.0rc1/notebook/static/6815.bundle.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6815], {
         56815: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => u
             });
-            var n = a(2922),
-                o = a(96049),
-                s = a(50845),
-                l = a(24554),
-                r = a(37267);
+            var n = a(44604),
+                o = a(53312),
+                s = a(29879),
+                l = a(23295),
+                r = a(12030);
             const i = "@jupyterlab/translation-extension:plugin",
                 c = {
                     id: "@jupyterlab/translation:translator",
                     description: "Provides the application translation object.",
                     autoStart: !0,
                     requires: [n.JupyterFrontEnd.IPaths, l.ISettingRegistry],
                     optional: [n.ILabShell],
```

### Comparing `notebook-7.2.0rc0/notebook/static/6853.bundle.js` & `notebook-7.2.0rc1/notebook/static/6853.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -19,27 +19,27 @@
                 LayoutRestorer: () => E.c,
                 Router: () => S,
                 addSemanticCommand: () => O,
                 createRendermimePlugin: () => m.aX,
                 createRendermimePlugins: () => m.as,
                 createSemanticCommand: () => D
             });
-            var n = i(96049),
-                s = i(37267);
+            var n = i(53312),
+                s = i(12030);
             const a = async function(e, t, i) {
                 const a = (i = i || s.nullTranslator).load("jupyterlab"),
                     r = a.__("Server Connection Error"),
                     o = a.__("A connection to the Jupyter server could not be established.\nJupyterLab will continue trying to reconnect.\nCheck your network connection or Jupyter server configuration.\n");
                 return (0, n.showErrorMessage)(r, {
                     message: o
                 })
             };
-            var r, o, d = i(10979),
-                l = i(70611),
-                h = i(22620),
+            var r, o, d = i(65903),
+                l = i(87408),
+                h = i(35613),
                 c = i(34771),
                 u = i(20998),
                 p = i(81997);
             class g extends c.Application {
                     constructor(e) {
                         super(e), this._formatChanged = new p.Signal(this), this.contextMenu = new h.ContextMenuSvg({
                             commands: this.commands,
@@ -90,15 +90,15 @@
                     e.suppressContextMenu = function(e) {
                         return null !== e.closest("[data-jp-suppress-context-menu]")
                     }
                 }(r || (r = {})),
                 function(e) {
                     e.contextMenu = "__internal:context-menu-info"
                 }(o || (o = {}));
-            var _ = i(1167),
+            var _ = i(68722),
                 m = i(75677),
                 f = i(33625),
                 v = i(49503),
                 y = i(97934),
                 w = i(63485);
             const b = "jp-SideBar",
                 P = "jp-mod-current",
```

### Comparing `notebook-7.2.0rc0/notebook/static/6893.bundle.js` & `notebook-7.2.0rc1/notebook/static/7684.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [6893, 7684], {
+    [7684, 6893], {
         56893: (t, e, o) => {
             o.r(e), o.d(e, {
                 CommandIDs: () => n,
                 default: () => i
             });
-            var n, a = o(2922),
-                r = o(96049),
-                s = o(1167),
-                u = o(37267);
+            var n, a = o(44604),
+                r = o(53312),
+                s = o(68722),
+                u = o(12030);
             ! function(t) {
                 t.controlPanel = "hub:control-panel", t.logout = "hub:logout", t.restart = "hub:restart"
             }(n || (n = {}));
             const i = [{
                 activate: function(t, e, o, a) {
                     const r = o.load("jupyterlab"),
                         u = e.urls.hubHost || "",
```

### Comparing `notebook-7.2.0rc0/notebook/static/69.bundle.js` & `notebook-7.2.0rc1/notebook/static/69.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/690.bundle.js` & `notebook-7.2.0rc1/notebook/static/690.bundle.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -5,31 +5,31 @@
             n.r(t), n.d(t, {
                 MIME_TYPE: () => d,
                 MIME_TYPES_JSONL: () => l,
                 RenderedJSON: () => p,
                 default: () => m,
                 rendererFactory: () => c
             });
-            var r = n(96049),
-                o = n(37267),
+            var r = n(53312),
+                o = n(12030),
                 s = n(63485),
                 i = n(78156),
                 a = n(37634);
             const d = "application/json",
                 l = ["text/jsonl", "application/jsonl", "application/json-lines"];
             class p extends s.Widget {
                 constructor(e) {
                     super(), this._rootDOM = null, this.addClass("jp-RenderedJSON"), this.addClass("CodeMirror"), this._mimeType = e.mimeType, this.translator = e.translator || o.nullTranslator
                 } [r.Printing.symbol]() {
                     return () => r.Printing.printWidget(this)
                 }
                 async renderModel(e) {
                     const {
                         Component: t
-                    } = await Promise.all([n.e(9752), n.e(998), n.e(2620), n.e(9269), n.e(2209)]).then(n.bind(n, 69752));
+                    } = await Promise.all([n.e(9752), n.e(998), n.e(5613), n.e(525), n.e(2209)]).then(n.bind(n, 69752));
                     let r;
                     if (l.indexOf(this._mimeType) >= 0) {
                         const t = (e.data[this._mimeType] || "").trim().split(/\n/);
                         r = JSON.parse(`[${t.join(",")}]`)
                     } else r = e.data[this._mimeType] || {};
                     const o = e.metadata[this._mimeType] || {};
                     return null === this._rootDOM && (this._rootDOM = (0, a.s)(this.node)), new Promise(((e, n) => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/6942.bundle.js` & `notebook-7.2.0rc1/notebook/static/6942.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6962.bundle.js` & `notebook-7.2.0rc1/notebook/static/6962.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6962], {
         56962: (t, e, r) => {
             r.r(e), r.d(e, {
                 default: () => T
             });
-            var n = r(2922),
-                a = r(96049),
-                o = r(81350),
-                s = r(24554),
-                i = r(37267),
-                c = r(22620);
+            var n = r(44604),
+                a = r(53312),
+                o = r(57957),
+                s = r(23295),
+                i = r(12030),
+                c = r(35613);
             const l = "@jupyterlab/htmlviewer-extension:plugin",
                 d = "HTML Viewer";
             var u;
             ! function(t) {
                 t.trustHTML = "htmlviewer:trust-html"
             }(u || (u = {}));
             const m = {
```

### Comparing `notebook-7.2.0rc0/notebook/static/6972.bundle.js` & `notebook-7.2.0rc1/notebook/static/6972.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/6999.bundle.js` & `notebook-7.2.0rc1/notebook/static/6999.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -212,15 +212,15 @@
                     for (; null !== (r = e.exec(t));) s.push({
                         text: r[0],
                         position: r.index
                     });
                     return Promise.resolve(s)
                 }
             };
-            var p, u = s(22620),
+            var p, u = s(35613),
                 g = s(97934);
             class m extends u.VDomModel {
                 constructor(e, t) {
                     if (super(), this.searchProvider = e, this._caseSensitive = !1, this._disposed = new i.Signal(this), this._parsingError = "", this._preserveCase = !1, this._initialQuery = "", this._filters = {}, this._replaceText = "", this._searchActive = !1, this._searchExpression = "", this._useRegex = !1, this._wholeWords = !1, this._filters = {}, this.searchProvider.getFilters) {
                         const e = this.searchProvider.getFilters();
                         for (const t in e) this._filters[t] = e[t].default
                     }
@@ -357,17 +357,17 @@
                     const i = t ? "gm" : "gim";
                     let n = s ? e : e.replace(/[-[\]/{}()*+?.\\^$|]/g, "\\$&");
                     r && (n = "\\b" + n + "\\b");
                     const a = new RegExp(n, i);
                     return a.test("") ? null : a
                 }
             }(p || (p = {}));
-            var _ = s(37267),
+            var _ = s(12030),
                 v = s(16934),
-                x = s(96049),
+                x = s(53312),
                 C = s(78156);
             const E = "jp-DocumentSearch-overlay-row",
                 f = "jp-DocumentSearch-input",
                 y = "jp-DocumentSearch-input-label",
                 S = "jp-DocumentSearch-input-wrapper",
                 b = "jp-DocumentSearch-input-button-off",
                 w = "jp-DocumentSearch-input-button-on",
```

### Comparing `notebook-7.2.0rc0/notebook/static/7005.bundle.js` & `notebook-7.2.0rc1/notebook/static/7005.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7010.bundle.js` & `notebook-7.2.0rc1/notebook/static/7010.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7022.bundle.js` & `notebook-7.2.0rc1/notebook/static/7022.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7054.bundle.js` & `notebook-7.2.0rc1/notebook/static/7054.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7097.bundle.js` & `notebook-7.2.0rc1/notebook/static/7097.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         87097: (t, e, i) => {
             i.d(e, {
                 diagram: () => T
             });
             var n = i(24028),
                 r = i(23617),
                 s = i(7259),
-                a = i(29197),
+                a = i(67406),
                 l = (i(27693), i(7608), i(31699), function() {
                     var t = function(t, e, i, n) {
                             for (i = i || {}, n = t.length; n--; i[t[n]] = e);
                             return i
                         },
                         e = [1, 3],
                         i = [1, 4],
```

### Comparing `notebook-7.2.0rc0/notebook/static/7153.bundle.js` & `notebook-7.2.0rc1/notebook/static/7153.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -73,15 +73,15 @@
         57153: (e, t, n) => {
             n.d(t, {
                 diagram: () => a
             });
             var r = n(31261),
                 l = n(3675),
                 o = n(24028);
-            n(23617), n(29197), n(7259), n(81779), n(27693), n(7608), n(31699);
+            n(23617), n(67406), n(7259), n(81779), n(27693), n(7608), n(31699);
             const a = {
                 parser: r.p,
                 db: r.f,
                 renderer: l.f,
                 styles: l.a,
                 init: e => {
                     e.flowchart || (e.flowchart = {}), e.flowchart.arrowMarkerAbsolute = e.arrowMarkerAbsolute, (0, o.p)({
@@ -93,15 +93,15 @@
             }
         },
         3675: (e, t, n) => {
             n.d(t, {
                 a: () => h,
                 f: () => u
             });
-            var r = n(29197),
+            var r = n(67406),
                 l = n(23617),
                 o = n(24028),
                 a = n(86281),
                 s = n(74193),
                 i = n(90267),
                 c = n(42528);
             const d = (e, t) => i.Z.lang.round(c.Z.parse(e)[t]);
```

### Comparing `notebook-7.2.0rc0/notebook/static/7154.bundle.js` & `notebook-7.2.0rc1/notebook/static/7154.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7170.bundle.js` & `notebook-7.2.0rc1/notebook/static/7170.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7179.bundle.js` & `notebook-7.2.0rc1/notebook/static/7179.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/721921bab0d001ebff02.woff` & `notebook-7.2.0rc1/notebook/static/721921bab0d001ebff02.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7226.bundle.js` & `notebook-7.2.0rc1/notebook/static/7226.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,17 +5,17 @@
             s.r(e), s.d(e, {
                 OutputArea: () => x,
                 OutputAreaModel: () => d,
                 OutputPrompt: () => v,
                 SimplifiedOutputArea: () => w,
                 Stdin: () => O
             });
-            var i, n = s(81692),
-                r = s(58959),
-                a = s(13408),
+            var i, n = s(81139),
+                r = s(31231),
+                a = s(81221),
                 o = s(33625),
                 h = s(20998),
                 u = s(81997);
             class d {
                 constructor(t = {}) {
                     if (this.clearNext = !1, this._lastStream = "", this._trusted = !1, this._isDisposed = !1, this._stateChanged = new u.Signal(this), this._changed = new u.Signal(this), this._trusted = !!t.trusted, this.contentFactory = t.contentFactory || d.defaultContentFactory, this.list = new r.ObservableList, t.values)
                         for (const e of t.values) {
@@ -167,17 +167,17 @@
                         do {
                             e = (t = e).replace(/[^\n]\x08/gm, "")
                         } while (e.length < t.length);
                         return t
                     }(t))
                 }
             }(i || (i = {}));
-            var l = s(96049),
-                c = s(70611),
-                p = s(37267),
+            var l = s(53312),
+                c = s(87408),
+                p = s(12030),
                 _ = s(14421),
                 m = s(63485);
             const g = "jp-OutputArea-child",
                 y = "jp-OutputArea-output",
                 f = "jp-OutputArea-prompt";
             class x extends m.Widget {
                 constructor(t) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/7252.bundle.js` & `notebook-7.2.0rc1/notebook/static/9685.bundle.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [7252, 9685], {
+    [9685, 7252], {
         79685: (e, t, r) => {
             r.r(t), r.d(t, {
                 default: () => k
             });
-            var n, a = r(2922),
-                o = r(96049),
-                d = r(1167),
-                i = r(97592),
-                c = r(13408),
-                s = r(24554),
-                w = r(87017),
-                m = r(37267);
+            var n, a = r(44604),
+                o = r(53312),
+                d = r(68722),
+                i = r(3991),
+                c = r(81221),
+                s = r(23295),
+                w = r(79426),
+                m = r(12030);
             ! function(e) {
                 e.markdownPreview = "markdownviewer:open", e.markdownEditor = "markdownviewer:edit"
             }(n || (n = {}));
             const p = "Markdown Preview",
                 l = {
                     activate: function(e, t, r, a, s, w, m) {
                         const k = r.load("jupyterlab"),
```

### Comparing `notebook-7.2.0rc0/notebook/static/7259.bundle.js` & `notebook-7.2.0rc1/notebook/static/7259.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
             var r = t(21845),
                 o = t(12451),
                 i = t(36004),
                 u = t(78795),
                 a = t(28099),
                 c = t(12930),
                 s = t(36735),
-                d = t(29197);
+                d = t(67406);
             class f {
                 constructor() {
                     var n = {};
                     n._next = n._prev = n, this._sentinel = n
                 }
                 dequeue() {
                     var n = this._sentinel,
@@ -1862,15 +1862,15 @@
             }
 
             function A(n, e) {
                 return R(n, e.v, e.w, e.name)
             }
             I.prototype._nodeCount = 0, I.prototype._edgeCount = 0
         },
-        29197: (n, e, t) => {
+        67406: (n, e, t) => {
             t.d(e, {
                 k: () => r.k
             });
             var r = t(7303)
         },
         40105: (n, e, t) => {
             t.d(e, {
@@ -2454,15 +2454,15 @@
                 u = Object.getOwnPropertySymbols;
             const a = u ? function(n) {
                 return null == n ? [] : (n = Object(n), (0, r.Z)(u(n), (function(e) {
                     return i.call(n, e)
                 })))
             } : o.Z
         },
-        14270: (n, e, t) => {
+        18625: (n, e, t) => {
             t.d(e, {
                 Z: () => s
             });
             var r = t(94022),
                 o = t(9028),
                 i = t(64058),
                 u = t(8616),
@@ -2581,27 +2581,27 @@
             t.d(e, {
                 Z: () => u
             });
             var r = Object.prototype.hasOwnProperty;
             const o = function(n, e) {
                 return null != n && r.call(n, e)
             };
-            var i = t(14270);
+            var i = t(18625);
             const u = function(n, e) {
                 return null != n && (0, i.Z)(n, e, o)
             }
         },
         94180: (n, e, t) => {
             t.d(e, {
                 Z: () => i
             });
             const r = function(n, e) {
                 return null != n && e in Object(n)
             };
-            var o = t(14270);
+            var o = t(18625);
             const i = function(n, e) {
                 return null != n && (0, o.Z)(n, e, r)
             }
         },
         59660: (n, e, t) => {
             t.d(e, {
                 Z: () => i
```

### Comparing `notebook-7.2.0rc0/notebook/static/7264.bundle.js` & `notebook-7.2.0rc1/notebook/static/7264.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/72bc573386dd1d48c5bb.woff` & `notebook-7.2.0rc1/notebook/static/72bc573386dd1d48c5bb.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7302.bundle.js` & `notebook-7.2.0rc1/notebook/static/3768.bundle.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [7302, 3768], {
+    [3768, 7302], {
         83768: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => F
             });
-            var n = o(96049),
-                r = o(1167),
-                i = o(42751),
-                a = o(24554),
-                s = o(15729),
-                l = o(1131),
-                d = o(37267),
-                c = o(22620),
+            var n = o(53312),
+                r = o(68722),
+                i = o(71427),
+                a = o(23295),
+                s = o(9235),
+                l = o(74258),
+                d = o(12030),
+                c = o(35613),
                 g = o(81997),
                 u = o(63485),
-                w = o(42367),
+                w = o(64803),
                 h = o(78156),
                 b = o.n(h);
             class p {
                 constructor(e) {
                     this._onSelectionChanged = () => {
                         var e, t, o, n, r, i;
                         const a = Array.from(this._browser.selectedItems()),
```

### Comparing `notebook-7.2.0rc0/notebook/static/7360.bundle.js` & `notebook-7.2.0rc1/notebook/static/7360.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7369.bundle.js` & `notebook-7.2.0rc1/notebook/static/7369.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7378.bundle.js` & `notebook-7.2.0rc1/notebook/static/7378.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7386.bundle.js` & `notebook-7.2.0rc1/notebook/static/7386.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,17 +2,17 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [7386, 4811], {
         37386: (e, t, o) => {
             o.r(t), o.d(t, {
                 CellBarExtension: () => u,
                 CellToolbarTracker: () => c
             });
-            var l = o(96049),
-                n = o(58959),
-                a = o(22620),
+            var l = o(53312),
+                n = o(31231),
+                a = o(35613),
                 i = o(33625),
                 s = o(81997);
             const r = ["text/plain", "application/vnd.jupyter.stdout", "application/vnd.jupyter.stderr"],
                 d = "jp-toolbar-overlap";
             class c {
                 constructor(e, t, o) {
                     if (this._isDisposed = !1, this._toolbar = null, this._toolbarItems = null, this._toolbarFactory = null, this._panel = e, this._previousActiveCell = this._panel.content.activeCell, this._toolbarItems = null != t ? t : null, this._toolbarFactory = null != o ? o : null, null === this._toolbarItems && null === this._toolbarFactory) throw Error("You must provide the toolbarFactory or the toolbar items.");
```

### Comparing `notebook-7.2.0rc0/notebook/static/7391.bundle.js` & `notebook-7.2.0rc1/notebook/static/7391.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
                 IEditorMimeTypeService: () => s,
                 IEditorServices: () => S,
                 IPositionModel: () => N,
                 JSONEditor: () => m,
                 LineCol: () => f
             });
             var s, o, n = i(57508),
-                r = i(58959),
+                r = i(31231),
                 a = i(81997);
             ! function(e) {
                 e.defaultMimeType = "text/plain"
             }(s || (s = {})),
             function(e) {
                 e.Model = class {
                     constructor(e = {}) {
@@ -47,16 +47,16 @@
                         return this._isDisposed
                     }
                     dispose() {
                         this._isDisposed || (this._isDisposed = !0, this._selections.dispose(), this.standaloneModel && this.sharedModel.dispose(), a.Signal.clearData(this))
                     }
                 }
             }(o || (o = {}));
-            var d = i(37267),
-                l = i(22620),
+            var d = i(12030),
+                l = i(35613),
                 h = i(20998),
                 c = i(63485);
             const u = "jp-mod-error";
             class m extends c.Widget {
                 constructor(e) {
                     super(), this._dataDirty = !1, this._inputDirty = !1, this._source = null, this._originalValue = h.JSONExt.emptyObject, this._changeGuard = !1, this.translator = e.translator || d.nullTranslator, this._trans = this.translator.load("jupyterlab"), this.addClass("jp-JSONEditor"), this.headerNode = document.createElement("div"), this.headerNode.className = "jp-JSONEditor-header", this.revertButtonNode = l.undoIcon.element({
                         tag: "span",
@@ -150,18 +150,18 @@
                             line: 0,
                             column: 1
                         })
                     }
                     this._changeGuard = !1, this.commitButtonNode.hidden = !0, this.revertButtonNode.hidden = !0
                 }
             }
-            var p = i(27829),
+            var p = i(71098),
                 _ = i(78156),
                 g = i.n(_),
-                v = i(96049);
+                v = i(53312);
             class C extends g().Component {
                 constructor(e) {
                     super(e), this._handleChange = e => {
                         this.setState({
                             value: e.currentTarget.value
                         })
                     }, this._handleSubmit = e => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/7427.bundle.js` & `notebook-7.2.0rc1/notebook/static/7427.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/745.bundle.js` & `notebook-7.2.0rc1/notebook/static/745.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7450.bundle.js` & `notebook-7.2.0rc1/notebook/static/7450.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7471.bundle.js` & `notebook-7.2.0rc1/notebook/static/7471.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [7471], {
-        15664: function(t, e, r) {
+        35663: function(t, e, r) {
             var n, o = this && this.__extends || (n = function(t, e) {
                 return n = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(t, e) {
                     t.__proto__ = e
                 } || function(t, e) {
@@ -1040,15 +1040,15 @@
                     this.constructor = t
                 }
                 n(t, e), t.prototype = null === e ? Object.create(e) : (r.prototype = e.prototype, new r)
             });
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.HTMLHandler = void 0;
-            var i = r(15664),
+            var i = r(35663),
                 s = r(99331),
                 a = function(t) {
                     function e() {
                         var e = null !== t && t.apply(this, arguments) || this;
                         return e.documentClass = s.HTMLDocument, e
                     }
                     return o(e, t), e.prototype.handlesDocument = function(t) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/7506.bundle.js` & `notebook-7.2.0rc1/notebook/static/7506.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -163,15 +163,15 @@
                 usersIcon: () => mt,
                 vegaIcon: () => gt,
                 wordIcon: () => vt,
                 yamlIcon: () => ft
             });
             var s = n(78156),
                 i = n.n(s),
-                r = n(1167);
+                r = n(68722);
 
             function o(e) {
                 return e.map((e => e && "object" == typeof e ? Object.keys(e).map((t => !!e[t] && t)) : "string" == typeof e ? e.split(/\s+/) : [])).reduce(((e, t) => e.concat(t)), []).filter((e => !!e))
             }
 
             function a(...e) {
                 return o(e).join(" ")
@@ -1341,15 +1341,15 @@
                 _onTitleChanged(e) {
                     this._setHeader()
                 }
                 _setHeader() {
                     this._collapsed ? this._header.addClass(wt) : this._header.removeClass(wt)
                 }
             }
-            var yt = n(37267),
+            var yt = n(12030),
                 xt = n(24246),
                 Ct = n(24885),
                 _t = n(99729),
                 St = n.n(_t),
                 jt = n(90104),
                 kt = n.n(jt),
                 It = n(14648),
@@ -7323,32 +7323,35 @@
                     r = i ? void 0 : t => {
                         var n;
                         0 === t.button && (t.preventDefault(), null === (n = e.onClick) || void 0 === n || n.call(e))
                     },
                     o = i ? t => {
                         var n;
                         0 === t.button && (null === (n = e.onClick) || void 0 === n || n.call(e))
-                    } : void 0;
+                    } : void 0,
+                    l = !1 === e.enabled && e.disabledTooltip ? e.disabledTooltip : e.pressed && e.pressedTooltip ? e.pressedTooltip : e.tooltip || e.iconLabel,
+                    c = !1 === e.enabled;
                 return s.createElement(io, {
                     appearance: "stealth",
                     className: e.className ? e.className + " jp-ToolbarButtonComponent" : "jp-ToolbarButtonComponent",
+                    "aria-disabled": c,
+                    "aria-label": e.label || l,
                     "aria-pressed": e.pressed,
-                    "aria-disabled": !1 === e.enabled,
                     ...e.dataset,
-                    disabled: !1 === e.enabled,
+                    disabled: c,
                     onClick: o,
                     onMouseDown: r,
                     onKeyDown: t => {
                         var n;
                         const {
                             key: s
                         } = t;
                         "Enter" !== s && " " !== s || null === (n = e.onClick) || void 0 === n || n.call(e)
                     },
-                    title: !1 === e.enabled && e.disabledTooltip ? e.disabledTooltip : e.pressed && e.pressedTooltip ? e.pressedTooltip : e.tooltip || e.iconLabel,
+                    title: l,
                     minimal: !0
                 }, (e.icon || e.iconClass) && s.createElement(b.resolveReact, {
                     icon: e.pressed && null !== (n = e.pressedIcon) && void 0 !== n ? n : e.icon,
                     iconClass: a(e.iconClass, "jp-Icon"),
                     tag: null
                 }), e.label && s.createElement("span", {
                     className: "jp-ToolbarButtonComponent-label"
```

### Comparing `notebook-7.2.0rc0/notebook/static/7534.bundle.js` & `notebook-7.2.0rc1/notebook/static/7534.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7543.bundle.js` & `notebook-7.2.0rc1/notebook/static/7543.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -13,17 +13,17 @@
                 SaveHandler: () => f,
                 SavingStatus: () => W,
                 isValidFileName: () => d,
                 renameDialog: () => c,
                 renameFile: () => l,
                 shouldOverwrite: () => h
             });
-            var n, i = s(96049),
-                a = s(1167),
-                o = s(37267),
+            var n, i = s(53312),
+                a = s(68722),
+                o = s(12030),
                 r = s(63485);
 
             function c(e, t, s) {
                 const n = (s = s || o.nullTranslator).load("jupyterlab"),
                     a = t.localPath.split("/").pop() || t.localPath;
                 return (0, i.showDialog)({
                     title: n.__("Rename File"),
@@ -84,15 +84,15 @@
                     a.textContent = e;
                     const r = document.createElement("label");
                     r.textContent = s.__("New Name"), r.className = "jp-new-name-title";
                     const c = document.createElement("input");
                     return n.appendChild(i), n.appendChild(a), n.appendChild(r), n.appendChild(c), n
                 }
             }(n || (n = {}));
-            var _ = s(10979),
+            var _ = s(65903),
                 u = s(33625),
                 m = s(20998),
                 p = s(14421),
                 v = s(81997);
             class f {
                 constructor(e) {
                     this._autosaveTimer = -1, this._minInterval = -1, this._interval = -1, this._isActive = !1, this._inDialog = !1, this._isDisposed = !1, this._multiplier = 10, this._context = e.context, this._isConnectedCallback = e.isConnectedCallback || (() => !0);
@@ -613,16 +613,16 @@
                 }
             }! function(e) {
                 e.saveHandlerProperty = new p.AttachedProperty({
                     name: "saveHandler",
                     create: () => {}
                 })
             }(y || (y = {}));
-            var P = s(27829),
-                b = s(22620),
+            var P = s(71098),
+                b = s(35613),
                 R = s(78156),
                 S = s.n(R);
 
             function T(e) {
                 return S().createElement(P.TextItem, {
                     source: e.name,
                     title: e.fullPath
```

### Comparing `notebook-7.2.0rc0/notebook/static/755.bundle.js` & `notebook-7.2.0rc1/notebook/static/755.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -68,15 +68,15 @@
             t.exports = o
         },
         23694: (t, r, e) => {
             var o = e(36301),
                 n = e(7354),
                 a = e(5863),
                 s = e(12367),
-                i = e(90748),
+                i = e(63878),
                 u = e(97569);
 
             function c(t) {
                 var r = this.__data__ = new o(t);
                 this.size = r.size
             }
             c.prototype.clear = n, c.prototype.delete = a, c.prototype.get = s, c.prototype.has = i, c.prototype.set = u, t.exports = c
@@ -565,15 +565,15 @@
             }
         },
         12367: t => {
             t.exports = function(t) {
                 return this.__data__.get(t)
             }
         },
-        90748: t => {
+        63878: t => {
             t.exports = function(t) {
                 return this.__data__.has(t)
             }
         },
         97569: (t, r, e) => {
             var o = e(36301),
                 n = e(44538),
```

### Comparing `notebook-7.2.0rc0/notebook/static/7582.bundle.js` & `notebook-7.2.0rc1/notebook/static/7582.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7603.bundle.js` & `notebook-7.2.0rc1/notebook/static/7603.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,35 +3,35 @@
     [7603], {
         97603: (e, t, n) => {
             n.r(t), n.d(t, {
                 Commands: () => S,
                 default: () => R,
                 tabSpaceStatus: () => L
             });
-            var o = n(2922),
-                r = n(96049),
-                a = n(52839),
-                i = n(49269),
-                d = n(89144),
-                c = n(80106),
-                l = n(26862),
-                s = n(42751),
-                u = n(42703),
-                m = n(65651),
-                g = n(52138),
-                p = n(50845),
-                f = n(24554),
-                v = n(27829),
-                h = n(87017),
-                C = n(37267),
-                b = n(22620),
+            var o = n(44604),
+                r = n(53312),
+                a = n(51429),
+                i = n(30525),
+                d = n(81002),
+                c = n(67260),
+                l = n(95183),
+                s = n(71427),
+                u = n(34663),
+                m = n(86810),
+                g = n(61907),
+                p = n(29879),
+                f = n(23295),
+                v = n(71098),
+                h = n(79426),
+                C = n(12030),
+                b = n(35613),
                 y = n(33625),
                 w = n(87797),
                 _ = n(24636),
-                x = n(1167);
+                x = n(68722);
             const k = "notebook:toggle-autoclosing-brackets",
                 T = "console:toggle-autoclosing-brackets";
             var E;
             ! function(e) {
                 e.createNew = "fileeditor:create-new", e.createNewMarkdown = "fileeditor:create-new-markdown-file", e.changeFontSize = "fileeditor:change-font-size", e.lineNumbers = "fileeditor:toggle-line-numbers", e.currentLineNumbers = "fileeditor:toggle-current-line-numbers", e.lineWrap = "fileeditor:toggle-line-wrap", e.currentLineWrap = "fileeditor:toggle-current-line-wrap", e.changeTabs = "fileeditor:change-tabs", e.matchBrackets = "fileeditor:toggle-match-brackets", e.currentMatchBrackets = "fileeditor:toggle-current-match-brackets", e.autoClosingBrackets = "fileeditor:toggle-autoclosing-brackets", e.autoClosingBracketsUniversal = "fileeditor:toggle-autoclosing-brackets-universal", e.createConsole = "fileeditor:create-console", e.replaceSelection = "fileeditor:replace-selection", e.restartConsole = "fileeditor:restart-console", e.runCode = "fileeditor:run-code", e.runAllCode = "fileeditor:run-all", e.markdownPreview = "fileeditor:markdown-preview", e.undo = "fileeditor:undo", e.redo = "fileeditor:redo", e.cut = "fileeditor:cut", e.copy = "fileeditor:copy", e.paste = "fileeditor:paste", e.selectAll = "fileeditor:select-all", e.invokeCompleter = "completer:invoke-file", e.selectCompleter = "completer:select-file", e.openCodeViewer = "code-viewer:open", e.changeTheme = "fileeditor:change-theme", e.changeLanguage = "fileeditor:change-language", e.find = "fileeditor:find", e.goToLine = "fileeditor:go-to-line"
             }(E || (E = {}));
             const I = "Editor";
@@ -183,17 +183,18 @@
                     var C;
                     e.addCommand(E.changeFontSize, {
                         execute: e => {
                             var o;
                             const r = Number(e.delta);
                             if (Number.isNaN(r)) return void console.error(`${E.changeFontSize}: delta arg must be a number`);
                             const a = window.getComputedStyle(document.documentElement),
-                                i = parseInt(a.getPropertyValue("--jp-code-font-size"), 10),
-                                d = (null !== (o = t.customStyles.fontSize) && void 0 !== o ? o : g.baseConfiguration.customStyles.fontSize) || i;
-                            return t.fontSize = d + r, n.set(l, "editorConfig", t).catch((e => {
+                                i = parseInt(a.getPropertyValue("--jp-code-font-size"), 10);
+                            t.customStyles || (t.customStyles = {});
+                            const d = (null !== (o = t.customStyles.fontSize) && void 0 !== o ? o : g.baseConfiguration.customStyles.fontSize) || i;
+                            return t.customStyles.fontSize = d + r, n.set(l, "editorConfig", t).catch((e => {
                                 console.error(`Failed to set ${l}: ${e.message}`)
                             }))
                         },
                         label: e => {
                             const t = Number(e.delta);
                             return Number.isNaN(t) && console.error(`${E.changeFontSize}: delta arg must be a number`), t > 0 ? e.isMenu ? o.__("Increase Text Editor Font Size") : o.__("Increase Font Size") : e.isMenu ? o.__("Decrease Text Editor Font Size") : o.__("Decrease Font Size")
                         }
```

### Comparing `notebook-7.2.0rc0/notebook/static/7639.bundle.js` & `notebook-7.2.0rc1/notebook/static/7639.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -35,15 +35,15 @@
                     }
                 }, e) : i.createElement("div", {
                     style: {
                         margin: `0px ${t}px`
                     }
                 }, e))))
             }
-            var n = s(22620),
+            var n = s(35613),
                 o = s(63485);
 
             function d(e) {
                 const t = new h(e);
                 return e.startHidden || t.launch(), t
             }
             class h extends o.Widget {
```

### Comparing `notebook-7.2.0rc0/notebook/static/7655.bundle.js` & `notebook-7.2.0rc1/notebook/static/7655.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,18 +2,18 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [7655], {
         97655: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => S,
                 lineColItem: () => w
             });
-            var r, n = o(2922),
-                i = o(52839),
-                a = o(27829),
-                s = o(37267),
+            var r, n = o(44604),
+                i = o(51429),
+                a = o(71098),
+                s = o(12030),
                 d = o(87797),
                 l = o(24636);
             ! function(e) {
                 e.deleteLine = "codemirror:delete-line", e.toggleBlockComment = "codemirror:toggle-block-comment", e.toggleComment = "codemirror:toggle-comment", e.selectNextOccurrence = "codemirror:select-next-occurrence"
             }(r || (r = {}));
             const c = ".cm-content",
                 m = {
@@ -59,17 +59,17 @@
                                 e && (0, l.selectNextOccurrence)(e)
                             },
                             isEnabled: a
                         })
                     }
                 };
             var u = o(17592),
-                g = o(49269),
-                p = o(24554),
-                h = o(22620),
+                g = o(30525),
+                p = o(23295),
+                h = o(35613),
                 v = o(20998),
                 y = o(27478),
                 f = o.n(y),
                 E = o(78156),
                 x = o.n(E);
             const b = "@jupyterlab/codemirror-extension:plugin",
                 C = {
```

### Comparing `notebook-7.2.0rc0/notebook/static/7674.bundle.js` & `notebook-7.2.0rc1/notebook/static/7674.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7679.bundle.js` & `notebook-7.2.0rc1/notebook/static/7679.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7684.bundle.js` & `notebook-7.2.0rc1/notebook/static/6893.bundle.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [7684, 6893], {
+    [6893, 7684], {
         56893: (t, e, o) => {
             o.r(e), o.d(e, {
                 CommandIDs: () => n,
                 default: () => i
             });
-            var n, a = o(2922),
-                r = o(96049),
-                s = o(1167),
-                u = o(37267);
+            var n, a = o(44604),
+                r = o(53312),
+                s = o(68722),
+                u = o(12030);
             ! function(t) {
                 t.controlPanel = "hub:control-panel", t.logout = "hub:logout", t.restart = "hub:restart"
             }(n || (n = {}));
             const i = [{
                 activate: function(t, e, o, a) {
                     const r = o.load("jupyterlab"),
                         u = e.urls.hubHost || "",
```

### Comparing `notebook-7.2.0rc0/notebook/static/7796.bundle.js` & `notebook-7.2.0rc1/notebook/static/7796.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7803.bundle.js` & `notebook-7.2.0rc1/notebook/static/7803.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7811.bundle.js` & `notebook-7.2.0rc1/notebook/static/7811.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7812.bundle.js` & `notebook-7.2.0rc1/notebook/static/7812.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
                 IMarkdownViewerTracker: () => a,
                 MarkdownDocument: () => w,
                 MarkdownViewer: () => f,
                 MarkdownViewerFactory: () => _,
                 MarkdownViewerTableOfContentsFactory: () => s,
                 MarkdownViewerTableOfContentsModel: () => i
             });
-            var r = n(87017);
+            var r = n(79426);
             class i extends r.TableOfContentsModel {
                 constructor(e, t, n) {
                     super(e, n), this.parser = t
                 }
                 get documentType() {
                     return "markdown-viewer"
                 }
@@ -66,19 +66,19 @@
                             e.content.rendered.disconnect(a), n.activeHeadingChanged.disconnect(o), n.headingsChanged.disconnect(a)
                         }))
                     })), n
                 }
             }
             var o = n(20998);
             const a = new o.Token("@jupyterlab/markdownviewer:IMarkdownViewerTracker", "A widget tracker for markdown\n  document viewers. Use this if you want to iterate over and interact with rendered markdown documents.");
-            var d = n(96049),
-                c = n(1167),
-                l = n(10979),
-                h = n(13408),
-                u = n(37267),
+            var d = n(53312),
+                c = n(68722),
+                l = n(65903),
+                h = n(81221),
+                u = n(12030),
                 g = n(81997),
                 m = n(63485);
             const p = "text/markdown";
             class f extends m.Widget {
                 constructor(e) {
                     super(), this._config = {
                         ...f.defaultConfig
```

### Comparing `notebook-7.2.0rc0/notebook/static/7817.bundle.js` & `notebook-7.2.0rc1/notebook/static/7817.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7819.bundle.js` & `notebook-7.2.0rc1/notebook/static/7819.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -164,18 +164,18 @@
                 npgettext(t, e, r, n, ...s) {
                     return this.ngettext(e, r, n, ...s)
                 }
                 dcnpgettext(t, e, r, n, s, ...a) {
                     return this.ngettext(r, n, s, ...a)
                 }
             });
-            var l = r(96692),
+            var l = r(41053),
                 o = r(20998),
-                u = r(1167),
-                c = r(70611);
+                u = r(68722),
+                c = r(87408);
             const h = "api/translations";
             async function _(t = "", e = "", r = {}, n = void 0) {
                 const s = null != n ? n : c.ServerConnection.makeSettings();
                 t = t || `${s.appUrl}/${h}`;
                 const a = u.URLExt.join(s.baseUrl, t),
                     i = u.URLExt.join(a, e);
                 if (!i.startsWith(a)) throw new Error("Can only be used for translations requests");
```

### Comparing `notebook-7.2.0rc0/notebook/static/7821.bundle.js` & `notebook-7.2.0rc1/notebook/static/7821.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7854.bundle.js` & `notebook-7.2.0rc1/notebook/static/7854.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,22 +2,22 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [7854], {
         97854: (e, n, t) => {
             t.r(n), t.d(n, {
                 CommandIDs: () => b,
                 default: () => k
             });
-            var s = t(2922),
-                o = t(96049),
-                i = t(15729),
-                a = t(91942),
-                r = t(96692),
-                l = t(37267),
-                c = t(22620),
-                d = t(1167),
+            var s = t(44604),
+                o = t(53312),
+                i = t(9235),
+                a = t(5094),
+                r = t(41053),
+                l = t(12030),
+                c = t(35613),
+                d = t(68722),
                 u = t(97934),
                 h = t(81997),
                 g = t(78156),
                 m = t.n(g);
             const p = "jp-mod-kernel";
             var _;
             ! function(e) {
@@ -107,15 +107,15 @@
                     }
                     get _summary() {
                         const e = this.children;
                         return 0 === e.length ? this.trans.__("No sessions connected") : 1 == e.length ? e[0].label() : this.trans.__("%1 and %2 more", e[0].label(), e.length - 1)
                     }
                 }, e.runningChanged = new h.Signal({})
             }(_ || (_ = {}));
-            var b, w = t(10979);
+            var b, w = t(65903);
             class f {
                 constructor(e) {
                     this._tabsChanged = new h.Signal(this), this._widgets = [], this._labShell = e, this._labShell.layoutModified.connect(this._emitTabsChanged, this)
                 }
                 get tabsChanged() {
                     return this._tabsChanged
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/7866.bundle.js` & `notebook-7.2.0rc1/notebook/static/7866.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7884.bundle.js` & `notebook-7.2.0rc1/notebook/static/7884.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7900.bundle.js` & `notebook-7.2.0rc1/notebook/static/8928.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [7900, 8928], {
+    [8928, 7900], {
         67900: (t, e, i) => {
             i.r(e), i.d(e, {
                 IImageTracker: () => r,
                 ImageViewer: () => l,
                 ImageViewerFactory: () => d
             });
             var s = i(20998);
             const r = new s.Token("@jupyterlab/imageviewer:IImageTracker", "A widget tracker for images.\n  Use this if you want to be able to iterate over and interact with images\n  viewed by the application.");
-            var a, o = i(1167),
-                n = i(96049),
-                c = i(10979),
+            var a, o = i(68722),
+                n = i(53312),
+                c = i(65903),
                 h = i(63485);
             class l extends h.Widget {
                 constructor(t) {
                     super(), this._scale = 1, this._matrix = [1, 0, 0, 1], this._colorinversion = 0, this._ready = new s.PromiseDelegate, this.context = t, this.node.tabIndex = 0, this.addClass("jp-ImageViewer"), this._img = document.createElement("img"), this.node.appendChild(this._img), this._onTitleChanged(), t.pathChanged.connect(this._onTitleChanged, this), t.ready.then((() => {
                         if (this.isDisposed) return;
                         const e = t.contentsModel;
                         this._mimeType = e.mimetype, this._render(), t.model.contentChanged.connect(this.update, this), t.fileChanged.connect(this.update, this), this._ready.resolve(void 0)
```

### Comparing `notebook-7.2.0rc0/notebook/static/7906.bundle.js` & `notebook-7.2.0rc1/notebook/static/7906.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [7906, 4382], {
         54382: (e, t, r) => {
             r.r(t), r.d(t, {
                 default: () => a
             });
-            var n = r(26862),
-                o = r(46807);
+            var n = r(95183),
+                o = r(59625);
             const c = "jp-mod-searchable",
                 a = [{
                     id: "@jupyter-notebook/documentsearch-extension:notebookShellWidgetListener",
                     requires: [o.INotebookShell, n.ISearchProviderRegistry],
                     autoStart: !0,
                     description: "A plugin to add document search functionalities",
                     activate: (e, t, r) => {
```

### Comparing `notebook-7.2.0rc0/notebook/static/792.bundle.js` & `notebook-7.2.0rc1/notebook/static/792.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7957.bundle.js` & `notebook-7.2.0rc1/notebook/static/7957.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7969.bundle.js` & `notebook-7.2.0rc1/notebook/static/7969.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7995.bundle.js` & `notebook-7.2.0rc1/notebook/static/7995.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/7997.bundle.js` & `notebook-7.2.0rc1/notebook/static/7997.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/79d088064beb3826054f.eot` & `notebook-7.2.0rc1/notebook/static/79d088064beb3826054f.eot`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8010.bundle.js` & `notebook-7.2.0rc1/notebook/static/8010.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8032.bundle.js` & `notebook-7.2.0rc1/notebook/static/8032.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8285.bundle.js` & `notebook-7.2.0rc1/notebook/static/8285.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8378.bundle.js` & `notebook-7.2.0rc1/notebook/static/8378.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8381.bundle.js` & `notebook-7.2.0rc1/notebook/static/8381.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8433.bundle.js` & `notebook-7.2.0rc1/notebook/static/8433.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8443.bundle.js` & `notebook-7.2.0rc1/notebook/static/8443.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8446.bundle.js` & `notebook-7.2.0rc1/notebook/static/8446.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8471.bundle.js` & `notebook-7.2.0rc1/notebook/static/8471.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,28 +6,28 @@
                 ToolbarItems: () => E,
                 default: () => T,
                 downloadPlugin: () => W,
                 openBrowserTabPlugin: () => F,
                 pathStatusPlugin: () => I,
                 savingStatusPlugin: () => S
             });
-            var o, a, r = n(2922),
-                i = n(96049),
-                l = n(1167),
-                d = n(91942),
-                s = n(24554),
-                c = n(27829),
-                u = n(37267),
-                m = n(22620),
+            var o, a, r = n(44604),
+                i = n(53312),
+                l = n(68722),
+                d = n(5094),
+                s = n(23295),
+                c = n(71098),
+                u = n(12030),
+                m = n(35613),
                 g = n(33625),
                 p = n(20998),
                 h = n(81997),
                 v = n(63485),
                 f = n(78156),
-                w = n(96692);
+                w = n(41053);
             ! function(e) {
                 e.clearRecents = "docmanager:clear-recents"
             }(o || (o = {})),
             function(e) {
                 e.recentsManager = "@jupyterlab/docmanager-extension:recents", e.reopenClosed = "@jupyterlab/docmanager-extension:reopen-recently-closed", e.mainPlugin = "@jupyterlab/docmanager-extension:plugin"
             }(a || (a = {}));
             const _ = {
```

### Comparing `notebook-7.2.0rc0/notebook/static/8479.bundle.js` & `notebook-7.2.0rc1/notebook/static/8479.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/85.bundle.js` & `notebook-7.2.0rc1/notebook/static/85.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8579.bundle.js` & `notebook-7.2.0rc1/notebook/static/8579.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [8579], {
         88579: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => q
             });
-            var n = o(2922),
-                a = o(96049),
-                i = o(80106),
-                r = o(1167),
-                d = o(91942),
-                l = o(10979),
-                s = o(50845),
-                c = o(13408),
-                p = o(24554),
-                u = o(37267),
-                g = o(46807),
-                m = o(18625),
+            var n = o(44604),
+                a = o(53312),
+                i = o(67260),
+                r = o(68722),
+                d = o(5094),
+                l = o(65903),
+                s = o(29879),
+                c = o(81221),
+                p = o(23295),
+                u = o(12030),
+                g = o(59625),
+                m = o(93712),
                 h = o(20998),
                 b = o(2549),
                 f = o(63485);
             const v = new RegExp("/(notebooks|edit)/(.*)"),
                 y = /\.ipynb$/;
             var k;
             ! function(e) {
```

### Comparing `notebook-7.2.0rc0/notebook/static/8633.bundle.js` & `notebook-7.2.0rc1/notebook/static/8633.bundle.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [8633], {
         98633: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => y
             });
-            var i, r = n(2922),
-                a = n(96049),
-                o = n(52839),
-                d = n(22620),
-                s = n(13408),
+            var i, r = n(44604),
+                a = n(53312),
+                o = n(51429),
+                d = n(35613),
+                s = n(81221),
                 c = n(24758),
-                l = n(57355),
-                g = n(24554),
-                u = n(96692),
-                p = n(37267);
+                l = n(9033),
+                g = n(23295),
+                u = n(41053),
+                p = n(12030);
             ! function(e) {
                 e.open = "settingeditor:open", e.openJSON = "settingeditor:open-json", e.revert = "settingeditor:revert", e.save = "settingeditor:save"
             }(i || (i = {}));
             const m = {
                     id: "@jupyterlab/settingeditor-extension:form-ui",
                     description: "Adds the interactive settings editor and provides its tracker.",
                     requires: [g.ISettingRegistry, u.IStateDB, p.ITranslator, d.IFormRendererRegistry, r.ILabStatus],
@@ -49,15 +49,15 @@
                                     "json" === l.get("settingEditorType").composite ? y.execute(i.openJSON) : (async e => {
                                         if (I.currentWidget && !I.currentWidget.isDisposed) return I.currentWidget.isAttached || S.add(I.currentWidget, "main", {
                                             type: "Settings"
                                         }), void S.activateById(I.currentWidget.id);
                                         const l = m.id,
                                             {
                                                 SettingsEditor: g
-                                            } = await n.e(1131).then(n.t.bind(n, 1131, 23)),
+                                            } = await n.e(4258).then(n.t.bind(n, 74258, 23)),
                                             h = new a.MainAreaWidget({
                                                 content: new g({
                                                     editorRegistry: s,
                                                     key: l,
                                                     registry: t,
                                                     state: r,
                                                     commands: y,
@@ -123,15 +123,15 @@
                                 if (I.currentWidget && !I.currentWidget.isDisposed) return I.currentWidget.isAttached || y.add(I.currentWidget, "main", {
                                     type: "Advanced Settings"
                                 }), void y.activateById(I.currentWidget.id);
                                 const r = m.id,
                                     g = e.restored,
                                     {
                                         JsonSettingEditor: u
-                                    } = await n.e(1131).then(n.t.bind(n, 1131, 23)),
+                                    } = await n.e(4258).then(n.t.bind(n, 74258, 23)),
                                     h = new u({
                                         commands: {
                                             registry: v,
                                             revert: i.revert,
                                             save: i.save
                                         },
                                         editorFactory: b,
```

### Comparing `notebook-7.2.0rc0/notebook/static/870673df72e70f87c91a.woff` & `notebook-7.2.0rc1/notebook/static/870673df72e70f87c91a.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8768.bundle.js` & `notebook-7.2.0rc1/notebook/static/8768.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8771.bundle.js` & `notebook-7.2.0rc1/notebook/static/8771.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,17 +4,17 @@
         68771: (e, t, n) => {
             n.r(t), n.d(t, {
                 ILauncher: () => a,
                 Launcher: () => p,
                 LauncherModel: () => u
             });
             const a = new(n(20998).Token)("@jupyterlab/launcher:ILauncher", "A service for the application activity launcher.\n  Use this to add your extension activities to the launcher panel.");
-            var s, r = n(96049),
-                c = n(37267),
-                o = n(22620),
+            var s, r = n(53312),
+                c = n(12030),
+                o = n(35613),
                 i = n(33625),
                 l = n(2549),
                 d = n(14421),
                 h = n(63485),
                 m = n(78156);
             class u extends o.VDomModel {
                 constructor() {
```

### Comparing `notebook-7.2.0rc0/notebook/static/8781.bundle.js` & `notebook-7.2.0rc1/notebook/static/8781.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,76 +1,76 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [8781], {
         67417: () => {},
         60880: (e, n, t) => {
             "use strict";
             t.r(n);
-            var o = t(1167);
+            var o = t(68722);
             async function a(e, n) {
                 try {
                     const t = (await window._JUPYTERLAB[e].get(n))();
                     return t.__scope__ = e, t
                 } catch (t) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${n}`), t
                 }
             }
             t(72761), t(67417), window.addEventListener("load", (async function() {
-                const e = [t(32374), t(18403), t(65028), t(70545)],
+                const e = [t(46037), t(87360), t(27854), t(92783)],
                     n = await Promise.all(e);
-                let r = [t(29272), t(99223), t(83421), t(25622), t(88378), t(66889), t(77429), t(95496).default.filter((({
+                let r = [t(9828), t(61092), t(74695), t(78390), t(90748), t(43200), t(28574), t(61072).default.filter((({
                     id: e
-                }) => ["@jupyterlab/application-extension:commands", "@jupyterlab/application-extension:context-menu", "@jupyterlab/application-extension:faviconbusy", "@jupyterlab/application-extension:router", "@jupyterlab/application-extension:top-bar", "@jupyterlab/application-extension:top-spacer"].includes(e))), t(61182).default.filter((({
+                }) => ["@jupyterlab/application-extension:commands", "@jupyterlab/application-extension:context-menu", "@jupyterlab/application-extension:faviconbusy", "@jupyterlab/application-extension:router", "@jupyterlab/application-extension:top-bar", "@jupyterlab/application-extension:top-spacer"].includes(e))), t(47494).default.filter((({
                     id: e
-                }) => ["@jupyterlab/apputils-extension:palette", "@jupyterlab/apputils-extension:notification", "@jupyterlab/apputils-extension:sanitizer", "@jupyterlab/apputils-extension:sessionDialogs", "@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:state", "@jupyterlab/apputils-extension:themes", "@jupyterlab/apputils-extension:themes-palette-menu", "@jupyterlab/apputils-extension:toolbar-registry", "@jupyterlab/apputils-extension:utilityCommands"].includes(e))), t(56823), t(5890).default.filter((({
+                }) => ["@jupyterlab/apputils-extension:palette", "@jupyterlab/apputils-extension:notification", "@jupyterlab/apputils-extension:sanitizer", "@jupyterlab/apputils-extension:sessionDialogs", "@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:state", "@jupyterlab/apputils-extension:themes", "@jupyterlab/apputils-extension:themes-palette-menu", "@jupyterlab/apputils-extension:toolbar-registry", "@jupyterlab/apputils-extension:utilityCommands"].includes(e))), t(60323), t(78917).default.filter((({
                     id: e
-                }) => ["@jupyterlab/completer-extension:base-service", "@jupyterlab/completer-extension:inline-completer", "@jupyterlab/completer-extension:inline-completer-factory", "@jupyterlab/completer-extension:inline-history", "@jupyterlab/completer-extension:manager"].includes(e))), t(28654).default.filter((({
+                }) => ["@jupyterlab/completer-extension:base-service", "@jupyterlab/completer-extension:inline-completer", "@jupyterlab/completer-extension:inline-completer-factory", "@jupyterlab/completer-extension:inline-history", "@jupyterlab/completer-extension:manager"].includes(e))), t(77089).default.filter((({
                     id: e
-                }) => ["@jupyterlab/console-extension:cell-executor", "@jupyterlab/console-extension:completer", "@jupyterlab/console-extension:factory", "@jupyterlab/console-extension:foreign", "@jupyterlab/console-extension:tracker"].includes(e))), t(61378), t(18602).default.filter((({
+                }) => ["@jupyterlab/console-extension:cell-executor", "@jupyterlab/console-extension:completer", "@jupyterlab/console-extension:factory", "@jupyterlab/console-extension:foreign", "@jupyterlab/console-extension:tracker"].includes(e))), t(20671), t(97708).default.filter((({
                     id: e
-                }) => ["@jupyterlab/docmanager-extension:plugin", "@jupyterlab/docmanager-extension:download", "@jupyterlab/docmanager-extension:contexts", "@jupyterlab/docmanager-extension:manager"].includes(e))), t(24124).default.filter((({
+                }) => ["@jupyterlab/docmanager-extension:plugin", "@jupyterlab/docmanager-extension:download", "@jupyterlab/docmanager-extension:contexts", "@jupyterlab/docmanager-extension:manager"].includes(e))), t(94414).default.filter((({
                     id: e
-                }) => ["@jupyterlab/documentsearch-extension:plugin"].includes(e))), t(57782).default.filter((({
+                }) => ["@jupyterlab/documentsearch-extension:plugin"].includes(e))), t(34409).default.filter((({
                     id: e
-                }) => ["@jupyterlab/filebrowser-extension:factory", "@jupyterlab/filebrowser-extension:default-file-browser"].includes(e))), t(63728).default.filter((({
+                }) => ["@jupyterlab/filebrowser-extension:factory", "@jupyterlab/filebrowser-extension:default-file-browser"].includes(e))), t(43258).default.filter((({
                     id: e
-                }) => ["@jupyterlab/fileeditor-extension:plugin"].includes(e))), t(70952).default.filter((({
+                }) => ["@jupyterlab/fileeditor-extension:plugin"].includes(e))), t(74516).default.filter((({
                     id: e
-                }) => ["@jupyterlab/help-extension:resources"].includes(e))), t(9269), t(94388), t(44250), t(39137).default.filter((({
+                }) => ["@jupyterlab/help-extension:resources"].includes(e))), t(89770), t(90388), t(77659), t(53440).default.filter((({
                     id: e
-                }) => ["@jupyterlab/mainmenu-extension:plugin"].includes(e))), t(8467), t(17420), t(56727), t(78578).default.filter((({
+                }) => ["@jupyterlab/mainmenu-extension:plugin"].includes(e))), t(41145), t(40364), t(75347), t(79680).default.filter((({
                     id: e
-                }) => ["@jupyterlab/notebook-extension:cell-executor", "@jupyterlab/notebook-extension:code-console", "@jupyterlab/notebook-extension:export", "@jupyterlab/notebook-extension:factory", "@jupyterlab/notebook-extension:tracker", "@jupyterlab/notebook-extension:widget-factory"].includes(e))), t(46456), t(53160), t(90856), t(99526), t(92396), t(68449), t(252), t(74572), t(31716)];
+                }) => ["@jupyterlab/notebook-extension:cell-executor", "@jupyterlab/notebook-extension:code-console", "@jupyterlab/notebook-extension:export", "@jupyterlab/notebook-extension:factory", "@jupyterlab/notebook-extension:tracker", "@jupyterlab/notebook-extension:widget-factory"].includes(e))), t(22413), t(57926), t(96291), t(1262), t(84228), t(97818), t(78608), t(53929), t(20531)];
                 switch (`/${o.PageConfig.getOption("notebookPage")}`) {
                     case "/tree":
-                        r = r.concat([t(48618), t(57782).default.filter((({
+                        r = r.concat([t(36488), t(34409).default.filter((({
                             id: e
-                        }) => ["@jupyterlab/filebrowser-extension:browser", "@jupyterlab/filebrowser-extension:download", "@jupyterlab/filebrowser-extension:file-upload-status", "@jupyterlab/filebrowser-extension:open-with", "@jupyterlab/filebrowser-extension:search", "@jupyterlab/filebrowser-extension:share-file"].includes(e))), t(78085), t(76156).default.filter((({
+                        }) => ["@jupyterlab/filebrowser-extension:browser", "@jupyterlab/filebrowser-extension:download", "@jupyterlab/filebrowser-extension:file-upload-status", "@jupyterlab/filebrowser-extension:open-with", "@jupyterlab/filebrowser-extension:search", "@jupyterlab/filebrowser-extension:share-file"].includes(e))), t(74733), t(27993).default.filter((({
                             id: e
-                        }) => ["@jupyterlab/running-extension:plugin"].includes(e))), t(39519)]);
+                        }) => ["@jupyterlab/running-extension:plugin"].includes(e))), t(86652)]);
                         break;
                     case "/notebooks":
-                        r = r.concat([t(18173), t(13375), t(40682).default.filter((({
+                        r = r.concat([t(54669), t(78007), t(98128).default.filter((({
                             id: e
-                        }) => ["@jupyterlab/debugger-extension:config", "@jupyterlab/debugger-extension:main", "@jupyterlab/debugger-extension:notebooks", "@jupyterlab/debugger-extension:service", "@jupyterlab/debugger-extension:sidebar", "@jupyterlab/debugger-extension:sources"].includes(e))), t(82818), t(78578).default.filter((({
+                        }) => ["@jupyterlab/debugger-extension:config", "@jupyterlab/debugger-extension:main", "@jupyterlab/debugger-extension:notebooks", "@jupyterlab/debugger-extension:service", "@jupyterlab/debugger-extension:sidebar", "@jupyterlab/debugger-extension:sources"].includes(e))), t(1598), t(79680).default.filter((({
                             id: e
-                        }) => ["@jupyterlab/notebook-extension:active-cell-tool", "@jupyterlab/notebook-extension:completer", "@jupyterlab/notebook-extension:metadata-editor", "@jupyterlab/notebook-extension:search", "@jupyterlab/notebook-extension:toc", "@jupyterlab/notebook-extension:tools", "@jupyterlab/notebook-extension:update-raw-mimetype"].includes(e))), t(65477).default.filter((({
+                        }) => ["@jupyterlab/notebook-extension:active-cell-tool", "@jupyterlab/notebook-extension:completer", "@jupyterlab/notebook-extension:copy-output", "@jupyterlab/notebook-extension:metadata-editor", "@jupyterlab/notebook-extension:search", "@jupyterlab/notebook-extension:toc", "@jupyterlab/notebook-extension:tools", "@jupyterlab/notebook-extension:update-raw-mimetype"].includes(e))), t(77619).default.filter((({
                             id: e
-                        }) => ["@jupyterlab/toc-extension:registry", "@jupyterlab/toc-extension:tracker"].includes(e))), t(65787).default.filter((({
+                        }) => ["@jupyterlab/toc-extension:registry", "@jupyterlab/toc-extension:tracker"].includes(e))), t(33e3).default.filter((({
                             id: e
                         }) => ["@jupyterlab/tooltip-extension:manager", "@jupyterlab/tooltip-extension:notebooks"].includes(e)))]);
                         break;
                     case "/consoles":
-                        r = r.concat([t(65787).default.filter((({
+                        r = r.concat([t(33e3).default.filter((({
                             id: e
                         }) => ["@jupyterlab/tooltip-extension:manager", "@jupyterlab/tooltip-extension:consoles"].includes(e)))]);
                         break;
                     case "/edit":
-                        r = r.concat([t(63728).default.filter((({
+                        r = r.concat([t(43258).default.filter((({
                             id: e
-                        }) => ["@jupyterlab/fileeditor-extension:completer", "@jupyterlab/fileeditor-extension:search"].includes(e))), t(73898)])
+                        }) => ["@jupyterlab/fileeditor-extension:completer", "@jupyterlab/fileeditor-extension:search"].includes(e))), t(66299)])
                 }
                 const i = [],
                     l = [];
 
                 function* s(e) {
                     let n;
                     n = Object.prototype.hasOwnProperty.call(e, "__esModule") ? e.default : e;
@@ -86,16 +86,16 @@
                             autoStart: n.autoStart,
                             enabled: !t,
                             extension: e.__scope__
                         }), t ? i.push(n.id) : yield n
                     }
                 }
                 const p = JSON.parse(o.PageConfig.getOption("federated_extensions")),
-                    b = [],
                     u = [],
+                    b = [],
                     d = [],
                     c = [];
                 (await Promise.allSettled(p.map((async e => (await async function(e, n) {
                     await
                     function(e) {
                         return new Promise(((n, t) => {
                             const o = document.createElement("script");
@@ -103,90 +103,90 @@
                         }))
                     }(e), await t.I("default");
                     const o = window._JUPYTERLAB[n];
                     await o.init(t.S.default)
                 }(`${o.URLExt.join(o.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))))).forEach((e => {
                     if ("rejected" === e.status) return void console.error(e.reason);
                     const n = e.value;
-                    n.extension && u.push(a(n.name, n.extension)), n.mimeExtension && d.push(a(n.name, n.mimeExtension)), n.style && !o.PageConfig.Extension.isDisabled(n.name) && c.push(a(n.name, n.style))
+                    n.extension && b.push(a(n.name, n.extension)), n.mimeExtension && d.push(a(n.name, n.mimeExtension)), n.style && !o.PageConfig.Extension.isDisabled(n.name) && c.push(a(n.name, n.style))
                 })), (await Promise.all(r)).forEach((e => {
-                    for (let n of s(e)) b.push(n)
-                })), (await Promise.allSettled(u)).forEach((e => {
+                    for (let n of s(e)) u.push(n)
+                })), (await Promise.allSettled(b)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (let n of s(e.value)) b.push(n);
+                        for (let n of s(e.value)) u.push(n);
                     else console.error(e.reason)
                 })), (await Promise.allSettled(d)).forEach((e => {
                     if ("fulfilled" === e.status)
                         for (let t of s(e.value)) n.push(t);
                     else console.error(e.reason)
                 })), (await Promise.allSettled(c)).filter((({
                     status: e
                 }) => "rejected" === e)).forEach((({
                     reason: e
                 }) => {
                     console.error(e)
-                })), o.PageConfig.setOption("allPlugins", '{"/":{"@jupyter-notebook/application-extension":true,"@jupyter-notebook/console-extension":true,"@jupyter-notebook/docmanager-extension":true,"@jupyter-notebook/documentsearch-extension":true,"@jupyter-notebook/help-extension":true,"@jupyter-notebook/notebook-extension":true,"@jupyter-notebook/terminal-extension":true,"@jupyterlab/application-extension":["@jupyterlab/application-extension:commands","@jupyterlab/application-extension:context-menu","@jupyterlab/application-extension:faviconbusy","@jupyterlab/application-extension:router","@jupyterlab/application-extension:top-bar","@jupyterlab/application-extension:top-spacer"],"@jupyterlab/apputils-extension":["@jupyterlab/apputils-extension:palette","@jupyterlab/apputils-extension:notification","@jupyterlab/apputils-extension:sanitizer","@jupyterlab/apputils-extension:sessionDialogs","@jupyterlab/apputils-extension:settings","@jupyterlab/apputils-extension:state","@jupyterlab/apputils-extension:themes","@jupyterlab/apputils-extension:themes-palette-menu","@jupyterlab/apputils-extension:toolbar-registry","@jupyterlab/apputils-extension:utilityCommands"],"@jupyterlab/codemirror-extension":true,"@jupyterlab/completer-extension":["@jupyterlab/completer-extension:base-service","@jupyterlab/completer-extension:inline-completer","@jupyterlab/completer-extension:inline-completer-factory","@jupyterlab/completer-extension:inline-history","@jupyterlab/completer-extension:manager"],"@jupyterlab/console-extension":["@jupyterlab/console-extension:cell-executor","@jupyterlab/console-extension:completer","@jupyterlab/console-extension:factory","@jupyterlab/console-extension:foreign","@jupyterlab/console-extension:tracker"],"@jupyterlab/csvviewer-extension":true,"@jupyterlab/docmanager-extension":["@jupyterlab/docmanager-extension:plugin","@jupyterlab/docmanager-extension:download","@jupyterlab/docmanager-extension:contexts","@jupyterlab/docmanager-extension:manager"],"@jupyterlab/documentsearch-extension":["@jupyterlab/documentsearch-extension:plugin"],"@jupyterlab/filebrowser-extension":["@jupyterlab/filebrowser-extension:factory","@jupyterlab/filebrowser-extension:default-file-browser"],"@jupyterlab/fileeditor-extension":["@jupyterlab/fileeditor-extension:plugin"],"@jupyterlab/help-extension":["@jupyterlab/help-extension:resources"],"@jupyterlab/htmlviewer-extension":true,"@jupyterlab/imageviewer-extension":true,"@jupyterlab/lsp-extension":true,"@jupyterlab/mainmenu-extension":["@jupyterlab/mainmenu-extension:plugin"],"@jupyterlab/markedparser-extension":true,"@jupyterlab/mathjax-extension":true,"@jupyterlab/mermaid-extension":true,"@jupyterlab/notebook-extension":["@jupyterlab/notebook-extension:cell-executor","@jupyterlab/notebook-extension:code-console","@jupyterlab/notebook-extension:export","@jupyterlab/notebook-extension:factory","@jupyterlab/notebook-extension:tracker","@jupyterlab/notebook-extension:widget-factory"],"@jupyterlab/pluginmanager-extension":true,"@jupyterlab/shortcuts-extension":true,"@jupyterlab/terminal-extension":true,"@jupyterlab/theme-light-extension":true,"@jupyterlab/theme-dark-extension":true,"@jupyterlab/theme-dark-high-contrast-extension":true,"@jupyterlab/translation-extension":true,"@jupyterlab/ui-components-extension":true,"@jupyterlab/hub-extension":true},"/tree":{"@jupyterlab/extensionmanager-extension":true,"@jupyterlab/filebrowser-extension":["@jupyterlab/filebrowser-extension:browser","@jupyterlab/filebrowser-extension:download","@jupyterlab/filebrowser-extension:file-upload-status","@jupyterlab/filebrowser-extension:open-with","@jupyterlab/filebrowser-extension:search","@jupyterlab/filebrowser-extension:share-file"],"@jupyter-notebook/tree-extension":true,"@jupyterlab/running-extension":["@jupyterlab/running-extension:plugin"],"@jupyterlab/settingeditor-extension":true},"/notebooks":{"@jupyterlab/celltags-extension":true,"@jupyterlab/cell-toolbar-extension":true,"@jupyterlab/debugger-extension":["@jupyterlab/debugger-extension:config","@jupyterlab/debugger-extension:main","@jupyterlab/debugger-extension:notebooks","@jupyterlab/debugger-extension:service","@jupyterlab/debugger-extension:sidebar","@jupyterlab/debugger-extension:sources"],"@jupyterlab/metadataform-extension":true,"@jupyterlab/notebook-extension":["@jupyterlab/notebook-extension:active-cell-tool","@jupyterlab/notebook-extension:completer","@jupyterlab/notebook-extension:metadata-editor","@jupyterlab/notebook-extension:search","@jupyterlab/notebook-extension:toc","@jupyterlab/notebook-extension:tools","@jupyterlab/notebook-extension:update-raw-mimetype"],"@jupyterlab/toc-extension":["@jupyterlab/toc-extension:registry","@jupyterlab/toc-extension:tracker"],"@jupyterlab/tooltip-extension":["@jupyterlab/tooltip-extension:manager","@jupyterlab/tooltip-extension:notebooks"]},"/consoles":{"@jupyterlab/tooltip-extension":["@jupyterlab/tooltip-extension:manager","@jupyterlab/tooltip-extension:consoles"]},"/edit":{"@jupyterlab/fileeditor-extension":["@jupyterlab/fileeditor-extension:completer","@jupyterlab/fileeditor-extension:search"],"@jupyterlab/markdownviewer-extension":true}}');
-                const j = new(0, t(46807).NotebookApp)({
+                })), o.PageConfig.setOption("allPlugins", '{"/":{"@jupyter-notebook/application-extension":true,"@jupyter-notebook/console-extension":true,"@jupyter-notebook/docmanager-extension":true,"@jupyter-notebook/documentsearch-extension":true,"@jupyter-notebook/help-extension":true,"@jupyter-notebook/notebook-extension":true,"@jupyter-notebook/terminal-extension":true,"@jupyterlab/application-extension":["@jupyterlab/application-extension:commands","@jupyterlab/application-extension:context-menu","@jupyterlab/application-extension:faviconbusy","@jupyterlab/application-extension:router","@jupyterlab/application-extension:top-bar","@jupyterlab/application-extension:top-spacer"],"@jupyterlab/apputils-extension":["@jupyterlab/apputils-extension:palette","@jupyterlab/apputils-extension:notification","@jupyterlab/apputils-extension:sanitizer","@jupyterlab/apputils-extension:sessionDialogs","@jupyterlab/apputils-extension:settings","@jupyterlab/apputils-extension:state","@jupyterlab/apputils-extension:themes","@jupyterlab/apputils-extension:themes-palette-menu","@jupyterlab/apputils-extension:toolbar-registry","@jupyterlab/apputils-extension:utilityCommands"],"@jupyterlab/codemirror-extension":true,"@jupyterlab/completer-extension":["@jupyterlab/completer-extension:base-service","@jupyterlab/completer-extension:inline-completer","@jupyterlab/completer-extension:inline-completer-factory","@jupyterlab/completer-extension:inline-history","@jupyterlab/completer-extension:manager"],"@jupyterlab/console-extension":["@jupyterlab/console-extension:cell-executor","@jupyterlab/console-extension:completer","@jupyterlab/console-extension:factory","@jupyterlab/console-extension:foreign","@jupyterlab/console-extension:tracker"],"@jupyterlab/csvviewer-extension":true,"@jupyterlab/docmanager-extension":["@jupyterlab/docmanager-extension:plugin","@jupyterlab/docmanager-extension:download","@jupyterlab/docmanager-extension:contexts","@jupyterlab/docmanager-extension:manager"],"@jupyterlab/documentsearch-extension":["@jupyterlab/documentsearch-extension:plugin"],"@jupyterlab/filebrowser-extension":["@jupyterlab/filebrowser-extension:factory","@jupyterlab/filebrowser-extension:default-file-browser"],"@jupyterlab/fileeditor-extension":["@jupyterlab/fileeditor-extension:plugin"],"@jupyterlab/help-extension":["@jupyterlab/help-extension:resources"],"@jupyterlab/htmlviewer-extension":true,"@jupyterlab/imageviewer-extension":true,"@jupyterlab/lsp-extension":true,"@jupyterlab/mainmenu-extension":["@jupyterlab/mainmenu-extension:plugin"],"@jupyterlab/markedparser-extension":true,"@jupyterlab/mathjax-extension":true,"@jupyterlab/mermaid-extension":true,"@jupyterlab/notebook-extension":["@jupyterlab/notebook-extension:cell-executor","@jupyterlab/notebook-extension:code-console","@jupyterlab/notebook-extension:export","@jupyterlab/notebook-extension:factory","@jupyterlab/notebook-extension:tracker","@jupyterlab/notebook-extension:widget-factory"],"@jupyterlab/pluginmanager-extension":true,"@jupyterlab/shortcuts-extension":true,"@jupyterlab/terminal-extension":true,"@jupyterlab/theme-light-extension":true,"@jupyterlab/theme-dark-extension":true,"@jupyterlab/theme-dark-high-contrast-extension":true,"@jupyterlab/translation-extension":true,"@jupyterlab/ui-components-extension":true,"@jupyterlab/hub-extension":true},"/tree":{"@jupyterlab/extensionmanager-extension":true,"@jupyterlab/filebrowser-extension":["@jupyterlab/filebrowser-extension:browser","@jupyterlab/filebrowser-extension:download","@jupyterlab/filebrowser-extension:file-upload-status","@jupyterlab/filebrowser-extension:open-with","@jupyterlab/filebrowser-extension:search","@jupyterlab/filebrowser-extension:share-file"],"@jupyter-notebook/tree-extension":true,"@jupyterlab/running-extension":["@jupyterlab/running-extension:plugin"],"@jupyterlab/settingeditor-extension":true},"/notebooks":{"@jupyterlab/celltags-extension":true,"@jupyterlab/cell-toolbar-extension":true,"@jupyterlab/debugger-extension":["@jupyterlab/debugger-extension:config","@jupyterlab/debugger-extension:main","@jupyterlab/debugger-extension:notebooks","@jupyterlab/debugger-extension:service","@jupyterlab/debugger-extension:sidebar","@jupyterlab/debugger-extension:sources"],"@jupyterlab/metadataform-extension":true,"@jupyterlab/notebook-extension":["@jupyterlab/notebook-extension:active-cell-tool","@jupyterlab/notebook-extension:completer","@jupyterlab/notebook-extension:copy-output","@jupyterlab/notebook-extension:metadata-editor","@jupyterlab/notebook-extension:search","@jupyterlab/notebook-extension:toc","@jupyterlab/notebook-extension:tools","@jupyterlab/notebook-extension:update-raw-mimetype"],"@jupyterlab/toc-extension":["@jupyterlab/toc-extension:registry","@jupyterlab/toc-extension:tracker"],"@jupyterlab/tooltip-extension":["@jupyterlab/tooltip-extension:manager","@jupyterlab/tooltip-extension:notebooks"]},"/consoles":{"@jupyterlab/tooltip-extension":["@jupyterlab/tooltip-extension:manager","@jupyterlab/tooltip-extension:consoles"]},"/edit":{"@jupyterlab/fileeditor-extension":["@jupyterlab/fileeditor-extension:completer","@jupyterlab/fileeditor-extension:search"],"@jupyterlab/markdownviewer-extension":true}}');
+                const j = new(0, t(59625).NotebookApp)({
                     mimeExtensions: n,
                     availablePlugins: l
                 });
-                j.registerPluginModules(b), "true" === (o.PageConfig.getOption("exposeAppInBrowser") || "").toLowerCase() && (window.jupyterapp = j), await j.start()
+                j.registerPluginModules(u), "true" === (o.PageConfig.getOption("exposeAppInBrowser") || "").toLowerCase() && (window.jupyterapp = j), await j.start()
             }))
         },
         72761: (e, n, t) => {
             "use strict";
             t.r(n), t(71818), t(70022), t(26238);
             var o = t(94830),
                 a = t.n(o),
                 r = t(80592),
                 i = t.n(r),
                 l = t(99763),
                 s = t.n(l),
                 p = t(28915),
-                b = t.n(p),
-                u = t(80366),
-                d = t.n(u),
+                u = t.n(p),
+                b = t(80366),
+                d = t.n(b),
                 c = t(17352),
                 j = t.n(c),
                 m = t(26633),
                 y = {};
-            y.styleTagTransform = j(), y.setAttributes = b(), y.insert = s().bind(null, "head"), y.domAPI = i(), y.insertStyleElement = d(), a()(m.Z, y), m.Z && m.Z.locals && m.Z.locals;
+            y.styleTagTransform = j(), y.setAttributes = u(), y.insert = s().bind(null, "head"), y.domAPI = i(), y.insertStyleElement = d(), a()(m.Z, y), m.Z && m.Z.locals && m.Z.locals;
             var x = t(93862),
                 g = {};
-            g.styleTagTransform = j(), g.setAttributes = b(), g.insert = s().bind(null, "head"), g.domAPI = i(), g.insertStyleElement = d(), a()(x.Z, g), x.Z && x.Z.locals && x.Z.locals, t(20959);
+            g.styleTagTransform = j(), g.setAttributes = u(), g.insert = s().bind(null, "head"), g.domAPI = i(), g.insertStyleElement = d(), a()(x.Z, g), x.Z && x.Z.locals && x.Z.locals, t(20959);
             var h = t(58027),
                 f = {};
-            f.styleTagTransform = j(), f.setAttributes = b(), f.insert = s().bind(null, "head"), f.domAPI = i(), f.insertStyleElement = d(), a()(h.Z, f), h.Z && h.Z.locals && h.Z.locals;
+            f.styleTagTransform = j(), f.setAttributes = u(), f.insert = s().bind(null, "head"), f.domAPI = i(), f.insertStyleElement = d(), a()(h.Z, f), h.Z && h.Z.locals && h.Z.locals;
             var A = t(99776),
                 k = {};
-            k.styleTagTransform = j(), k.setAttributes = b(), k.insert = s().bind(null, "head"), k.domAPI = i(), k.insertStyleElement = d(), a()(A.Z, k), A.Z && A.Z.locals && A.Z.locals;
-            var w = t(64399),
-                v = {};
-            v.styleTagTransform = j(), v.setAttributes = b(), v.insert = s().bind(null, "head"), v.domAPI = i(), v.insertStyleElement = d(), a()(w.Z, v), w.Z && w.Z.locals && w.Z.locals;
+            k.styleTagTransform = j(), k.setAttributes = u(), k.insert = s().bind(null, "head"), k.domAPI = i(), k.insertStyleElement = d(), a()(A.Z, k), A.Z && A.Z.locals && A.Z.locals;
+            var v = t(64399),
+                w = {};
+            w.styleTagTransform = j(), w.setAttributes = u(), w.insert = s().bind(null, "head"), w.domAPI = i(), w.insertStyleElement = d(), a()(v.Z, w), v.Z && v.Z.locals && v.Z.locals;
             var T = t(11112),
                 P = {};
-            P.styleTagTransform = j(), P.setAttributes = b(), P.insert = s().bind(null, "head"), P.domAPI = i(), P.insertStyleElement = d(), a()(T.Z, P), T.Z && T.Z.locals && T.Z.locals;
+            P.styleTagTransform = j(), P.setAttributes = u(), P.insert = s().bind(null, "head"), P.domAPI = i(), P.insertStyleElement = d(), a()(T.Z, P), T.Z && T.Z.locals && T.Z.locals;
             var Z = t(49482),
                 B = {};
-            B.styleTagTransform = j(), B.setAttributes = b(), B.insert = s().bind(null, "head"), B.domAPI = i(), B.insertStyleElement = d(), a()(Z.Z, B), Z.Z && Z.Z.locals && Z.Z.locals;
+            B.styleTagTransform = j(), B.setAttributes = u(), B.insert = s().bind(null, "head"), B.domAPI = i(), B.insertStyleElement = d(), a()(Z.Z, B), Z.Z && Z.Z.locals && Z.Z.locals;
             var S = t(71564),
-                N = {};
-            N.styleTagTransform = j(), N.setAttributes = b(), N.insert = s().bind(null, "head"), N.domAPI = i(), N.insertStyleElement = d(), a()(S.Z, N), S.Z && S.Z.locals && S.Z.locals;
-            var C = t(8173),
+                C = {};
+            C.styleTagTransform = j(), C.setAttributes = u(), C.insert = s().bind(null, "head"), C.domAPI = i(), C.insertStyleElement = d(), a()(S.Z, C), S.Z && S.Z.locals && S.Z.locals;
+            var N = t(8173),
                 E = {};
-            E.styleTagTransform = j(), E.setAttributes = b(), E.insert = s().bind(null, "head"), E.domAPI = i(), E.insertStyleElement = d(), a()(C.Z, E), C.Z && C.Z.locals && C.Z.locals, t(40360);
+            E.styleTagTransform = j(), E.setAttributes = u(), E.insert = s().bind(null, "head"), E.domAPI = i(), E.insertStyleElement = d(), a()(N.Z, E), N.Z && N.Z.locals && N.Z.locals, t(40360);
             var D = t(30546),
                 z = {};
-            z.styleTagTransform = j(), z.setAttributes = b(), z.insert = s().bind(null, "head"), z.domAPI = i(), z.insertStyleElement = d(), a()(D.Z, z), D.Z && D.Z.locals && D.Z.locals;
+            z.styleTagTransform = j(), z.setAttributes = u(), z.insert = s().bind(null, "head"), z.domAPI = i(), z.insertStyleElement = d(), a()(D.Z, z), D.Z && D.Z.locals && D.Z.locals;
             var F = t(94623),
                 L = {};
-            L.styleTagTransform = j(), L.setAttributes = b(), L.insert = s().bind(null, "head"), L.domAPI = i(), L.insertStyleElement = d(), a()(F.Z, L), F.Z && F.Z.locals && F.Z.locals;
+            L.styleTagTransform = j(), L.setAttributes = u(), L.insert = s().bind(null, "head"), L.domAPI = i(), L.insertStyleElement = d(), a()(F.Z, L), F.Z && F.Z.locals && F.Z.locals;
             var M = t(99402),
-                O = {};
-            O.styleTagTransform = j(), O.setAttributes = b(), O.insert = s().bind(null, "head"), O.domAPI = i(), O.insertStyleElement = d(), a()(M.Z, O), M.Z && M.Z.locals && M.Z.locals, t(32723), t(82649), t(15491), t(92645), t(18934), t(24017), t(72867), t(93751), t(75617), t(91532), t(20603), t(17066), t(39380), t(9755), t(82164), t(94938), t(53555), t(86258), t(11575), t(10887), t(26449), t(3727), t(97635), t(16856), t(46165), t(8604), t(26053), t(84221), t(53927), t(67074), t(47275), t(58068), t(41346), t(74768), t(65315), t(87635), t(37609), t(49733), t(40745)
+                I = {};
+            I.styleTagTransform = j(), I.setAttributes = u(), I.insert = s().bind(null, "head"), I.domAPI = i(), I.insertStyleElement = d(), a()(M.Z, I), M.Z && M.Z.locals && M.Z.locals, t(32723), t(82649), t(15491), t(92645), t(18934), t(24017), t(72867), t(93751), t(75617), t(91532), t(20603), t(17066), t(39380), t(9755), t(82164), t(94938), t(53555), t(86258), t(11575), t(10887), t(26449), t(3727), t(97635), t(16856), t(46165), t(8604), t(26053), t(84221), t(53927), t(67074), t(47275), t(58068), t(41346), t(74768), t(65315), t(87635), t(37609), t(49733), t(40745)
         },
         58027: (e, n, t) => {
             "use strict";
             t.d(n, {
                 Z: () => l
             });
             var o = t(66846),
@@ -275,15 +275,15 @@
             });
             var o = t(66846),
                 a = t.n(o),
                 r = t(11368),
                 i = t.n(r),
                 l = t(99686),
                 s = i()(a());
-            s.i(l.Z), s.push([e.id, "/*-----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n|\n| Distributed under the terms of the Modified BSD License.\n|----------------------------------------------------------------------------*/\n\n/**\n  Document oriented look for the notebook.\n  This includes changes to the look and feel of the JupyterLab Notebook\n  component like:\n  - scrollbar to the right of the page\n  - drop shadow on the notebook\n  - smaller empty space at the bottom of the notebook\n  - compact view on mobile\n*/\n\n/* Keep the notebook centered on the page */\n\nbody[data-notebook='notebooks'] .jp-NotebookPanel-toolbar {\n  padding-left: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n  padding-right: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-outer {\n  width: unset !important;\n  padding-top: unset;\n  padding-left: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n  padding-right: calc(\n    calc(\n        100% - var(--jp-notebook-max-width) - var(--jp-notebook-padding-offset)\n      ) * 0.5\n  ) !important;\n  background: var(--jp-layout-color2);\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-inner {\n  margin-top: var(--jp-notebook-toolbar-margin-bottom);\n}\n\nbody[data-notebook='notebooks'] .jp-Notebook-cell {\n  background: var(--jp-layout-color0);\n  padding-left: calc(2 * var(--jp-cell-padding));\n  padding-right: calc(2 * var(--jp-cell-padding));\n}\n\n/* Empty space at the bottom of the notebook (similar to classic) */\nbody[data-notebook='notebooks']\n  .jp-Notebook.jp-mod-scrollPastEnd\n  .jp-WindowedPanel-outer::after {\n  min-height: 100px;\n}\n\n/* Workaround for disabling the full windowing mode */\nbody[data-notebook='notebooks']\n  .jp-Toolbar-item[data-jp-item-name='scrollbar'] {\n  display: none;\n}\n\n/* Fix background colors */\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-outer > * {\n  background: var(--jp-layout-color0);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook.jp-mod-commandMode\n  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {\n  background: var(--jp-layout-color0) !important;\n}\n\n/**\n  Extra padding to the first and and last cell of the notebook.\n  TODO: revisit when https://github.com/jupyterlab/jupyterlab/issues/13151 is fixed\n*/\n.jp-Notebook-cell[data-windowed-list-index='0'] {\n  padding-top: calc(2 * var(--jp-notebook-padding));\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-viewport > *:last-child {\n  padding-bottom: calc(2 * var(--jp-notebook-padding));\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::before {\n  content: ' ';\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 11px;\n}\n\n/* Cell toolbar adjustments */\n\nbody[data-notebook='notebooks'] .jp-cell-toolbar {\n  background: unset;\n  box-shadow: unset;\n}\n\n/** first code cell on mobile\n    (keep the selector above the media query)\n*/\nbody[data-notebook='notebooks']\n  .jp-CodeCell[data-windowed-list-index='0']\n  .jp-cell-toolbar {\n  top: unset;\n}\n\n@media only screen and (max-width: 760px) {\n  /* first code cell on mobile */\n  body[data-notebook='notebooks']\n    .jp-CodeCell[data-windowed-list-index='0']\n    .jp-cell-toolbar {\n    top: var(--jp-notebook-padding);\n  }\n\n  body[data-notebook='notebooks'] .jp-MarkdownCell .jp-cell-toolbar,\n  body[data-notebook='notebooks'] .jp-RawCell .jp-cell-toolbar {\n    top: calc(0.5 * var(--jp-notebook-padding));\n  }\n}\n\n/* Tweak the notebook footer (to add a new cell) */\nbody[data-notebook='notebooks'] .jp-Notebook-footer {\n  width: 100%;\n  margin-left: unset;\n  background: unset;\n}\n\n/* Mobile View */\n\nbody[data-format='mobile'] .jp-NotebookCheckpoint {\n  display: none;\n}\n\nbody[data-format='mobile'] .jp-WindowedPanel-outer > *:first-child {\n  margin-top: 0;\n}\n\nbody[data-format='mobile'] .jp-ToolbarButton .jp-DebuggerBugButton {\n  display: none;\n}\n\n/* Virtual Notebook fixes */\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-viewport {\n  background: var(--jp-layout-color0);\n  padding: unset;\n}\n\n/* Notebook box shadow */\n\nbody[data-notebook='notebooks']\n  .jp-WindowedPanel-outer\n  > *:first-child:not(:last-child) {\n  box-shadow: var(--jp-elevation-z4);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  > *:first-child:last-child::before {\n  content: '';\n  position: absolute;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  right: 0;\n  box-shadow: 0px 0px 12px 1px var(--jp-shadow-umbra-color);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::after,\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::before {\n  content: ' ';\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 11px;\n}\n\n/* Additional customizations of the components on the notebook page */\n\n.jp-NotebookKernelLogo {\n  flex: 0 0 auto;\n  display: flex;\n  align-items: center;\n  text-align: center;\n  margin-right: 8px;\n}\n\n.jp-NotebookKernelLogo img {\n  max-width: 28px;\n  max-height: 28px;\n  display: flex;\n}\n\n.jp-NotebookKernelStatus {\n  margin: 0;\n  font-weight: normal;\n  font-size: var(--jp-ui-font-size1);\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: var(--jp-private-title-panel-height);\n  padding-left: var(--jp-kernel-status-padding);\n  padding-right: var(--jp-kernel-status-padding);\n}\n\n.jp-NotebookKernelStatus-error {\n  background-color: var(--jp-error-color0);\n}\n\n.jp-NotebookKernelStatus-warn {\n  background-color: var(--jp-warn-color0);\n}\n\n.jp-NotebookKernelStatus-info {\n  background-color: var(--jp-info-color0);\n}\n\n.jp-NotebookKernelStatus-fade {\n  animation: 0.5s fade-out forwards;\n}\n\n.jp-NotebookTrustedStatus {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  margin-top: 4px;\n  margin-bottom: 4px;\n  border: solid 1px var(--jp-border-color2);\n  cursor: help;\n}\n\n.jp-NotebookTrustedStatus-not-trusted {\n  cursor: pointer;\n}\n\n@keyframes fade-out {\n  0% {\n    opacity: 1;\n  }\n  100% {\n    opacity: 0;\n  }\n}\n\n#jp-title h1 {\n  cursor: pointer;\n  font-size: 18px;\n  margin: 0;\n  font-weight: normal;\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: calc(1.5 * var(--jp-private-title-panel-height));\n  text-overflow: ellipsis;\n  overflow: hidden;\n  white-space: nowrap;\n}\n\n#jp-title h1:hover {\n  background: var(--jp-layout-color2);\n}\n\n.jp-NotebookCheckpoint {\n  font-size: 14px;\n  margin-left: 5px;\n  margin-right: 5px;\n  font-weight: normal;\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: calc(1.5 * var(--jp-private-title-panel-height));\n  text-overflow: ellipsis;\n  overflow: hidden;\n  white-space: nowrap;\n}\n\n.jp-skiplink {\n  position: absolute;\n  top: -100em;\n}\n\n.jp-skiplink:focus-within {\n  position: absolute;\n  z-index: 10000;\n  top: 0;\n  left: 46%;\n  margin: 0 auto;\n  padding: 1em;\n  width: 15%;\n  box-shadow: var(--jp-elevation-z4);\n  border-radius: 4px;\n  background: var(--jp-layout-color0);\n  text-align: center;\n}\n\n.jp-skiplink:focus-within a {\n  text-decoration: underline;\n  color: var(--jp-content-link-color);\n}\n", ""]);
+            s.i(l.Z), s.push([e.id, "/*-----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n|\n| Distributed under the terms of the Modified BSD License.\n|----------------------------------------------------------------------------*/\n\n/**\n  Document oriented look for the notebook.\n  This includes changes to the look and feel of the JupyterLab Notebook\n  component like:\n  - scrollbar to the right of the page\n  - drop shadow on the notebook\n  - smaller empty space at the bottom of the notebook\n  - compact view on mobile\n*/\n\n/* Keep the notebook centered on the page */\n\nbody[data-notebook='notebooks'] .jp-NotebookPanel-toolbar {\n  padding-left: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n  padding-right: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-outer {\n  width: unset !important;\n  padding-top: unset;\n  padding-left: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n  padding-right: calc(\n    calc(\n        100% - var(--jp-notebook-max-width) - var(--jp-notebook-padding-offset)\n      ) * 0.5\n  ) !important;\n  background: var(--jp-layout-color2);\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-inner {\n  margin-top: var(--jp-notebook-toolbar-margin-bottom);\n  /* Adjustments for the extra top and bottom notebook padding */\n  margin-bottom: calc(4 * var(--jp-notebook-padding));\n}\n\nbody[data-notebook='notebooks'] .jp-Notebook-cell {\n  background: var(--jp-layout-color0);\n  padding-left: calc(2 * var(--jp-cell-padding));\n  padding-right: calc(2 * var(--jp-cell-padding));\n}\n\n/* Empty space at the bottom of the notebook (similar to classic) */\nbody[data-notebook='notebooks']\n  .jp-Notebook.jp-mod-scrollPastEnd\n  .jp-WindowedPanel-outer::after {\n  min-height: 100px;\n}\n\n/* Fix background colors */\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-outer > * {\n  background: var(--jp-layout-color0);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook.jp-mod-commandMode\n  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {\n  background: var(--jp-layout-color0) !important;\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::before {\n  content: ' ';\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 11px;\n}\n\n/* Cell toolbar adjustments */\n\nbody[data-notebook='notebooks'] .jp-cell-toolbar {\n  background: unset;\n  box-shadow: unset;\n}\n\n/** first code cell on mobile\n    (keep the selector above the media query)\n*/\nbody[data-notebook='notebooks']\n  .jp-CodeCell[data-windowed-list-index='0']\n  .jp-cell-toolbar {\n  top: unset;\n}\n\n@media only screen and (max-width: 760px) {\n  /* first code cell on mobile */\n  body[data-notebook='notebooks']\n    .jp-CodeCell[data-windowed-list-index='0']\n    .jp-cell-toolbar {\n    top: var(--jp-notebook-padding);\n  }\n\n  body[data-notebook='notebooks'] .jp-MarkdownCell .jp-cell-toolbar,\n  body[data-notebook='notebooks'] .jp-RawCell .jp-cell-toolbar {\n    top: calc(0.5 * var(--jp-notebook-padding));\n  }\n}\n\n/* Tweak the notebook footer (to add a new cell) */\nbody[data-notebook='notebooks'] .jp-Notebook-footer {\n  background: unset;\n  width: 100%;\n  margin-left: unset;\n}\n\n/* Mobile View */\n\nbody[data-format='mobile'] .jp-NotebookCheckpoint {\n  display: none;\n}\n\nbody[data-format='mobile'] .jp-WindowedPanel-outer > *:first-child {\n  margin-top: 0;\n}\n\nbody[data-format='mobile'] .jp-ToolbarButton .jp-DebuggerBugButton {\n  display: none;\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-viewport {\n  background: var(--jp-layout-color0);\n  box-shadow: var(--jp-elevation-z4);\n  padding: unset;\n\n  /* Extra padding at the top and bottom so the notebook looks nicer */\n  padding-top: calc(2 * var(--jp-notebook-padding));\n  padding-bottom: calc(2 * var(--jp-notebook-padding));\n}\n\n/* Notebook box shadow */\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  > *:first-child:last-child::before {\n  content: '';\n  position: absolute;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  right: 0;\n  box-shadow: 0px 0px 12px 1px var(--jp-shadow-umbra-color);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::after,\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::before {\n  content: ' ';\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 11px;\n}\n\n/* Additional customizations of the components on the notebook page */\n\n.jp-NotebookKernelLogo {\n  flex: 0 0 auto;\n  display: flex;\n  align-items: center;\n  text-align: center;\n  margin-right: 8px;\n}\n\n.jp-NotebookKernelLogo img {\n  max-width: 28px;\n  max-height: 28px;\n  display: flex;\n}\n\n.jp-NotebookKernelStatus {\n  margin: 0;\n  font-weight: normal;\n  font-size: var(--jp-ui-font-size1);\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: var(--jp-private-title-panel-height);\n  padding-left: var(--jp-kernel-status-padding);\n  padding-right: var(--jp-kernel-status-padding);\n}\n\n.jp-NotebookKernelStatus-error {\n  background-color: var(--jp-error-color0);\n}\n\n.jp-NotebookKernelStatus-warn {\n  background-color: var(--jp-warn-color0);\n}\n\n.jp-NotebookKernelStatus-info {\n  background-color: var(--jp-info-color0);\n}\n\n.jp-NotebookKernelStatus-fade {\n  animation: 0.5s fade-out forwards;\n}\n\n.jp-NotebookTrustedStatus {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  margin-top: 4px;\n  margin-bottom: 4px;\n  border: solid 1px var(--jp-border-color2);\n  cursor: help;\n}\n\n.jp-NotebookTrustedStatus-not-trusted {\n  cursor: pointer;\n}\n\n@keyframes fade-out {\n  0% {\n    opacity: 1;\n  }\n  100% {\n    opacity: 0;\n  }\n}\n\n#jp-title h1 {\n  cursor: pointer;\n  font-size: 18px;\n  margin: 0;\n  font-weight: normal;\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: calc(1.5 * var(--jp-private-title-panel-height));\n  text-overflow: ellipsis;\n  overflow: hidden;\n  white-space: nowrap;\n}\n\n#jp-title h1:hover {\n  background: var(--jp-layout-color2);\n}\n\n.jp-NotebookCheckpoint {\n  font-size: 14px;\n  margin-left: 5px;\n  margin-right: 5px;\n  font-weight: normal;\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: calc(1.5 * var(--jp-private-title-panel-height));\n  text-overflow: ellipsis;\n  overflow: hidden;\n  white-space: nowrap;\n}\n\n.jp-skiplink {\n  position: absolute;\n  top: -100em;\n}\n\n.jp-skiplink:focus-within {\n  position: absolute;\n  z-index: 10000;\n  top: 0;\n  left: 46%;\n  margin: 0 auto;\n  padding: 1em;\n  width: 15%;\n  box-shadow: var(--jp-elevation-z4);\n  border-radius: 4px;\n  background: var(--jp-layout-color0);\n  text-align: center;\n}\n\n.jp-skiplink:focus-within a {\n  text-decoration: underline;\n  color: var(--jp-content-link-color);\n}\n", ""]);
             const p = s
         },
         99686: (e, n, t) => {
             "use strict";
             t.d(n, {
                 Z: () => l
             });
```

### Comparing `notebook-7.2.0rc0/notebook/static/8801.bundle.js` & `notebook-7.2.0rc1/notebook/static/8801.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/883.bundle.js` & `notebook-7.2.0rc1/notebook/static/883.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8845.bundle.js` & `notebook-7.2.0rc1/notebook/static/8845.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -63,15 +63,15 @@
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.AmsConfiguration = e.AmsTags = void 0;
             var i = r(63401),
                 s = r(75377),
                 l = r(75723),
                 c = r(14880);
-            r(27798);
+            r(16925);
             var u = r(65695),
                 d = function(t) {
                     function e() {
                         return null !== t && t.apply(this, arguments) || this
                     }
                     return a(e, t), e
                 }(l.AbstractTags);
@@ -217,15 +217,15 @@
                     }
                 }, e.prototype.EndTable = function() {
                     t.prototype.EndTable.call(this), this.center && this.maxrow <= 2 && (delete this.arraydef.width, delete this.global.indentalign)
                 }, e
             }(s.EqnArrayItem);
             e.FlalignItem = f
         },
-        27798: function(t, e, r) {
+        16925: function(t, e, r) {
             var n = this && this.__createBinding || (Object.create ? function(t, e, r, n) {
                     void 0 === n && (n = r);
                     var o = Object.getOwnPropertyDescriptor(e, r);
                     o && !("get" in o ? !e.__esModule : o.writable || o.configurable) || (o = {
                         enumerable: !0,
                         get: function() {
                             return e[r]
```

### Comparing `notebook-7.2.0rc0/notebook/static/8845.bundle.js.LICENSE.txt` & `notebook-7.2.0rc1/notebook/static/8845.bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8875.bundle.js` & `notebook-7.2.0rc1/notebook/static/8875.bundle.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [8875, 1650], {
         71650: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => s
             });
-            var n = o(1167),
-                a = o(91942),
-                i = o(46807),
+            var n = o(68722),
+                a = o(5094),
+                i = o(59625),
                 d = o(81997);
             const s = [{
                 id: "@jupyter-notebook/docmanager-extension:opener",
                 autoStart: !0,
                 optional: [i.INotebookPathOpener, i.INotebookShell],
                 provides: a.IDocumentWidgetOpener,
                 description: "Open documents in a new browser tab",
```

### Comparing `notebook-7.2.0rc0/notebook/static/88b98cad3688915e50da.woff` & `notebook-7.2.0rc1/notebook/static/88b98cad3688915e50da.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8907.bundle.js` & `notebook-7.2.0rc1/notebook/static/8907.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,16 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [8907, 1198], {
         41198: (t, e, s) => {
             s.r(e), s.d(e, {
                 IPropertyInspectorProvider: () => c,
                 SideBarPropertyInspectorProvider: () => a
             });
-            var n = s(37267),
-                r = s(22620),
+            var n = s(12030),
+                r = s(35613),
                 o = s(81997),
                 i = s(63485);
             const c = new(s(20998).Token)("@jupyterlab/property-inspector:IPropertyInspectorProvider", "A service to registry new widget in the property inspector side panel.");
             class h extends i.Widget {
                 constructor() {
                     super(), this._tracker = new i.FocusTracker, this._inspectors = new Map, this.addClass("jp-PropertyInspector"), this._tracker = new i.FocusTracker, this._tracker.currentChanged.connect(this._onCurrentChanged, this)
                 }
```

### Comparing `notebook-7.2.0rc0/notebook/static/8928.bundle.js` & `notebook-7.2.0rc1/notebook/static/7900.bundle.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [8928, 7900], {
+    [7900, 8928], {
         67900: (t, e, i) => {
             i.r(e), i.d(e, {
                 IImageTracker: () => r,
                 ImageViewer: () => l,
                 ImageViewerFactory: () => d
             });
             var s = i(20998);
             const r = new s.Token("@jupyterlab/imageviewer:IImageTracker", "A widget tracker for images.\n  Use this if you want to be able to iterate over and interact with images\n  viewed by the application.");
-            var a, o = i(1167),
-                n = i(96049),
-                c = i(10979),
+            var a, o = i(68722),
+                n = i(53312),
+                c = i(65903),
                 h = i(63485);
             class l extends h.Widget {
                 constructor(t) {
                     super(), this._scale = 1, this._matrix = [1, 0, 0, 1], this._colorinversion = 0, this._ready = new s.PromiseDelegate, this.context = t, this.node.tabIndex = 0, this.addClass("jp-ImageViewer"), this._img = document.createElement("img"), this.node.appendChild(this._img), this._onTitleChanged(), t.pathChanged.connect(this._onTitleChanged, this), t.ready.then((() => {
                         if (this.isDisposed) return;
                         const e = t.contentsModel;
                         this._mimeType = e.mimetype, this._render(), t.model.contentChanged.connect(this.update, this), t.fileChanged.connect(this.update, this), this._ready.resolve(void 0)
```

### Comparing `notebook-7.2.0rc0/notebook/static/8929.bundle.js` & `notebook-7.2.0rc1/notebook/static/8929.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/893.bundle.js` & `notebook-7.2.0rc1/notebook/static/893.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,24 +2,24 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [893], {
         30893: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => T,
                 fileUploadStatus: () => B
             });
-            var r = o(2922),
-                n = o(96049),
-                a = o(1167),
-                i = o(91942),
-                s = o(42751),
-                l = o(24554),
-                d = o(96692),
-                c = o(27829),
-                u = o(37267),
-                m = o(22620),
+            var r = o(44604),
+                n = o(53312),
+                a = o(68722),
+                i = o(5094),
+                s = o(71427),
+                l = o(23295),
+                d = o(41053),
+                c = o(71098),
+                u = o(12030),
+                m = o(35613),
                 p = o(33625),
                 h = o(16934);
             const w = "FileBrowser",
                 f = "@jupyterlab/filebrowser-extension:browser";
             var g;
             ! function(e) {
                 e.copy = "filebrowser:copy", e.copyDownloadLink = "filebrowser:copy-download-link", e.cut = "filebrowser:cut", e.del = "filebrowser:delete", e.download = "filebrowser:download", e.duplicate = "filebrowser:duplicate", e.hideBrowser = "filebrowser:hide-main", e.goToPath = "filebrowser:go-to-path", e.goUp = "filebrowser:go-up", e.openPath = "filebrowser:open-path", e.openUrl = "filebrowser:open-url", e.open = "filebrowser:open", e.openBrowserTab = "filebrowser:open-browser-tab", e.paste = "filebrowser:paste", e.createNewDirectory = "filebrowser:create-new-directory", e.createNewFile = "filebrowser:create-new-file", e.createNewMarkdownFile = "filebrowser:create-new-markdown-file", e.refresh = "filebrowser:refresh", e.rename = "filebrowser:rename", e.copyShareableLink = "filebrowser:share-main", e.copyPath = "filebrowser:copy-path", e.showBrowser = "filebrowser:activate", e.shutdown = "filebrowser:shutdown", e.toggleBrowser = "filebrowser:toggle-main", e.toggleNavigateToCurrentDirectory = "filebrowser:toggle-navigate-to-current-directory", e.toggleLastModified = "filebrowser:toggle-last-modified", e.toggleShowFullPath = "filebrowser:toggle-show-full-path", e.toggleFileSize = "filebrowser:toggle-file-size", e.toggleSortNotebooksFirst = "filebrowser:toggle-sort-notebooks-first", e.search = "filebrowser:search", e.toggleHiddenFiles = "filebrowser:toggle-hidden-files", e.toggleFileCheckboxes = "filebrowser:toggle-file-checkboxes"
```

### Comparing `notebook-7.2.0rc0/notebook/static/8937.bundle.js` & `notebook-7.2.0rc1/notebook/static/8937.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8979.bundle.js` & `notebook-7.2.0rc1/notebook/static/8979.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8983.bundle.js` & `notebook-7.2.0rc1/notebook/static/8983.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/899.bundle.js` & `notebook-7.2.0rc1/notebook/static/899.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8ea8791754915a898a31.woff2` & `notebook-7.2.0rc1/notebook/static/8ea8791754915a898a31.woff2`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/8ea8dbb1b02e6f730f55.woff` & `notebook-7.2.0rc1/notebook/static/8ea8dbb1b02e6f730f55.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/901.bundle.js` & `notebook-7.2.0rc1/notebook/static/901.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -275,19 +275,19 @@
         },
         75677: (e, t, r) => {
             r.d(t, {
                 aX: () => y,
                 as: () => h,
                 w2: () => u
             });
-            var i = r(96049),
-                n = r(10979),
-                s = r(13408),
-                a = r(37267),
-                o = r(22620),
+            var i = r(53312),
+                n = r(65903),
+                s = r(81221),
+                a = r(12030),
+                o = r(35613),
                 d = r(20998),
                 c = r(14421),
                 l = r(67863);
             const u = new d.Token("@jupyterlab/application:IMimeDocumentTracker", "A widget tracker for documents rendered using a mime renderer extension. Use this if you want to list and interact with documents rendered by such extensions.");
 
             function h(e) {
                 const t = [],
```

### Comparing `notebook-7.2.0rc0/notebook/static/9022.bundle.js` & `notebook-7.2.0rc1/notebook/static/9022.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9037.bundle.js` & `notebook-7.2.0rc1/notebook/static/9037.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/906.bundle.js` & `notebook-7.2.0rc1/notebook/static/906.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9060.bundle.js` & `notebook-7.2.0rc1/notebook/static/9060.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9068.bundle.js` & `notebook-7.2.0rc1/notebook/static/9068.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [9068], {
         59068: (l, n, e) => {
             e.r(n), e.d(n, {
                 jupyterIcon: () => m
             });
-            const m = new(e(22620).LabIcon)({
+            const m = new(e(35613).LabIcon)({
                 name: "notebook-ui-components:jupyter",
                 svgstr: '<svg width="189" height="51" version="2.0" viewBox="0 0 189 51" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">\n <title>Jupyter</title>\n <g class="jp-icon3" transform="translate(-1638 -2093)" fill="#616161">\n  <g style="mix-blend-mode:normal">\n   <g style="mix-blend-mode:normal">\n    <g style="mix-blend-mode:normal">\n     <g style="mix-blend-mode:normal">\n      <g style="mix-blend-mode:normal">\n       <use transform="translate(1688.9 2106.2)" style="mix-blend-mode:normal" xlink:href="#path0_fill"/>\n      </g>\n     </g>\n     <g style="mix-blend-mode:normal">\n      <g style="mix-blend-mode:normal">\n       <use transform="translate(1705.4 2106.2)" style="mix-blend-mode:normal" xlink:href="#path1_fill"/>\n      </g>\n     </g>\n     <g style="mix-blend-mode:normal">\n      <g style="mix-blend-mode:normal">\n       <use transform="translate(1730.2 2105.7)" style="mix-blend-mode:normal" xlink:href="#path2_fill"/>\n      </g>\n     </g>\n     <g style="mix-blend-mode:normal">\n      <g style="mix-blend-mode:normal">\n       <use transform="translate(1752.9 2106.2)" style="mix-blend-mode:normal" xlink:href="#path3_fill"/>\n      </g>\n     </g>\n     <g style="mix-blend-mode:normal">\n      <g style="mix-blend-mode:normal">\n       <use transform="translate(1775.8 2100)" style="mix-blend-mode:normal" xlink:href="#path4_fill"/>\n      </g>\n     </g>\n     <g style="mix-blend-mode:normal">\n      <g style="mix-blend-mode:normal">\n       <use transform="translate(1791.8 2105.7)" style="mix-blend-mode:normal" xlink:href="#path5_fill"/>\n      </g>\n     </g>\n     <g style="mix-blend-mode:normal">\n      <g style="mix-blend-mode:normal">\n       <use transform="translate(1815.8 2105.7)" style="mix-blend-mode:normal" xlink:href="#path6_fill"/>\n      </g>\n     </g>\n    </g>\n   </g>\n   <g style="mix-blend-mode:normal">\n    <g style="mix-blend-mode:normal">\n     <g style="mix-blend-mode:normal">\n      <use transform="translate(1669.3 2093.3)" fill="#767677" style="mix-blend-mode:normal" xlink:href="#path7_fill"/>\n     </g>\n    </g>\n    <g style="mix-blend-mode:normal">\n     <g style="mix-blend-mode:normal">\n      <use transform="translate(1639.7 2124)" fill="#F37726" style="mix-blend-mode:normal" xlink:href="#path8_fill"/>\n     </g>\n    </g>\n    <g style="mix-blend-mode:normal">\n     <g style="mix-blend-mode:normal">\n      <use transform="translate(1639.7 2097.5)" fill="#F37726" style="mix-blend-mode:normal" xlink:href="#path9_fill"/>\n     </g>\n    </g>\n    <g style="mix-blend-mode:normal">\n     <g style="mix-blend-mode:normal">\n      <use transform="translate(1639.8 2135.8)" fill="#989798" style="mix-blend-mode:normal" xlink:href="#path10_fill"/>\n     </g>\n    </g>\n    <g style="mix-blend-mode:normal">\n     <g style="mix-blend-mode:normal">\n      <use transform="translate(1638.4 2098.1)" fill="#6F7070" style="mix-blend-mode:normal" xlink:href="#path11_fill"/>\n     </g>\n    </g>\n   </g>\n  </g>\n </g>\n <defs>\n  <path id="path0_fill" d="m5.6259 17.928c0 5.1461-0.3925 6.8263-1.4392 8.0666-1.1426 1.0559-2.637 1.6399-4.1867 1.6362l0.39251 3.0612c2.402 0.0333 4.7305-0.8352 6.5331-2.4366 1.8753-1.9529 2.5295-4.6535 2.5295-8.7967v-19.458h-3.8378v17.954l0.00872-0.0264z"/>\n  <path id="path1_fill" d="m17.741 15.623c0 2.2168 0 4.1696 0.1744 5.8498h-3.3581l-0.218-3.5187h-0.0873c-0.7069 1.2298-1.7261 2.2473-2.9526 2.9477-1.2265 0.7005-2.6159 1.0585-4.0252 1.0372-3.3145 0-7.2744-1.8649-7.2744-9.3948v-12.544h3.8378v11.902c0 4.0817 1.2211 6.8262 4.7014 6.8262 1.0917-0.0201 2.1533-0.3647 3.0516-0.9907 0.8984-0.6259 1.5936-1.5053 1.9986-2.5279 0.2328-0.6395 0.351-1.3157 0.3489-1.9969v-13.195h3.8379v15.605h-0.0349z"/>\n  <path id="path2_fill" d="m0.17445 7.5363c0-2.7446-0.087223-4.9613-0.17445-7.0374h3.4453l0.17445 3.677h0.08722c0.75374-1.3174 1.85-2.4022 3.1705-3.137 1.3205-0.73485 2.8149-1.0919 4.322-1.0326 5.0939 0 8.9317 4.3983 8.9317 10.908 0 7.7147-4.6141 11.524-9.5946 11.524-1.2785 0.0541-2.5489-0.2281-3.6867-0.8187-1.1377-0.5907-2.1036-1.4696-2.8028-2.5504h-0.08723v11.656h-3.7942v-23.223l0.008722 0.03519zm3.7942 5.7179c0.01001 0.5349 0.0684 1.0679 0.17444 1.5922 0.31262 1.3003 1.0491 2.4571 2.0914 3.2849 1.0423 0.8279 2.33 1.2788 3.6567 1.2805 4.0559 0 6.4022-3.3691 6.4022-8.2864 0-4.3016-2.2242-7.9786-6.2714-7.9786-1.3611 0.03841-2.6704 0.53457-3.7198 1.4096-1.0494 0.87505-1.7786 2.0788-2.0718 3.4198-0.15373 0.51742-0.24166 1.0524-0.26167 1.5922v3.6858z"/>\n  <path id="path3_fill" d="m4.1606 0 4.6141 12.676c0.47973 1.4163 1.0031 3.1053 1.352 4.3984h0.0872c0.3925-1.2843 0.8286-2.9293 1.352-4.4775l4.1867-12.588h4.0559l-5.7481 15.297c-2.7475 7.3541-4.6141 11.128-7.2308 13.433-1.3222 1.2403-2.9429 2.1106-4.7014 2.5246l-0.95946-3.2811c1.2303-0.4134 2.3704-1.0615 3.3581-1.9089 1.3957-1.1762 2.5006-2.664 3.2273-4.3456 0.15514-0.2904 0.25848-0.606 0.30528-0.9324-0.03445-0.3518-0.12272-0.696-0.26167-1.0205l-7.7978-19.766h4.1867l-0.02616-0.0087967z"/>\n  <path id="path4_fill" d="m7.0215 0v6.1577h5.4864v2.9733h-5.4864v11.559c0 2.639 0.7414 4.1696 2.8784 4.1696 0.74972 0.0118 1.4976-0.077 2.2242-0.2639l0.1744 2.9293c-1.0915 0.3877-2.2451 0.5667-3.4017 0.5278-0.76701 0.0474-1.535-0.0744-2.2506-0.357-0.71554-0.2826-1.3614-0.7191-1.8925-1.2792-1.0903-1.1523-1.4828-3.0612-1.4828-5.5858v-11.7h-3.2709v-2.9733h3.2709v-5.1461l3.7506-1.0116z"/>\n  <path id="path5_fill" d="m3.6285 11.928c0.08723 5.278 3.4017 7.4508 7.2308 7.4508 2.0019 0.0634 3.9934-0.3149 5.8353-1.1084l0.6542 2.7886c-2.2069 0.9347-4.585 1.3874-6.9779 1.3283-6.4894 0-10.371-4.3456-10.371-10.82 0-6.4743 3.7506-11.568 9.8912-11.568 6.8819 0 8.7223 6.1577 8.7223 10.107-0.0065 0.6091-0.0501 1.2172-0.1308 1.8209h-14.854zm11.243-2.7885c0.0436-2.4807-1.003-6.3424-5.3119-6.3424-3.8814 0-5.5736 3.633-5.8789 6.3424h11.199-0.0087z"/>\n  <path id="path6_fill" d="m0.17445 7.1785c0-2.5246-0.043612-4.6974-0.17445-6.6943h3.3581l0.13083 4.2136h0.17445c0.95946-2.8853 3.2709-4.6974 5.8353-4.6974 0.36765-0.0054214 0.73435 0.038958 1.0902 0.13195v3.677c-0.4296-0.09447-0.86861-0.13874-1.3083-0.13195-2.7039 0-4.6141 2.0848-5.1375 5.0053-0.10796 0.60107-0.16631 1.2101-0.17445 1.8209v11.436h-3.7942v-14.761z"/>\n  <path id="path7_fill" d="m5.8935 2.844c0.02536 0.58765-0.12268 1.1697-0.42538 1.6724-0.3027 0.50277-0.74647 0.9037-1.2752 1.1521-0.52869 0.24837-1.1186 0.333-1.6949 0.2432-0.57639-0.08981-1.1134-0.35001-1.5432-0.7477-0.42973-0.39768-0.73284-0.91498-0.87099-1.4864-0.13815-0.57146-0.10513-1.1714 0.094877-1.7239 0.20001-0.55254 0.55803-1.0328 1.0288-1.3801 0.47072-0.34728 1.033-0.54595 1.6157-0.57087 0.78063-0.033384 1.5425 0.24712 2.1182 0.77988 0.57569 0.53276 0.91814 1.2742 0.95211 2.0614z"/>\n  <path id="path8_fill" d="m18.265 7.1341c-7.8501 0-14.706-2.8765-18.265-7.1341 1.3254 3.8204 3.7956 7.1308 7.0686 9.473 3.2731 2.3422 7.1871 3.6004 11.2 3.6004s7.9273-1.2582 11.2-3.6004c3.273-2.3422 5.7432-5.6526 7.0686-9.473-3.5675 4.2576-10.423 7.1341-18.273 7.1341z"/>\n  <path id="path9_fill" d="m18.273 5.9393c7.8502 0 14.706 2.8765 18.265 7.1341-1.3254-3.8204-3.7956-7.1308-7.0686-9.473-3.2731-2.3422-7.1871-3.6004-11.2-3.6004s-7.9273 1.2582-11.2 3.6004c-3.273 2.3422-5.7432 5.6526-7.0686 9.473 3.5674-4.2488 10.423-7.1341 18.273-7.1341z"/>\n  <path id="path10_fill" d="m7.4279 3.5834c0.03219 0.74092-0.15434 1.4748-0.53596 2.1088s-0.94118 1.1394-1.6078 1.4525c-0.66664 0.31303-1.4104 0.41954-2.1371 0.30603s-1.4037-0.44193-1.9452-0.94368c-0.54151-0.50175-0.92323-1.1543-1.0968-1.8749-0.17359-0.72067-0.13125-1.4771 0.12166-2.1735 0.25291-0.69639 0.70502-1.3014 1.2991-1.7385 0.59407-0.4371 1.3034-0.68659 2.0381-0.7169 0.98278-0.040537 1.9414 0.31357 2.6657 0.9847 0.72432 0.67112 1.1552 1.6045 1.1983 2.5955z"/>\n  <path id="path11_fill" d="m2.2747 4.3963c-0.43108 0.01879-0.858-0.09184-1.2267-0.31786-0.36872-0.22603-0.66266-0.55729-0.84462-0.95187s-0.24375-0.83473-0.17756-1.2648c0.066192-0.43001 0.25739-0.83055 0.5494-1.1509 0.29201-0.32037 0.6717-0.54618 1.091-0.64882 0.41931-0.10265 0.85939-0.077531 1.2645 0.072176 0.40515 0.14971 0.75716 0.41727 1.0115 0.76882 0.2543 0.35156 0.39947 0.7713 0.41713 1.2061 0.02364 0.58191-0.18257 1.1495-0.57338 1.5783-0.39081 0.42878-0.93431 0.6837-1.5113 0.70883z"/>\n </defs>\n</svg>\n'
             })
         }
     }
 ]);
```

### Comparing `notebook-7.2.0rc0/notebook/static/911.bundle.js` & `notebook-7.2.0rc1/notebook/static/911.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9136.bundle.js` & `notebook-7.2.0rc1/notebook/static/9136.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1270,15 +1270,15 @@
                 U = new URL(o(11893), o.b),
                 N = new URL(o(23326), o.b),
                 q = new URL(o(65110), o.b),
                 $ = new URL(o(1357), o.b),
                 G = new URL(o(17779), o.b),
                 W = new URL(o(32174), o.b),
                 X = new URL(o(44540), o.b),
-                Y = new URL(o(59681), o.b),
+                Y = new URL(o(43237), o.b),
                 K = new URL(o(13593), o.b),
                 Q = new URL(o(75517), o.b),
                 nn = new URL(o(98311), o.b),
                 en = new URL(o(90717), o.b),
                 on = new URL(o(25075), o.b),
                 tn = new URL(o(81856), o.b),
                 rn = new URL(o(52101), o.b),
@@ -3094,15 +3094,15 @@
         },
         16084: n => {
             n.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 20 20'%3e %3cg class='jp-icon2' fill='%23414141'%3e %3crect x='2' y='2' width='16' height='16'/%3e %3c/g%3e %3cg class='jp-icon-accent2' fill='white'%3e %3cpath d='M7.6%2c8h0.9l3.5%2c8h-1.1L10%2c14H6l-0.9%2c2H4L7.6%2c8z M8%2c9.1L6.4%2c13h3.2L8%2c9.1z'/%3e %3cpath d='M16.6%2c9.8c-0.2%2c0.1-0.4%2c0.1-0.7%2c0.1c-0.2%2c0-0.4-0.1-0.6-0.2c-0.1-0.1-0.2-0.4-0.2-0.7 c-0.3%2c0.3-0.6%2c0.5-0.9%2c0.7c-0.3%2c0.1-0.7%2c0.2-1.1%2c0.2c-0.3%2c0-0.5%2c0-0.7-0.1c-0.2-0.1-0.4-0.2-0.6-0.3c-0.2-0.1-0.3-0.3-0.4-0.5 c-0.1-0.2-0.1-0.4-0.1-0.7c0-0.3%2c0.1-0.6%2c0.2-0.8c0.1-0.2%2c0.3-0.4%2c0.4-0.5C12%2c7%2c12.2%2c6.9%2c12.5%2c6.8c0.2-0.1%2c0.5-0.1%2c0.7-0.2 c0.3-0.1%2c0.5-0.1%2c0.7-0.1c0.2%2c0%2c0.4-0.1%2c0.6-0.1c0.2%2c0%2c0.3-0.1%2c0.4-0.2c0.1-0.1%2c0.2-0.2%2c0.2-0.4c0-1-1.1-1-1.3-1 c-0.4%2c0-1.4%2c0-1.4%2c1.2h-0.9c0-0.4%2c0.1-0.7%2c0.2-1c0.1-0.2%2c0.3-0.4%2c0.5-0.6c0.2-0.2%2c0.5-0.3%2c0.8-0.3C13.3%2c4%2c13.6%2c4%2c13.9%2c4 c0.3%2c0%2c0.5%2c0%2c0.8%2c0.1c0.3%2c0%2c0.5%2c0.1%2c0.7%2c0.2c0.2%2c0.1%2c0.4%2c0.3%2c0.5%2c0.5C16%2c5%2c16%2c5.2%2c16%2c5.6v2.9c0%2c0.2%2c0%2c0.4%2c0%2c0.5 c0%2c0.1%2c0.1%2c0.2%2c0.3%2c0.2c0.1%2c0%2c0.2%2c0%2c0.3%2c0V9.8z M15.2%2c6.9c-1.2%2c0.6-3.1%2c0.2-3.1%2c1.4c0%2c1.4%2c3.1%2c1%2c3.1-0.5V6.9z'/%3e %3c/g%3e %3c/svg%3e"
         },
         32174: n => {
             n.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 24 24'%3e %3cg class='jp-icon3' fill='white'%3e %3cpath d='M14%2c12V19.88C14.04%2c20.18 13.94%2c20.5 13.71%2c20.71C13.32%2c21.1 12.69%2c21.1 12.3%2c20.71L10.29%2c18.7C10.06%2c18.47 9.96%2c18.16 10%2c17.87V12H9.97L4.21%2c4.62C3.87%2c4.19 3.95%2c3.56 4.38%2c3.22C4.57%2c3.08 4.78%2c3 5%2c3V3H19V3C19.22%2c3 19.43%2c3.08 19.62%2c3.22C20.05%2c3.56 20.13%2c4.19 19.79%2c4.62L14.03%2c12H14Z' /%3e %3c/g%3e %3cg class='jp-icon-dot' fill='white'%3e %3ccircle cx='18' cy='17' r='3'%3e%3c/circle%3e %3c/g%3e %3c/svg%3e"
         },
-        59681: n => {
+        43237: n => {
             n.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 24 24'%3e %3cg class='jp-icon3' fill='white'%3e %3cpath d='M14%2c12V19.88C14.04%2c20.18 13.94%2c20.5 13.71%2c20.71C13.32%2c21.1 12.69%2c21.1 12.3%2c20.71L10.29%2c18.7C10.06%2c18.47 9.96%2c18.16 10%2c17.87V12H9.97L4.21%2c4.62C3.87%2c4.19 3.95%2c3.56 4.38%2c3.22C4.57%2c3.08 4.78%2c3 5%2c3V3H19V3C19.22%2c3 19.43%2c3.08 19.62%2c3.22C20.05%2c3.56 20.13%2c4.19 19.79%2c4.62L14.03%2c12H14Z' /%3e %3c/g%3e %3c/svg%3e"
         },
         24213: n => {
             n.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 20 20'%3e %3cg class='jp-icon2' fill='%23414141'%3e %3crect x='2' y='2' width='16' height='16'/%3e %3c/g%3e %3cg class='jp-icon-accent2' fill='white'%3e %3ccircle class='st2' cx='5.5' cy='14.5' r='1.5'/%3e %3crect x='12' y='4' class='st2' width='1' height='8'/%3e %3crect x='8.5' y='7.5' transform='matrix(0.866 -0.5 0.5 0.866 -2.3255 7.3219)' class='st2' width='8' height='1'/%3e %3crect x='12' y='4' transform='matrix(0.5 -0.866 0.866 0.5 -0.6779 14.8252)' class='st2' width='1' height='8'/%3e %3c/g%3e %3c/svg%3e"
         },
         63879: n => {
             n.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 20 20'%3e %3cg class='jp-icon2' fill='%23414141'%3e %3crect x='2' y='2' width='16' height='16'/%3e %3c/g%3e %3cg class='jp-icon-accent2' transform='translate(.43 .0401)' fill='white'%3e %3cpath d='m4.14 8.76q0.0682-1.89 2.42-1.89 1.16 0 1.68 0.42 0.567 0.41 0.567 1.16v3.47q0 0.462 0.514 0.462 0.103 0 0.2-0.0231v0.714q-0.399 0.103-0.651 0.103-0.452 0-0.693-0.22-0.231-0.2-0.284-0.662-0.956 0.872-2 0.872-0.903 0-1.47-0.472-0.525-0.472-0.525-1.26 0-0.262 0.0452-0.472 0.0567-0.22 0.116-0.378 0.0682-0.168 0.231-0.304 0.158-0.147 0.262-0.242 0.116-0.0914 0.368-0.168 0.262-0.0914 0.399-0.126 0.136-0.0452 0.472-0.103 0.336-0.0578 0.504-0.0798 0.158-0.0231 0.567-0.0798 0.556-0.0682 0.777-0.221 0.22-0.152 0.22-0.441v-0.252q0-0.43-0.357-0.662-0.336-0.231-0.976-0.231-0.662 0-0.998 0.262-0.336 0.252-0.399 0.798zm1.89 3.68q0.788 0 1.26-0.41 0.504-0.42 0.504-0.903v-1.05q-0.284 0.136-0.861 0.231-0.567 0.0914-0.987 0.158-0.42 0.0682-0.766 0.326-0.336 0.252-0.336 0.704t0.304 0.704 0.861 0.252z' stroke-width='1.05'/%3e %3cpath d='m10 4.56h0.945v3.15q0.651-0.976 1.89-0.976 1.16 0 1.89 0.84 0.682 0.84 0.682 2.31 0 1.47-0.704 2.42-0.704 0.882-1.89 0.882-1.26 0-1.89-1.02v0.766h-0.85zm2.62 3.04q-0.746 0-1.16 0.64-0.452 0.63-0.452 1.68 0 1.05 0.452 1.68t1.16 0.63q0.777 0 1.26-0.63 0.494-0.64 0.494-1.68 0-1.05-0.472-1.68-0.462-0.64-1.26-0.64z' stroke-width='1.05'/%3e %3cpath d='m2.73 15.8 13.6 0.0081c0.0069 0 0-2.6 0-2.6 0-0.0078-1.15 0-1.15 0-0.0069 0-0.0083 1.5-0.0083 1.5-2e-3 -0.0014-11.3-0.0014-11.3-0.0014l-0.00592-1.5c0-0.0078-1.17 0.0013-1.17 0.0013z' stroke-width='.975'/%3e %3c/g%3e %3c/svg%3e"
```

### Comparing `notebook-7.2.0rc0/notebook/static/9151.bundle.js` & `notebook-7.2.0rc1/notebook/static/9151.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,19 +2,19 @@
     [9151], {
         59151: (e, t, r) => {
             "use strict";
             r.r(t), r.d(t, {
                 ExtensionsPanel: () => R,
                 ListModel: () => p
             });
-            var n, s = r(96049),
-                a = r(1167),
-                i = r(70611),
-                o = r(37267),
-                l = r(22620),
+            var n, s = r(53312),
+                a = r(68722),
+                i = r(87408),
+                o = r(12030),
+                l = r(35613),
                 h = r(97934),
                 c = r(38873),
                 u = r(78156);
             class p extends l.VDomModel {
                     constructor(e, t) {
                         super(), this.actionError = null, this.installedError = null, this.searchError = null, this.promptReload = !1, this._isDisclaimed = !1, this._isEnabled = !1, this._isLoadingInstalledExtensions = !1, this._isSearching = !1, this._query = "", this._page = 1, this._pagination = 30, this._lastPage = 1, this._pendingActions = [];
                         const r = JSON.parse(a.PageConfig.getOption("extensionManager") || "{}");
```

### Comparing `notebook-7.2.0rc0/notebook/static/9161.bundle.js` & `notebook-7.2.0rc1/notebook/static/9161.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,17 +2,17 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [9161], {
         79161: (e, a, r) => {
             r.r(a), r.d(a, {
                 CommandIDs: () => t,
                 default: () => d
             });
-            var t, n = r(96049),
-                o = r(83149),
-                i = r(37267);
+            var t, n = r(53312),
+                o = r(8337),
+                i = r(12030);
             ! function(e) {
                 e.copySource = "mermaid:copy-source"
             }(t || (t = {}));
             const d = [{
                 id: "@jupyterlab/mermaid-extension:core",
                 description: "Provides the Mermaid manager.",
                 autoStart: !0,
```

### Comparing `notebook-7.2.0rc0/notebook/static/9222.bundle.js` & `notebook-7.2.0rc1/notebook/static/9222.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9233.bundle.js` & `notebook-7.2.0rc1/notebook/static/9233.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9234.bundle.js` & `notebook-7.2.0rc1/notebook/static/9234.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9239.bundle.js` & `notebook-7.2.0rc1/notebook/static/9239.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9250.bundle.js` & `notebook-7.2.0rc1/notebook/static/9250.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9268.bundle.js` & `notebook-7.2.0rc1/notebook/static/9268.bundle.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -3,18 +3,18 @@
     [9268, 3129], {
         79268: (e, n, r) => {
             r.r(n), r.d(n, {
                 createMarkdownParser: () => l,
                 default: () => u
             });
             var t = r(20998),
-                a = r(1167),
-                i = r(49269),
-                o = r(13408),
-                s = r(83149);
+                a = r(68722),
+                i = r(30525),
+                o = r(81221),
+                s = r(8337);
             const c = "```~~~";
 
             function l(e, n) {
                 return {
                     render: r => d.render(r, e, n)
                 }
             }
```

### Comparing `notebook-7.2.0rc0/notebook/static/9331.bundle.js` & `notebook-7.2.0rc1/notebook/static/9331.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9335.bundle.js` & `notebook-7.2.0rc1/notebook/static/9335.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [9335], {
         89335: (e, a, t) => {
             t.r(a), t.d(a, {
                 default: () => c
             });
-            var r = t(17894),
-                d = t(24554),
-                o = t(37267),
-                i = t(22620),
+            var r = t(25460),
+                d = t(23295),
+                o = t(12030),
+                i = t(35613),
                 m = t(20998),
-                s = t(40465);
+                s = t(12077);
             const n = "@jupyterlab/metadataform-extension:metadataforms";
             var l;
             ! function(e) {
                 e.loadSettingsMetadataForm = async function(e, a, t, r, d) {
                     var o;
                     let i, l = {};
```

### Comparing `notebook-7.2.0rc0/notebook/static/9341.bundle.js` & `notebook-7.2.0rc1/notebook/static/9341.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -14,21 +14,21 @@
                 IDefaultFileBrowser: () => le,
                 IFileBrowserCommands: () => de,
                 IFileBrowserFactory: () => ae,
                 LARGE_FILE_SIZE: () => Q,
                 TogglableHiddenFileBrowserModel: () => se,
                 Uploader: () => he
             });
-            var i = s(96049),
-                r = s(1167),
-                n = s(70611),
-                o = s(37267),
-                a = s(22620),
+            var i = s(53312),
+                r = s(68722),
+                n = s(87408),
+                o = s(12030),
+                a = s(35613),
                 l = s(63485),
-                d = s(91942),
+                d = s(5094),
                 h = s(33625),
                 c = s(20998),
                 m = s(18395);
             const u = "jp-BreadCrumbs-home",
                 p = "jp-BreadCrumbs-preferred",
                 _ = "jp-BreadCrumbs-item",
                 f = ["/", "../../", "../", ""],
@@ -201,15 +201,15 @@
                     for (let t = 0; t < 4; t++) {
                         const t = document.createElement("span");
                         t.textContent = "/", e.push(t)
                     }
                     return e
                 }
             }(w || (w = {}));
-            var b = s(10979),
+            var b = s(65903),
                 C = s(99615),
                 E = s(49503),
                 D = s(81997),
                 L = s(24475);
             const I = "jp-DirListing-header",
                 x = "jp-DirListing-headerItem",
                 k = "jp-DirListing-headerItemText",
@@ -1683,15 +1683,15 @@
                 e.createUploadInput = function() {
                     const e = document.createElement("input");
                     return e.type = "file", e.multiple = !0, e
                 }, e.translateToolTip = function(e) {
                     return (e = e || o.nullTranslator).load("jupyterlab").__("Upload Files")
                 }
             }(ce || (ce = {}));
-            var me = s(27829),
+            var me = s(71098),
                 ue = s(78156),
                 pe = s.n(ue);
 
             function _e(e) {
                 const t = (e.translator || o.nullTranslator).load("jupyterlab");
                 return pe().createElement(me.GroupItem, {
                     spacing: 4
```

### Comparing `notebook-7.2.0rc0/notebook/static/9380.bundle.js` & `notebook-7.2.0rc1/notebook/static/9380.bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [9380], {
         19380: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => c
             });
-            var a = o(96049),
-                n = o(50845),
-                r = o(37267),
-                u = o(18625),
+            var a = o(53312),
+                n = o(29879),
+                r = o(12030),
+                u = o(93712),
                 l = o(78156);
             const s = [{
                 text: "About Jupyter",
                 url: "https://jupyter.org"
             }, {
                 text: "Markdown Reference",
                 url: "https://commonmark.org/help/"
```

### Comparing `notebook-7.2.0rc0/notebook/static/9425.bundle.js` & `notebook-7.2.0rc1/notebook/static/9425.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9558.bundle.js` & `notebook-7.2.0rc1/notebook/static/9558.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9604.bundle.js` & `notebook-7.2.0rc1/notebook/static/9604.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9605.bundle.js` & `notebook-7.2.0rc1/notebook/static/9605.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -52,25 +52,25 @@
                 createDefaultFactory: () => be,
                 createToolbarFactory: () => Ce,
                 setToolbar: () => xe,
                 showDialog: () => b,
                 showErrorMessage: () => y,
                 translateKernelStatuses: () => A
             });
-            var n, i, s = r(22620),
-                o = r(37267),
+            var n, i, s = r(35613),
+                o = r(12030),
                 a = r(63485),
                 l = r(78156),
                 c = r.n(l),
-                u = r(1167),
+                u = r(68722),
                 d = r(33625),
                 h = r(20998),
                 p = r(81997),
                 f = r(49503),
-                m = r(96692);
+                m = r(41053);
             class g {
                 constructor(e) {
                     this._currentChanged = new p.Signal(this), this._deferred = null, this._isDisposed = !1, this._widgetAdded = new p.Signal(this), this._widgetUpdated = new p.Signal(this);
                     const t = this._focusTracker = new a.FocusTracker,
                         r = this._pool = new m.RestorablePool(e);
                     this.namespace = e.namespace, t.currentChanged.connect(((e, t) => {
                         t.newValue !== this.currentWidget && (r.current = t.newValue)
@@ -979,15 +979,15 @@
                     if (1 === c.length) {
                         const e = c[0];
                         return console.warn("No exact match found for " + e + ", using kernel " + e + " that matches language=" + s), e
                     }
                     return l
                 }, e.populateKernelSelect = n
             }(i || (i = {}));
-            var C, x, E, S, T = r(27829);
+            var C, x, E, S, T = r(71098);
 
             function A(e) {
                 const t = (e = e || o.nullTranslator).load("jupyterlab");
                 return {
                     unknown: t.__("Unknown"),
                     starting: t.__("Starting"),
                     idle: t.__("Idle"),
@@ -1451,15 +1451,15 @@
                 }
                 getValue() {
                     let e = [];
                     for (let t of this._list.options) t.selected && !t.classList.contains("hidden") && e.push(t.value || t.text);
                     return e
                 }
             }
-            var z, K, W, Y = r(70611);
+            var z, K, W, Y = r(87408);
             ! function(e) {
                 function t(t) {
                     return !("object" != typeof t || !t) && e.symbol in t
                 }
                 async function r(e) {
                     const t = "string" == typeof e,
                         r = function() {
@@ -2609,16 +2609,16 @@
                         case "spacer":
                             return s.Toolbar.createSpacerItem();
                         default:
                             return new a.Widget
                     }
                 }
             }
-            var ye = r(58959),
-                _e = r(24554);
+            var ye = r(31231),
+                _e = r(23295);
             const ve = 50,
                 we = "jupyter.lab.toolbars";
 
             function Ce(e, t, r, n, i, s = "toolbar") {
                 const o = new ye.ObservableList({
                     itemCmp: (e, t) => h.JSONExt.deepEqual(e, t)
                 });
```

### Comparing `notebook-7.2.0rc0/notebook/static/9638.bundle.js` & `notebook-7.2.0rc1/notebook/static/9638.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,17 +4,17 @@
         68771: (e, t, n) => {
             n.r(t), n.d(t, {
                 ILauncher: () => a,
                 Launcher: () => p,
                 LauncherModel: () => u
             });
             const a = new(n(20998).Token)("@jupyterlab/launcher:ILauncher", "A service for the application activity launcher.\n  Use this to add your extension activities to the launcher panel.");
-            var s, r = n(96049),
-                c = n(37267),
-                o = n(22620),
+            var s, r = n(53312),
+                c = n(12030),
+                o = n(35613),
                 i = n(33625),
                 l = n(2549),
                 d = n(14421),
                 h = n(63485),
                 m = n(78156);
             class u extends o.VDomModel {
                 constructor() {
```

### Comparing `notebook-7.2.0rc0/notebook/static/9674eb1bd55047179038.svg` & `notebook-7.2.0rc1/notebook/static/9674eb1bd55047179038.svg`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9676.bundle.js` & `notebook-7.2.0rc1/notebook/static/9676.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9680.bundle.js` & `notebook-7.2.0rc1/notebook/static/9680.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
                 IMarkdownViewerTracker: () => a,
                 MarkdownDocument: () => w,
                 MarkdownViewer: () => f,
                 MarkdownViewerFactory: () => _,
                 MarkdownViewerTableOfContentsFactory: () => s,
                 MarkdownViewerTableOfContentsModel: () => i
             });
-            var r = n(87017);
+            var r = n(79426);
             class i extends r.TableOfContentsModel {
                 constructor(e, t, n) {
                     super(e, n), this.parser = t
                 }
                 get documentType() {
                     return "markdown-viewer"
                 }
@@ -66,19 +66,19 @@
                             e.content.rendered.disconnect(a), n.activeHeadingChanged.disconnect(o), n.headingsChanged.disconnect(a)
                         }))
                     })), n
                 }
             }
             var o = n(20998);
             const a = new o.Token("@jupyterlab/markdownviewer:IMarkdownViewerTracker", "A widget tracker for markdown\n  document viewers. Use this if you want to iterate over and interact with rendered markdown documents.");
-            var d = n(96049),
-                c = n(1167),
-                l = n(10979),
-                h = n(13408),
-                u = n(37267),
+            var d = n(53312),
+                c = n(68722),
+                l = n(65903),
+                h = n(81221),
+                u = n(12030),
                 g = n(81997),
                 m = n(63485);
             const p = "text/markdown";
             class f extends m.Widget {
                 constructor(e) {
                     super(), this._config = {
                         ...f.defaultConfig
```

### Comparing `notebook-7.2.0rc0/notebook/static/9685.bundle.js` & `notebook-7.2.0rc1/notebook/static/7252.bundle.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [9685, 7252], {
+    [7252, 9685], {
         79685: (e, t, r) => {
             r.r(t), r.d(t, {
                 default: () => k
             });
-            var n, a = r(2922),
-                o = r(96049),
-                d = r(1167),
-                i = r(97592),
-                c = r(13408),
-                s = r(24554),
-                w = r(87017),
-                m = r(37267);
+            var n, a = r(44604),
+                o = r(53312),
+                d = r(68722),
+                i = r(3991),
+                c = r(81221),
+                s = r(23295),
+                w = r(79426),
+                m = r(12030);
             ! function(e) {
                 e.markdownPreview = "markdownviewer:open", e.markdownEditor = "markdownviewer:edit"
             }(n || (n = {}));
             const p = "Markdown Preview",
                 l = {
                     activate: function(e, t, r, a, s, w, m) {
                         const k = r.load("jupyterlab"),
```

### Comparing `notebook-7.2.0rc0/notebook/static/9752.bundle.js` & `notebook-7.2.0rc1/notebook/static/9752.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2,17 +2,17 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [9752], {
         69752: (e, t, r) => {
             "use strict";
             r.d(t, {
                 Component: () => ne
             });
-            var a = r(49269),
-                n = r(37267),
-                s = r(22620),
+            var a = r(30525),
+                n = r(12030),
+                s = r(35613),
                 o = r(92209),
                 i = r(20998),
                 l = r(78156),
                 u = r.n(l),
                 c = r(5464),
                 b = r.n(c);
```

### Comparing `notebook-7.2.0rc0/notebook/static/9799.bundle.js` & `notebook-7.2.0rc1/notebook/static/9799.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9821.bundle.js` & `notebook-7.2.0rc1/notebook/static/9821.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,21 +3,21 @@
     [9821], {
         69821: (e, t, n) => {
             n.r(t), n.d(t, {
                 IPluginManager: () => y,
                 PluginListModel: () => h,
                 Plugins: () => g
             });
-            var i = n(96049),
-                s = n(1167),
-                a = n(70611),
-                r = n(22620),
+            var i = n(53312),
+                s = n(68722),
+                a = n(87408),
+                r = n(35613),
                 l = n(81997),
                 o = n(20998),
-                d = n(37267),
+                d = n(12030),
                 c = n(78156);
 
             function u(e) {
                 return c.createElement("div", {
                     className: "jp-pluginmanager-PluginInUseMessage"
                 }, e.trans.__('While the plugin "%1" is not required by other enabled plugins, some plugins provide optional features depending on it. These plugins are:', e.plugin.id), c.createElement("ul", null, e.optionalDependants.map((e => c.createElement("li", {
                     key: "optionalDependantsDialog-" + e.id
```

### Comparing `notebook-7.2.0rc0/notebook/static/9834b82ad26e2a37583d.woff2` & `notebook-7.2.0rc1/notebook/static/9834b82ad26e2a37583d.woff2`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/9852.bundle.js` & `notebook-7.2.0rc1/notebook/static/9852.bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,16 +4,16 @@
         22924: (t, e, o) => {
             o.r(e), o.d(e, {
                 FormWidget: () => r,
                 IMetadataFormProvider: () => g,
                 MetadataFormProvider: () => v,
                 MetadataFormWidget: () => _
             });
-            var a = o(96049),
-                i = o(22620),
+            var a = o(53312),
+                i = o(35613),
                 s = o(27478),
                 l = o.n(s),
                 d = o(78156),
                 n = o.n(d);
             class r extends a.ReactWidget {
                 constructor(t) {
                     super(), this.addClass("jp-FormWidget"), this._props = t
@@ -36,17 +36,17 @@
                         },
                         compact: !0,
                         showModifiedFromDefault: this._props.showModified,
                         translator: this._props.translator
                     })
                 }
             }
-            var h, m = o(17894),
-                p = o(24554),
-                c = o(37267),
+            var h, m = o(25460),
+                p = o(23295),
+                c = o(12030),
                 u = o(20998),
                 f = o(63485);
             class _ extends m.NotebookTools.Tool {
                 constructor(t) {
                     super(), this.updateMetadata = (t, e) => {
                         var o, a, i, s, l, d, n, r;
                         if (null == this.notebookTools) return;
```

### Comparing `notebook-7.2.0rc0/notebook/static/9866.bundle.js` & `notebook-7.2.0rc1/notebook/static/9866.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/a009bea404f7a500ded4.woff` & `notebook-7.2.0rc1/notebook/static/a009bea404f7a500ded4.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/a3b9817780214caf01e8.svg` & `notebook-7.2.0rc1/notebook/static/a3b9817780214caf01e8.svg`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/af04542b29eaac04550a.woff` & `notebook-7.2.0rc1/notebook/static/af04542b29eaac04550a.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/af6397503fcefbd61397.ttf` & `notebook-7.2.0rc1/notebook/static/af6397503fcefbd61397.ttf`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/af96f67d7accf5fd2a4a.woff` & `notebook-7.2.0rc1/notebook/static/af96f67d7accf5fd2a4a.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/b418136e3b384baaadec.woff` & `notebook-7.2.0rc1/notebook/static/b418136e3b384baaadec.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/be0a084962d8066884f7.svg` & `notebook-7.2.0rc1/notebook/static/be0a084962d8066884f7.svg`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/bundle.js` & `notebook-7.2.0rc1/notebook/static/bundle.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,497 +1,497 @@
 var _JUPYTERLAB;
 (() => {
-    var e, t, r, l, a, n, o, i, s, u, m, c, h, p, d, b, f, P, y, j, g = {
-            37559: (e, t, r) => {
-                Promise.all([r.e(9136), r.e(1167), r.e(6807), r.e(8602), r.e(8781)]).then(r.bind(r, 60880))
+    var e, t, l, r, a, n, o, i, s, u, m, h, p, d, b, f, P, y, c, j, g = {
+            37559: (e, t, l) => {
+                Promise.all([l.e(9136), l.e(8722), l.e(9625), l.e(7708), l.e(8781)]).then(l.bind(l, 60880))
             },
-            68444: (e, t, r) => {
-                r.p = function(e) {
+            68444: (e, t, l) => {
+                l.p = function(e) {
                     let t = Object.create(null);
                     if ("undefined" != typeof document && document) {
                         const e = document.getElementById("jupyter-config-data");
                         e && (t = JSON.parse(e.textContent || "{}"))
                     }
                     return t.fullStaticUrl || ""
                 }() + "/"
             }
         },
         x = {};
 
     function v(e) {
         var t = x[e];
         if (void 0 !== t) return t.exports;
-        var r = x[e] = {
+        var l = x[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
-        return g[e].call(r.exports, r, r.exports, v), r.loaded = !0, r.exports
+        return g[e].call(l.exports, l, l.exports, v), l.loaded = !0, l.exports
     }
     v.m = g, v.c = x, v.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
         return v.d(t, {
             a: t
         }), t
-    }, t = Object.getPrototypeOf ? e => Object.getPrototypeOf(e) : e => e.__proto__, v.t = function(r, l) {
-        if (1 & l && (r = this(r)), 8 & l) return r;
-        if ("object" == typeof r && r) {
-            if (4 & l && r.__esModule) return r;
-            if (16 & l && "function" == typeof r.then) return r
+    }, t = Object.getPrototypeOf ? e => Object.getPrototypeOf(e) : e => e.__proto__, v.t = function(l, r) {
+        if (1 & r && (l = this(l)), 8 & r) return l;
+        if ("object" == typeof l && l) {
+            if (4 & r && l.__esModule) return l;
+            if (16 & r && "function" == typeof l.then) return l
         }
         var a = Object.create(null);
         v.r(a);
         var n = {};
         e = e || [null, t({}), t([]), t(t)];
-        for (var o = 2 & l && r;
-            "object" == typeof o && !~e.indexOf(o); o = t(o)) Object.getOwnPropertyNames(o).forEach((e => n[e] = () => r[e]));
-        return n.default = () => r, v.d(a, n), a
+        for (var o = 2 & r && l;
+            "object" == typeof o && !~e.indexOf(o); o = t(o)) Object.getOwnPropertyNames(o).forEach((e => n[e] = () => l[e]));
+        return n.default = () => l, v.d(a, n), a
     }, v.d = (e, t) => {
-        for (var r in t) v.o(t, r) && !v.o(e, r) && Object.defineProperty(e, r, {
+        for (var l in t) v.o(t, l) && !v.o(e, l) && Object.defineProperty(e, l, {
             enumerable: !0,
-            get: t[r]
+            get: t[l]
         })
-    }, v.f = {}, v.e = e => Promise.all(Object.keys(v.f).reduce(((t, r) => (v.f[r](e, t), t)), [])), v.u = e => e + ".bundle.js", v.g = function() {
+    }, v.f = {}, v.e = e => Promise.all(Object.keys(v.f).reduce(((t, l) => (v.f[l](e, t), t)), [])), v.u = e => e + ".bundle.js", v.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), v.hmd = e => ((e = Object.create(e)).children || (e.children = []), Object.defineProperty(e, "exports", {
         enumerable: !0,
         set: () => {
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
-    }), e), v.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), r = {}, l = "_JUPYTERLAB.CORE_OUTPUT:", v.l = (e, t, a, n) => {
-        if (r[e]) r[e].push(t);
+    }), e), v.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), l = {}, r = "_JUPYTERLAB.CORE_OUTPUT:", v.l = (e, t, a, n) => {
+        if (l[e]) l[e].push(t);
         else {
             var o, i;
             if (void 0 !== a)
                 for (var s = document.getElementsByTagName("script"), u = 0; u < s.length; u++) {
                     var m = s[u];
-                    if (m.getAttribute("src") == e || m.getAttribute("data-webpack") == l + a) {
+                    if (m.getAttribute("src") == e || m.getAttribute("data-webpack") == r + a) {
                         o = m;
                         break
                     }
                 }
-            o || (i = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, v.nc && o.setAttribute("nonce", v.nc), o.setAttribute("data-webpack", l + a), o.src = e), r[e] = [t];
-            var c = (t, l) => {
-                    o.onerror = o.onload = null, clearTimeout(h);
-                    var a = r[e];
-                    if (delete r[e], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(l))), t) return t(l)
+            o || (i = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, v.nc && o.setAttribute("nonce", v.nc), o.setAttribute("data-webpack", r + a), o.src = e), l[e] = [t];
+            var h = (t, r) => {
+                    o.onerror = o.onload = null, clearTimeout(p);
+                    var a = l[e];
+                    if (delete l[e], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(r))), t) return t(r)
                 },
-                h = setTimeout(c.bind(null, void 0, {
+                p = setTimeout(h.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = c.bind(null, o.onerror), o.onload = c.bind(null, o.onload), i && document.head.appendChild(o)
+            o.onerror = h.bind(null, o.onerror), o.onload = h.bind(null, o.onload), i && document.head.appendChild(o)
         }
     }, v.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, v.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         v.S = {};
         var e = {},
             t = {};
-        v.I = (r, l) => {
-            l || (l = []);
-            var a = t[r];
-            if (a || (a = t[r] = {}), !(l.indexOf(a) >= 0)) {
-                if (l.push(a), e[r]) return e[r];
-                v.o(v.S, r) || (v.S[r] = {});
-                var n = v.S[r],
+        v.I = (l, r) => {
+            r || (r = []);
+            var a = t[l];
+            if (a || (a = t[l] = {}), !(r.indexOf(a) >= 0)) {
+                if (r.push(a), e[l]) return e[l];
+                v.o(v.S, l) || (v.S[l] = {});
+                var n = v.S[l],
                     o = "_JUPYTERLAB.CORE_OUTPUT",
-                    i = (e, t, r, l) => {
+                    i = (e, t, l, r) => {
                         var a = n[e] = n[e] || {},
                             i = a[t];
-                        (!i || !i.loaded && (!l != !i.eager ? l : o > i.from)) && (a[t] = {
-                            get: r,
+                        (!i || !i.loaded && (!r != !i.eager ? r : o > i.from)) && (a[t] = {
+                            get: l,
                             from: o,
-                            eager: !!l
+                            eager: !!r
                         })
                     },
                     s = [];
-                return "default" === r && (i("@codemirror/commands", "6.3.3", (() => Promise.all([v.e(7450), v.e(3546), v.e(9843), v.e(9352), v.e(7592)]).then((() => () => v(67450))))), i("@codemirror/lang-markdown", "6.2.4", (() => Promise.all([v.e(5850), v.e(9239), v.e(9799), v.e(7866), v.e(6271), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(7592)]).then((() => () => v(76271))))), i("@codemirror/language", "6.10.1", (() => Promise.all([v.e(1584), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(31584))))), i("@codemirror/search", "6.5.6", (() => Promise.all([v.e(5261), v.e(3546), v.e(9843)]).then((() => () => v(25261))))), i("@codemirror/state", "6.4.1", (() => v.e(2323).then((() => () => v(92323))))), i("@codemirror/view", "6.26.1", (() => Promise.all([v.e(2955), v.e(9843)]).then((() => () => v(22955))))), i("@jupyter-notebook/application-extension", "7.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(1167), v.e(2922), v.e(4554), v.e(3408), v.e(2549), v.e(979), v.e(845), v.e(1942), v.e(106), v.e(6807), v.e(8625), v.e(8579)]).then((() => () => v(88579))))), i("@jupyter-notebook/application", "7.2.0-rc.0", (() => Promise.all([v.e(901), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(3625), v.e(1167), v.e(2922), v.e(3408), v.e(2549), v.e(7934), v.e(979), v.e(9503), v.e(4421), v.e(5135)]).then((() => () => v(45135))))), i("@jupyter-notebook/console-extension", "7.2.0-rc.0", (() => Promise.all([v.e(3625), v.e(1167), v.e(2922), v.e(106), v.e(6807), v.e(4645)]).then((() => () => v(94645))))), i("@jupyter-notebook/docmanager-extension", "7.2.0-rc.0", (() => Promise.all([v.e(1997), v.e(1167), v.e(1942), v.e(6807), v.e(1650)]).then((() => () => v(71650))))), i("@jupyter-notebook/documentsearch-extension", "7.2.0-rc.0", (() => Promise.all([v.e(6862), v.e(6807), v.e(4382)]).then((() => () => v(54382))))), i("@jupyter-notebook/help-extension", "7.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(8156), v.e(845), v.e(8625), v.e(9380)]).then((() => () => v(19380))))), i("@jupyter-notebook/notebook-extension", "7.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(8156), v.e(1167), v.e(4554), v.e(7934), v.e(845), v.e(1942), v.e(7894), v.e(6807), v.e(5573)]).then((() => () => v(5573))))), i("@jupyter-notebook/terminal-extension", "7.2.0-rc.0", (() => Promise.all([v.e(3625), v.e(1167), v.e(2922), v.e(6807), v.e(9200), v.e(5601)]).then((() => () => v(95601))))), i("@jupyter-notebook/tree-extension", "7.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(1167), v.e(4554), v.e(2751), v.e(5729), v.e(1131), v.e(2367), v.e(3768)]).then((() => () => v(83768))))), i("@jupyter-notebook/tree", "7.2.0-rc.0", (() => Promise.all([v.e(998), v.e(3485), v.e(2620), v.e(3146)]).then((() => () => v(73146))))), i("@jupyter-notebook/ui-components", "7.2.0-rc.0", (() => Promise.all([v.e(2620), v.e(9068)]).then((() => () => v(59068))))), i("@jupyter/ydoc", "2.0.1", (() => Promise.all([v.e(35), v.e(998), v.e(1997), v.e(7843)]).then((() => () => v(50035))))), i("@jupyterlab/application-extension", "4.2.0-rc.0", (() => Promise.all([v.e(3881), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(3625), v.e(1167), v.e(2922), v.e(4554), v.e(2549), v.e(7829), v.e(6692), v.e(6934), v.e(6724)]).then((() => () => v(92871))))), i("@jupyterlab/application", "4.2.0-rc.0", (() => Promise.all([v.e(901), v.e(6853), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(3625), v.e(1167), v.e(3408), v.e(2549), v.e(7934), v.e(979), v.e(611), v.e(9503), v.e(4421), v.e(4771)]).then((() => () => v(76853))))), i("@jupyterlab/apputils-extension", "4.2.0-rc.0", (() => Promise.all([v.e(5099), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(3625), v.e(1167), v.e(2922), v.e(4554), v.e(2549), v.e(7934), v.e(979), v.e(7829), v.e(611), v.e(845), v.e(8395), v.e(6692), v.e(6934), v.e(8005), v.e(3892)]).then((() => () => v(25099))))), i("@jupyterlab/apputils", "4.3.0-rc.0", (() => Promise.all([v.e(9605), v.e(998), v.e(7267), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(4554), v.e(2549), v.e(7829), v.e(611), v.e(9503), v.e(8395), v.e(6692), v.e(8959), v.e(3752)]).then((() => () => v(89605))))), i("@jupyterlab/attachments", "4.2.0-rc.0", (() => Promise.all([v.e(1997), v.e(3408), v.e(8959), v.e(4042)]).then((() => () => v(44042))))), i("@jupyterlab/cell-toolbar-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(4554), v.e(2122)]).then((() => () => v(92122))))), i("@jupyterlab/cell-toolbar", "4.2.0-rc.0", (() => Promise.all([v.e(6049), v.e(2620), v.e(1997), v.e(3625), v.e(8959), v.e(7386)]).then((() => () => v(37386))))), i("@jupyterlab/cells", "4.2.0-rc.0", (() => Promise.all([v.e(2479), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(3408), v.e(7934), v.e(9503), v.e(2839), v.e(8395), v.e(7017), v.e(6862), v.e(3546), v.e(9269), v.e(4475), v.e(7508), v.e(6726), v.e(8289)]).then((() => () => v(72479))))), i("@jupyterlab/celltags-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(2620), v.e(8156), v.e(3625), v.e(7894), v.e(5346)]).then((() => () => v(15346))))), i("@jupyterlab/codeeditor", "4.2.0-rc.0", (() => Promise.all([v.e(7391), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(7829), v.e(8959), v.e(7508)]).then((() => () => v(77391))))), i("@jupyterlab/codemirror-extension", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(2620), v.e(8156), v.e(2922), v.e(4554), v.e(7829), v.e(2839), v.e(9269), v.e(7478), v.e(3831), v.e(7592), v.e(7655)]).then((() => () => v(97655))))), i("@jupyterlab/codemirror", "4.2.0-rc.0", (() => Promise.all([v.e(9799), v.e(5263), v.e(998), v.e(7267), v.e(1997), v.e(1167), v.e(2839), v.e(6862), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(3831), v.e(7592), v.e(7843)]).then((() => () => v(95263))))), i("@jupyterlab/completer-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(2620), v.e(8156), v.e(4554), v.e(6934), v.e(9144), v.e(3340)]).then((() => () => v(33340))))), i("@jupyterlab/completer", "4.2.0-rc.0", (() => Promise.all([v.e(2944), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(3625), v.e(1167), v.e(3408), v.e(9503), v.e(2839), v.e(8395), v.e(3546), v.e(9843)]).then((() => () => v(62944))))), i("@jupyterlab/console-extension", "4.2.0-rc.0", (() => Promise.all([v.e(6748), v.e(998), v.e(7267), v.e(6049), v.e(2620), v.e(3625), v.e(2922), v.e(4554), v.e(3408), v.e(2549), v.e(2839), v.e(845), v.e(4421), v.e(2751), v.e(106), v.e(5651), v.e(9144)]).then((() => () => v(86748))))), i("@jupyterlab/console", "4.2.0-rc.0", (() => Promise.all([v.e(2636), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(1167), v.e(3408), v.e(8959), v.e(3546), v.e(9843), v.e(9615), v.e(7406), v.e(7508)]).then((() => () => v(72636))))), i("@jupyterlab/coreutils", "6.2.0-rc.0", (() => Promise.all([v.e(2866), v.e(998), v.e(1997)]).then((() => () => v(2866))))), i("@jupyterlab/csvviewer-extension", "4.2.0-rc.0", (() => Promise.all([v.e(1827), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(1167), v.e(2922), v.e(4554), v.e(979), v.e(845), v.e(6862)]).then((() => () => v(41827))))), i("@jupyterlab/csvviewer", "4.2.0-rc.0", (() => Promise.all([v.e(8032), v.e(998), v.e(7267), v.e(3485), v.e(2620), v.e(1997), v.e(1167), v.e(979), v.e(9072), v.e(5313)]).then((() => () => v(65313))))), i("@jupyterlab/debugger-extension", "4.2.0-rc.0", (() => Promise.all([v.e(2184), v.e(7267), v.e(6049), v.e(1167), v.e(2922), v.e(4554), v.e(3408), v.e(979), v.e(2839), v.e(7894), v.e(106), v.e(7406), v.e(2703), v.e(8603), v.e(9713)]).then((() => () => v(42184))))), i("@jupyterlab/debugger", "4.2.0-rc.0", (() => Promise.all([v.e(1884), v.e(6621), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(3408), v.e(7934), v.e(2839), v.e(8959), v.e(3546), v.e(9843), v.e(7406)]).then((() => () => v(36621))))), i("@jupyterlab/docmanager-extension", "4.2.0-rc.0", (() => Promise.all([v.e(8471), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(2922), v.e(4554), v.e(7829), v.e(6692), v.e(1942)]).then((() => () => v(8471))))), i("@jupyterlab/docmanager", "4.2.0-rc.0", (() => Promise.all([v.e(7543), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(2549), v.e(7934), v.e(979), v.e(7829), v.e(9503), v.e(4421)]).then((() => () => v(37543))))), i("@jupyterlab/docregistry", "4.2.0-rc.0", (() => Promise.all([v.e(2489), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(3408), v.e(2549), v.e(9503), v.e(2839)]).then((() => () => v(72489))))), i("@jupyterlab/documentsearch-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(2922), v.e(4554), v.e(6862), v.e(4212)]).then((() => () => v(24212))))), i("@jupyterlab/documentsearch", "4.2.0-rc.0", (() => Promise.all([v.e(6999), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(2549), v.e(7934), v.e(6934)]).then((() => () => v(36999))))), i("@jupyterlab/extensionmanager-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(2620), v.e(2922), v.e(4554), v.e(2311)]).then((() => () => v(22311))))), i("@jupyterlab/extensionmanager", "4.2.0-rc.0", (() => Promise.all([v.e(9151), v.e(7267), v.e(6049), v.e(2620), v.e(8156), v.e(1167), v.e(7934), v.e(611)]).then((() => () => v(59151))))), i("@jupyterlab/filebrowser-extension", "4.2.0-rc.0", (() => Promise.all([v.e(893), v.e(7267), v.e(6049), v.e(2620), v.e(3625), v.e(1167), v.e(2922), v.e(4554), v.e(7829), v.e(6692), v.e(1942), v.e(6934), v.e(2751)]).then((() => () => v(30893))))), i("@jupyterlab/filebrowser", "4.2.0-rc.0", (() => Promise.all([v.e(9341), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(7934), v.e(979), v.e(7829), v.e(611), v.e(9503), v.e(8395), v.e(1942), v.e(4475), v.e(9615)]).then((() => () => v(39341))))), i("@jupyterlab/fileeditor-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7603), v.e(7267), v.e(6049), v.e(2620), v.e(3625), v.e(1167), v.e(2922), v.e(4554), v.e(7829), v.e(2839), v.e(845), v.e(7017), v.e(6862), v.e(9269), v.e(2751), v.e(106), v.e(2138), v.e(5651), v.e(2703), v.e(9144), v.e(3831)]).then((() => () => v(97603))))), i("@jupyterlab/fileeditor", "4.2.0-rc.0", (() => Promise.all([v.e(1833), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(979), v.e(7829), v.e(2839), v.e(7017), v.e(9269), v.e(2138)]).then((() => () => v(31833))))), i("@jupyterlab/help-extension", "4.2.0-rc.0", (() => Promise.all([v.e(1496), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(1167), v.e(2922), v.e(611), v.e(845), v.e(4475)]).then((() => () => v(91496))))), i("@jupyterlab/htmlviewer-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(2620), v.e(2922), v.e(4554), v.e(6962)]).then((() => () => v(56962))))), i("@jupyterlab/htmlviewer", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(2620), v.e(1997), v.e(8156), v.e(1167), v.e(979), v.e(5325)]).then((() => () => v(35325))))), i("@jupyterlab/hub-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(1167), v.e(2922), v.e(6893)]).then((() => () => v(56893))))), i("@jupyterlab/imageviewer-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(2922), v.e(6139)]).then((() => () => v(56139))))), i("@jupyterlab/imageviewer", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(6049), v.e(3485), v.e(1167), v.e(979), v.e(7900)]).then((() => () => v(67900))))), i("@jupyterlab/javascript-extension", "4.2.0-rc.0", (() => Promise.all([v.e(3408), v.e(5733)]).then((() => () => v(65733))))), i("@jupyterlab/json-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(8156), v.e(8005), v.e(690)]).then((() => () => v(60690))))), i("@jupyterlab/launcher", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(3625), v.e(2549), v.e(4421), v.e(8771)]).then((() => () => v(68771))))), i("@jupyterlab/logconsole", "4.2.0-rc.0", (() => Promise.all([v.e(2089), v.e(998), v.e(7267), v.e(3485), v.e(1997), v.e(3408), v.e(6726)]).then((() => () => v(2089))))), i("@jupyterlab/lsp-extension", "4.2.0-rc.0", (() => Promise.all([v.e(3466), v.e(998), v.e(7267), v.e(6049), v.e(2620), v.e(1997), v.e(8156), v.e(4554), v.e(7934), v.e(2138), v.e(5729)]).then((() => () => v(83466))))), i("@jupyterlab/lsp", "4.2.0-rc.0", (() => Promise.all([v.e(3512), v.e(998), v.e(7267), v.e(6049), v.e(1997), v.e(1167), v.e(979), v.e(611)]).then((() => () => v(13512))))), i("@jupyterlab/mainmenu-extension", "4.2.0-rc.0", (() => Promise.all([v.e(545), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(3625), v.e(1167), v.e(2922), v.e(4554), v.e(611), v.e(845), v.e(1942), v.e(2751)]).then((() => () => v(60545))))), i("@jupyterlab/mainmenu", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(6049), v.e(3485), v.e(2620), v.e(3625), v.e(2007)]).then((() => () => v(12007))))), i("@jupyterlab/markdownviewer-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(1167), v.e(2922), v.e(4554), v.e(3408), v.e(7017), v.e(5910), v.e(9685)]).then((() => () => v(79685))))), i("@jupyterlab/markdownviewer", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(1997), v.e(1167), v.e(3408), v.e(979), v.e(7017), v.e(9680)]).then((() => () => v(99680))))), i("@jupyterlab/markedparser-extension", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(1167), v.e(3408), v.e(9269), v.e(3149), v.e(9268)]).then((() => () => v(79268))))), i("@jupyterlab/mathjax-extension", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(3408), v.e(1408)]).then((() => () => v(11408))))), i("@jupyterlab/mermaid-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(3149), v.e(9161)]).then((() => () => v(79161))))), i("@jupyterlab/mermaid", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(3485), v.e(1167), v.e(2615)]).then((() => () => v(92615))))), i("@jupyterlab/metadataform-extension", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(2620), v.e(4554), v.e(7894), v.e(465), v.e(9335)]).then((() => () => v(89335))))), i("@jupyterlab/metadataform", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(4554), v.e(7894), v.e(7478), v.e(2924)]).then((() => () => v(22924))))), i("@jupyterlab/nbformat", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(3325)]).then((() => () => v(23325))))), i("@jupyterlab/notebook-extension", "4.2.0-rc.0", (() => Promise.all([v.e(1962), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(3625), v.e(1167), v.e(2922), v.e(4554), v.e(3408), v.e(2549), v.e(7934), v.e(7829), v.e(611), v.e(9503), v.e(2839), v.e(845), v.e(6692), v.e(1942), v.e(8959), v.e(7017), v.e(6862), v.e(9269), v.e(7894), v.e(2751), v.e(2138), v.e(7406), v.e(5651), v.e(9144), v.e(6724), v.e(8603), v.e(465), v.e(8602)]).then((() => () => v(51962))))), i("@jupyterlab/notebook", "4.2.0-rc.0", (() => Promise.all([v.e(374), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(7934), v.e(979), v.e(7829), v.e(611), v.e(9503), v.e(2839), v.e(8395), v.e(8959), v.e(4421), v.e(7017), v.e(6862), v.e(4475), v.e(2138), v.e(9615), v.e(7406), v.e(7508), v.e(1692)]).then((() => () => v(90374))))), i("@jupyterlab/observables", "5.2.0-rc.0", (() => Promise.all([v.e(170), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503)]).then((() => () => v(10170))))), i("@jupyterlab/outputarea", "4.2.0-rc.0", (() => Promise.all([v.e(7226), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(1997), v.e(3625), v.e(3408), v.e(611), v.e(8959), v.e(4421), v.e(1692)]).then((() => () => v(47226))))), i("@jupyterlab/pdf-extension", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(3485), v.e(2549), v.e(4058)]).then((() => () => v(84058))))), i("@jupyterlab/pluginmanager-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(2620), v.e(2922), v.e(7355), v.e(3187)]).then((() => () => v(53187))))), i("@jupyterlab/pluginmanager", "4.2.0-rc.0", (() => Promise.all([v.e(9821), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(1167), v.e(611)]).then((() => () => v(69821))))), i("@jupyterlab/property-inspector", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(3485), v.e(2620), v.e(1997), v.e(1198)]).then((() => () => v(41198))))), i("@jupyterlab/rendermime-interfaces", "3.10.0-rc.0", (() => v.e(5297).then((() => () => v(75297))))), i("@jupyterlab/rendermime", "4.2.0-rc.0", (() => Promise.all([v.e(2401), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(1997), v.e(1167), v.e(8959), v.e(1692), v.e(1070)]).then((() => () => v(72401))))), i("@jupyterlab/running-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7854), v.e(7267), v.e(6049), v.e(2620), v.e(1997), v.e(8156), v.e(1167), v.e(2922), v.e(7934), v.e(979), v.e(6692), v.e(1942), v.e(5729)]).then((() => () => v(97854))))), i("@jupyterlab/running", "4.2.0-rc.0", (() => Promise.all([v.e(1809), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(2549), v.e(8395)]).then((() => () => v(1809))))), i("@jupyterlab/services", "7.2.0-rc.0", (() => Promise.all([v.e(3676), v.e(998), v.e(1997), v.e(1167), v.e(2549), v.e(7934), v.e(6692)]).then((() => () => v(83676))))), i("@jupyterlab/settingeditor-extension", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(6049), v.e(2620), v.e(2922), v.e(4554), v.e(3408), v.e(2839), v.e(6692), v.e(7355), v.e(8633)]).then((() => () => v(98633))))), i("@jupyterlab/settingeditor", "4.2.0-rc.0", (() => Promise.all([v.e(3360), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(3408), v.e(7934), v.e(2839), v.e(6692), v.e(7478)]).then((() => () => v(63360))))), i("@jupyterlab/settingregistry", "4.2.0-rc.0", (() => Promise.all([v.e(7796), v.e(5649), v.e(998), v.e(1997), v.e(2549), v.e(6934)]).then((() => () => v(5649))))), i("@jupyterlab/shortcuts-extension", "5.0.0-rc.0", (() => Promise.all([v.e(113), v.e(998), v.e(7267), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(4554), v.e(2549), v.e(8395), v.e(6934), v.e(554)]).then((() => () => v(113))))), i("@jupyterlab/statedb", "4.2.0-rc.0", (() => Promise.all([v.e(4526), v.e(998), v.e(1997), v.e(4421)]).then((() => () => v(34526))))), i("@jupyterlab/statusbar", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(3485), v.e(2620), v.e(8156), v.e(3625), v.e(2549), v.e(3680)]).then((() => () => v(53680))))), i("@jupyterlab/terminal-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(2922), v.e(4554), v.e(611), v.e(845), v.e(5729), v.e(5651), v.e(9200), v.e(5912)]).then((() => () => v(15912))))), i("@jupyterlab/terminal", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(7267), v.e(3485), v.e(9503), v.e(8395), v.e(3213)]).then((() => () => v(53213))))), i("@jupyterlab/theme-dark-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(6627)]).then((() => () => v(6627))))), i("@jupyterlab/theme-dark-high-contrast-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(5254)]).then((() => () => v(95254))))), i("@jupyterlab/theme-light-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(5426)]).then((() => () => v(45426))))), i("@jupyterlab/toc-extension", "6.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(2620), v.e(2922), v.e(4554), v.e(7017), v.e(62)]).then((() => () => v(40062))))), i("@jupyterlab/toc", "6.2.0-rc.0", (() => Promise.all([v.e(5921), v.e(998), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(1167), v.e(3408), v.e(2549)]).then((() => () => v(75921))))), i("@jupyterlab/tooltip-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(3485), v.e(3625), v.e(1167), v.e(3408), v.e(7894), v.e(106), v.e(2703), v.e(5327), v.e(6604)]).then((() => () => v(6604))))), i("@jupyterlab/tooltip", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(3485), v.e(2620), v.e(3408), v.e(1647)]).then((() => () => v(51647))))), i("@jupyterlab/translation-extension", "4.2.0-rc.0", (() => Promise.all([v.e(7267), v.e(6049), v.e(2922), v.e(4554), v.e(845), v.e(6815)]).then((() => () => v(56815))))), i("@jupyterlab/translation", "4.2.0-rc.0", (() => Promise.all([v.e(7819), v.e(998), v.e(1167), v.e(611), v.e(6692)]).then((() => () => v(57819))))), i("@jupyterlab/ui-components-extension", "4.2.0-rc.0", (() => Promise.all([v.e(2620), v.e(3863)]).then((() => () => v(73863))))), i("@jupyterlab/ui-components", "4.2.0-rc.0", (() => Promise.all([v.e(1884), v.e(755), v.e(7811), v.e(7506), v.e(998), v.e(7267), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(2549), v.e(7934), v.e(9503), v.e(4421), v.e(6934), v.e(4475), v.e(8005), v.e(4885)]).then((() => () => v(7506))))), i("@jupyterlab/vega5-extension", "4.2.0-rc.0", (() => Promise.all([v.e(3485), v.e(6061)]).then((() => () => v(16061))))), i("@jupyterlab/workspaces", "4.2.0-rc.0", (() => Promise.all([v.e(998), v.e(1997), v.e(7934), v.e(1828)]).then((() => () => v(11828))))), i("@lezer/common", "1.2.1", (() => v.e(7997).then((() => () => v(97997))))), i("@lezer/highlight", "1.2.0", (() => Promise.all([v.e(3797), v.e(9352)]).then((() => () => v(23797))))), i("@lumino/algorithm", "2.0.1", (() => v.e(5614).then((() => () => v(15614))))), i("@lumino/application", "2.3.1", (() => Promise.all([v.e(6731), v.e(998), v.e(3485), v.e(6934)]).then((() => () => v(16731))))), i("@lumino/commands", "2.3.0", (() => Promise.all([v.e(3301), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(8395), v.e(554)]).then((() => () => v(43301))))), i("@lumino/coreutils", "2.1.2", (() => v.e(2756).then((() => () => v(12756))))), i("@lumino/datagrid", "2.3.1", (() => Promise.all([v.e(8929), v.e(998), v.e(3485), v.e(1997), v.e(3625), v.e(9503), v.e(8395), v.e(9615), v.e(554)]).then((() => () => v(98929))))), i("@lumino/disposable", "2.1.2", (() => Promise.all([v.e(1997), v.e(5451)]).then((() => () => v(65451))))), i("@lumino/domutils", "2.0.1", (() => v.e(1696).then((() => () => v(1696))))), i("@lumino/dragdrop", "2.1.4", (() => Promise.all([v.e(4291), v.e(2549)]).then((() => () => v(54291))))), i("@lumino/keyboard", "2.0.1", (() => v.e(9222).then((() => () => v(19222))))), i("@lumino/messaging", "2.0.1", (() => Promise.all([v.e(7821), v.e(3625)]).then((() => () => v(77821))))), i("@lumino/polling", "2.1.2", (() => Promise.all([v.e(998), v.e(1997), v.e(4271)]).then((() => () => v(64271))))), i("@lumino/properties", "2.0.1", (() => v.e(3733).then((() => () => v(13733))))), i("@lumino/signaling", "2.1.2", (() => Promise.all([v.e(998), v.e(3625), v.e(409)]).then((() => () => v(40409))))), i("@lumino/virtualdom", "2.0.1", (() => Promise.all([v.e(5234), v.e(3625)]).then((() => () => v(85234))))), i("@lumino/widgets", "2.3.2", (() => Promise.all([v.e(911), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503), v.e(8395), v.e(4421), v.e(6934), v.e(4475), v.e(9615), v.e(554)]).then((() => () => v(30911))))), i("@rjsf/utils", "5.16.1", (() => Promise.all([v.e(755), v.e(7811), v.e(7995), v.e(8156)]).then((() => () => v(57995))))), i("@rjsf/validator-ajv8", "5.15.1", (() => Promise.all([v.e(755), v.e(7796), v.e(131), v.e(4885)]).then((() => () => v(70131))))), i("marked-gfm-heading-id", "3.1.1", (() => v.e(7179).then((() => () => v(67179))))), i("marked-mangle", "1.1.5", (() => v.e(1869).then((() => () => v(81869))))), i("marked", "9.1.6", (() => v.e(3079).then((() => () => v(33079))))), i("react-dom", "18.2.0", (() => Promise.all([v.e(1542), v.e(8156)]).then((() => () => v(31542))))), i("react-toastify", "9.1.3", (() => Promise.all([v.e(8156), v.e(5777)]).then((() => () => v(25777))))), i("react", "18.2.0", (() => v.e(7378).then((() => () => v(27378))))), i("yjs", "13.6.8", (() => v.e(7957).then((() => () => v(67957)))))), e[r] = s.length ? Promise.all(s).then((() => e[r] = 1)) : 1
+                return "default" === l && (i("@codemirror/commands", "6.3.3", (() => Promise.all([v.e(7450), v.e(3546), v.e(9843), v.e(9352), v.e(7592)]).then((() => () => v(67450))))), i("@codemirror/lang-markdown", "6.2.4", (() => Promise.all([v.e(5850), v.e(9239), v.e(9799), v.e(7866), v.e(6271), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(7592)]).then((() => () => v(76271))))), i("@codemirror/language", "6.10.1", (() => Promise.all([v.e(1584), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(31584))))), i("@codemirror/search", "6.5.6", (() => Promise.all([v.e(5261), v.e(3546), v.e(9843)]).then((() => () => v(25261))))), i("@codemirror/state", "6.4.1", (() => v.e(2323).then((() => () => v(92323))))), i("@codemirror/view", "6.26.1", (() => Promise.all([v.e(2955), v.e(9843)]).then((() => () => v(22955))))), i("@jupyter-notebook/application-extension", "7.2.0-rc.1", (() => Promise.all([v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(8722), v.e(4604), v.e(3295), v.e(1221), v.e(2549), v.e(5903), v.e(9879), v.e(5094), v.e(7260), v.e(9625), v.e(3712), v.e(8579)]).then((() => () => v(88579))))), i("@jupyter-notebook/application", "7.2.0-rc.1", (() => Promise.all([v.e(901), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(3625), v.e(8722), v.e(4604), v.e(1221), v.e(2549), v.e(7934), v.e(5903), v.e(9503), v.e(4421), v.e(5135)]).then((() => () => v(45135))))), i("@jupyter-notebook/console-extension", "7.2.0-rc.1", (() => Promise.all([v.e(3625), v.e(8722), v.e(4604), v.e(7260), v.e(9625), v.e(4645)]).then((() => () => v(94645))))), i("@jupyter-notebook/docmanager-extension", "7.2.0-rc.1", (() => Promise.all([v.e(1997), v.e(8722), v.e(5094), v.e(9625), v.e(1650)]).then((() => () => v(71650))))), i("@jupyter-notebook/documentsearch-extension", "7.2.0-rc.1", (() => Promise.all([v.e(5183), v.e(9625), v.e(4382)]).then((() => () => v(54382))))), i("@jupyter-notebook/help-extension", "7.2.0-rc.1", (() => Promise.all([v.e(2030), v.e(3312), v.e(8156), v.e(9879), v.e(3712), v.e(9380)]).then((() => () => v(19380))))), i("@jupyter-notebook/notebook-extension", "7.2.0-rc.1", (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(8156), v.e(8722), v.e(3295), v.e(7934), v.e(9879), v.e(5094), v.e(5460), v.e(9625), v.e(5573)]).then((() => () => v(5573))))), i("@jupyter-notebook/terminal-extension", "7.2.0-rc.1", (() => Promise.all([v.e(3625), v.e(8722), v.e(4604), v.e(9625), v.e(5333), v.e(5601)]).then((() => () => v(95601))))), i("@jupyter-notebook/tree-extension", "7.2.0-rc.1", (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(8722), v.e(3295), v.e(1427), v.e(9235), v.e(4258), v.e(4803), v.e(3768)]).then((() => () => v(83768))))), i("@jupyter-notebook/tree", "7.2.0-rc.1", (() => Promise.all([v.e(998), v.e(3485), v.e(5613), v.e(3146)]).then((() => () => v(73146))))), i("@jupyter-notebook/ui-components", "7.2.0-rc.1", (() => Promise.all([v.e(5613), v.e(9068)]).then((() => () => v(59068))))), i("@jupyter/ydoc", "2.0.1", (() => Promise.all([v.e(35), v.e(998), v.e(1997), v.e(7843)]).then((() => () => v(50035))))), i("@jupyterlab/application-extension", "4.2.0", (() => Promise.all([v.e(3881), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(3625), v.e(8722), v.e(4604), v.e(3295), v.e(2549), v.e(1098), v.e(1053), v.e(6934), v.e(7872)]).then((() => () => v(92871))))), i("@jupyterlab/application", "4.2.0", (() => Promise.all([v.e(901), v.e(6853), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(3625), v.e(8722), v.e(1221), v.e(2549), v.e(7934), v.e(5903), v.e(7408), v.e(9503), v.e(4421), v.e(4771)]).then((() => () => v(76853))))), i("@jupyterlab/apputils-extension", "4.2.0", (() => Promise.all([v.e(5099), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(3625), v.e(8722), v.e(4604), v.e(3295), v.e(2549), v.e(7934), v.e(5903), v.e(1098), v.e(7408), v.e(9879), v.e(8395), v.e(1053), v.e(6934), v.e(8005), v.e(2164)]).then((() => () => v(25099))))), i("@jupyterlab/apputils", "4.3.0", (() => Promise.all([v.e(9605), v.e(998), v.e(2030), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(3295), v.e(2549), v.e(1098), v.e(7408), v.e(9503), v.e(8395), v.e(1053), v.e(1231), v.e(3752)]).then((() => () => v(89605))))), i("@jupyterlab/attachments", "4.2.0", (() => Promise.all([v.e(1997), v.e(1221), v.e(1231), v.e(4042)]).then((() => () => v(44042))))), i("@jupyterlab/cell-toolbar-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(3295), v.e(2122)]).then((() => () => v(92122))))), i("@jupyterlab/cell-toolbar", "4.2.0", (() => Promise.all([v.e(3312), v.e(5613), v.e(1997), v.e(3625), v.e(1231), v.e(7386)]).then((() => () => v(37386))))), i("@jupyterlab/cells", "4.2.0", (() => Promise.all([v.e(2479), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(1221), v.e(7934), v.e(9503), v.e(1429), v.e(8395), v.e(9426), v.e(5183), v.e(3546), v.e(525), v.e(4475), v.e(7508), v.e(4946), v.e(2193)]).then((() => () => v(72479))))), i("@jupyterlab/celltags-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(5613), v.e(8156), v.e(3625), v.e(5460), v.e(5346)]).then((() => () => v(15346))))), i("@jupyterlab/codeeditor", "4.2.0", (() => Promise.all([v.e(7391), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(1098), v.e(1231), v.e(7508)]).then((() => () => v(77391))))), i("@jupyterlab/codemirror-extension", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(5613), v.e(8156), v.e(4604), v.e(3295), v.e(1098), v.e(1429), v.e(525), v.e(7478), v.e(3831), v.e(7592), v.e(7655)]).then((() => () => v(97655))))), i("@jupyterlab/codemirror", "4.2.0", (() => Promise.all([v.e(9799), v.e(5263), v.e(998), v.e(2030), v.e(1997), v.e(8722), v.e(1429), v.e(5183), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(3831), v.e(7592), v.e(7843)]).then((() => () => v(95263))))), i("@jupyterlab/completer-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(5613), v.e(8156), v.e(3295), v.e(6934), v.e(1002), v.e(3340)]).then((() => () => v(33340))))), i("@jupyterlab/completer", "4.2.0", (() => Promise.all([v.e(2944), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(3625), v.e(8722), v.e(1221), v.e(9503), v.e(1429), v.e(8395), v.e(3546), v.e(9843)]).then((() => () => v(62944))))), i("@jupyterlab/console-extension", "4.2.0", (() => Promise.all([v.e(6748), v.e(998), v.e(2030), v.e(3312), v.e(5613), v.e(3625), v.e(4604), v.e(3295), v.e(1221), v.e(2549), v.e(1429), v.e(9879), v.e(4421), v.e(1427), v.e(7260), v.e(6810), v.e(1002)]).then((() => () => v(86748))))), i("@jupyterlab/console", "4.2.0", (() => Promise.all([v.e(2636), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8722), v.e(1221), v.e(1231), v.e(3546), v.e(9843), v.e(9615), v.e(3166), v.e(7508)]).then((() => () => v(72636))))), i("@jupyterlab/coreutils", "6.2.0", (() => Promise.all([v.e(2866), v.e(998), v.e(1997)]).then((() => () => v(2866))))), i("@jupyterlab/csvviewer-extension", "4.2.0", (() => Promise.all([v.e(1827), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8722), v.e(4604), v.e(3295), v.e(5903), v.e(9879), v.e(5183)]).then((() => () => v(41827))))), i("@jupyterlab/csvviewer", "4.2.0", (() => Promise.all([v.e(8032), v.e(998), v.e(2030), v.e(3485), v.e(5613), v.e(1997), v.e(8722), v.e(5903), v.e(9072), v.e(5313)]).then((() => () => v(65313))))), i("@jupyterlab/debugger-extension", "4.2.0", (() => Promise.all([v.e(2184), v.e(2030), v.e(3312), v.e(8722), v.e(4604), v.e(3295), v.e(1221), v.e(5903), v.e(1429), v.e(5460), v.e(7260), v.e(3166), v.e(4663), v.e(4182), v.e(3050)]).then((() => () => v(42184))))), i("@jupyterlab/debugger", "4.2.0", (() => Promise.all([v.e(1884), v.e(6621), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(1221), v.e(7934), v.e(1429), v.e(1231), v.e(3546), v.e(9843), v.e(3166)]).then((() => () => v(36621))))), i("@jupyterlab/docmanager-extension", "4.2.0", (() => Promise.all([v.e(8471), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(4604), v.e(3295), v.e(1098), v.e(1053), v.e(5094)]).then((() => () => v(8471))))), i("@jupyterlab/docmanager", "4.2.0", (() => Promise.all([v.e(7543), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(2549), v.e(7934), v.e(5903), v.e(1098), v.e(9503), v.e(4421)]).then((() => () => v(37543))))), i("@jupyterlab/docregistry", "4.2.0", (() => Promise.all([v.e(2489), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(1221), v.e(2549), v.e(9503), v.e(1429)]).then((() => () => v(72489))))), i("@jupyterlab/documentsearch-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(4604), v.e(3295), v.e(5183), v.e(4212)]).then((() => () => v(24212))))), i("@jupyterlab/documentsearch", "4.2.0", (() => Promise.all([v.e(6999), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(2549), v.e(7934), v.e(6934)]).then((() => () => v(36999))))), i("@jupyterlab/extensionmanager-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(5613), v.e(4604), v.e(3295), v.e(2311)]).then((() => () => v(22311))))), i("@jupyterlab/extensionmanager", "4.2.0", (() => Promise.all([v.e(9151), v.e(2030), v.e(3312), v.e(5613), v.e(8156), v.e(8722), v.e(7934), v.e(7408)]).then((() => () => v(59151))))), i("@jupyterlab/filebrowser-extension", "4.2.0", (() => Promise.all([v.e(893), v.e(2030), v.e(3312), v.e(5613), v.e(3625), v.e(8722), v.e(4604), v.e(3295), v.e(1098), v.e(1053), v.e(5094), v.e(6934), v.e(1427)]).then((() => () => v(30893))))), i("@jupyterlab/filebrowser", "4.2.0", (() => Promise.all([v.e(9341), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(7934), v.e(5903), v.e(1098), v.e(7408), v.e(9503), v.e(8395), v.e(5094), v.e(4475), v.e(9615)]).then((() => () => v(39341))))), i("@jupyterlab/fileeditor-extension", "4.2.0", (() => Promise.all([v.e(7603), v.e(2030), v.e(3312), v.e(5613), v.e(3625), v.e(8722), v.e(4604), v.e(3295), v.e(1098), v.e(1429), v.e(9879), v.e(9426), v.e(5183), v.e(525), v.e(1427), v.e(7260), v.e(1907), v.e(6810), v.e(4663), v.e(1002), v.e(3831)]).then((() => () => v(97603))))), i("@jupyterlab/fileeditor", "4.2.0", (() => Promise.all([v.e(1833), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(5903), v.e(1098), v.e(1429), v.e(9426), v.e(525), v.e(1907)]).then((() => () => v(31833))))), i("@jupyterlab/help-extension", "4.2.0", (() => Promise.all([v.e(1496), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(8722), v.e(4604), v.e(7408), v.e(9879), v.e(4475)]).then((() => () => v(91496))))), i("@jupyterlab/htmlviewer-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(5613), v.e(4604), v.e(3295), v.e(6962)]).then((() => () => v(56962))))), i("@jupyterlab/htmlviewer", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(5613), v.e(1997), v.e(8156), v.e(8722), v.e(5903), v.e(5325)]).then((() => () => v(35325))))), i("@jupyterlab/hub-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(8722), v.e(4604), v.e(6893)]).then((() => () => v(56893))))), i("@jupyterlab/imageviewer-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(4604), v.e(6139)]).then((() => () => v(56139))))), i("@jupyterlab/imageviewer", "4.2.0", (() => Promise.all([v.e(998), v.e(3312), v.e(3485), v.e(8722), v.e(5903), v.e(7900)]).then((() => () => v(67900))))), i("@jupyterlab/javascript-extension", "4.2.0", (() => Promise.all([v.e(1221), v.e(5733)]).then((() => () => v(65733))))), i("@jupyterlab/json-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(8156), v.e(8005), v.e(690)]).then((() => () => v(60690))))), i("@jupyterlab/launcher", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(3625), v.e(2549), v.e(4421), v.e(8771)]).then((() => () => v(68771))))), i("@jupyterlab/logconsole", "4.2.0", (() => Promise.all([v.e(2089), v.e(998), v.e(2030), v.e(3485), v.e(1997), v.e(1221), v.e(4946)]).then((() => () => v(2089))))), i("@jupyterlab/lsp-extension", "4.2.0", (() => Promise.all([v.e(3466), v.e(998), v.e(2030), v.e(3312), v.e(5613), v.e(1997), v.e(8156), v.e(3295), v.e(7934), v.e(1907), v.e(9235)]).then((() => () => v(83466))))), i("@jupyterlab/lsp", "4.2.0", (() => Promise.all([v.e(3512), v.e(998), v.e(2030), v.e(3312), v.e(1997), v.e(8722), v.e(5903), v.e(7408)]).then((() => () => v(13512))))), i("@jupyterlab/mainmenu-extension", "4.2.0", (() => Promise.all([v.e(545), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(3625), v.e(8722), v.e(4604), v.e(3295), v.e(7408), v.e(9879), v.e(5094), v.e(1427)]).then((() => () => v(60545))))), i("@jupyterlab/mainmenu", "4.2.0", (() => Promise.all([v.e(998), v.e(3312), v.e(3485), v.e(5613), v.e(3625), v.e(2007)]).then((() => () => v(12007))))), i("@jupyterlab/markdownviewer-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(8722), v.e(4604), v.e(3295), v.e(1221), v.e(9426), v.e(3991), v.e(9685)]).then((() => () => v(79685))))), i("@jupyterlab/markdownviewer", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(1997), v.e(8722), v.e(1221), v.e(5903), v.e(9426), v.e(9680)]).then((() => () => v(99680))))), i("@jupyterlab/markedparser-extension", "4.2.0", (() => Promise.all([v.e(998), v.e(8722), v.e(1221), v.e(525), v.e(8337), v.e(9268)]).then((() => () => v(79268))))), i("@jupyterlab/mathjax-extension", "4.2.0", (() => Promise.all([v.e(998), v.e(1221), v.e(1408)]).then((() => () => v(11408))))), i("@jupyterlab/mermaid-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(8337), v.e(9161)]).then((() => () => v(79161))))), i("@jupyterlab/mermaid", "4.2.0", (() => Promise.all([v.e(998), v.e(3485), v.e(8722), v.e(2615)]).then((() => () => v(92615))))), i("@jupyterlab/metadataform-extension", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(5613), v.e(3295), v.e(5460), v.e(2077), v.e(9335)]).then((() => () => v(89335))))), i("@jupyterlab/metadataform", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(3295), v.e(5460), v.e(7478), v.e(2924)]).then((() => () => v(22924))))), i("@jupyterlab/nbformat", "4.2.0", (() => Promise.all([v.e(998), v.e(3325)]).then((() => () => v(23325))))), i("@jupyterlab/notebook-extension", "4.2.0", (() => Promise.all([v.e(1962), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(3625), v.e(8722), v.e(4604), v.e(3295), v.e(1221), v.e(2549), v.e(7934), v.e(1098), v.e(7408), v.e(9503), v.e(1429), v.e(9879), v.e(1053), v.e(5094), v.e(1231), v.e(9426), v.e(5183), v.e(525), v.e(5460), v.e(1427), v.e(1907), v.e(3166), v.e(6810), v.e(1002), v.e(7872), v.e(4182), v.e(2077), v.e(7708)]).then((() => () => v(51962))))), i("@jupyterlab/notebook", "4.2.0", (() => Promise.all([v.e(374), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(7934), v.e(5903), v.e(1098), v.e(7408), v.e(9503), v.e(1429), v.e(8395), v.e(1231), v.e(4421), v.e(9426), v.e(5183), v.e(4475), v.e(1907), v.e(9615), v.e(3166), v.e(7508), v.e(1139)]).then((() => () => v(90374))))), i("@jupyterlab/observables", "5.2.0", (() => Promise.all([v.e(170), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503)]).then((() => () => v(10170))))), i("@jupyterlab/outputarea", "4.2.0", (() => Promise.all([v.e(7226), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(1997), v.e(3625), v.e(1221), v.e(7408), v.e(1231), v.e(4421), v.e(1139)]).then((() => () => v(47226))))), i("@jupyterlab/pdf-extension", "4.2.0", (() => Promise.all([v.e(998), v.e(3485), v.e(2549), v.e(4058)]).then((() => () => v(84058))))), i("@jupyterlab/pluginmanager-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(5613), v.e(4604), v.e(9033), v.e(3187)]).then((() => () => v(53187))))), i("@jupyterlab/pluginmanager", "4.2.0", (() => Promise.all([v.e(9821), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(8722), v.e(7408)]).then((() => () => v(69821))))), i("@jupyterlab/property-inspector", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(3485), v.e(5613), v.e(1997), v.e(1198)]).then((() => () => v(41198))))), i("@jupyterlab/rendermime-interfaces", "3.10.0", (() => v.e(5297).then((() => () => v(75297))))), i("@jupyterlab/rendermime", "4.2.0", (() => Promise.all([v.e(2401), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(1997), v.e(8722), v.e(1231), v.e(1139), v.e(2425)]).then((() => () => v(72401))))), i("@jupyterlab/running-extension", "4.2.0", (() => Promise.all([v.e(7854), v.e(2030), v.e(3312), v.e(5613), v.e(1997), v.e(8156), v.e(8722), v.e(4604), v.e(7934), v.e(5903), v.e(1053), v.e(5094), v.e(9235)]).then((() => () => v(97854))))), i("@jupyterlab/running", "4.2.0", (() => Promise.all([v.e(1809), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(2549), v.e(8395)]).then((() => () => v(1809))))), i("@jupyterlab/services", "7.2.0", (() => Promise.all([v.e(3676), v.e(998), v.e(1997), v.e(8722), v.e(2549), v.e(7934), v.e(1053)]).then((() => () => v(83676))))), i("@jupyterlab/settingeditor-extension", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(3312), v.e(5613), v.e(4604), v.e(3295), v.e(1221), v.e(1429), v.e(1053), v.e(9033), v.e(8633)]).then((() => () => v(98633))))), i("@jupyterlab/settingeditor", "4.2.0", (() => Promise.all([v.e(3360), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(1221), v.e(7934), v.e(1429), v.e(1053), v.e(7478)]).then((() => () => v(63360))))), i("@jupyterlab/settingregistry", "4.2.0", (() => Promise.all([v.e(7796), v.e(5649), v.e(998), v.e(1997), v.e(2549), v.e(6934)]).then((() => () => v(5649))))), i("@jupyterlab/shortcuts-extension", "5.0.0", (() => Promise.all([v.e(113), v.e(998), v.e(2030), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(3295), v.e(2549), v.e(8395), v.e(6934), v.e(554)]).then((() => () => v(113))))), i("@jupyterlab/statedb", "4.2.0", (() => Promise.all([v.e(4526), v.e(998), v.e(1997), v.e(4421)]).then((() => () => v(34526))))), i("@jupyterlab/statusbar", "4.2.0", (() => Promise.all([v.e(998), v.e(3485), v.e(5613), v.e(8156), v.e(3625), v.e(2549), v.e(3680)]).then((() => () => v(53680))))), i("@jupyterlab/terminal-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(4604), v.e(3295), v.e(7408), v.e(9879), v.e(9235), v.e(6810), v.e(5333), v.e(5912)]).then((() => () => v(15912))))), i("@jupyterlab/terminal", "4.2.0", (() => Promise.all([v.e(998), v.e(2030), v.e(3485), v.e(9503), v.e(8395), v.e(3213)]).then((() => () => v(53213))))), i("@jupyterlab/theme-dark-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(6627)]).then((() => () => v(6627))))), i("@jupyterlab/theme-dark-high-contrast-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(5254)]).then((() => () => v(95254))))), i("@jupyterlab/theme-light-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(5426)]).then((() => () => v(45426))))), i("@jupyterlab/toc-extension", "6.2.0", (() => Promise.all([v.e(2030), v.e(5613), v.e(4604), v.e(3295), v.e(9426), v.e(62)]).then((() => () => v(40062))))), i("@jupyterlab/toc", "6.2.0", (() => Promise.all([v.e(5921), v.e(998), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(8722), v.e(1221), v.e(2549)]).then((() => () => v(75921))))), i("@jupyterlab/tooltip-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3485), v.e(3625), v.e(8722), v.e(1221), v.e(5460), v.e(7260), v.e(4663), v.e(7865), v.e(6604)]).then((() => () => v(6604))))), i("@jupyterlab/tooltip", "4.2.0", (() => Promise.all([v.e(998), v.e(3485), v.e(5613), v.e(1221), v.e(1647)]).then((() => () => v(51647))))), i("@jupyterlab/translation-extension", "4.2.0", (() => Promise.all([v.e(2030), v.e(3312), v.e(4604), v.e(3295), v.e(9879), v.e(6815)]).then((() => () => v(56815))))), i("@jupyterlab/translation", "4.2.0", (() => Promise.all([v.e(7819), v.e(998), v.e(8722), v.e(7408), v.e(1053)]).then((() => () => v(57819))))), i("@jupyterlab/ui-components-extension", "4.2.0", (() => Promise.all([v.e(5613), v.e(3863)]).then((() => () => v(73863))))), i("@jupyterlab/ui-components", "4.2.0", (() => Promise.all([v.e(1884), v.e(755), v.e(7811), v.e(7506), v.e(998), v.e(2030), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(2549), v.e(7934), v.e(9503), v.e(4421), v.e(6934), v.e(4475), v.e(8005), v.e(4885)]).then((() => () => v(7506))))), i("@jupyterlab/vega5-extension", "4.2.0", (() => Promise.all([v.e(3485), v.e(6061)]).then((() => () => v(16061))))), i("@jupyterlab/workspaces", "4.2.0", (() => Promise.all([v.e(998), v.e(1997), v.e(7934), v.e(1828)]).then((() => () => v(11828))))), i("@lezer/common", "1.2.1", (() => v.e(7997).then((() => () => v(97997))))), i("@lezer/highlight", "1.2.0", (() => Promise.all([v.e(3797), v.e(9352)]).then((() => () => v(23797))))), i("@lumino/algorithm", "2.0.1", (() => v.e(5614).then((() => () => v(15614))))), i("@lumino/application", "2.3.1", (() => Promise.all([v.e(6731), v.e(998), v.e(3485), v.e(6934)]).then((() => () => v(16731))))), i("@lumino/commands", "2.3.0", (() => Promise.all([v.e(3301), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(8395), v.e(554)]).then((() => () => v(43301))))), i("@lumino/coreutils", "2.1.2", (() => v.e(2756).then((() => () => v(12756))))), i("@lumino/datagrid", "2.3.1", (() => Promise.all([v.e(8929), v.e(998), v.e(3485), v.e(1997), v.e(3625), v.e(9503), v.e(8395), v.e(9615), v.e(554)]).then((() => () => v(98929))))), i("@lumino/disposable", "2.1.2", (() => Promise.all([v.e(1997), v.e(5451)]).then((() => () => v(65451))))), i("@lumino/domutils", "2.0.1", (() => v.e(1696).then((() => () => v(1696))))), i("@lumino/dragdrop", "2.1.4", (() => Promise.all([v.e(4291), v.e(2549)]).then((() => () => v(54291))))), i("@lumino/keyboard", "2.0.1", (() => v.e(9222).then((() => () => v(19222))))), i("@lumino/messaging", "2.0.1", (() => Promise.all([v.e(7821), v.e(3625)]).then((() => () => v(77821))))), i("@lumino/polling", "2.1.2", (() => Promise.all([v.e(998), v.e(1997), v.e(4271)]).then((() => () => v(64271))))), i("@lumino/properties", "2.0.1", (() => v.e(3733).then((() => () => v(13733))))), i("@lumino/signaling", "2.1.2", (() => Promise.all([v.e(998), v.e(3625), v.e(409)]).then((() => () => v(40409))))), i("@lumino/virtualdom", "2.0.1", (() => Promise.all([v.e(5234), v.e(3625)]).then((() => () => v(85234))))), i("@lumino/widgets", "2.3.2", (() => Promise.all([v.e(911), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503), v.e(8395), v.e(4421), v.e(6934), v.e(4475), v.e(9615), v.e(554)]).then((() => () => v(30911))))), i("@rjsf/utils", "5.16.1", (() => Promise.all([v.e(755), v.e(7811), v.e(7995), v.e(8156)]).then((() => () => v(57995))))), i("@rjsf/validator-ajv8", "5.15.1", (() => Promise.all([v.e(755), v.e(7796), v.e(131), v.e(4885)]).then((() => () => v(70131))))), i("marked-gfm-heading-id", "3.1.1", (() => v.e(7179).then((() => () => v(67179))))), i("marked-mangle", "1.1.5", (() => v.e(1869).then((() => () => v(81869))))), i("marked", "9.1.6", (() => v.e(3079).then((() => () => v(33079))))), i("react-dom", "18.2.0", (() => Promise.all([v.e(1542), v.e(8156)]).then((() => () => v(31542))))), i("react-toastify", "9.1.3", (() => Promise.all([v.e(8156), v.e(5777)]).then((() => () => v(25777))))), i("react", "18.2.0", (() => v.e(7378).then((() => () => v(27378))))), i("yjs", "13.6.8", (() => v.e(7957).then((() => () => v(67957)))))), e[l] = s.length ? Promise.all(s).then((() => e[l] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         v.g.importScripts && (e = v.g.location + "");
         var t = v.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
-            var r = t.getElementsByTagName("script");
-            if (r.length)
-                for (var l = r.length - 1; l > -1 && !e;) e = r[l--].src
+            var l = t.getElementsByTagName("script");
+            if (l.length)
+                for (var r = l.length - 1; r > -1 && !e;) e = l[r--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), v.p = e
     })(), a = e => {
         var t = e => e.split(".").map((e => +e == e ? +e : e)),
-            r = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            l = r[1] ? t(r[1]) : [];
-        return r[2] && (l.length++, l.push.apply(l, t(r[2]))), r[3] && (l.push([]), l.push.apply(l, t(r[3]))), l
+            l = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
+            r = l[1] ? t(l[1]) : [];
+        return l[2] && (r.length++, r.push.apply(r, t(l[2]))), l[3] && (r.push([]), r.push.apply(r, t(l[3]))), r
     }, n = (e, t) => {
         e = a(e), t = a(t);
-        for (var r = 0;;) {
-            if (r >= e.length) return r < t.length && "u" != (typeof t[r])[0];
-            var l = e[r],
-                n = (typeof l)[0];
-            if (r >= t.length) return "u" == n;
-            var o = t[r],
+        for (var l = 0;;) {
+            if (l >= e.length) return l < t.length && "u" != (typeof t[l])[0];
+            var r = e[l],
+                n = (typeof r)[0];
+            if (l >= t.length) return "u" == n;
+            var o = t[l],
                 i = (typeof o)[0];
             if (n != i) return "o" == n && "n" == i || "s" == i || "u" == n;
-            if ("o" != n && "u" != n && l != o) return l < o;
-            r++
+            if ("o" != n && "u" != n && r != o) return r < o;
+            l++
         }
     }, o = e => {
         var t = e[0],
-            r = "";
+            l = "";
         if (1 === e.length) return "*";
         if (t + .5) {
-            r += 0 == t ? ">=" : -1 == t ? "<" : 1 == t ? "^" : 2 == t ? "~" : t > 0 ? "=" : "!=";
-            for (var l = 1, a = 1; a < e.length; a++) l--, r += "u" == (typeof(i = e[a]))[0] ? "-" : (l > 0 ? "." : "") + (l = 2, i);
-            return r
+            l += 0 == t ? ">=" : -1 == t ? "<" : 1 == t ? "^" : 2 == t ? "~" : t > 0 ? "=" : "!=";
+            for (var r = 1, a = 1; a < e.length; a++) r--, l += "u" == (typeof(i = e[a]))[0] ? "-" : (r > 0 ? "." : "") + (r = 2, i);
+            return l
         }
         var n = [];
         for (a = 1; a < e.length; a++) {
             var i = e[a];
             n.push(0 === i ? "not(" + s() + ")" : 1 === i ? "(" + s() + " || " + s() + ")" : 2 === i ? n.pop() + " " + n.pop() : o(i))
         }
         return s();
 
         function s() {
             return n.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, t) => {
         if (0 in e) {
             t = a(t);
-            var r = e[0],
-                l = r < 0;
-            l && (r = -r - 1);
+            var l = e[0],
+                r = l < 0;
+            r && (l = -l - 1);
             for (var n = 0, o = 1, s = !0;; o++, n++) {
-                var u, m, c = o < e.length ? (typeof e[o])[0] : "";
-                if (n >= t.length || "o" == (m = (typeof(u = t[n]))[0])) return !s || ("u" == c ? o > r && !l : "" == c != l);
+                var u, m, h = o < e.length ? (typeof e[o])[0] : "";
+                if (n >= t.length || "o" == (m = (typeof(u = t[n]))[0])) return !s || ("u" == h ? o > l && !r : "" == h != r);
                 if ("u" == m) {
-                    if (!s || "u" != c) return !1
+                    if (!s || "u" != h) return !1
                 } else if (s)
-                    if (c == m)
-                        if (o <= r) {
+                    if (h == m)
+                        if (o <= l) {
                             if (u != e[o]) return !1
                         } else {
-                            if (l ? u > e[o] : u < e[o]) return !1;
+                            if (r ? u > e[o] : u < e[o]) return !1;
                             u != e[o] && (s = !1)
                         }
-                else if ("s" != c && "n" != c) {
-                    if (l || o <= r) return !1;
+                else if ("s" != h && "n" != h) {
+                    if (r || o <= l) return !1;
                     s = !1, o--
                 } else {
-                    if (o <= r || m < c != l) return !1;
+                    if (o <= l || m < h != r) return !1;
                     s = !1
-                } else "s" != c && "n" != c && (s = !1, o--)
+                } else "s" != h && "n" != h && (s = !1, o--)
             }
         }
-        var h = [],
-            p = h.pop.bind(h);
+        var p = [],
+            d = p.pop.bind(p);
         for (n = 1; n < e.length; n++) {
-            var d = e[n];
-            h.push(1 == d ? p() | p() : 2 == d ? p() & p() : d ? i(d, t) : !p())
+            var b = e[n];
+            p.push(1 == b ? d() | d() : 2 == b ? d() & d() : b ? i(b, t) : !d())
         }
-        return !!p()
+        return !!d()
     }, s = (e, t) => {
-        var r = e[t];
-        return Object.keys(r).reduce(((e, t) => !e || !r[e].loaded && n(e, t) ? t : e), 0)
-    }, u = (e, t, r, l) => "Unsatisfied version " + r + " from " + (r && e[t][r].from) + " of shared singleton module " + t + " (required " + o(l) + ")", m = (e, t, r, l) => {
-        var a = s(e, r);
-        return i(l, a) || h(u(e, r, a, l)), p(e[r][a])
-    }, c = (e, t, r) => {
         var l = e[t];
-        return (t = Object.keys(l).reduce(((e, t) => !i(r, t) || e && !n(e, t) ? e : t), 0)) && l[t]
-    }, h = e => {
+        return Object.keys(l).reduce(((e, t) => !e || !l[e].loaded && n(e, t) ? t : e), 0)
+    }, u = (e, t, l, r) => "Unsatisfied version " + l + " from " + (l && e[t][l].from) + " of shared singleton module " + t + " (required " + o(r) + ")", m = (e, t, l, r) => {
+        var a = s(e, l);
+        return i(r, a) || p(u(e, l, a, r)), d(e[l][a])
+    }, h = (e, t, l) => {
+        var r = e[t];
+        return (t = Object.keys(r).reduce(((e, t) => !i(l, t) || e && !n(e, t) ? e : t), 0)) && r[t]
+    }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), b = (d = e => function(t, r, l, a) {
+    }, d = e => (e.loaded = 1, e.get()), f = (b = e => function(t, l, r, a) {
         var n = v.I(t);
-        return n && n.then ? n.then(e.bind(e, t, v.S[t], r, l, a)) : e(t, v.S[t], r, l, a)
-    })(((e, t, r, l, a) => t && v.o(t, r) ? m(t, 0, r, l) : a())), f = d(((e, t, r, l, a) => {
-        var n = t && v.o(t, r) && c(t, r, l);
-        return n ? p(n) : a()
-    })), P = {}, y = {
-        1167: () => b("default", "@jupyterlab/coreutils", [2, 6, 2, 0, , "rc", 0], (() => Promise.all([v.e(2866), v.e(998), v.e(1997)]).then((() => () => v(2866))))),
-        46807: () => f("default", "@jupyter-notebook/application", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(901), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(3625), v.e(1167), v.e(2922), v.e(3408), v.e(2549), v.e(7934), v.e(979), v.e(9503), v.e(4421), v.e(5135)]).then((() => () => v(45135))))),
-        18602: () => f("default", "@jupyterlab/docmanager-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(8471), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(2922), v.e(4554), v.e(7829), v.e(6692), v.e(1942)]).then((() => () => v(8471))))),
-        252: () => f("default", "@jupyterlab/translation-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(2922), v.e(4554), v.e(845), v.e(6815)]).then((() => () => v(56815))))),
-        5890: () => f("default", "@jupyterlab/completer-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(2620), v.e(8156), v.e(4554), v.e(6934), v.e(9144), v.e(3340)]).then((() => () => v(33340))))),
-        8467: () => f("default", "@jupyterlab/markedparser-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3408), v.e(9269), v.e(3149), v.e(3129)]).then((() => () => v(79268))))),
-        9269: () => f("default", "@jupyterlab/htmlviewer-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(2620), v.e(2922), v.e(4554), v.e(6962)]).then((() => () => v(56962))))),
-        13375: () => f("default", "@jupyterlab/cell-toolbar-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(4554), v.e(2122)]).then((() => () => v(92122))))),
-        17420: () => f("default", "@jupyterlab/mathjax-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3408), v.e(1408)]).then((() => () => v(11408))))),
-        18173: () => f("default", "@jupyterlab/celltags-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(2620), v.e(8156), v.e(3625), v.e(7894), v.e(5346)]).then((() => () => v(15346))))),
-        18403: () => f("default", "@jupyterlab/json-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(8156), v.e(8005), v.e(690)]).then((() => () => v(60690))))),
-        24124: () => f("default", "@jupyterlab/documentsearch-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(2922), v.e(4554), v.e(6862), v.e(4212)]).then((() => () => v(24212))))),
-        25622: () => f("default", "@jupyter-notebook/documentsearch-extension", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(6862), v.e(7906)]).then((() => () => v(54382))))),
-        28654: () => f("default", "@jupyterlab/console-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(6748), v.e(998), v.e(7267), v.e(6049), v.e(2620), v.e(3625), v.e(2922), v.e(4554), v.e(3408), v.e(2549), v.e(2839), v.e(845), v.e(4421), v.e(2751), v.e(106), v.e(5651), v.e(9144)]).then((() => () => v(86748))))),
-        29272: () => f("default", "@jupyter-notebook/application-extension", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2922), v.e(4554), v.e(3408), v.e(2549), v.e(979), v.e(845), v.e(1942), v.e(106), v.e(8625), v.e(8579)]).then((() => () => v(88579))))),
-        31716: () => f("default", "@jupyterlab/hub-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(2922), v.e(7684)]).then((() => () => v(56893))))),
-        32374: () => f("default", "@jupyterlab/javascript-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(3408), v.e(5733)]).then((() => () => v(65733))))),
-        39137: () => f("default", "@jupyterlab/mainmenu-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(545), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(3625), v.e(2922), v.e(4554), v.e(611), v.e(845), v.e(1942), v.e(2751)]).then((() => () => v(60545))))),
-        39519: () => f("default", "@jupyterlab/settingeditor-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(7267), v.e(6049), v.e(2620), v.e(2922), v.e(4554), v.e(3408), v.e(2839), v.e(6692), v.e(7355), v.e(8633)]).then((() => () => v(98633))))),
-        40682: () => f("default", "@jupyterlab/debugger-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2184), v.e(7267), v.e(6049), v.e(2922), v.e(4554), v.e(3408), v.e(979), v.e(2839), v.e(7894), v.e(106), v.e(7406), v.e(2703), v.e(8603), v.e(9713)]).then((() => () => v(42184))))),
-        44250: () => f("default", "@jupyterlab/lsp-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(3466), v.e(998), v.e(7267), v.e(6049), v.e(2620), v.e(1997), v.e(8156), v.e(4554), v.e(7934), v.e(2138), v.e(5729)]).then((() => () => v(83466))))),
-        46456: () => f("default", "@jupyterlab/pluginmanager-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(2620), v.e(2922), v.e(7355), v.e(3187)]).then((() => () => v(53187))))),
-        48618: () => f("default", "@jupyterlab/extensionmanager-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(2620), v.e(2922), v.e(4554), v.e(2311)]).then((() => () => v(22311))))),
-        53160: () => f("default", "@jupyterlab/shortcuts-extension", [2, 5, 0, 0, , "rc", 0], (() => Promise.all([v.e(113), v.e(998), v.e(7267), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(4554), v.e(2549), v.e(8395), v.e(6934), v.e(554)]).then((() => () => v(113))))),
-        56727: () => f("default", "@jupyterlab/mermaid-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(3149), v.e(9161)]).then((() => () => v(79161))))),
-        56823: () => f("default", "@jupyterlab/codemirror-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(7267), v.e(2620), v.e(8156), v.e(2922), v.e(4554), v.e(7829), v.e(2839), v.e(9269), v.e(7478), v.e(3831), v.e(7592), v.e(7655)]).then((() => () => v(97655))))),
-        57782: () => f("default", "@jupyterlab/filebrowser-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(893), v.e(7267), v.e(6049), v.e(2620), v.e(3625), v.e(2922), v.e(4554), v.e(7829), v.e(6692), v.e(1942), v.e(6934), v.e(2751)]).then((() => () => v(30893))))),
-        61182: () => f("default", "@jupyterlab/apputils-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(5099), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(3625), v.e(2922), v.e(4554), v.e(2549), v.e(7934), v.e(979), v.e(7829), v.e(611), v.e(845), v.e(8395), v.e(6692), v.e(6934), v.e(8005), v.e(3892)]).then((() => () => v(25099))))),
-        61378: () => f("default", "@jupyterlab/csvviewer-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1827), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(2922), v.e(4554), v.e(979), v.e(845), v.e(6862)]).then((() => () => v(41827))))),
-        63728: () => f("default", "@jupyterlab/fileeditor-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7603), v.e(7267), v.e(6049), v.e(2620), v.e(3625), v.e(2922), v.e(4554), v.e(7829), v.e(2839), v.e(845), v.e(7017), v.e(6862), v.e(9269), v.e(2751), v.e(106), v.e(2138), v.e(5651), v.e(2703), v.e(9144), v.e(3831)]).then((() => () => v(97603))))),
-        65028: () => f("default", "@jupyterlab/pdf-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3485), v.e(2549), v.e(4058)]).then((() => () => v(84058))))),
-        65477: () => f("default", "@jupyterlab/toc-extension", [2, 6, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(2620), v.e(2922), v.e(4554), v.e(7017), v.e(62)]).then((() => () => v(40062))))),
-        65787: () => f("default", "@jupyterlab/tooltip-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(3485), v.e(3625), v.e(3408), v.e(7894), v.e(106), v.e(2703), v.e(5327), v.e(2088)]).then((() => () => v(6604))))),
-        66889: () => f("default", "@jupyter-notebook/notebook-extension", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(8156), v.e(4554), v.e(7934), v.e(845), v.e(1942), v.e(7894), v.e(5573)]).then((() => () => v(5573))))),
-        68449: () => f("default", "@jupyterlab/theme-dark-high-contrast-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(5254)]).then((() => () => v(95254))))),
-        70545: () => f("default", "@jupyterlab/vega5-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(3485), v.e(6061)]).then((() => () => v(16061))))),
-        70952: () => f("default", "@jupyterlab/help-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1496), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(2922), v.e(611), v.e(845), v.e(4475)]).then((() => () => v(91496))))),
-        73898: () => f("default", "@jupyterlab/markdownviewer-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(2922), v.e(4554), v.e(3408), v.e(7017), v.e(5910), v.e(7252)]).then((() => () => v(79685))))),
-        74572: () => f("default", "@jupyterlab/ui-components-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2620), v.e(3863)]).then((() => () => v(73863))))),
-        76156: () => f("default", "@jupyterlab/running-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7854), v.e(7267), v.e(6049), v.e(2620), v.e(1997), v.e(8156), v.e(2922), v.e(7934), v.e(979), v.e(6692), v.e(1942), v.e(5729)]).then((() => () => v(97854))))),
-        77429: () => f("default", "@jupyter-notebook/terminal-extension", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(3625), v.e(2922), v.e(9200), v.e(1684)]).then((() => () => v(95601))))),
-        78085: () => f("default", "@jupyter-notebook/tree-extension", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(4554), v.e(2751), v.e(5729), v.e(1131), v.e(2367), v.e(7302)]).then((() => () => v(83768))))),
-        78578: () => f("default", "@jupyterlab/notebook-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1962), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(3625), v.e(2922), v.e(4554), v.e(3408), v.e(2549), v.e(7934), v.e(7829), v.e(611), v.e(9503), v.e(2839), v.e(845), v.e(6692), v.e(1942), v.e(8959), v.e(7017), v.e(6862), v.e(9269), v.e(7894), v.e(2751), v.e(2138), v.e(7406), v.e(5651), v.e(9144), v.e(6724), v.e(8603), v.e(465)]).then((() => () => v(51962))))),
-        82818: () => f("default", "@jupyterlab/metadataform-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(7267), v.e(2620), v.e(4554), v.e(7894), v.e(465), v.e(9335)]).then((() => () => v(89335))))),
-        83421: () => f("default", "@jupyter-notebook/docmanager-extension", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(1997), v.e(1942), v.e(8875)]).then((() => () => v(71650))))),
-        88378: () => f("default", "@jupyter-notebook/help-extension", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(8156), v.e(845), v.e(8625), v.e(9380)]).then((() => () => v(19380))))),
-        90856: () => f("default", "@jupyterlab/terminal-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(2922), v.e(4554), v.e(611), v.e(845), v.e(5729), v.e(5651), v.e(9200), v.e(5912)]).then((() => () => v(15912))))),
-        92396: () => f("default", "@jupyterlab/theme-dark-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(6627)]).then((() => () => v(6627))))),
-        94388: () => f("default", "@jupyterlab/imageviewer-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(2922), v.e(6139)]).then((() => () => v(56139))))),
-        95496: () => f("default", "@jupyterlab/application-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(3881), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(3625), v.e(2922), v.e(4554), v.e(2549), v.e(7829), v.e(6692), v.e(6934), v.e(6724)]).then((() => () => v(92871))))),
-        99223: () => f("default", "@jupyter-notebook/console-extension", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(3625), v.e(2922), v.e(106), v.e(6345)]).then((() => () => v(94645))))),
-        99526: () => f("default", "@jupyterlab/theme-light-extension", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7267), v.e(6049), v.e(5426)]).then((() => () => v(45426))))),
-        3546: () => b("default", "@codemirror/view", [2, 6, 26, 1], (() => Promise.all([v.e(2955), v.e(9843)]).then((() => () => v(22955))))),
-        89843: () => b("default", "@codemirror/state", [2, 6, 4, 1], (() => v.e(2323).then((() => () => v(92323))))),
-        79352: () => b("default", "@lezer/common", [2, 1, 2, 1], (() => v.e(7997).then((() => () => v(97997))))),
-        17592: () => f("default", "@codemirror/language", [1, 6, 10, 1], (() => Promise.all([v.e(1584), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(31584))))),
-        92209: () => b("default", "@lezer/highlight", [2, 1, 2, 0], (() => Promise.all([v.e(3797), v.e(9352)]).then((() => () => v(23797))))),
-        20998: () => b("default", "@lumino/coreutils", [2, 2, 1, 2], (() => v.e(2756).then((() => () => v(12756))))),
-        37267: () => b("default", "@jupyterlab/translation", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7819), v.e(998), v.e(1167), v.e(611), v.e(6692)]).then((() => () => v(57819))))),
-        96049: () => b("default", "@jupyterlab/apputils", [2, 4, 3, 0, , "rc", 0], (() => Promise.all([v.e(9605), v.e(998), v.e(7267), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(4554), v.e(2549), v.e(7829), v.e(611), v.e(9503), v.e(8395), v.e(6692), v.e(8959), v.e(3752)]).then((() => () => v(89605))))),
-        63485: () => b("default", "@lumino/widgets", [2, 2, 3, 2], (() => Promise.all([v.e(911), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503), v.e(8395), v.e(4421), v.e(6934), v.e(4475), v.e(9615), v.e(554)]).then((() => () => v(30911))))),
-        2922: () => b("default", "@jupyterlab/application", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(901), v.e(6853), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(3625), v.e(1167), v.e(3408), v.e(2549), v.e(7934), v.e(979), v.e(611), v.e(9503), v.e(4421), v.e(4771)]).then((() => () => v(76853))))),
-        24554: () => b("default", "@jupyterlab/settingregistry", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7796), v.e(5649), v.e(998), v.e(1997), v.e(2549), v.e(6934)]).then((() => () => v(5649))))),
-        13408: () => b("default", "@jupyterlab/rendermime", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2401), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(1997), v.e(1167), v.e(8959), v.e(1692), v.e(1070)]).then((() => () => v(72401))))),
-        2549: () => b("default", "@lumino/disposable", [2, 2, 1, 2], (() => Promise.all([v.e(1997), v.e(5451)]).then((() => () => v(65451))))),
-        10979: () => f("default", "@jupyterlab/docregistry", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2489), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(3408), v.e(2549), v.e(9503), v.e(2839)]).then((() => () => v(72489))))),
-        50845: () => b("default", "@jupyterlab/mainmenu", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3485), v.e(2620), v.e(3625), v.e(2607)]).then((() => () => v(12007))))),
-        91942: () => b("default", "@jupyterlab/docmanager", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7543), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(2549), v.e(7934), v.e(979), v.e(7829), v.e(9503), v.e(4421)]).then((() => () => v(37543))))),
-        80106: () => b("default", "@jupyterlab/console", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2636), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(1167), v.e(3408), v.e(8959), v.e(3546), v.e(9843), v.e(9615), v.e(7406), v.e(7508)]).then((() => () => v(72636))))),
-        18625: () => f("default", "@jupyter-notebook/ui-components", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(2620), v.e(9068)]).then((() => () => v(59068))))),
-        22620: () => b("default", "@jupyterlab/ui-components", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1884), v.e(755), v.e(7811), v.e(7506), v.e(998), v.e(7267), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(2549), v.e(7934), v.e(9503), v.e(4421), v.e(6934), v.e(4475), v.e(8005), v.e(4885)]).then((() => () => v(7506))))),
-        81997: () => b("default", "@lumino/signaling", [2, 2, 1, 2], (() => Promise.all([v.e(998), v.e(3625), v.e(409)]).then((() => () => v(40409))))),
-        33625: () => b("default", "@lumino/algorithm", [2, 2, 0, 1], (() => v.e(5614).then((() => () => v(15614))))),
-        97934: () => f("default", "@lumino/polling", [1, 2, 1, 2], (() => Promise.all([v.e(998), v.e(1997), v.e(4271)]).then((() => () => v(64271))))),
-        49503: () => b("default", "@lumino/messaging", [2, 2, 0, 1], (() => Promise.all([v.e(7821), v.e(3625)]).then((() => () => v(77821))))),
-        14421: () => b("default", "@lumino/properties", [2, 2, 0, 1], (() => v.e(3733).then((() => () => v(13733))))),
-        26862: () => b("default", "@jupyterlab/documentsearch", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(6999), v.e(998), v.e(7267), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(2549), v.e(7934), v.e(6934)]).then((() => () => v(36999))))),
-        78156: () => b("default", "react", [2, 18, 2, 0], (() => v.e(7378).then((() => () => v(27378))))),
-        17894: () => b("default", "@jupyterlab/notebook", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(374), v.e(998), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(7934), v.e(979), v.e(7829), v.e(611), v.e(9503), v.e(2839), v.e(8395), v.e(8959), v.e(4421), v.e(7017), v.e(6862), v.e(4475), v.e(2138), v.e(9615), v.e(7406), v.e(7508), v.e(1692)]).then((() => () => v(90374))))),
-        69200: () => b("default", "@jupyterlab/terminal", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(7267), v.e(3485), v.e(9503), v.e(8395), v.e(3213)]).then((() => () => v(53213))))),
-        42751: () => b("default", "@jupyterlab/filebrowser", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(9341), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(7934), v.e(979), v.e(7829), v.e(611), v.e(9503), v.e(8395), v.e(1942), v.e(4475), v.e(9615)]).then((() => () => v(39341))))),
-        15729: () => f("default", "@jupyterlab/running", [1, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1809), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(2549), v.e(8395)]).then((() => () => v(1809))))),
-        1131: () => b("default", "@jupyterlab/settingeditor", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(3360), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(1167), v.e(3408), v.e(7934), v.e(2839), v.e(6692), v.e(7478)]).then((() => () => v(63360))))),
-        42367: () => b("default", "@jupyter-notebook/tree", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(4837)]).then((() => () => v(73146))))),
-        17843: () => b("default", "yjs", [2, 13, 6, 8], (() => v.e(7957).then((() => () => v(67957))))),
-        27829: () => b("default", "@jupyterlab/statusbar", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3485), v.e(8156), v.e(3625), v.e(2549), v.e(7639)]).then((() => () => v(53680))))),
-        96692: () => b("default", "@jupyterlab/statedb", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(4526), v.e(998), v.e(1997), v.e(4421)]).then((() => () => v(34526))))),
-        16934: () => b("default", "@lumino/commands", [2, 2, 3, 0], (() => Promise.all([v.e(3301), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(8395), v.e(554)]).then((() => () => v(43301))))),
-        66724: () => f("default", "@jupyterlab/property-inspector", [1, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1997), v.e(8907)]).then((() => () => v(41198))))),
-        70611: () => b("default", "@jupyterlab/services", [2, 7, 2, 0, , "rc", 0], (() => Promise.all([v.e(3676), v.e(998), v.e(1997), v.e(1167), v.e(2549), v.e(7934), v.e(6692)]).then((() => () => v(83676))))),
-        34771: () => b("default", "@lumino/application", [2, 2, 3, 1], (() => Promise.all([v.e(6731), v.e(6934)]).then((() => () => v(16731))))),
-        18395: () => b("default", "@lumino/domutils", [2, 2, 0, 1], (() => v.e(1696).then((() => () => v(1696))))),
-        38005: () => b("default", "react-dom", [2, 18, 2, 0], (() => v.e(1542).then((() => () => v(31542))))),
-        13892: () => f("default", "@jupyterlab/workspaces", [1, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1997), v.e(5166)]).then((() => () => v(11828))))),
-        58959: () => b("default", "@jupyterlab/observables", [2, 5, 2, 0, , "rc", 0], (() => Promise.all([v.e(170), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503)]).then((() => () => v(10170))))),
-        5510: () => b("default", "@jupyterlab/cell-toolbar", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2620), v.e(1997), v.e(3625), v.e(8959), v.e(4811)]).then((() => () => v(37386))))),
-        52839: () => b("default", "@jupyterlab/codeeditor", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7391), v.e(998), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(7829), v.e(8959), v.e(7508)]).then((() => () => v(77391))))),
-        87017: () => f("default", "@jupyterlab/toc", [1, 6, 2, 0, , "rc", 0], (() => Promise.all([v.e(5921), v.e(998), v.e(6049), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(1167), v.e(3408), v.e(2549)]).then((() => () => v(75921))))),
-        49269: () => b("default", "@jupyterlab/codemirror", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(9799), v.e(5263), v.e(998), v.e(7267), v.e(1997), v.e(1167), v.e(2839), v.e(6862), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(3831), v.e(7592), v.e(7843)]).then((() => () => v(95263))))),
-        24475: () => b("default", "@lumino/virtualdom", [2, 2, 0, 1], (() => Promise.all([v.e(5234), v.e(3625)]).then((() => () => v(85234))))),
-        57508: () => b("default", "@jupyter/ydoc", [2, 2, 0, 1], (() => Promise.all([v.e(35), v.e(7843)]).then((() => () => v(50035))))),
-        36726: () => b("default", "@jupyterlab/outputarea", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(7226), v.e(6049), v.e(3625), v.e(611), v.e(8959), v.e(4421), v.e(1692)]).then((() => () => v(47226))))),
-        98289: () => f("default", "@jupyterlab/attachments", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(8959), v.e(134)]).then((() => () => v(44042))))),
-        27478: () => f("default", "@rjsf/validator-ajv8", [1, 5, 13, 4], (() => Promise.all([v.e(755), v.e(7796), v.e(131), v.e(4885)]).then((() => () => v(70131))))),
-        24636: () => f("default", "@codemirror/search", [1, 6, 5, 6], (() => Promise.all([v.e(5261), v.e(3546), v.e(9843)]).then((() => () => v(25261))))),
-        87797: () => f("default", "@codemirror/commands", [1, 6, 3, 3], (() => Promise.all([v.e(7450), v.e(3546), v.e(9843), v.e(9352), v.e(7592)]).then((() => () => v(67450))))),
-        89144: () => b("default", "@jupyterlab/completer", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2944), v.e(998), v.e(6049), v.e(3485), v.e(1997), v.e(3625), v.e(1167), v.e(3408), v.e(9503), v.e(2839), v.e(8395), v.e(3546), v.e(9843)]).then((() => () => v(62944))))),
-        65651: () => f("default", "@jupyterlab/launcher", [1, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3485), v.e(8156), v.e(3625), v.e(2549), v.e(4421), v.e(9638)]).then((() => () => v(68771))))),
-        99615: () => b("default", "@lumino/dragdrop", [2, 2, 1, 4], (() => Promise.all([v.e(4291), v.e(2549)]).then((() => () => v(54291))))),
-        67406: () => f("default", "@jupyterlab/cells", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2479), v.e(998), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(3408), v.e(7934), v.e(9503), v.e(2839), v.e(8395), v.e(7017), v.e(6862), v.e(3546), v.e(9269), v.e(4475), v.e(7508), v.e(6726), v.e(8289)]).then((() => () => v(72479))))),
-        59072: () => f("default", "@lumino/datagrid", [1, 2, 3, 1], (() => Promise.all([v.e(8929), v.e(3625), v.e(9503), v.e(8395), v.e(9615), v.e(554)]).then((() => () => v(98929))))),
-        42703: () => b("default", "@jupyterlab/fileeditor", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1833), v.e(998), v.e(6049), v.e(3485), v.e(2620), v.e(8156), v.e(979), v.e(7829), v.e(2839), v.e(7017), v.e(9269), v.e(2138)]).then((() => () => v(31833))))),
-        98603: () => f("default", "@jupyterlab/logconsole", [1, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(2089), v.e(998), v.e(3485), v.e(1997), v.e(6726)]).then((() => () => v(2089))))),
-        49713: () => b("default", "@jupyterlab/debugger", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(1884), v.e(6621), v.e(998), v.e(3485), v.e(2620), v.e(1997), v.e(8156), v.e(3625), v.e(7934), v.e(8959), v.e(3546), v.e(9843)]).then((() => () => v(36621))))),
-        49922: () => b("default", "@jupyterlab/extensionmanager", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(9151), v.e(8156), v.e(1167), v.e(7934), v.e(611)]).then((() => () => v(59151))))),
-        52138: () => b("default", "@jupyterlab/lsp", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(3512), v.e(998), v.e(1997), v.e(1167), v.e(979), v.e(611)]).then((() => () => v(13512))))),
-        81350: () => b("default", "@jupyterlab/htmlviewer", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(1997), v.e(8156), v.e(1167), v.e(979), v.e(377)]).then((() => () => v(35325))))),
-        94889: () => b("default", "@jupyterlab/imageviewer", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3485), v.e(1167), v.e(979), v.e(8928)]).then((() => () => v(67900))))),
-        97592: () => b("default", "@jupyterlab/markdownviewer", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3485), v.e(1997), v.e(979), v.e(7812)]).then((() => () => v(99680))))),
-        83149: () => b("default", "@jupyterlab/mermaid", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(3485), v.e(1167), v.e(2615)]).then((() => () => v(92615))))),
-        40465: () => b("default", "@jupyterlab/metadataform", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(6049), v.e(3485), v.e(8156), v.e(7478), v.e(9852)]).then((() => () => v(22924))))),
-        81692: () => f("default", "@jupyterlab/nbformat", [1, 4, 2, 0, , "rc", 0], (() => v.e(2813).then((() => () => v(23325))))),
-        57355: () => f("default", "@jupyterlab/pluginmanager", [1, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(9821), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(1167), v.e(611)]).then((() => () => v(69821))))),
-        41070: () => b("default", "@jupyterlab/rendermime-interfaces", [2, 3, 10, 0, , "rc", 0], (() => v.e(5297).then((() => () => v(75297))))),
-        80554: () => f("default", "@lumino/keyboard", [1, 2, 0, 1], (() => v.e(9222).then((() => () => v(19222))))),
-        15327: () => b("default", "@jupyterlab/tooltip", [2, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(998), v.e(2620), v.e(2167)]).then((() => () => v(51647))))),
-        24885: () => f("default", "@rjsf/utils", [1, 5, 13, 4], (() => Promise.all([v.e(7811), v.e(7995), v.e(8156)]).then((() => () => v(57995))))),
-        60053: () => f("default", "react-toastify", [1, 9, 0, 8], (() => v.e(5765).then((() => () => v(25777))))),
-        51120: () => f("default", "@codemirror/lang-markdown", [1, 6, 2, 4], (() => Promise.all([v.e(5850), v.e(9239), v.e(9799), v.e(7866), v.e(6271), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(76271))))),
-        37544: () => f("default", "@jupyterlab/csvviewer", [1, 4, 2, 0, , "rc", 0], (() => Promise.all([v.e(8032), v.e(9072), v.e(8060)]).then((() => () => v(65313))))),
-        74329: () => f("default", "marked", [1, 9, 1, 2], (() => v.e(3079).then((() => () => v(33079))))),
-        24152: () => f("default", "marked-gfm-heading-id", [1, 3, 1, 0], (() => v.e(7179).then((() => () => v(67179))))),
-        29853: () => f("default", "marked-mangle", [1, 1, 1, 4], (() => v.e(1869).then((() => () => v(81869)))))
+        return n && n.then ? n.then(e.bind(e, t, v.S[t], l, r, a)) : e(t, v.S[t], l, r, a)
+    })(((e, t, l, r, a) => t && v.o(t, l) ? m(t, 0, l, r) : a())), P = b(((e, t, l, r, a) => {
+        var n = t && v.o(t, l) && h(t, l, r);
+        return n ? d(n) : a()
+    })), y = {}, c = {
+        68722: () => f("default", "@jupyterlab/coreutils", [2, 6, 2, 0], (() => Promise.all([v.e(2866), v.e(998), v.e(1997)]).then((() => () => v(2866))))),
+        59625: () => P("default", "@jupyter-notebook/application", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(901), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(3625), v.e(8722), v.e(4604), v.e(1221), v.e(2549), v.e(7934), v.e(5903), v.e(9503), v.e(4421), v.e(5135)]).then((() => () => v(45135))))),
+        97708: () => P("default", "@jupyterlab/docmanager-extension", [2, 4, 2, 0], (() => Promise.all([v.e(8471), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(4604), v.e(3295), v.e(1098), v.e(1053), v.e(5094)]).then((() => () => v(8471))))),
+        1262: () => P("default", "@jupyterlab/theme-light-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(5426)]).then((() => () => v(45426))))),
+        1598: () => P("default", "@jupyterlab/metadataform-extension", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(2030), v.e(5613), v.e(3295), v.e(5460), v.e(2077), v.e(9335)]).then((() => () => v(89335))))),
+        9828: () => P("default", "@jupyter-notebook/application-extension", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(4604), v.e(3295), v.e(1221), v.e(2549), v.e(5903), v.e(9879), v.e(5094), v.e(7260), v.e(3712), v.e(8579)]).then((() => () => v(88579))))),
+        20531: () => P("default", "@jupyterlab/hub-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(4604), v.e(7684)]).then((() => () => v(56893))))),
+        20671: () => P("default", "@jupyterlab/csvviewer-extension", [2, 4, 2, 0], (() => Promise.all([v.e(1827), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(4604), v.e(3295), v.e(5903), v.e(9879), v.e(5183)]).then((() => () => v(41827))))),
+        22413: () => P("default", "@jupyterlab/pluginmanager-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(5613), v.e(4604), v.e(9033), v.e(3187)]).then((() => () => v(53187))))),
+        27854: () => P("default", "@jupyterlab/pdf-extension", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(3485), v.e(2549), v.e(4058)]).then((() => () => v(84058))))),
+        27993: () => P("default", "@jupyterlab/running-extension", [2, 4, 2, 0], (() => Promise.all([v.e(7854), v.e(2030), v.e(3312), v.e(5613), v.e(1997), v.e(8156), v.e(4604), v.e(7934), v.e(5903), v.e(1053), v.e(5094), v.e(9235)]).then((() => () => v(97854))))),
+        28574: () => P("default", "@jupyter-notebook/terminal-extension", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(3625), v.e(4604), v.e(5333), v.e(1684)]).then((() => () => v(95601))))),
+        33e3: () => P("default", "@jupyterlab/tooltip-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3485), v.e(3625), v.e(1221), v.e(5460), v.e(7260), v.e(4663), v.e(7865), v.e(2088)]).then((() => () => v(6604))))),
+        34409: () => P("default", "@jupyterlab/filebrowser-extension", [2, 4, 2, 0], (() => Promise.all([v.e(893), v.e(2030), v.e(3312), v.e(5613), v.e(3625), v.e(4604), v.e(3295), v.e(1098), v.e(1053), v.e(5094), v.e(6934), v.e(1427)]).then((() => () => v(30893))))),
+        36488: () => P("default", "@jupyterlab/extensionmanager-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(5613), v.e(4604), v.e(3295), v.e(2311)]).then((() => () => v(22311))))),
+        40364: () => P("default", "@jupyterlab/mathjax-extension", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(1221), v.e(1408)]).then((() => () => v(11408))))),
+        41145: () => P("default", "@jupyterlab/markedparser-extension", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(1221), v.e(525), v.e(8337), v.e(3129)]).then((() => () => v(79268))))),
+        43200: () => P("default", "@jupyter-notebook/notebook-extension", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(8156), v.e(3295), v.e(7934), v.e(9879), v.e(5094), v.e(5460), v.e(5573)]).then((() => () => v(5573))))),
+        43258: () => P("default", "@jupyterlab/fileeditor-extension", [2, 4, 2, 0], (() => Promise.all([v.e(7603), v.e(2030), v.e(3312), v.e(5613), v.e(3625), v.e(4604), v.e(3295), v.e(1098), v.e(1429), v.e(9879), v.e(9426), v.e(5183), v.e(525), v.e(1427), v.e(7260), v.e(1907), v.e(6810), v.e(4663), v.e(1002), v.e(3831)]).then((() => () => v(97603))))),
+        46037: () => P("default", "@jupyterlab/javascript-extension", [2, 4, 2, 0], (() => Promise.all([v.e(1221), v.e(5733)]).then((() => () => v(65733))))),
+        47494: () => P("default", "@jupyterlab/apputils-extension", [2, 4, 2, 0], (() => Promise.all([v.e(5099), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(3625), v.e(4604), v.e(3295), v.e(2549), v.e(7934), v.e(5903), v.e(1098), v.e(7408), v.e(9879), v.e(8395), v.e(1053), v.e(6934), v.e(8005), v.e(2164)]).then((() => () => v(25099))))),
+        53440: () => P("default", "@jupyterlab/mainmenu-extension", [2, 4, 2, 0], (() => Promise.all([v.e(545), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(3625), v.e(4604), v.e(3295), v.e(7408), v.e(9879), v.e(5094), v.e(1427)]).then((() => () => v(60545))))),
+        53929: () => P("default", "@jupyterlab/ui-components-extension", [2, 4, 2, 0], (() => Promise.all([v.e(5613), v.e(3863)]).then((() => () => v(73863))))),
+        54669: () => P("default", "@jupyterlab/celltags-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(5613), v.e(8156), v.e(3625), v.e(5460), v.e(5346)]).then((() => () => v(15346))))),
+        57926: () => P("default", "@jupyterlab/shortcuts-extension", [2, 5, 0, 0], (() => Promise.all([v.e(113), v.e(998), v.e(2030), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(3295), v.e(2549), v.e(8395), v.e(6934), v.e(554)]).then((() => () => v(113))))),
+        60323: () => P("default", "@jupyterlab/codemirror-extension", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(2030), v.e(5613), v.e(8156), v.e(4604), v.e(3295), v.e(1098), v.e(1429), v.e(525), v.e(7478), v.e(3831), v.e(7592), v.e(7655)]).then((() => () => v(97655))))),
+        61072: () => P("default", "@jupyterlab/application-extension", [2, 4, 2, 0], (() => Promise.all([v.e(3881), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(3625), v.e(4604), v.e(3295), v.e(2549), v.e(1098), v.e(1053), v.e(6934), v.e(7872)]).then((() => () => v(92871))))),
+        61092: () => P("default", "@jupyter-notebook/console-extension", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(3625), v.e(4604), v.e(7260), v.e(6345)]).then((() => () => v(94645))))),
+        66299: () => P("default", "@jupyterlab/markdownviewer-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(4604), v.e(3295), v.e(1221), v.e(9426), v.e(3991), v.e(7252)]).then((() => () => v(79685))))),
+        74516: () => P("default", "@jupyterlab/help-extension", [2, 4, 2, 0], (() => Promise.all([v.e(1496), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(4604), v.e(7408), v.e(9879), v.e(4475)]).then((() => () => v(91496))))),
+        74695: () => P("default", "@jupyter-notebook/docmanager-extension", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(1997), v.e(5094), v.e(8875)]).then((() => () => v(71650))))),
+        74733: () => P("default", "@jupyter-notebook/tree-extension", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3295), v.e(1427), v.e(9235), v.e(4258), v.e(4803), v.e(7302)]).then((() => () => v(83768))))),
+        75347: () => P("default", "@jupyterlab/mermaid-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(8337), v.e(9161)]).then((() => () => v(79161))))),
+        77089: () => P("default", "@jupyterlab/console-extension", [2, 4, 2, 0], (() => Promise.all([v.e(6748), v.e(998), v.e(2030), v.e(3312), v.e(5613), v.e(3625), v.e(4604), v.e(3295), v.e(1221), v.e(2549), v.e(1429), v.e(9879), v.e(4421), v.e(1427), v.e(7260), v.e(6810), v.e(1002)]).then((() => () => v(86748))))),
+        77619: () => P("default", "@jupyterlab/toc-extension", [2, 6, 2, 0], (() => Promise.all([v.e(2030), v.e(5613), v.e(4604), v.e(3295), v.e(9426), v.e(62)]).then((() => () => v(40062))))),
+        77659: () => P("default", "@jupyterlab/lsp-extension", [2, 4, 2, 0], (() => Promise.all([v.e(3466), v.e(998), v.e(2030), v.e(3312), v.e(5613), v.e(1997), v.e(8156), v.e(3295), v.e(7934), v.e(1907), v.e(9235)]).then((() => () => v(83466))))),
+        78007: () => P("default", "@jupyterlab/cell-toolbar-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(3295), v.e(2122)]).then((() => () => v(92122))))),
+        78390: () => P("default", "@jupyter-notebook/documentsearch-extension", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(5183), v.e(7906)]).then((() => () => v(54382))))),
+        78608: () => P("default", "@jupyterlab/translation-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(4604), v.e(3295), v.e(9879), v.e(6815)]).then((() => () => v(56815))))),
+        78917: () => P("default", "@jupyterlab/completer-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(5613), v.e(8156), v.e(3295), v.e(6934), v.e(1002), v.e(3340)]).then((() => () => v(33340))))),
+        79680: () => P("default", "@jupyterlab/notebook-extension", [2, 4, 2, 0], (() => Promise.all([v.e(1962), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(3625), v.e(4604), v.e(3295), v.e(1221), v.e(2549), v.e(7934), v.e(1098), v.e(7408), v.e(9503), v.e(1429), v.e(9879), v.e(1053), v.e(5094), v.e(1231), v.e(9426), v.e(5183), v.e(525), v.e(5460), v.e(1427), v.e(1907), v.e(3166), v.e(6810), v.e(1002), v.e(7872), v.e(4182), v.e(2077)]).then((() => () => v(51962))))),
+        84228: () => P("default", "@jupyterlab/theme-dark-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(6627)]).then((() => () => v(6627))))),
+        86652: () => P("default", "@jupyterlab/settingeditor-extension", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(2030), v.e(3312), v.e(5613), v.e(4604), v.e(3295), v.e(1221), v.e(1429), v.e(1053), v.e(9033), v.e(8633)]).then((() => () => v(98633))))),
+        87360: () => P("default", "@jupyterlab/json-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(8156), v.e(8005), v.e(690)]).then((() => () => v(60690))))),
+        89770: () => P("default", "@jupyterlab/htmlviewer-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(5613), v.e(4604), v.e(3295), v.e(6962)]).then((() => () => v(56962))))),
+        90388: () => P("default", "@jupyterlab/imageviewer-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(4604), v.e(6139)]).then((() => () => v(56139))))),
+        90748: () => P("default", "@jupyter-notebook/help-extension", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(2030), v.e(3312), v.e(8156), v.e(9879), v.e(3712), v.e(9380)]).then((() => () => v(19380))))),
+        92783: () => P("default", "@jupyterlab/vega5-extension", [2, 4, 2, 0], (() => Promise.all([v.e(3485), v.e(6061)]).then((() => () => v(16061))))),
+        94414: () => P("default", "@jupyterlab/documentsearch-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(4604), v.e(3295), v.e(5183), v.e(4212)]).then((() => () => v(24212))))),
+        96291: () => P("default", "@jupyterlab/terminal-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(4604), v.e(3295), v.e(7408), v.e(9879), v.e(9235), v.e(6810), v.e(5333), v.e(5912)]).then((() => () => v(15912))))),
+        97818: () => P("default", "@jupyterlab/theme-dark-high-contrast-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2030), v.e(3312), v.e(5254)]).then((() => () => v(95254))))),
+        98128: () => P("default", "@jupyterlab/debugger-extension", [2, 4, 2, 0], (() => Promise.all([v.e(2184), v.e(2030), v.e(3312), v.e(4604), v.e(3295), v.e(1221), v.e(5903), v.e(1429), v.e(5460), v.e(7260), v.e(3166), v.e(4663), v.e(4182), v.e(3050)]).then((() => () => v(42184))))),
+        3546: () => f("default", "@codemirror/view", [2, 6, 26, 1], (() => Promise.all([v.e(2955), v.e(9843)]).then((() => () => v(22955))))),
+        89843: () => f("default", "@codemirror/state", [2, 6, 4, 1], (() => v.e(2323).then((() => () => v(92323))))),
+        79352: () => f("default", "@lezer/common", [2, 1, 2, 1], (() => v.e(7997).then((() => () => v(97997))))),
+        17592: () => P("default", "@codemirror/language", [1, 6, 10, 1], (() => Promise.all([v.e(1584), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(31584))))),
+        92209: () => f("default", "@lezer/highlight", [2, 1, 2, 0], (() => Promise.all([v.e(3797), v.e(9352)]).then((() => () => v(23797))))),
+        20998: () => f("default", "@lumino/coreutils", [2, 2, 1, 2], (() => v.e(2756).then((() => () => v(12756))))),
+        12030: () => f("default", "@jupyterlab/translation", [2, 4, 2, 0], (() => Promise.all([v.e(7819), v.e(998), v.e(8722), v.e(7408), v.e(1053)]).then((() => () => v(57819))))),
+        53312: () => f("default", "@jupyterlab/apputils", [2, 4, 3, 0], (() => Promise.all([v.e(9605), v.e(998), v.e(2030), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(3295), v.e(2549), v.e(1098), v.e(7408), v.e(9503), v.e(8395), v.e(1053), v.e(1231), v.e(3752)]).then((() => () => v(89605))))),
+        63485: () => f("default", "@lumino/widgets", [2, 2, 3, 2], (() => Promise.all([v.e(911), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503), v.e(8395), v.e(4421), v.e(6934), v.e(4475), v.e(9615), v.e(554)]).then((() => () => v(30911))))),
+        44604: () => f("default", "@jupyterlab/application", [2, 4, 2, 0], (() => Promise.all([v.e(901), v.e(6853), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(3625), v.e(8722), v.e(1221), v.e(2549), v.e(7934), v.e(5903), v.e(7408), v.e(9503), v.e(4421), v.e(4771)]).then((() => () => v(76853))))),
+        23295: () => f("default", "@jupyterlab/settingregistry", [2, 4, 2, 0], (() => Promise.all([v.e(7796), v.e(5649), v.e(998), v.e(1997), v.e(2549), v.e(6934)]).then((() => () => v(5649))))),
+        81221: () => f("default", "@jupyterlab/rendermime", [2, 4, 2, 0], (() => Promise.all([v.e(2401), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(1997), v.e(8722), v.e(1231), v.e(1139), v.e(2425)]).then((() => () => v(72401))))),
+        2549: () => f("default", "@lumino/disposable", [2, 2, 1, 2], (() => Promise.all([v.e(1997), v.e(5451)]).then((() => () => v(65451))))),
+        65903: () => P("default", "@jupyterlab/docregistry", [2, 4, 2, 0], (() => Promise.all([v.e(2489), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(1221), v.e(2549), v.e(9503), v.e(1429)]).then((() => () => v(72489))))),
+        29879: () => f("default", "@jupyterlab/mainmenu", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(3485), v.e(5613), v.e(3625), v.e(2607)]).then((() => () => v(12007))))),
+        5094: () => f("default", "@jupyterlab/docmanager", [2, 4, 2, 0], (() => Promise.all([v.e(7543), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(2549), v.e(7934), v.e(5903), v.e(1098), v.e(9503), v.e(4421)]).then((() => () => v(37543))))),
+        67260: () => f("default", "@jupyterlab/console", [2, 4, 2, 0], (() => Promise.all([v.e(2636), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8722), v.e(1221), v.e(1231), v.e(3546), v.e(9843), v.e(9615), v.e(3166), v.e(7508)]).then((() => () => v(72636))))),
+        93712: () => P("default", "@jupyter-notebook/ui-components", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(5613), v.e(9068)]).then((() => () => v(59068))))),
+        35613: () => f("default", "@jupyterlab/ui-components", [2, 4, 2, 0], (() => Promise.all([v.e(1884), v.e(755), v.e(7811), v.e(7506), v.e(998), v.e(2030), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(2549), v.e(7934), v.e(9503), v.e(4421), v.e(6934), v.e(4475), v.e(8005), v.e(4885)]).then((() => () => v(7506))))),
+        81997: () => f("default", "@lumino/signaling", [2, 2, 1, 2], (() => Promise.all([v.e(998), v.e(3625), v.e(409)]).then((() => () => v(40409))))),
+        33625: () => f("default", "@lumino/algorithm", [2, 2, 0, 1], (() => v.e(5614).then((() => () => v(15614))))),
+        97934: () => P("default", "@lumino/polling", [1, 2, 1, 2], (() => Promise.all([v.e(998), v.e(1997), v.e(4271)]).then((() => () => v(64271))))),
+        49503: () => f("default", "@lumino/messaging", [2, 2, 0, 1], (() => Promise.all([v.e(7821), v.e(3625)]).then((() => () => v(77821))))),
+        14421: () => f("default", "@lumino/properties", [2, 2, 0, 1], (() => v.e(3733).then((() => () => v(13733))))),
+        95183: () => f("default", "@jupyterlab/documentsearch", [2, 4, 2, 0], (() => Promise.all([v.e(6999), v.e(998), v.e(2030), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(2549), v.e(7934), v.e(6934)]).then((() => () => v(36999))))),
+        78156: () => f("default", "react", [2, 18, 2, 0], (() => v.e(7378).then((() => () => v(27378))))),
+        25460: () => f("default", "@jupyterlab/notebook", [2, 4, 2, 0], (() => Promise.all([v.e(374), v.e(998), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(7934), v.e(5903), v.e(1098), v.e(7408), v.e(9503), v.e(1429), v.e(8395), v.e(1231), v.e(4421), v.e(9426), v.e(5183), v.e(4475), v.e(1907), v.e(9615), v.e(3166), v.e(7508), v.e(1139)]).then((() => () => v(90374))))),
+        5333: () => f("default", "@jupyterlab/terminal", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(2030), v.e(3485), v.e(9503), v.e(8395), v.e(3213)]).then((() => () => v(53213))))),
+        71427: () => f("default", "@jupyterlab/filebrowser", [2, 4, 2, 0], (() => Promise.all([v.e(9341), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(7934), v.e(5903), v.e(1098), v.e(7408), v.e(9503), v.e(8395), v.e(5094), v.e(4475), v.e(9615)]).then((() => () => v(39341))))),
+        9235: () => P("default", "@jupyterlab/running", [1, 4, 2, 0], (() => Promise.all([v.e(1809), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(2549), v.e(8395)]).then((() => () => v(1809))))),
+        74258: () => f("default", "@jupyterlab/settingeditor", [2, 4, 2, 0], (() => Promise.all([v.e(3360), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(8722), v.e(1221), v.e(7934), v.e(1429), v.e(1053), v.e(7478)]).then((() => () => v(63360))))),
+        64803: () => f("default", "@jupyter-notebook/tree", [2, 7, 2, 0, , "rc", 1], (() => Promise.all([v.e(998), v.e(4837)]).then((() => () => v(73146))))),
+        17843: () => f("default", "yjs", [2, 13, 6, 8], (() => v.e(7957).then((() => () => v(67957))))),
+        71098: () => f("default", "@jupyterlab/statusbar", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(3485), v.e(8156), v.e(3625), v.e(2549), v.e(7639)]).then((() => () => v(53680))))),
+        41053: () => f("default", "@jupyterlab/statedb", [2, 4, 2, 0], (() => Promise.all([v.e(4526), v.e(998), v.e(1997), v.e(4421)]).then((() => () => v(34526))))),
+        16934: () => f("default", "@lumino/commands", [2, 2, 3, 0], (() => Promise.all([v.e(3301), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(8395), v.e(554)]).then((() => () => v(43301))))),
+        77872: () => P("default", "@jupyterlab/property-inspector", [1, 4, 2, 0], (() => Promise.all([v.e(1997), v.e(8907)]).then((() => () => v(41198))))),
+        87408: () => f("default", "@jupyterlab/services", [2, 7, 2, 0], (() => Promise.all([v.e(3676), v.e(998), v.e(1997), v.e(8722), v.e(2549), v.e(7934), v.e(1053)]).then((() => () => v(83676))))),
+        34771: () => f("default", "@lumino/application", [2, 2, 3, 1], (() => Promise.all([v.e(6731), v.e(6934)]).then((() => () => v(16731))))),
+        18395: () => f("default", "@lumino/domutils", [2, 2, 0, 1], (() => v.e(1696).then((() => () => v(1696))))),
+        38005: () => f("default", "react-dom", [2, 18, 2, 0], (() => v.e(1542).then((() => () => v(31542))))),
+        72164: () => P("default", "@jupyterlab/workspaces", [1, 4, 2, 0], (() => Promise.all([v.e(1997), v.e(5166)]).then((() => () => v(11828))))),
+        31231: () => f("default", "@jupyterlab/observables", [2, 5, 2, 0], (() => Promise.all([v.e(170), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503)]).then((() => () => v(10170))))),
+        82426: () => f("default", "@jupyterlab/cell-toolbar", [2, 4, 2, 0], (() => Promise.all([v.e(5613), v.e(1997), v.e(3625), v.e(1231), v.e(4811)]).then((() => () => v(37386))))),
+        51429: () => f("default", "@jupyterlab/codeeditor", [2, 4, 2, 0], (() => Promise.all([v.e(7391), v.e(998), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(1098), v.e(1231), v.e(7508)]).then((() => () => v(77391))))),
+        79426: () => P("default", "@jupyterlab/toc", [1, 6, 2, 0], (() => Promise.all([v.e(5921), v.e(998), v.e(3312), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(8722), v.e(1221), v.e(2549)]).then((() => () => v(75921))))),
+        30525: () => f("default", "@jupyterlab/codemirror", [2, 4, 2, 0], (() => Promise.all([v.e(9799), v.e(5263), v.e(998), v.e(2030), v.e(1997), v.e(8722), v.e(1429), v.e(5183), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(3831), v.e(7592), v.e(7843)]).then((() => () => v(95263))))),
+        24475: () => f("default", "@lumino/virtualdom", [2, 2, 0, 1], (() => Promise.all([v.e(5234), v.e(3625)]).then((() => () => v(85234))))),
+        57508: () => f("default", "@jupyter/ydoc", [2, 2, 0, 1], (() => Promise.all([v.e(35), v.e(7843)]).then((() => () => v(50035))))),
+        44946: () => f("default", "@jupyterlab/outputarea", [2, 4, 2, 0], (() => Promise.all([v.e(7226), v.e(3312), v.e(3625), v.e(7408), v.e(1231), v.e(4421), v.e(1139)]).then((() => () => v(47226))))),
+        42193: () => P("default", "@jupyterlab/attachments", [2, 4, 2, 0], (() => Promise.all([v.e(1231), v.e(134)]).then((() => () => v(44042))))),
+        27478: () => P("default", "@rjsf/validator-ajv8", [1, 5, 13, 4], (() => Promise.all([v.e(755), v.e(7796), v.e(131), v.e(4885)]).then((() => () => v(70131))))),
+        24636: () => P("default", "@codemirror/search", [1, 6, 5, 6], (() => Promise.all([v.e(5261), v.e(3546), v.e(9843)]).then((() => () => v(25261))))),
+        87797: () => P("default", "@codemirror/commands", [1, 6, 3, 3], (() => Promise.all([v.e(7450), v.e(3546), v.e(9843), v.e(9352), v.e(7592)]).then((() => () => v(67450))))),
+        81002: () => f("default", "@jupyterlab/completer", [2, 4, 2, 0], (() => Promise.all([v.e(2944), v.e(998), v.e(3312), v.e(3485), v.e(1997), v.e(3625), v.e(8722), v.e(1221), v.e(9503), v.e(1429), v.e(8395), v.e(3546), v.e(9843)]).then((() => () => v(62944))))),
+        86810: () => P("default", "@jupyterlab/launcher", [1, 4, 2, 0], (() => Promise.all([v.e(998), v.e(3485), v.e(8156), v.e(3625), v.e(2549), v.e(4421), v.e(9638)]).then((() => () => v(68771))))),
+        99615: () => f("default", "@lumino/dragdrop", [2, 2, 1, 4], (() => Promise.all([v.e(4291), v.e(2549)]).then((() => () => v(54291))))),
+        73166: () => P("default", "@jupyterlab/cells", [2, 4, 2, 0], (() => Promise.all([v.e(2479), v.e(998), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(1221), v.e(7934), v.e(9503), v.e(1429), v.e(8395), v.e(9426), v.e(5183), v.e(3546), v.e(525), v.e(4475), v.e(7508), v.e(4946), v.e(2193)]).then((() => () => v(72479))))),
+        59072: () => P("default", "@lumino/datagrid", [1, 2, 3, 1], (() => Promise.all([v.e(8929), v.e(3625), v.e(9503), v.e(8395), v.e(9615), v.e(554)]).then((() => () => v(98929))))),
+        34663: () => f("default", "@jupyterlab/fileeditor", [2, 4, 2, 0], (() => Promise.all([v.e(1833), v.e(998), v.e(3312), v.e(3485), v.e(5613), v.e(8156), v.e(5903), v.e(1098), v.e(1429), v.e(9426), v.e(525), v.e(1907)]).then((() => () => v(31833))))),
+        44182: () => P("default", "@jupyterlab/logconsole", [1, 4, 2, 0], (() => Promise.all([v.e(2089), v.e(998), v.e(3485), v.e(1997), v.e(4946)]).then((() => () => v(2089))))),
+        63050: () => f("default", "@jupyterlab/debugger", [2, 4, 2, 0], (() => Promise.all([v.e(1884), v.e(6621), v.e(998), v.e(3485), v.e(5613), v.e(1997), v.e(8156), v.e(3625), v.e(7934), v.e(1231), v.e(3546), v.e(9843)]).then((() => () => v(36621))))),
+        95411: () => f("default", "@jupyterlab/extensionmanager", [2, 4, 2, 0], (() => Promise.all([v.e(9151), v.e(8156), v.e(8722), v.e(7934), v.e(7408)]).then((() => () => v(59151))))),
+        61907: () => f("default", "@jupyterlab/lsp", [2, 4, 2, 0], (() => Promise.all([v.e(3512), v.e(998), v.e(1997), v.e(8722), v.e(5903), v.e(7408)]).then((() => () => v(13512))))),
+        57957: () => f("default", "@jupyterlab/htmlviewer", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(1997), v.e(8156), v.e(8722), v.e(5903), v.e(377)]).then((() => () => v(35325))))),
+        43269: () => f("default", "@jupyterlab/imageviewer", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(3485), v.e(8722), v.e(5903), v.e(8928)]).then((() => () => v(67900))))),
+        3991: () => f("default", "@jupyterlab/markdownviewer", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(3485), v.e(1997), v.e(5903), v.e(7812)]).then((() => () => v(99680))))),
+        8337: () => f("default", "@jupyterlab/mermaid", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(3485), v.e(8722), v.e(2615)]).then((() => () => v(92615))))),
+        12077: () => f("default", "@jupyterlab/metadataform", [2, 4, 2, 0], (() => Promise.all([v.e(3312), v.e(3485), v.e(8156), v.e(7478), v.e(9852)]).then((() => () => v(22924))))),
+        81139: () => P("default", "@jupyterlab/nbformat", [1, 4, 2, 0], (() => v.e(2813).then((() => () => v(23325))))),
+        9033: () => P("default", "@jupyterlab/pluginmanager", [1, 4, 2, 0], (() => Promise.all([v.e(9821), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(8722), v.e(7408)]).then((() => () => v(69821))))),
+        22425: () => f("default", "@jupyterlab/rendermime-interfaces", [2, 3, 10, 0], (() => v.e(5297).then((() => () => v(75297))))),
+        80554: () => P("default", "@lumino/keyboard", [1, 2, 0, 1], (() => v.e(9222).then((() => () => v(19222))))),
+        27865: () => f("default", "@jupyterlab/tooltip", [2, 4, 2, 0], (() => Promise.all([v.e(998), v.e(5613), v.e(2167)]).then((() => () => v(51647))))),
+        24885: () => P("default", "@rjsf/utils", [1, 5, 13, 4], (() => Promise.all([v.e(7811), v.e(7995), v.e(8156)]).then((() => () => v(57995))))),
+        60053: () => P("default", "react-toastify", [1, 9, 0, 8], (() => v.e(5765).then((() => () => v(25777))))),
+        51120: () => P("default", "@codemirror/lang-markdown", [1, 6, 2, 4], (() => Promise.all([v.e(5850), v.e(9239), v.e(9799), v.e(7866), v.e(6271), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(76271))))),
+        16478: () => P("default", "@jupyterlab/csvviewer", [1, 4, 2, 0], (() => Promise.all([v.e(8032), v.e(9072), v.e(8060)]).then((() => () => v(65313))))),
+        74329: () => P("default", "marked", [1, 9, 1, 2], (() => v.e(3079).then((() => () => v(33079))))),
+        24152: () => P("default", "marked-gfm-heading-id", [1, 3, 1, 0], (() => v.e(7179).then((() => () => v(67179))))),
+        29853: () => P("default", "marked-mangle", [1, 1, 1, 4], (() => v.e(1869).then((() => () => v(81869)))))
     }, j = {
         53: [60053],
-        106: [80106],
-        465: [40465],
+        525: [30525],
         554: [80554],
-        611: [70611],
-        845: [50845],
-        979: [10979],
         998: [20998],
-        1070: [41070],
+        1002: [81002],
+        1053: [41053],
+        1098: [71098],
         1120: [51120],
-        1131: [1131],
-        1167: [1167],
-        1692: [81692],
-        1942: [91942],
+        1139: [81139],
+        1221: [81221],
+        1231: [31231],
+        1427: [71427],
+        1429: [51429],
+        1907: [61907],
         1997: [81997],
-        2122: [5510],
-        2138: [52138],
+        2030: [12030],
+        2077: [12077],
+        2122: [82426],
+        2164: [72164],
+        2193: [42193],
         2209: [92209],
-        2311: [49922],
-        2367: [42367],
+        2311: [95411],
+        2425: [22425],
         2549: [2549],
-        2620: [22620],
-        2703: [42703],
-        2751: [42751],
-        2839: [52839],
-        2922: [2922],
-        3149: [83149],
-        3408: [13408],
+        3050: [63050],
+        3166: [73166],
+        3295: [23295],
+        3312: [53312],
         3485: [63485],
         3546: [3546],
         3625: [33625],
+        3712: [93712],
         3831: [24636, 87797],
-        3892: [13892],
+        3991: [3991],
         4152: [24152],
+        4182: [44182],
+        4258: [74258],
         4329: [74329],
         4421: [14421],
         4475: [24475],
-        4554: [24554],
+        4604: [44604],
+        4663: [34663],
         4771: [34771],
+        4803: [64803],
         4885: [24885],
-        5327: [15327],
-        5651: [65651],
-        5729: [15729],
-        5910: [97592],
-        6017: [37544],
-        6049: [96049],
-        6139: [94889],
-        6692: [96692],
-        6724: [66724],
-        6726: [36726],
-        6807: [46807],
-        6862: [26862],
+        4946: [44946],
+        5094: [5094],
+        5183: [95183],
+        5333: [5333],
+        5460: [25460],
+        5613: [35613],
+        5903: [65903],
+        6017: [16478],
+        6139: [43269],
+        6810: [86810],
         6934: [16934],
-        6962: [81350],
-        7017: [87017],
-        7267: [37267],
-        7355: [57355],
-        7406: [67406],
+        6962: [57957],
+        7260: [67260],
+        7408: [87408],
         7478: [27478],
         7508: [57508],
         7592: [17592],
-        7829: [27829],
+        7708: [97708],
         7843: [17843],
-        7894: [17894],
+        7865: [27865],
+        7872: [77872],
         7934: [97934],
         8005: [38005],
         8156: [78156],
-        8289: [98289],
+        8337: [8337],
         8395: [18395],
-        8602: [18602],
-        8603: [98603],
-        8625: [18625],
-        8781: [252, 5890, 8467, 9269, 13375, 17420, 18173, 18403, 24124, 25622, 28654, 29272, 31716, 32374, 39137, 39519, 40682, 44250, 46456, 48618, 53160, 56727, 56823, 57782, 61182, 61378, 63728, 65028, 65477, 65787, 66889, 68449, 70545, 70952, 73898, 74572, 76156, 77429, 78085, 78578, 82818, 83421, 88378, 90856, 92396, 94388, 95496, 99223, 99526],
-        8959: [58959],
+        8722: [68722],
+        8781: [1262, 1598, 9828, 20531, 20671, 22413, 27854, 27993, 28574, 33e3, 34409, 36488, 40364, 41145, 43200, 43258, 46037, 47494, 53440, 53929, 54669, 57926, 60323, 61072, 61092, 66299, 74516, 74695, 74733, 75347, 77089, 77619, 77659, 78007, 78390, 78608, 78917, 79680, 84228, 86652, 87360, 89770, 90388, 90748, 92783, 94414, 96291, 97818, 98128],
+        9033: [9033],
         9072: [59072],
-        9144: [89144],
-        9200: [69200],
-        9269: [49269],
+        9235: [9235],
         9352: [79352],
+        9426: [79426],
         9503: [49503],
         9615: [99615],
-        9713: [49713],
+        9625: [59625],
         9843: [89843],
-        9853: [29853]
+        9853: [29853],
+        9879: [29879]
     }, v.f.consumes = (e, t) => {
         v.o(j, e) && j[e].forEach((e => {
-            if (v.o(P, e)) return t.push(P[e]);
-            var r = t => {
-                    P[e] = 0, v.m[e] = r => {
-                        delete v.c[e], r.exports = t()
+            if (v.o(y, e)) return t.push(y[e]);
+            var l = t => {
+                    y[e] = 0, v.m[e] = l => {
+                        delete v.c[e], l.exports = t()
                     }
                 },
-                l = t => {
-                    delete P[e], v.m[e] = r => {
+                r = t => {
+                    delete y[e], v.m[e] = l => {
                         throw delete v.c[e], t
                     }
                 };
             try {
-                var a = y[e]();
-                a.then ? t.push(P[e] = a.then(r).catch(l)) : r(a)
+                var a = c[e]();
+                a.then ? t.push(y[e] = a.then(l).catch(r)) : l(a)
             } catch (e) {
-                l(e)
+                r(e)
             }
         }))
     }, (() => {
         v.b = document.baseURI || self.location.href;
         var e = {
             179: 0
         };
-        v.f.j = (t, r) => {
-            var l = v.o(e, t) ? e[t] : void 0;
-            if (0 !== l)
-                if (l) r.push(l[2]);
-                else if (/^(1(1(20|31|67)|06|070|692|942|997)|2((20|54|83)9|138|367|620|703|751|922)|3(149|408|485|546|625|831|892)|4((47|6|88)5|152|329|421|554|771)|5(3|327|54|651|729|910)|6(72[46]|049|11|692|807|862|934)|7(8(29|43|94)|017|267|355|406|478|508|592|934)|8(6(02|03|25)|(00|39|4)5|156|289|959)|9((50|71|84|85)3|072|144|200|269|352|615|79|98))$/.test(t)) e[t] = 0;
+        v.f.j = (t, l) => {
+            var r = v.o(e, t) ? e[t] : void 0;
+            if (0 !== r)
+                if (r) l.push(r[2]);
+                else if (/^(1(0(02|53|98)|42[79]|120|139|221|231|907|997)|2(030|077|164|193|209|425|549)|3((29|48|62)5|[37]12|050|166|546|831|991)|4(152|182|258|329|421|475|604|663|771|803|885|946)|5((|18|33|61|90)3|094|25|460|54)|7(8(43|65|72)|([457]0|47)8|260|592|934)|8(005|156|337|395|722)|9(8(43|53|79)|(23|61|62)5|033|072|352|426|503|98)|6810|6934)$/.test(t)) e[t] = 0;
             else {
-                var a = new Promise(((r, a) => l = e[t] = [r, a]));
-                r.push(l[2] = a);
+                var a = new Promise(((l, a) => r = e[t] = [l, a]));
+                l.push(r[2] = a);
                 var n = v.p + v.u(t),
                     o = new Error;
-                v.l(n, (r => {
-                    if (v.o(e, t) && (0 !== (l = e[t]) && (e[t] = void 0), l)) {
-                        var a = r && ("load" === r.type ? "missing" : r.type),
-                            n = r && r.target && r.target.src;
-                        o.message = "Loading chunk " + t + " failed.\n(" + a + ": " + n + ")", o.name = "ChunkLoadError", o.type = a, o.request = n, l[1](o)
+                v.l(n, (l => {
+                    if (v.o(e, t) && (0 !== (r = e[t]) && (e[t] = void 0), r)) {
+                        var a = l && ("load" === l.type ? "missing" : l.type),
+                            n = l && l.target && l.target.src;
+                        o.message = "Loading chunk " + t + " failed.\n(" + a + ": " + n + ")", o.name = "ChunkLoadError", o.type = a, o.request = n, r[1](o)
                     }
                 }), "chunk-" + t, t)
             }
         };
-        var t = (t, r) => {
-                var l, a, [n, o, i] = r,
+        var t = (t, l) => {
+                var r, a, [n, o, i] = l,
                     s = 0;
                 if (n.some((t => 0 !== e[t]))) {
-                    for (l in o) v.o(o, l) && (v.m[l] = o[l]);
+                    for (r in o) v.o(o, r) && (v.m[r] = o[r]);
                     i && i(v)
                 }
-                for (t && t(r); s < n.length; s++) a = n[s], v.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (t && t(l); s < n.length; s++) a = n[s], v.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
-            r = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || [];
-        r.forEach(t.bind(null, 0)), r.push = t.bind(null, r.push.bind(r))
+            l = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || [];
+        l.forEach(t.bind(null, 0)), l.push = t.bind(null, l.push.bind(l))
     })(), v.nc = void 0, v(68444);
     var k = v(37559);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).CORE_OUTPUT = k
 })();
```

### Comparing `notebook-7.2.0rc0/notebook/static/c49810b53ecc0d87d802.woff` & `notebook-7.2.0rc1/notebook/static/c49810b53ecc0d87d802.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/c56da8d69f1a0208b8e0.woff` & `notebook-7.2.0rc1/notebook/static/c56da8d69f1a0208b8e0.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/cb9e9e693192413cde2b.woff` & `notebook-7.2.0rc1/notebook/static/cb9e9e693192413cde2b.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/cda59d6efffa685830fd.ttf` & `notebook-7.2.0rc1/notebook/static/cda59d6efffa685830fd.ttf`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/e4299464e7b012968eed.eot` & `notebook-7.2.0rc1/notebook/static/e4299464e7b012968eed.eot`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/e42a88444448ac3d6054.woff2` & `notebook-7.2.0rc1/notebook/static/e42a88444448ac3d6054.woff2`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/e8711bbb871afd8e9dea.ttf` & `notebook-7.2.0rc1/notebook/static/e8711bbb871afd8e9dea.ttf`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/f9217f66874b0c01cd8c.woff` & `notebook-7.2.0rc1/notebook/static/f9217f66874b0c01cd8c.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/fc6ddf5df402b263cfb1.woff` & `notebook-7.2.0rc1/notebook/static/fc6ddf5df402b263cfb1.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/static/third-party-licenses.json` & `notebook-7.2.0rc1/notebook/static/third-party-licenses.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98241643454039%*

 * *Differences: {"'packages'": "{23: {'versionInfo': '7.2.0-rc.1'}, 24: {'versionInfo': '7.2.0-rc.1'}, 25: "*

 * *               "{'versionInfo': '7.2.0-rc.1'}, 26: {'versionInfo': '7.2.0-rc.1'}, 27: "*

 * *               "{'versionInfo': '7.2.0-rc.1'}, 28: {'versionInfo': '7.2.0-rc.1'}, 29: "*

 * *               "{'versionInfo': '7.2.0-rc.1'}, 30: {'versionInfo': '7.2.0-rc.1'}, 31: "*

 * *               "{'versionInfo': '7.2.0-rc.1'}, 32: {'versionInfo': '7.2.0-rc.1'}, 33: "*

 * *               "{'versionInfo': '7.2.0-rc.1'}, 37: {'versionInfo':  […]*

```diff
@@ -138,75 +138,75 @@
             "name": "@fortawesome/fontawesome-free",
             "versionInfo": "5.15.4"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/application",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/application-extension",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/console-extension",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/docmanager-extension",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/documentsearch-extension",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/help-extension",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/notebook-extension",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/terminal-extension",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/tree",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/tree-extension",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/ui-components",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0-rc.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/react-components",
             "versionInfo": "0.15.3"
         },
@@ -222,549 +222,549 @@
             "name": "@jupyter/ydoc",
             "versionInfo": "2.0.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/application",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/application-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/apputils",
-            "versionInfo": "4.3.0-rc.0"
+            "versionInfo": "4.3.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/apputils-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/attachments",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/cell-toolbar",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/cell-toolbar-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/cells",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/celltags-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/codeeditor",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/codemirror",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/codemirror-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/completer",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/completer-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/console",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/console-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/coreutils",
-            "versionInfo": "6.2.0-rc.0"
+            "versionInfo": "6.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/csvviewer",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/csvviewer-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/debugger",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/debugger-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/docmanager",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/docmanager-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/docregistry",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/documentsearch",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/documentsearch-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/extensionmanager",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/extensionmanager-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/filebrowser",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/filebrowser-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/fileeditor",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/fileeditor-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/help-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/htmlviewer",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/htmlviewer-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/hub-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/imageviewer",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/imageviewer-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/inspector",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/javascript-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/json-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/launcher",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/logconsole",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/lsp",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/lsp-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/mainmenu",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/mainmenu-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/markdownviewer",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/markdownviewer-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/markedparser-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/mathjax-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/mermaid",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/mermaid-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/metadataform",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/metadataform-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/nbformat",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/notebook",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/notebook-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/observables",
-            "versionInfo": "5.2.0-rc.0"
+            "versionInfo": "5.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/outputarea",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/pdf-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/pluginmanager",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/pluginmanager-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/property-inspector",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/rendermime",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/rendermime-interfaces",
-            "versionInfo": "3.10.0-rc.0"
+            "versionInfo": "3.10.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/running",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/running-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/services",
-            "versionInfo": "7.2.0-rc.0"
+            "versionInfo": "7.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/settingeditor",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/settingeditor-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/settingregistry",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/shortcuts-extension",
-            "versionInfo": "5.0.0-rc.0"
+            "versionInfo": "5.0.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/statedb",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/statusbar",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/terminal",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/terminal-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/theme-dark-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/theme-dark-high-contrast-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/theme-light-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/toc",
-            "versionInfo": "6.2.0-rc.0"
+            "versionInfo": "6.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/toc-extension",
-            "versionInfo": "6.2.0-rc.0"
+            "versionInfo": "6.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/tooltip",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/tooltip-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/translation",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/translation-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/ui-components",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/ui-components-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/vega5-extension",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/workspaces",
-            "versionInfo": "4.2.0-rc.0"
+            "versionInfo": "4.2.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (C) 2018 by Marijn Haverbeke <marijn@haverbeke.berlin> and others\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@lezer/common",
             "versionInfo": "1.2.1"
         },
```

### Comparing `notebook-7.2.0rc0/notebook/templates/consoles.html` & `notebook-7.2.0rc1/notebook/templates/consoles.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/templates/edit.html` & `notebook-7.2.0rc1/notebook/templates/edit.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/templates/error.html` & `notebook-7.2.0rc1/notebook/templates/error.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/templates/notebooks.html` & `notebook-7.2.0rc1/notebook/templates/notebooks.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/templates/terminals.html` & `notebook-7.2.0rc1/notebook/templates/terminals.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/notebook/templates/tree.html` & `notebook-7.2.0rc1/notebook/templates/tree.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/tests/conftest.py` & `notebook-7.2.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/tests/test_app.py` & `notebook-7.2.0rc1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/.gitignore` & `notebook-7.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/LICENSE` & `notebook-7.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/README.md` & `notebook-7.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0rc0/pyproject.toml` & `notebook-7.2.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.11", "jupyterlab>=4.2.0rc0,<4.3"]
+requires = ["hatchling>=1.11", "jupyterlab>=4.2.0,<4.3"]
 build-backend = "hatchling.build"
 
 [project]
 name = "notebook"
 description = "Jupyter Notebook - A web-based notebook environment for interactive computing"
 readme = "README.md"
 license = { file = "LICENSE" }
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 dependencies = [
     "jupyter_server>=2.4.0,<3",
-    "jupyterlab>=4.2.0rc0,<4.3",
+    "jupyterlab>=4.2.0,<4.3",
     "jupyterlab_server>=2.27.1,<3",
     "notebook_shim>=0.2,<0.3",
     "tornado>=6.2.0",
 ]
 dynamic = ["version"]
 
 [project.scripts]
@@ -171,15 +171,15 @@
 npm = ["jlpm"]
 
 [tool.jupyter-releaser.options]
 version-cmd = "jlpm run release:bump --force --skip-commit"
 
 [tool.jupyter-releaser.hooks]
 before-bump-version = [
-    "python -m pip install -U \"jupyterlab>=4.2.0rc0,<4.3\"",
+    "python -m pip install -U \"jupyterlab>=4.2.0,<4.3\"",
     "jlpm",
     "jlpm run build:utils",
     "python -m pip install hatch"
 ]
 before-build-npm = [
     "jlpm clean",
     "jlpm build:prod"
```

### Comparing `notebook-7.2.0rc0/PKG-INFO` & `notebook-7.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: notebook
-Version: 7.2.0rc0
+Version: 7.2.0rc1
 Summary: Jupyter Notebook - A web-based notebook environment for interactive computing
 Project-URL: Documentation, https://jupyter-notebook.readthedocs.io/
 Project-URL: Homepage, https://github.com/jupyter/notebook
 Project-URL: Source, https://github.com/jupyter/notebook
 Project-URL: Tracker, https://github.com/jupyter/notebook/issues
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
@@ -51,15 +51,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: jupyter-server<3,>=2.4.0
 Requires-Dist: jupyterlab-server<3,>=2.27.1
-Requires-Dist: jupyterlab<4.3,>=4.2.0rc0
+Requires-Dist: jupyterlab<4.3,>=4.2.0
 Requires-Dist: notebook-shim<0.3,>=0.2
 Requires-Dist: tornado>=6.2.0
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == 'docs'
```

