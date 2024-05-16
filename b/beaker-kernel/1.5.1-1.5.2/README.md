# Comparing `tmp/beaker_kernel-1.5.1.tar.gz` & `tmp/beaker_kernel-1.5.2.tar.gz`

## Comparing `beaker_kernel-1.5.1.tar` & `beaker_kernel-1.5.2.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/kernel.json
--rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/kernel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/default/__init__.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/default/agent.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/default/context.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/default/default_payload.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/__init__.py
--rw-r--r--   0        0        0     6485 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/agent.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/context.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/default_payload.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_documentation.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_package_structure.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_variable_info.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_variables.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/__init__.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/agent.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/agent_tasks.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/autodiscovery.py
--rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/context.py
--rw-r--r--   0        0        0    13694 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/jupyter_kernel_proxy.py
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/utils.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/__init__.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/base.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/julia.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/python.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/rlang.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/__init__.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/admin_utils.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/dev.py
--rw-r--r--   0        0        0    13482 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/.empty
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/admin.html
--rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/beaker.svg
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/favicon.ico
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/index.html
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/admin.06bbaee6.css
--rw-r--r--   0        0        0   122158 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/chunk-vendors.f59cad43.css
--rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/index.622cafdc.css
--rw-r--r--   0        0        0    72204 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.0112589c.ttf
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.ba3f916d.woff2
--rw-r--r--   0        0        0    72280 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.f8b9e8a4.woff
--rw-r--r--   0        0        0    72380 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.ffecb254.eot
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add-above.ee286b1c.svg
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add-below.bcf3422e.svg
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add.8f2126a6.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bad.2c188c60.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bell.bccaf100.svg
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/blank.a4bbd63d.svg
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bug-dot.326bc45a.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bug.e30064ad.svg
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/build.e3fdf668.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-down-empty-thin.f6894985.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-down-empty.16b5c137.svg
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-down.1600b64a.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-left.d607c024.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-right.45b8bd09.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-up-empty-thin.912759a9.svg
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-up.9b98d201.svg
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/case-sensitive.eaefe455.svg
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/check.0991dc26.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/circle-empty.4dad54e2.svg
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/circle.114607e4.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/clear.f255d27d.svg
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/close.563b4f49.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/code-check.99d4f00e.svg
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/code.fbdeee94.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/collapse-all.41b2dc7a.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/console.57361ea6.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/copy.2bfc5d39.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/copyright.f38f4ec0.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/cut.18edde39.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/delete.a777a562.svg
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/download.e0245bbf.svg
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/duplicate.8815451e.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/edit.7fbc6db4.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/ellipses.dba28113.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/error.0caf9ea6.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/expand-all.81b631fe.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/extension.50386a9c.svg
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/fast-forward.f82230c4.svg
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/file-upload.44fd837e.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/file.80a9f304.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/filter-dot.47fa93c4.svg
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/filter-list.9e70c93a.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/filter.538fe88b.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/folder-favorite.7f8c9bd5.svg
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/folder.0d235aaf.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/home.32ae995c.svg
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/html5.ea435392.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/image.82357447.svg
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/info.4d82eb41.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/inspector.791cc05d.svg
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/json.a2c296bb.svg
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/julia.499ac74e.svg
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyter-favicon.b19d8551.svg
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyter.a48871a7.svg
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyterlab-wordmark.6280567a.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/kernel.273d3780.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/keyboard.3b314c65.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/launch.6417683d.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/launcher.0453ed19.svg
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/line-form.3e38ab09.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/link.170ecd8b.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/list.c48a0dd4.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/markdown.60974264.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/move-down.5e4a3948.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/move-up.fa81409d.svg
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/new-folder.e3dd5db9.svg
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/not-trusted.8bc17823.svg
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/notebook.9b4747ea.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/numbering.60a6786d.svg
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/offline-bolt.8d942d9a.svg
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/palette.14c4709b.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/paste.3d3cadcf.svg
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/pdf.f6a1dc59.svg
--rw-r--r--   0        0        0   291454 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/primeicons.943ab24c.svg
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/python.0ffed0a2.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/r-kernel.cb4265e1.svg
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/react.c81f1b87.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/redo.ecef5f0c.svg
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/refresh.dae7f1f4.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/regex.fa85da44.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/run.cbdeb7c0.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/running.9890c96a.svg
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/save.2c9f21a7.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/search.77371ff0.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/settings.454fe53f.svg
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/share.ccbe241a.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/spreadsheet.486ad38c.svg
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/stop.88696d03.svg
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/tab.67683cb0.svg
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/table-rows.1053696f.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/tag.8887c8e5.svg
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/terminal.0a8eb862.svg
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/text-editor.52a85e17.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/toc.05490e17.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/tree-view.0a94d13b.svg
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/trusted.3ac2122f.svg
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/undo.0c5afedd.svg
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/user.a13160b1.svg
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/users.cba8edb3.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/vega.c0ae7146.svg
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/word.c993422c.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/yaml.267ef972.svg
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/admin.595fbd46.js
--rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/admin.595fbd46.js.map
--rw-r--r--   0        0        0  3111348 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js
--rw-r--r--   0        0        0 10024731 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js.map
--rw-r--r--   0        0        0    80016 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/index.e38a09de.js
--rw-r--r--   0        0        0   369507 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/index.e38a09de.js.map
--rw-r--r--   0        0        0   187164 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/theme.css
--rw-r--r--   0        0        0    32196 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff
--rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff2
--rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff
--rw-r--r--   0        0        0    24712 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff2
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff
--rw-r--r--   0        0        0    25320 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff2
--rw-r--r--   0        0        0   178553 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/theme.css
--rw-r--r--   0        0        0    32196 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff
--rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff2
--rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff
--rw-r--r--   0        0        0    24712 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff2
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff
--rw-r--r--   0        0        0    25320 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff2
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/LICENSE.txt
--rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/README.md
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/hatch_build.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/kernel.json
+-rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/kernel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/default/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/default/agent.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/default/context.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/default/default_payload.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/__init__.py
+-rw-r--r--   0        0        0     6485 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/agent.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/context.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/default_payload.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/procedures/python3/get_documentation.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/procedures/python3/get_package_structure.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/procedures/python3/get_variable_info.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/procedures/python3/get_variables.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/procedures/python3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/__init__.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/agent.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/agent_tasks.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/autodiscovery.py
+-rw-r--r--   0        0        0    17071 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/context.py
+-rw-r--r--   0        0        0    13694 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/jupyter_kernel_proxy.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/utils.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/__init__.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/base.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/julia.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/python.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/rlang.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/__init__.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/admin_utils.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/dev.py
+-rw-r--r--   0        0        0    13482 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/.empty
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/admin.html
+-rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/beaker.svg
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/favicon.ico
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/index.html
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/css/admin.06bbaee6.css
+-rw-r--r--   0        0        0   122158 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/css/chunk-vendors.f59cad43.css
+-rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/css/index.622cafdc.css
+-rw-r--r--   0        0        0    72204 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/fonts/primeicons.0112589c.ttf
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/fonts/primeicons.ba3f916d.woff2
+-rw-r--r--   0        0        0    72280 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/fonts/primeicons.f8b9e8a4.woff
+-rw-r--r--   0        0        0    72380 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/fonts/primeicons.ffecb254.eot
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/add-above.ee286b1c.svg
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/add-below.bcf3422e.svg
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/add.8f2126a6.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/bad.2c188c60.svg
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/bell.bccaf100.svg
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/blank.a4bbd63d.svg
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/bug-dot.326bc45a.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/bug.e30064ad.svg
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/build.e3fdf668.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/caret-down-empty-thin.f6894985.svg
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/caret-down-empty.16b5c137.svg
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/caret-down.1600b64a.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/caret-left.d607c024.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/caret-right.45b8bd09.svg
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/caret-up-empty-thin.912759a9.svg
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/caret-up.9b98d201.svg
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/case-sensitive.eaefe455.svg
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/check.0991dc26.svg
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/circle-empty.4dad54e2.svg
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/circle.114607e4.svg
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/clear.f255d27d.svg
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/close.563b4f49.svg
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/code-check.99d4f00e.svg
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/code.fbdeee94.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/collapse-all.41b2dc7a.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/console.57361ea6.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/copy.2bfc5d39.svg
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/copyright.f38f4ec0.svg
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/cut.18edde39.svg
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/delete.a777a562.svg
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/download.e0245bbf.svg
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/duplicate.8815451e.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/edit.7fbc6db4.svg
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/ellipses.dba28113.svg
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/error.0caf9ea6.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/expand-all.81b631fe.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/extension.50386a9c.svg
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/fast-forward.f82230c4.svg
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/file-upload.44fd837e.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/file.80a9f304.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/filter-dot.47fa93c4.svg
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/filter-list.9e70c93a.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/filter.538fe88b.svg
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/folder-favorite.7f8c9bd5.svg
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/folder.0d235aaf.svg
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/home.32ae995c.svg
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/html5.ea435392.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/image.82357447.svg
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/info.4d82eb41.svg
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/inspector.791cc05d.svg
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/json.a2c296bb.svg
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/julia.499ac74e.svg
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/jupyter-favicon.b19d8551.svg
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/jupyter.a48871a7.svg
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/jupyterlab-wordmark.6280567a.svg
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/kernel.273d3780.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/keyboard.3b314c65.svg
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/launch.6417683d.svg
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/launcher.0453ed19.svg
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/line-form.3e38ab09.svg
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/link.170ecd8b.svg
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/list.c48a0dd4.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/markdown.60974264.svg
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/move-down.5e4a3948.svg
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/move-up.fa81409d.svg
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/new-folder.e3dd5db9.svg
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/not-trusted.8bc17823.svg
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/notebook.9b4747ea.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/numbering.60a6786d.svg
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/offline-bolt.8d942d9a.svg
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/palette.14c4709b.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/paste.3d3cadcf.svg
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/pdf.f6a1dc59.svg
+-rw-r--r--   0        0        0   291454 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/primeicons.943ab24c.svg
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/python.0ffed0a2.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/r-kernel.cb4265e1.svg
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/react.c81f1b87.svg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/redo.ecef5f0c.svg
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/refresh.dae7f1f4.svg
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/regex.fa85da44.svg
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/run.cbdeb7c0.svg
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/running.9890c96a.svg
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/save.2c9f21a7.svg
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/search.77371ff0.svg
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/settings.454fe53f.svg
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/share.ccbe241a.svg
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/spreadsheet.486ad38c.svg
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/stop.88696d03.svg
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/tab.67683cb0.svg
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/table-rows.1053696f.svg
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/tag.8887c8e5.svg
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/terminal.0a8eb862.svg
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/text-editor.52a85e17.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/toc.05490e17.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/tree-view.0a94d13b.svg
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/trusted.3ac2122f.svg
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/undo.0c5afedd.svg
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/user.a13160b1.svg
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/users.cba8edb3.svg
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/vega.c0ae7146.svg
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/word.c993422c.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/yaml.267ef972.svg
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/admin.595fbd46.js
+-rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/admin.595fbd46.js.map
+-rw-r--r--   0        0        0  3111348 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js
+-rw-r--r--   0        0        0 10024731 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js.map
+-rw-r--r--   0        0        0    80016 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/index.e38a09de.js
+-rw-r--r--   0        0        0   369507 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/index.e38a09de.js.map
+-rw-r--r--   0        0        0   187164 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/theme.css
+-rw-r--r--   0        0        0    32196 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff
+-rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff2
+-rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff
+-rw-r--r--   0        0        0    24712 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff2
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff
+-rw-r--r--   0        0        0    25320 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff2
+-rw-r--r--   0        0        0   178553 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/theme.css
+-rw-r--r--   0        0        0    32196 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff
+-rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff2
+-rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff
+-rw-r--r--   0        0        0    24712 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff2
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff
+-rw-r--r--   0        0        0    25320 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff2
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/README.md
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/hatch_build.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 beaker_kernel-1.5.2/PKG-INFO
```

### Comparing `beaker_kernel-1.5.1/beaker_kernel/kernel.py` & `beaker_kernel-1.5.2/beaker_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/contexts/default/agent.py` & `beaker_kernel-1.5.2/beaker_kernel/contexts/default/agent.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/contexts/default/context.py` & `beaker_kernel-1.5.2/beaker_kernel/contexts/default/context.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/agent.py` & `beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/agent.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/context.py` & `beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 from beaker_kernel.lib.subkernels.python import PythonSubkernel
 
 from .agent import PyPackageAgent
 
 if TYPE_CHECKING:
     from beaker_kernel.kernel import LLMKernel
     from beaker_kernel.lib.agent import BaseAgent
-    from beaker_kernel.lib.subkernels.base import BaseSubkernel
 
 class PyPackageContext(BaseContext):
 
     agent_cls: "BaseAgent" = PyPackageAgent
 
     def __init__(self, beaker_kernel: "LLMKernel", config: Dict[str, Any]):
         super().__init__(beaker_kernel, self.agent_cls, config)
         if not isinstance(self.subkernel, PythonSubkernel):
             raise ValueError("This context is only valid for Python.")
 
     async def setup(self, context_info=None, parent_header=None):
         await self.execute(self.get_code("setup", {}))
-        return await super().setup(config["context_info"], parent_header)
+        return await super().setup(context_info, parent_header)
```

### Comparing `beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_documentation.py` & `beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/procedures/python3/get_documentation.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/setup.py` & `beaker_kernel-1.5.2/beaker_kernel/contexts/pypackage/procedures/python3/setup.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/agent.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import re
 import typing
 
 from archytas.react import ReActAgent, Undefined
 from archytas.tool_utils import AgentRef, LoopControllerRef, ReactContextRef, tool
 
-from beaker_kernel.lib.utils import togglable_tool
+from beaker_kernel.lib.utils import env_enabled
 
 if typing.TYPE_CHECKING:
     from .context import BaseContext
 
 logger = logging.getLogger(__name__)
 
 class BaseAgent(ReActAgent):
@@ -36,14 +36,15 @@
             verbose=self.context.beaker_kernel.verbose,
             spinner=None,
             rich_print=False,
             allow_ask_user=False,
             thought_handler=context.beaker_kernel.handle_thoughts,
             **kwargs
         )
+        
 
     def get_info(self):
         """
         Returns info about the agent for communication with the kernel.
         """
         info = {
             "name": self.__class__.__name__,
@@ -68,15 +69,15 @@
             stream="iopub",
             msg_or_type="llm_observation",
             content=content,
             parent_header=parent_header,
         )
         return super().display_observation(observation)
 
-    @togglable_tool("ENABLE_USER_PROMPT")
+    @tool()
     async def ask_user(
         self, query: str, agent: AgentRef, loop: LoopControllerRef, react_context: ReactContextRef,
     ) -> str:
         """
         Sends a query to the user and returns their response
 
         Args:
```

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/agent_tasks.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/agent_tasks.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/autodiscovery.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/context.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 import inspect
 import json
 import logging
 import os.path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
 import requests
 
-from .jupyter_kernel_proxy import InterceptionFilter, JupyterMessage
+from jinja2 import Environment, FileSystemLoader, Template, select_autoescape
+
+from archytas.tool_utils import collect_tools_from_object
 
 from beaker_kernel.lib.autodiscovery import autodiscover
 from beaker_kernel.lib.utils import action, get_socket, server_token, server_url
 
-from jinja2 import Environment, FileSystemLoader, Template, select_autoescape
+
+from .jupyter_kernel_proxy import InterceptionFilter, JupyterMessage
 
 if TYPE_CHECKING:
     from archytas.react import ReActAgent
 
     from beaker_kernel.kernel import LLMKernel
 
     from .agent import BaseAgent
     from .subkernels.base import BaseSubkernel
 
 logger = logging.getLogger(__name__)
 
+TOOL_TOGGLE_PREFIX = "TOOL_ENABLED_"
+
 
 class BaseContext:
     beaker_kernel: "LLMKernel"
     subkernel: "BaseSubkernel"
     config: Dict[str, Any]
     agent: "ReActAgent"
 
@@ -37,21 +42,22 @@
     WEIGHT: int = 50  # Used for auto-sorting in drop-downs, etc. Lower weights are listed earlier.
 
     def __init__(self, beaker_kernel: "LLMKernel", agent_cls: "BaseAgent", config: Dict[str, Any]):
         self.intercepts = []
         self.jinja_env = None
         self.templates = {}
         self.beaker_kernel = beaker_kernel
+        self.config = config
+        self.subkernel = self.get_subkernel()
         self.agent = agent_cls(
             context=self,
-            tools=[],
+            tools=self.subkernel.tools,
         )
-        self.config = config
-        self.subkernel = self.get_subkernel()
 
+        self.disable_tools()
 
         # Add intercepts, by inspecting the instance and extracting matching methods
         self._collect_and_register_intercepts(self)
         self._collect_and_register_intercepts(self.subkernel)
 
         # Set auto-context from agent
         if getattr(self, "auto_context", None) is not None:
@@ -72,14 +78,30 @@
                     template_name, _ = os.path.splitext(template_file)
                     template = self.jinja_env.get_template(template_file)
                     self.templates[template_name] = template
                 except UnicodeDecodeError:
                     # For templates, this indicates a binary file which can't be a template, so throw a warning and skip.
                     logger.warn(f"File '{template_name}' in context '{self.__class__.__name__}' is not a valid template file as it cannot be decoded to a unicode string.")
 
+    def disable_tools(self):
+        # TODO: Identical toolnames don't work
+        toggles = {
+            attr.removeprefix(TOOL_TOGGLE_PREFIX).lower(): value == "true"
+            for attr, value in os.environ.items() if attr.startswith(TOOL_TOGGLE_PREFIX)
+        }
+        toggles.update({
+            attr.removeprefix(TOOL_TOGGLE_PREFIX).lower(): getattr(self, attr) 
+            for attr in dir(self) if attr.startswith(TOOL_TOGGLE_PREFIX)
+        })
+        disabled_tools = [
+            tool
+            for tool, enabled in toggles.items() if not enabled
+        ]
+        self.agent.disable(*disabled_tools)
+
     async def setup(self, context_info=None, parent_header=None):
         if context_info:
             self.config["context_info"] = context_info
 
         if callable(getattr(self.agent, 'setup', None)):
             await self.agent.setup(self.config["context_info"], parent_header=parent_header)
 
@@ -186,31 +208,33 @@
             "procedures": list(self.templates.keys()),
             "agent": agent_details,
             "debug": self.beaker_kernel.debug_enabled,
             "verbose": self.beaker_kernel.verbose,
         }
         return payload
 
+    async def get_subkernel_state(self):
+        fetch_state_code = self.subkernel.FETCH_STATE_CODE
+        state = await self.evaluate(fetch_state_code)
+        return state["return"]
 
-    @action()
-    async def get_subkernel_state(self, message):
+    @action(action_name="get_subkernel_state")
+    async def get_subkernel_state_action(self, message):
         """
         Fetches the state of the subkernel, including all defined variables, imports, and functions.
         """
-        fetch_state_code = self.subkernel.FETCH_STATE_CODE
-        state = await self.beaker_kernel.evaluate(fetch_state_code)
-        result = state["return"]
+        state = await self.get_subkernel_state()
         self.send_response(
             stream="iopub",
             msg_or_type="get_subkernel_state_response",
-            content=result,
+            content=state,
             parent_header=message.header,
         )
-        return result
-    get_subkernel_state._default_payload = "{}"
+        return state
+    get_subkernel_state_action._default_payload = "{}"
 
 
     @action()
     async def get_agent_history(self, message):
         """
         Returns all of the history for the LLM agent.
         """
```

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/jupyter_kernel_proxy.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/jupyter_kernel_proxy.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/utils.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import json
 import logging
 import sys
 import traceback
+import warnings
 from contextlib import AbstractAsyncContextManager
 from functools import wraps, update_wrapper
 from typing import Any, TYPE_CHECKING
 
 from archytas.tool_utils import tool
 
 from .jupyter_kernel_proxy import ( KERNEL_SOCKETS, KERNEL_SOCKETS_NAMES,
@@ -160,26 +161,14 @@
         magic_prefix = "%" + (magic_word or fn.__name__)
         setattr(fn, "_magic_prefix", magic_prefix)
         update_wrapper(register_magic, fn)
         return fn
     return register_magic
 
 
-def togglable_tool(env_var, *, name: str | None = None):
-    """
-    Register tool if it is enabled in environment
-    """
-    ENABLE = os.environ.get(env_var, "false").lower() == "true"
-    if not ENABLE:
-        def disable(_fn):
-            return
-        return disable
-    else:
-        return tool(name=name)
-
 class LogMessageEncoder(json.JSONEncoder):
     def default(self, o: Any) -> Any:
         try:
             return super().default(o)
         except:
             return str(o)
 
@@ -189,7 +178,14 @@
         # if callable(o):
         #     # return f"Function named"
         #     return super().default(o)
         try:
             return super().default(o)
         except:
             return str(o)
+
+
+def togglable_tool(env_var, *, name: str | None = None):
+    warnings.warn("This decorator is deprecated and will be removed in version 1.6.0")
+    def noop(fn):
+        return fn
+    return noop
```

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/base.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import Any, Callable
 import hashlib
 import shutil
 from tempfile import mkdtemp
 from os import makedirs, environ
 import requests
 
+from archytas.tool_utils import AgentRef, tool
+
 from ..utils import server_url, server_token, env_enabled, action
 from ..jupyter_kernel_proxy import ProxyKernelClient
 
 Checkpoint = dict[str, str]
 
 class JsonStateEncoder(json.JSONEncoder):
     pass
@@ -18,22 +20,27 @@
 class BaseSubkernel(abc.ABC):
     DISPLAY_NAME: str
     SLUG: str
     KERNEL_NAME: str
 
     WEIGHT: int = 50  # Used for auto-sorting in drop-downs, etc. Lower weights are listed earlier.
 
+    TOOLS: list[tuple[Callable, bool]]  = []
 
     FETCH_STATE_CODE: str = ""
 
     @classmethod
     @abc.abstractmethod
     def parse_subkernel_return(cls, execution_result) -> Any:
         ...
 
+    @property
+    def tools(self):
+        return [tool for tool, condition in self.TOOLS if condition]
+
     def __init__(self, jupyter_id: str, subkernel_configuration: dict, context):
         self.jupyter_id = jupyter_id
         self.connected_kernel = ProxyKernelClient(subkernel_configuration)
         self.context = context
     
     def send_response(self, stream, msg_or_type, content=None, channel=None, parent_header={}, parent_identities=None):
         return self.context.send_response(stream, msg_or_type, content, channel, parent_header, parent_identities)
@@ -55,17 +62,48 @@
                 )
                 if res.status_code == 204:
                     self.jupyter_id = None
             except requests.exceptions.HTTPError as err:
                 print(err)
 
 
+@tool()
+async def run_code(code: str, agent: AgentRef) -> str:
+    """
+    Execute code in the user's session. After execution,
+    the state of the kernel will be rolled back to before this tool
+    was used.
+
+    This tool can be help answer questions about the kernel state. For
+    example, a user may ask something about a dictionary `d` and using 
+    run code with the `code` of `d.keys()`.
+
+    This tool can also be used to double check if code will work before 
+    returning it as a final answer.
+
+    Note that this tool does not capture `stdout` AND only returns the
+    results of the last expression evaluated.
+
+    Args:
+        code (str): Code to run directly in Jupyter.
+    Returns:
+        str: Result of the `expr`
+    
+    """
+    result = await agent.context.subkernel.execute_and_rollback(code)
+    return result
+
+
 class BaseCheckpointableSubkernel(BaseSubkernel):
     SERIALIZATION_EXTENSION: str = "storage"
 
+    TOOLS = [
+        (run_code, env_enabled("ENABLE_CHECKPOINTS"))
+    ]
+
     def __init__(self, jupyter_id: str, subkernel_configuration: dict, context):
         super().__init__(jupyter_id, subkernel_configuration, context)
         self.checkpoints_enabled = env_enabled("ENABLE_CHECKPOINTS")
         if self.checkpoints_enabled:
             self.checkpoints : list[Checkpoint] = []
             self.storage_prefix = mkdtemp()
             makedirs(self.storage_prefix, exist_ok=True)
@@ -124,7 +162,16 @@
 
 
     def cleanup(self):
         super().cleanup()
         if self.checkpoints_enabled:
             shutil.rmtree(self.storage_prefix, ignore_errors=True)
             self.checkpoints = []
+
+
+    async def execute_and_rollback(self, code: str):
+        checkpoint_index = await self.add_checkpoint()
+        result = await self.evaluate(code)
+        await self.rollback(checkpoint_index)
+        return str(result["return"])
+
+
```

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/julia.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/julia.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/python.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/python.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/rlang.py` & `beaker_kernel-1.5.2/beaker_kernel/lib/subkernels/rlang.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/admin_utils.py` & `beaker_kernel-1.5.2/beaker_kernel/server/admin_utils.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/dev.py` & `beaker_kernel-1.5.2/beaker_kernel/server/dev.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,23 +64,31 @@
             except ImportError:
                 logger.error("Error reloading")
 
             if app_subprocess:
                 app_subprocess.terminate()
 
 
-def create_observer():
+def create_observer(extra_dirs=None):
     contexts = autodiscover("contexts")
     subkernels = autodiscover("subkernels")
     modules = set([inspect.getmodule(beaker_kernel)])
     modules.update([inspect.getmodule(cls) for _, cls in contexts.items()])
     modules.update([inspect.getmodule(cls) for _, cls in subkernels.items()])
-    all_paths = sorted([os.path.dirname(inspect.getabsfile(mod)) for mod in modules], key=lambda f: len(f))
+    mod_paths = [os.path.dirname(inspect.getabsfile(mod)) for mod in modules]
+    all_paths: list[str] = mod_paths[:]
+    if extra_dirs:
+        all_paths.extend([
+            extra_dir for extra_dir in extra_dirs
+            if os.path.exists(extra_dir)
+        ])
+    # Sort by length so we add more general paths before more specific/subpaths
+    sorted_paths = sorted(all_paths, key=lambda f: len(f))
     paths = set()
-    for path in all_paths:
+    for path in sorted_paths:
         is_subpath = False
         for saved_path in paths:
             if path.startswith(saved_path):
                 is_subpath = True
                 break
         if not is_subpath:
             paths.add(path)
@@ -103,17 +111,25 @@
         args.append("--debug")
     serverapp = DevBeakerJupyterApp.initialize_server(argv=args)
     serverapp.start()
 
 
 if __name__ == "__main__":
     if "watch" in sys.argv:
-        observer = create_observer()
         args = sys.argv[:]
         args.remove("watch")
+        extra_dirs = []
+        while "--extra_watch_dir" in args:
+            idx = args.index("--extra_watch_dir")
+            args.pop(idx)  # Pop the flag
+            extra_dir = args.pop(idx)  # Value is now in the index where the flag was
+            logger.warn(f"Adding extra watch dir {extra_dir}")
+            extra_dirs.append(extra_dir)
+
+        observer = create_observer(extra_dirs)
         try:
             while True:
                 app_subprocess = subprocess.Popen([
                         sys.executable,
                         *args,
                     ],
                     env=os.environ
```

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/main.py` & `beaker_kernel-1.5.2/beaker_kernel/server/main.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/admin.html` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/admin.html`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/beaker.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/beaker.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/favicon.ico` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/index.html` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/index.html`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/admin.06bbaee6.css` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/css/admin.06bbaee6.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/chunk-vendors.f59cad43.css` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/css/chunk-vendors.f59cad43.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/index.622cafdc.css` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/css/index.622cafdc.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.0112589c.ttf` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/fonts/primeicons.0112589c.ttf`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.ba3f916d.woff2` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/fonts/primeicons.ba3f916d.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.f8b9e8a4.woff` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/fonts/primeicons.f8b9e8a4.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.ffecb254.eot` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/fonts/primeicons.ffecb254.eot`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add-above.ee286b1c.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/add-above.ee286b1c.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add-below.bcf3422e.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/add-below.bcf3422e.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bell.bccaf100.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/bell.bccaf100.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bug-dot.326bc45a.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/bug-dot.326bc45a.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bug.e30064ad.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/bug.e30064ad.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/build.e3fdf668.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/build.e3fdf668.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/case-sensitive.eaefe455.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/case-sensitive.eaefe455.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/copyright.f38f4ec0.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/copyright.f38f4ec0.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/cut.18edde39.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/cut.18edde39.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/duplicate.8815451e.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/duplicate.8815451e.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/html5.ea435392.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/html5.ea435392.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/info.4d82eb41.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/info.4d82eb41.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/json.a2c296bb.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/json.a2c296bb.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/julia.499ac74e.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/julia.499ac74e.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyter-favicon.b19d8551.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/jupyter-favicon.b19d8551.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyter.a48871a7.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/jupyter.a48871a7.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyterlab-wordmark.6280567a.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/jupyterlab-wordmark.6280567a.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/move-down.5e4a3948.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/move-down.5e4a3948.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/move-up.fa81409d.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/move-up.fa81409d.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/not-trusted.8bc17823.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/not-trusted.8bc17823.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/palette.14c4709b.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/palette.14c4709b.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/pdf.f6a1dc59.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/pdf.f6a1dc59.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/primeicons.943ab24c.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/primeicons.943ab24c.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/python.0ffed0a2.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/python.0ffed0a2.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/react.c81f1b87.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/react.c81f1b87.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/regex.fa85da44.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/regex.fa85da44.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/settings.454fe53f.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/settings.454fe53f.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/share.ccbe241a.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/share.ccbe241a.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/tag.8887c8e5.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/tag.8887c8e5.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/terminal.0a8eb862.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/terminal.0a8eb862.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/trusted.3ac2122f.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/trusted.3ac2122f.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/users.cba8edb3.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/users.cba8edb3.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/word.c993422c.svg` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/img/word.c993422c.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/admin.595fbd46.js` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/admin.595fbd46.js`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/admin.595fbd46.js.map` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/admin.595fbd46.js.map`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js.map` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js.map`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/index.e38a09de.js` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/index.e38a09de.js`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/index.e38a09de.js.map` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/static/js/index.e38a09de.js.map`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/theme.css` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/theme.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff2` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff2` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff2` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/theme.css` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/theme.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff2` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff2` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff2` & `beaker_kernel-1.5.2/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/.gitignore` & `beaker_kernel-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/LICENSE.txt` & `beaker_kernel-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/README.md` & `beaker_kernel-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/hatch_build.py` & `beaker_kernel-1.5.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.1/pyproject.toml` & `beaker_kernel-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "jupyter-client"]
 build-backend = "hatchling.build"
 
 [project]
 name = "beaker-kernel"
-version = "1.5.1"
+version = "1.5.2"
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Matthew Printz", email = "matt@jataware.com" },
@@ -26,15 +26,15 @@
   "jupyterlab~=4.0",
   "jupyterlab-server>=2.22.1,<3",
   "requests>=2.24,<3",
   "pandas==1.3.3",
   "matplotlib~=3.7.1",
   "xarray==0.19.0",
   "numpy~=1.24.3",
-  "archytas~=1.1.5",
+  "archytas~=1.1.6",
   "pyzmq~=26.0.2",
   "six~=1.16.0",
   "tornado~=6.4.0",
   "scipy~=1.11.1",
   "jinja2~=3.1.2",
   "watchdog~=3.0",
 ]
```

### Comparing `beaker_kernel-1.5.1/PKG-INFO` & `beaker_kernel-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: beaker-kernel
-Version: 1.5.1
+Version: 1.5.2
 Project-URL: Documentation, https://github.com/unknown/beaker-kernel#readme
 Project-URL: Issues, https://github.com/unknown/beaker-kernel/issues
 Project-URL: Source, https://github.com/unknown/beaker-kernel
 Author-email: Matthew Printz <matt@jataware.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: archytas~=1.1.5
+Requires-Dist: archytas~=1.1.6
 Requires-Dist: dill
 Requires-Dist: jinja2~=3.1.2
 Requires-Dist: jupyterlab-server<3,>=2.22.1
 Requires-Dist: jupyterlab~=4.0
 Requires-Dist: matplotlib~=3.7.1
 Requires-Dist: numpy~=1.24.3
 Requires-Dist: pandas==1.3.3
```

