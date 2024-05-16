# Comparing `tmp/libreflow-2.4.2.tar.gz` & `tmp/libreflow-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow-2.4.2.tar", last modified: Fri May  3 16:07:29 2024, max compression
+gzip compressed data, was "libreflow-2.4.3.tar", last modified: Thu May 16 16:00:52 2024, max compression
```

## Comparing `libreflow-2.4.2.tar` & `libreflow-2.4.3.tar`

### file list

```diff
@@ -1,353 +1,353 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.619908 libreflow-2.4.2/
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-05-03 16:07:20.000000 libreflow-2.4.2/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    72084 2024-05-03 16:07:20.000000 libreflow-2.4.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1047 2024-05-03 16:07:20.000000 libreflow-2.4.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-03 16:07:20.000000 libreflow-2.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    73121 2024-05-03 16:07:29.619908 libreflow-2.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1640 2024-05-03 16:07:20.000000 libreflow-2.4.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-03 16:07:29.619908 libreflow-2.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2405 2024-05-03 16:07:20.000000 libreflow-2.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.535909 libreflow-2.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.619908 libreflow-2.4.2/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-05-03 16:07:29.620908 libreflow-2.4.2/src/libreflow/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.552909 libreflow-2.4.2/src/libreflow/baseflow/
--rw-rw-rw-   0 root         (0) root         (0)    31651 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6008 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     7427 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/departments.py
--rw-rw-rw-   0 root         (0) root         (0)    34140 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/entity_manager.py
--rw-rw-rw-   0 root         (0) root         (0)   201280 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/file.py
--rw-rw-rw-   0 root         (0) root         (0)    28331 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/film.py
--rw-rw-rw-   0 root         (0) root         (0)    35159 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/kitsu.py
--rw-rw-rw-   0 root         (0) root         (0)     4875 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4712 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/maputils.py
--rw-rw-rw-   0 root         (0) root         (0)    18934 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/mytasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/runactions.py
--rw-rw-rw-   0 root         (0) root         (0)    15138 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/runners.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/shot.py
--rw-rw-rw-   0 root         (0) root         (0)    49390 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/site.py
--rw-rw-rw-   0 root         (0) root         (0)    19053 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/task.py
--rw-rw-rw-   0 root         (0) root         (0)    72943 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/task_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.554909 libreflow-2.4.2/src/libreflow/baseflow/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25652 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/controller.py
--rw-rw-rw-   0 root         (0) root         (0)    13555 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/delegate.py
--rw-rw-rw-   0 root         (0) root         (0)    11242 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/file.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/file_cell.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/file_history.py
--rw-rw-rw-   0 root         (0) root         (0)    12971 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/file_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.555909 libreflow-2.4.2/src/libreflow/baseflow/ui/importfiles/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/importfiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7233 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/importfiles/custom_widget.py
--rw-rw-rw-   0 root         (0) root         (0)    12827 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/importfiles/files_list.py
--rw-rw-rw-   0 root         (0) root         (0)    17843 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/importfiles/target_wizard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.557909 libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17306 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/components.py
--rw-rw-rw-   0 root         (0) root         (0)    14000 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/edit_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     7051 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/file_list.py
--rw-rw-rw-   0 root         (0) root         (0)    49203 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/mytasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/qmodel.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/qmodel.py
--rw-rw-rw-   0 root         (0) root         (0)    18098 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/ui/task.py
--rw-rw-rw-   0 root         (0) root         (0)    16888 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/baseflow/users.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.557909 libreflow-2.4.2/src/libreflow/custom_home/
--rw-rw-rw-   0 root         (0) root         (0)     7239 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/custom_home/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4642 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/custom_home/ui.py
--rw-rw-rw-   0 root         (0) root         (0)   211828 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/custom_home/wizard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.558909 libreflow-2.4.2/src/libreflow/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.559908 libreflow-2.4.2/src/libreflow/examples/demoflow/
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/demoflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/demoflow/film.py
--rw-rw-rw-   0 root         (0) root         (0)     2889 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/demoflow/lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.560909 libreflow-2.4.2/src/libreflow/examples/majorque/
--rw-rw-rw-   0 root         (0) root         (0)     2435 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/majorque/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/majorque/departments.py
--rw-rw-rw-   0 root         (0) root         (0)    10006 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/majorque/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5209 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/majorque/film.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/majorque/kitsu.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/majorque/lib.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/majorque/runners.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/examples/majorque/users.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/gui.py
--rw-rw-rw-   0 root         (0) root         (0)     5674 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/jobs_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/jobs_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.561909 libreflow-2.4.2/src/libreflow/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.568909 libreflow-2.4.2/src/libreflow/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.abc
--rw-rw-rw-   0 root         (0) root         (0)     8621 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.aep
--rw-rw-rw-   0 root         (0) root         (0)   323555 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.ai
--rw-rw-rw-   0 root         (0) root         (0)   120981 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.blend
--rw-rw-rw-   0 root         (0) root         (0)    32284 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.fbx
--rw-rw-rw-   0 root         (0) root         (0)    20632 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.jpg
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.jsx
--rw-rw-rw-   0 root         (0) root         (0)    65344 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.kra
--rw-rw-rw-   0 root         (0) root         (0)    11248 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.mov
--rw-rw-rw-   0 root         (0) root         (0)  1263464 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.mp4
--rw-rw-rw-   0 root         (0) root         (0)     1651 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.nk
--rw-rw-rw-   0 root         (0) root         (0)    63071 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.obj
--rw-rw-rw-   0 root         (0) root         (0)    36592 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.png
--rw-rw-rw-   0 root         (0) root         (0)   417005 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.psb
--rw-rw-rw-   0 root         (0) root         (0)   397099 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.psd
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.txt
--rw-rw-rw-   0 root         (0) root         (0)     1232 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.usd
--rw-rw-rw-   0 root         (0) root         (0)    88244 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/file_templates/template.wav
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.569908 libreflow-2.4.2/src/libreflow/resources/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    86400 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/fonts/SpaceGrotesk-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)    86504 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/fonts/SpaceGrotesk-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.569908 libreflow-2.4.2/src/libreflow/resources/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.570909 libreflow-2.4.2/src/libreflow/resources/icons/applications/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/applications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/applications/rv.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.571909 libreflow-2.4.2/src/libreflow/resources/icons/flow/
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6763 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/flow/alembic.png
--rw-rw-rw-   0 root         (0) root         (0)     5862 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/flow/explorer.png
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/flow/photoshop.png
--rw-rw-rw-   0 root         (0) root         (0)    10783 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/flow/quicktime.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.577909 libreflow-2.4.2/src/libreflow/resources/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/add-file.png
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/add-folder.png
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)      821 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/check-box-empty-dark.png
--rw-rw-rw-   0 root         (0) root         (0)    10906 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/clean.png
--rw-rw-rw-   0 root         (0) root         (0)     1411 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/close.png
--rw-rw-rw-   0 root         (0) root         (0)     4867 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/compositing.png
--rw-rw-rw-   0 root         (0) root         (0)      868 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/duplicate.png
--rw-rw-rw-   0 root         (0) root         (0)    17838 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/location-worldwide-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)    17853 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/location-worldwide.png
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/maximize.png
--rw-rw-rw-   0 root         (0) root         (0)    18568 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/menu.png
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/menu_dots.png
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/minimize.png
--rw-rw-rw-   0 root         (0) root         (0)     5694 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/misc.png
--rw-rw-rw-   0 root         (0) root         (0)     2029 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/mytasks-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/mytasks.png
--rw-rw-rw-   0 root         (0) root         (0)     1524 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-left-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)      930 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-left.png
--rw-rw-rw-   0 root         (0) root         (0)     2254 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-refresh-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-refresh.png
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-right-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     1596 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/ref-broken.png
--rw-rw-rw-   0 root         (0) root         (0)     1513 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/ref.png
--rw-rw-rw-   0 root         (0) root         (0)     2360 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/refresh.png
--rw-rw-rw-   0 root         (0) root         (0)     6914 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/send.png
--rw-rw-rw-   0 root         (0) root         (0)    13652 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/gui/send2.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.579908 libreflow-2.4.2/src/libreflow/resources/icons/history/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/check.png
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/done.png
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/init.png
--rw-rw-rw-   0 root         (0) root         (0)      838 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/retake.png
--rw-rw-rw-   0 root         (0) root         (0)      831 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/wfa.png
--rw-rw-rw-   0 root         (0) root         (0)     1427 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/wip.png
--rw-rw-rw-   0 root         (0) root         (0)      944 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/working_copy.png
--rw-rw-rw-   0 root         (0) root         (0)     1499 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/history/working_copy_mine.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.597909 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)     1755 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/3d-object.png
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/active_site.png
--rw-rw-rw-   0 root         (0) root         (0)     1617 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/afterfx.png
--rw-rw-rw-   0 root         (0) root         (0)     6101 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/archive.png
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/available.png
--rw-rw-rw-   0 root         (0) root         (0)     6331 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/blank.png
--rw-rw-rw-   0 root         (0) root         (0)     1438 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/blender.png
--rw-rw-rw-   0 root         (0) root         (0)     1556 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/checked-symbol-colored.png
--rw-rw-rw-   0 root         (0) root         (0)     1566 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/checked-symbol.png
--rw-rw-rw-   0 root         (0) root         (0)     1711 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/circle-shape-outline.png
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/circle-shape-right-eye-outline.png
--rw-rw-rw-   0 root         (0) root         (0)     1730 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/circular-shape-right-eye-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/circular-shape-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/clean.png
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/clipboard.png
--rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/compare-previews.png
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/cross-mark-on-a-black-circle-background-colored.png
--rw-rw-rw-   0 root         (0) root         (0)     3131 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/custom_home_star.png
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/delete.png
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/dependencies.png
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/download.png
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/downloadable.png
--rw-rw-rw-   0 root         (0) root         (0)     1424 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/duplicate.png
--rw-rw-rw-   0 root         (0) root         (0)    15134 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/edit-blank.png
--rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/edit-lock-green.png
--rw-rw-rw-   0 root         (0) root         (0)     2610 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/edit-lock-red.png
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/error.png
--rw-rw-rw-   0 root         (0) root         (0)     2052 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/exchange.png
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/exclamation-sign-colored.png
--rw-rw-rw-   0 root         (0) root         (0)     2027 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/fbx.png
--rw-rw-rw-   0 root         (0) root         (0)     6192 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/firefox.png
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/hide.png
--rw-rw-rw-   0 root         (0) root         (0)     6372 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/history.png
--rw-rw-rw-   0 root         (0) root         (0)     1419 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/illustrator.png
--rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/json.png
--rw-rw-rw-   0 root         (0) root         (0)     1498 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/jsx.png
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu.svg
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_done.png
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_oklodv.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_omit.png
--rw-rw-rw-   0 root         (0) root         (0)     1124 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_retake.png
--rw-rw-rw-   0 root         (0) root         (0)     1040 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_todo.png
--rw-rw-rw-   0 root         (0) root         (0)     1126 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_wfa.png
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_wip.png
--rw-rw-rw-   0 root         (0) root         (0)     2866 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/krita.png
--rw-rw-rw-   0 root         (0) root         (0)     1167 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/lock-green.png
--rw-rw-rw-   0 root         (0) root         (0)     1171 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/lock-red.png
--rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/log_out.png
--rw-rw-rw-   0 root         (0) root         (0)    37128 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/multi-share-option.png
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/nuke.png
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/origin-site.png
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/padlock.png
--rw-rw-rw-   0 root         (0) root         (0)     1575 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/padlock_green.png
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/padlock_red.png
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/premiere-pro.png
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/publish-ae.png
--rw-rw-rw-   0 root         (0) root         (0)     1082 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/publish-blender.png
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/publish.png
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/quicktime.png
--rw-rw-rw-   0 root         (0) root         (0)     1699 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/refresh.png
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/request.png
--rw-rw-rw-   0 root         (0) root         (0)     1338 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/requestable.png
--rw-rw-rw-   0 root         (0) root         (0)     1160 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/run.png
--rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/show.png
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/stop.png
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/sync.png
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/sync_arrow.png
--rw-rw-rw-   0 root         (0) root         (0)     2143 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/time_format.png
--rw-rw-rw-   0 root         (0) root         (0)     1606 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/unavailable.png
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/upload.png
--rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/vscodium.png
--rw-rw-rw-   0 root         (0) root         (0)    73670 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/waiting.png
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/warning.png
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/libreflow/watch.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.600909 libreflow-2.4.2/src/libreflow/resources/icons/status/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/done.png
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/err.png
--rw-rw-rw-   0 root         (0) root         (0)     3014 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/inv.png
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/none.png
--rw-rw-rw-   0 root         (0) root         (0)     2999 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/nys.png
--rw-rw-rw-   0 root         (0) root         (0)     3130 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/oop.png
--rw-rw-rw-   0 root         (0) root         (0)     3112 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/rtk.png
--rw-rw-rw-   0 root         (0) root         (0)     3113 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/rvw.png
--rw-rw-rw-   0 root         (0) root         (0)     3212 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/wait.png
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/warn.png
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/status/wip.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.602908 libreflow-2.4.2/src/libreflow/resources/icons/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/animation.svg
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/clean.svg
--rw-rw-rw-   0 root         (0) root         (0)     1350 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/colo.svg
--rw-rw-rw-   0 root         (0) root         (0)     1762 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/compositing.svg
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/design.svg
--rw-rw-rw-   0 root         (0) root         (0)     1440 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/layout.svg
--rw-rw-rw-   0 root         (0) root         (0)      903 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/lighting.svg
--rw-rw-rw-   0 root         (0) root         (0)     1421 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/modeling.svg
--rw-rw-rw-   0 root         (0) root         (0)     1267 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/rigging.svg
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/icons/tasks/shading.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.602908 libreflow-2.4.2/src/libreflow/resources/mark_sequence/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/mark_sequence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.603908 libreflow-2.4.2/src/libreflow/resources/mark_sequence/fields/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/mark_sequence/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/mark_sequence/fields/default.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.604909 libreflow-2.4.2/src/libreflow/resources/mark_sequence/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   313408 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/mark_sequence/fonts/LiberationMono-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/mark_sequence/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.604909 libreflow-2.4.2/src/libreflow/resources/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.604909 libreflow-2.4.2/src/libreflow/resources/scripts/blender/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/scripts/blender/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6076 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/scripts/blender/disable_save_keymap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.605908 libreflow-2.4.2/src/libreflow/resources/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.605908 libreflow-2.4.2/src/libreflow/resources/styles/lfs_tech/
--rw-rw-rw-   0 root         (0) root         (0)     3280 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/styles/lfs_tech/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10517 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.606908 libreflow-2.4.2/src/libreflow/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16095 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/scripts/mark_sequence.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/scripts/minio_file_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/scripts/minio_file_uploader.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/scripts/session_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1251 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/session.py
--rw-rw-rw-   0 root         (0) root         (0)     3401 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/sync.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/sync_jobs_cleaner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.607909 libreflow-2.4.2/src/libreflow/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/b3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.609908 libreflow-2.4.2/src/libreflow/utils/flow/
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14474 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/flow/action_values.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/flow/context_values.py
--rw-rw-rw-   0 root         (0) root         (0)     5358 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/flow/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/flow/file_processing.py
--rw-rw-rw-   0 root         (0) root         (0)    16613 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/flow/import_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5412 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/flow/process_files.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/flow/values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.609908 libreflow-2.4.2/src/libreflow/utils/kabaret/
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.610908 libreflow-2.4.2/src/libreflow/utils/kabaret/flow_entities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/flow_entities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9034 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/flow_entities/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.611909 libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/
--rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2747 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/demo_flow.py
--rw-rw-rw-   0 root         (0) root         (0)    27913 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_actor.py
--rw-rw-rw-   0 root         (0) root         (0)     6738 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_flow.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_flow_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4660 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_node.py
--rw-rw-rw-   0 root         (0) root         (0)    11242 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.612908 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.612908 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/actor/
--rw-rw-rw-   0 root         (0) root         (0)     4584 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/actor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.612908 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/flow/
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5670 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/runner_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.613908 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/views/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18305 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/views/subprocess_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.614909 libreflow-2.4.2/src/libreflow/utils/kabaret/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18769 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/ui/flow_view.py
--rw-rw-rw-   0 root         (0) root         (0)     6555 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/ui/main_window.py
--rw-rw-rw-   0 root         (0) root         (0)    20792 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/ui/navigation_control.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/kabaret/ui/widget_view.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/os.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.615908 libreflow-2.4.2/src/libreflow/utils/search/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/actor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.615908 libreflow-2.4.2/src/libreflow/utils/search/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.617909 libreflow-2.4.2/src/libreflow/utils/search/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      885 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/export.png
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/filter-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/filter-enabled.png
--rw-rw-rw-   0 root         (0) root         (0)      901 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/import.png
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/magn-glass.png
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/minus-button.png
--rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/plus-button.png
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/remove.png
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/data/icons/run-button.png
--rw-rw-rw-   0 root         (0) root         (0)    16126 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/search/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.618909 libreflow-2.4.2/src/libreflow/utils/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20399 2024-05-03 16:07:20.000000 libreflow-2.4.2/src/libreflow/utils/ui/file_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:07:29.618909 libreflow-2.4.2/src/libreflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)    73121 2024-05-03 16:07:29.000000 libreflow-2.4.2/src/libreflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14481 2024-05-03 16:07:29.000000 libreflow-2.4.2/src/libreflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 16:07:29.000000 libreflow-2.4.2/src/libreflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      212 2024-05-03 16:07:29.000000 libreflow-2.4.2/src/libreflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-03 16:07:29.000000 libreflow-2.4.2/src/libreflow.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    70144 2024-05-03 16:07:20.000000 libreflow-2.4.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.740069 libreflow-2.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-05-16 16:00:42.000000 libreflow-2.4.3/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    72196 2024-05-16 16:00:42.000000 libreflow-2.4.3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2024-05-16 16:00:42.000000 libreflow-2.4.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-16 16:00:42.000000 libreflow-2.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    73233 2024-05-16 16:00:52.740069 libreflow-2.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2024-05-16 16:00:42.000000 libreflow-2.4.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-16 16:00:52.740069 libreflow-2.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2405 2024-05-16 16:00:42.000000 libreflow-2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.662069 libreflow-2.4.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.741069 libreflow-2.4.3/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)      911 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-05-16 16:00:52.741069 libreflow-2.4.3/src/libreflow/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.678069 libreflow-2.4.3/src/libreflow/baseflow/
+-rw-rw-rw-   0 root         (0) root         (0)    31651 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6047 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     7427 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/departments.py
+-rw-rw-rw-   0 root         (0) root         (0)    34140 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/entity_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)   201280 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)    28331 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)    35159 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/kitsu.py
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4712 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/maputils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18934 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/mytasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/runactions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15138 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/runners.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/shot.py
+-rw-rw-rw-   0 root         (0) root         (0)    49390 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/site.py
+-rw-rw-rw-   0 root         (0) root         (0)    19053 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/task.py
+-rw-rw-rw-   0 root         (0) root         (0)    72943 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/task_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.680069 libreflow-2.4.3/src/libreflow/baseflow/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25652 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    13555 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/delegate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11242 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/file.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/file_cell.py
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/file_history.py
+-rw-rw-rw-   0 root         (0) root         (0)    12971 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/file_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.681069 libreflow-2.4.3/src/libreflow/baseflow/ui/importfiles/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/importfiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7233 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/importfiles/custom_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)    12827 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/importfiles/files_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    17843 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/importfiles/target_wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.682069 libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17306 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/components.py
+-rw-rw-rw-   0 root         (0) root         (0)    14000 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/edit_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     7051 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/file_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    49203 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/mytasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/qmodel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/qmodel.py
+-rw-rw-rw-   0 root         (0) root         (0)    18098 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/ui/task.py
+-rw-rw-rw-   0 root         (0) root         (0)    16888 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/baseflow/users.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.683069 libreflow-2.4.3/src/libreflow/custom_home/
+-rw-rw-rw-   0 root         (0) root         (0)     7239 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/custom_home/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4642 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/custom_home/ui.py
+-rw-rw-rw-   0 root         (0) root         (0)   211828 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/custom_home/wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.683069 libreflow-2.4.3/src/libreflow/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.684069 libreflow-2.4.3/src/libreflow/examples/demoflow/
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/demoflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/demoflow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/demoflow/lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.685069 libreflow-2.4.3/src/libreflow/examples/majorque/
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/majorque/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/majorque/departments.py
+-rw-rw-rw-   0 root         (0) root         (0)    10006 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/majorque/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5209 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/majorque/film.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/majorque/kitsu.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/majorque/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/majorque/runners.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/examples/majorque/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     5674 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/jobs_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/jobs_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.686069 libreflow-2.4.3/src/libreflow/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.693069 libreflow-2.4.3/src/libreflow/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.abc
+-rw-rw-rw-   0 root         (0) root         (0)     8621 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.aep
+-rw-rw-rw-   0 root         (0) root         (0)   323555 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.ai
+-rw-rw-rw-   0 root         (0) root         (0)   120981 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.blend
+-rw-rw-rw-   0 root         (0) root         (0)    32284 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.fbx
+-rw-rw-rw-   0 root         (0) root         (0)    20632 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.jpg
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.jsx
+-rw-rw-rw-   0 root         (0) root         (0)    65344 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.kra
+-rw-rw-rw-   0 root         (0) root         (0)    11248 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.mov
+-rw-rw-rw-   0 root         (0) root         (0)  1263464 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.mp4
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.nk
+-rw-rw-rw-   0 root         (0) root         (0)    63071 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.obj
+-rw-rw-rw-   0 root         (0) root         (0)    36592 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.png
+-rw-rw-rw-   0 root         (0) root         (0)   417005 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.psb
+-rw-rw-rw-   0 root         (0) root         (0)   397099 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.psd
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.usd
+-rw-rw-rw-   0 root         (0) root         (0)    88244 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/file_templates/template.wav
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.695069 libreflow-2.4.3/src/libreflow/resources/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    86400 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/fonts/SpaceGrotesk-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    86504 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/fonts/SpaceGrotesk-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.695069 libreflow-2.4.3/src/libreflow/resources/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.695069 libreflow-2.4.3/src/libreflow/resources/icons/applications/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/applications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/applications/rv.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.696069 libreflow-2.4.3/src/libreflow/resources/icons/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6763 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/flow/alembic.png
+-rw-rw-rw-   0 root         (0) root         (0)     5862 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/flow/explorer.png
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/flow/photoshop.png
+-rw-rw-rw-   0 root         (0) root         (0)    10783 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/flow/quicktime.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.703069 libreflow-2.4.3/src/libreflow/resources/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/add-file.png
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/add-folder.png
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/arrow-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)      821 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/check-box-empty-dark.png
+-rw-rw-rw-   0 root         (0) root         (0)    10906 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/clean.png
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/close.png
+-rw-rw-rw-   0 root         (0) root         (0)     4867 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/compositing.png
+-rw-rw-rw-   0 root         (0) root         (0)      868 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/duplicate.png
+-rw-rw-rw-   0 root         (0) root         (0)    17838 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/location-worldwide-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)    17853 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/location-worldwide.png
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/maximize.png
+-rw-rw-rw-   0 root         (0) root         (0)    18568 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/menu.png
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/menu_dots.png
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/minimize.png
+-rw-rw-rw-   0 root         (0) root         (0)     5694 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/misc.png
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/mytasks-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/mytasks.png
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-left-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)      930 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-left.png
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-refresh-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-refresh.png
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-right-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/ref-broken.png
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/ref.png
+-rw-rw-rw-   0 root         (0) root         (0)     2360 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/refresh.png
+-rw-rw-rw-   0 root         (0) root         (0)     6914 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/send.png
+-rw-rw-rw-   0 root         (0) root         (0)    13652 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/gui/send2.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.704069 libreflow-2.4.3/src/libreflow/resources/icons/history/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/check.png
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/done.png
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/init.png
+-rw-rw-rw-   0 root         (0) root         (0)      838 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/retake.png
+-rw-rw-rw-   0 root         (0) root         (0)      831 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/wfa.png
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/wip.png
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/working_copy.png
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/history/working_copy_mine.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.720069 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/3d-object.png
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/active_site.png
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/afterfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     6101 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/archive.png
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/available.png
+-rw-rw-rw-   0 root         (0) root         (0)     6331 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/blank.png
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/blender.png
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/checked-symbol-colored.png
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/checked-symbol.png
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/circle-shape-outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/circle-shape-right-eye-outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     1730 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/circular-shape-right-eye-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/circular-shape-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/clean.png
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/clipboard.png
+-rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/compare-previews.png
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/cross-mark-on-a-black-circle-background-colored.png
+-rw-rw-rw-   0 root         (0) root         (0)     3131 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/custom_home_star.png
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/dependencies.png
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/download.png
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/downloadable.png
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/duplicate.png
+-rw-rw-rw-   0 root         (0) root         (0)    15134 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/edit-blank.png
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/edit-lock-green.png
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/edit-lock-red.png
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/error.png
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/exchange.png
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/exclamation-sign-colored.png
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/fbx.png
+-rw-rw-rw-   0 root         (0) root         (0)     6192 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/firefox.png
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/hide.png
+-rw-rw-rw-   0 root         (0) root         (0)     6372 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/history.png
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/illustrator.png
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/json.png
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/jsx.png
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_done.png
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_oklodv.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_omit.png
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_retake.png
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_todo.png
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_wfa.png
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_wip.png
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/krita.png
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/lock-green.png
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/lock-red.png
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/log_out.png
+-rw-rw-rw-   0 root         (0) root         (0)    37128 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/multi-share-option.png
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/nuke.png
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/origin-site.png
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/padlock.png
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/padlock_green.png
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/padlock_red.png
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/premiere-pro.png
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/publish-ae.png
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/publish-blender.png
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/publish.png
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/quicktime.png
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/refresh.png
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/request.png
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/requestable.png
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/run.png
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/show.png
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/stop.png
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/sync.png
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/sync_arrow.png
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/time_format.png
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/unavailable.png
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/upload.png
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/vscodium.png
+-rw-rw-rw-   0 root         (0) root         (0)    73670 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/waiting.png
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/warning.png
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/libreflow/watch.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.723069 libreflow-2.4.3/src/libreflow/resources/icons/status/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/done.png
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/err.png
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/inv.png
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/none.png
+-rw-rw-rw-   0 root         (0) root         (0)     2999 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/nys.png
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/oop.png
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/rtk.png
+-rw-rw-rw-   0 root         (0) root         (0)     3113 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/rvw.png
+-rw-rw-rw-   0 root         (0) root         (0)     3212 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/wait.png
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/warn.png
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/status/wip.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.725069 libreflow-2.4.3/src/libreflow/resources/icons/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/animation.svg
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/clean.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/colo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/compositing.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/design.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/layout.svg
+-rw-rw-rw-   0 root         (0) root         (0)      903 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/lighting.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/modeling.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/rigging.svg
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/icons/tasks/shading.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.725069 libreflow-2.4.3/src/libreflow/resources/mark_sequence/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/mark_sequence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.726069 libreflow-2.4.3/src/libreflow/resources/mark_sequence/fields/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/mark_sequence/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/mark_sequence/fields/default.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.726069 libreflow-2.4.3/src/libreflow/resources/mark_sequence/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   313408 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/mark_sequence/fonts/LiberationMono-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/mark_sequence/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.727069 libreflow-2.4.3/src/libreflow/resources/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.727069 libreflow-2.4.3/src/libreflow/resources/scripts/blender/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/scripts/blender/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6076 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/scripts/blender/disable_save_keymap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.727069 libreflow-2.4.3/src/libreflow/resources/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.728069 libreflow-2.4.3/src/libreflow/resources/styles/lfs_tech/
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/styles/lfs_tech/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10517 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.729069 libreflow-2.4.3/src/libreflow/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16095 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/scripts/mark_sequence.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/scripts/minio_file_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/scripts/minio_file_uploader.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/scripts/session_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     3401 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/sync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/sync_jobs_cleaner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.729069 libreflow-2.4.3/src/libreflow/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/b3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.731069 libreflow-2.4.3/src/libreflow/utils/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14474 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/flow/action_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/flow/context_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/flow/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/flow/file_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)    16613 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/flow/import_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5412 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/flow/process_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/flow/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.731069 libreflow-2.4.3/src/libreflow/utils/kabaret/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.732069 libreflow-2.4.3/src/libreflow/utils/kabaret/flow_entities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/flow_entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9034 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/flow_entities/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.733069 libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2747 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/demo_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)    27913 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6738 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_flow_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4660 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    11242 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.734069 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.734069 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/actor/
+-rw-rw-rw-   0 root         (0) root         (0)     4584 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/actor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.734069 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5670 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/runner_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.735069 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/views/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18305 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/views/subprocess_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.736069 libreflow-2.4.3/src/libreflow/utils/kabaret/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18769 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/ui/flow_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     6555 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/ui/main_window.py
+-rw-rw-rw-   0 root         (0) root         (0)    20792 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/ui/navigation_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/kabaret/ui/widget_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/os.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.736069 libreflow-2.4.3/src/libreflow/utils/search/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/actor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.737069 libreflow-2.4.3/src/libreflow/utils/search/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.739069 libreflow-2.4.3/src/libreflow/utils/search/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      885 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/export.png
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/filter-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/filter-enabled.png
+-rw-rw-rw-   0 root         (0) root         (0)      901 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/import.png
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/magn-glass.png
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/minus-button.png
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/plus-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/remove.png
+-rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/data/icons/run-button.png
+-rw-rw-rw-   0 root         (0) root         (0)    16126 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/search/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.739069 libreflow-2.4.3/src/libreflow/utils/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20399 2024-05-16 16:00:42.000000 libreflow-2.4.3/src/libreflow/utils/ui/file_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:00:52.739069 libreflow-2.4.3/src/libreflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    73233 2024-05-16 16:00:52.000000 libreflow-2.4.3/src/libreflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14481 2024-05-16 16:00:52.000000 libreflow-2.4.3/src/libreflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 16:00:52.000000 libreflow-2.4.3/src/libreflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2024-05-16 16:00:52.000000 libreflow-2.4.3/src/libreflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-16 16:00:52.000000 libreflow-2.4.3/src/libreflow.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70144 2024-05-16 16:00:42.000000 libreflow-2.4.3/versioneer.py
```

### Comparing `libreflow-2.4.2/CHANGELOG.md` & `libreflow-2.4.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.4.3] - 2024-05-16
+
+### Changed
+
+* Activate the filter (search bar) on the assets and asset families map.
+
 ## [2.4.2] - 2024-05-03
 
 ### Added
 
 * mrViewer added in runners list for playback movies.
 
 ## [2.4.1] - 2024-04-27
```

### Comparing `libreflow-2.4.2/LICENSE` & `libreflow-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/PKG-INFO` & `libreflow-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow
-Version: 2.4.2
+Version: 2.4.3
 Summary: An example flow for kabaret
 Home-page: https://gitlab.com/lfs.coop/libreflow
 Author: Flavio Perez
 Author-email: flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -47,14 +47,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.4.3] - 2024-05-16
+
+### Changed
+
+* Activate the filter (search bar) on the assets and asset families map.
+
 ## [2.4.2] - 2024-05-03
 
 ### Added
 
 * mrViewer added in runners list for playback movies.
 
 ## [2.4.1] - 2024-04-27
```

### Comparing `libreflow-2.4.2/README.md` & `libreflow-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/setup.py` & `libreflow-2.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/__init__.py` & `libreflow-2.4.3/src/libreflow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/__init__.py` & `libreflow-2.4.3/src/libreflow/baseflow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/asset.py` & `libreflow-2.4.3/src/libreflow/baseflow/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     ICON = ('icons.flow', 'asset_family')
 
     code = Property().ui(hidden=True)
     display_name = Property().ui(hidden=True)
 
     assets = flow.Child(AssetCollection).injectable().ui(
-        expanded=True
+        expanded=True, show_filter=True
     )
 
     @classmethod
     def get_source_display(cls, oid):
         split = oid.split('/')
         indices = list(range(len(split) - 1, 2, -2))
         return ' – '.join([split[i] for i in reversed(indices)])
@@ -119,15 +119,15 @@
     """
 
     ICON = ('icons.flow', 'asset_family')
 
     code = Property().ui(hidden=True)
     display_name = Property().ui(hidden=True)
 
-    asset_families = flow.Child(AssetFamilyCollection).injectable()
+    asset_families = flow.Child(AssetFamilyCollection).ui(show_filter=True).injectable()
 
     @classmethod
     def get_source_display(cls, oid):
         split = oid.split('/')
         indices = list(range(len(split) - 1, 2, -2))
         return ' – '.join([split[i] for i in reversed(indices)])
```

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/departments.py` & `libreflow-2.4.3/src/libreflow/baseflow/departments.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/dependency.py` & `libreflow-2.4.3/src/libreflow/baseflow/dependency.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/entity_manager.py` & `libreflow-2.4.3/src/libreflow/baseflow/entity_manager.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/file.py` & `libreflow-2.4.3/src/libreflow/baseflow/file.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/film.py` & `libreflow-2.4.3/src/libreflow/baseflow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/kitsu.py` & `libreflow-2.4.3/src/libreflow/baseflow/kitsu.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/lib.py` & `libreflow-2.4.3/src/libreflow/baseflow/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/maputils.py` & `libreflow-2.4.3/src/libreflow/baseflow/maputils.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/mytasks.py` & `libreflow-2.4.3/src/libreflow/baseflow/mytasks.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/runactions.py` & `libreflow-2.4.3/src/libreflow/baseflow/runactions.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/runners.py` & `libreflow-2.4.3/src/libreflow/baseflow/runners.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/shot.py` & `libreflow-2.4.3/src/libreflow/baseflow/shot.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/site.py` & `libreflow-2.4.3/src/libreflow/baseflow/site.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/task.py` & `libreflow-2.4.3/src/libreflow/baseflow/task.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/task_manager.py` & `libreflow-2.4.3/src/libreflow/baseflow/task_manager.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/controller.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/controller.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/delegate.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/delegate.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/file.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/file.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/file_history.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/file_history.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/file_list.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/file_list.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/importfiles/custom_widget.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/importfiles/custom_widget.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/importfiles/files_list.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/importfiles/files_list.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/importfiles/target_wizard.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/importfiles/target_wizard.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/components.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/components.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/edit_dialog.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/edit_dialog.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/file_list.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/file_list.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/mytasks.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/mytasks.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/mytasks/qmodel.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/mytasks/qmodel.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/qmodel.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/qmodel.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/ui/task.py` & `libreflow-2.4.3/src/libreflow/baseflow/ui/task.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/baseflow/users.py` & `libreflow-2.4.3/src/libreflow/baseflow/users.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/custom_home/__init__.py` & `libreflow-2.4.3/src/libreflow/custom_home/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/custom_home/ui.py` & `libreflow-2.4.3/src/libreflow/custom_home/ui.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/custom_home/wizard.py` & `libreflow-2.4.3/src/libreflow/custom_home/wizard.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/demoflow/film.py` & `libreflow-2.4.3/src/libreflow/examples/demoflow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/demoflow/lib.py` & `libreflow-2.4.3/src/libreflow/examples/demoflow/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/majorque/__init__.py` & `libreflow-2.4.3/src/libreflow/examples/majorque/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/majorque/departments.py` & `libreflow-2.4.3/src/libreflow/examples/majorque/departments.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/majorque/file.py` & `libreflow-2.4.3/src/libreflow/examples/majorque/file.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/majorque/film.py` & `libreflow-2.4.3/src/libreflow/examples/majorque/film.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/majorque/kitsu.py` & `libreflow-2.4.3/src/libreflow/examples/majorque/kitsu.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/majorque/lib.py` & `libreflow-2.4.3/src/libreflow/examples/majorque/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/examples/majorque/runners.py` & `libreflow-2.4.3/src/libreflow/examples/majorque/runners.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/gui.py` & `libreflow-2.4.3/src/libreflow/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/jobs_cleaner.py` & `libreflow-2.4.3/src/libreflow/jobs_cleaner.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/jobs_node.py` & `libreflow-2.4.3/src/libreflow/jobs_node.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.abc` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.abc`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.aep` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.aep`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.ai` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.ai`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.blend` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.fbx` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.fbx`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.jpg` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.jpg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.kra` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.kra`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.mov` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.mov`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.mp4` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.mp4`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.nk` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.nk`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.obj` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.obj`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.png` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.psb` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.psb`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.psd` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.psd`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.usd` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.usd`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/file_templates/template.wav` & `libreflow-2.4.3/src/libreflow/resources/file_templates/template.wav`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/fonts/SpaceGrotesk-Bold.ttf` & `libreflow-2.4.3/src/libreflow/resources/fonts/SpaceGrotesk-Bold.ttf`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/fonts/SpaceGrotesk-Regular.ttf` & `libreflow-2.4.3/src/libreflow/resources/fonts/SpaceGrotesk-Regular.ttf`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/applications/rv.png` & `libreflow-2.4.3/src/libreflow/resources/icons/applications/rv.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/flow/alembic.png` & `libreflow-2.4.3/src/libreflow/resources/icons/flow/alembic.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/flow/explorer.png` & `libreflow-2.4.3/src/libreflow/resources/icons/flow/explorer.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/flow/photoshop.png` & `libreflow-2.4.3/src/libreflow/resources/icons/flow/photoshop.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/flow/quicktime.png` & `libreflow-2.4.3/src/libreflow/resources/icons/flow/quicktime.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/add-file.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/add-file.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/add-folder.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/add-folder.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/arrow-down.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/arrow-down.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/arrow-right.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/check-box-empty-dark.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/check-box-empty-dark.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/clean.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/clean.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/close.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/close.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/compositing.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/compositing.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/duplicate.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/duplicate.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/location-worldwide-disabled.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/location-worldwide-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/location-worldwide.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/location-worldwide.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/maximize.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/maximize.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/menu.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/menu.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/menu_dots.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/menu_dots.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/minimize.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/minimize.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/misc.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/misc.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/mytasks-disabled.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/mytasks-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/mytasks.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/mytasks.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-left-disabled.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-left-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-left.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-left.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-refresh-disabled.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-refresh-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-refresh.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-refresh.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-right-disabled.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-right-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/nav-arrow-right.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/nav-arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/ref-broken.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/ref-broken.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/ref.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/ref.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/refresh.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/refresh.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/send.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/send.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/gui/send2.png` & `libreflow-2.4.3/src/libreflow/resources/icons/gui/send2.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/history/check.png` & `libreflow-2.4.3/src/libreflow/resources/icons/history/check.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/history/done.png` & `libreflow-2.4.3/src/libreflow/resources/icons/history/done.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/history/retake.png` & `libreflow-2.4.3/src/libreflow/resources/icons/history/retake.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/history/wfa.png` & `libreflow-2.4.3/src/libreflow/resources/icons/history/wfa.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/history/wip.png` & `libreflow-2.4.3/src/libreflow/resources/icons/history/wip.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/history/working_copy.png` & `libreflow-2.4.3/src/libreflow/resources/icons/history/working_copy.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/history/working_copy_mine.png` & `libreflow-2.4.3/src/libreflow/resources/icons/history/working_copy_mine.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/3d-object.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/3d-object.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/active_site.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/active_site.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/afterfx.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/afterfx.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/archive.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/archive.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/available.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/available.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/blank.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/blank.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/blender.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/blender.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/checked-symbol-colored.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/checked-symbol-colored.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/checked-symbol.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/checked-symbol.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/circle-shape-outline.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/circle-shape-outline.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/circle-shape-right-eye-outline.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/circle-shape-right-eye-outline.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/circular-shape-right-eye-silhouette.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/circular-shape-right-eye-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/circular-shape-silhouette.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/circular-shape-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/clean.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/clean.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/clipboard.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/clipboard.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/compare-previews.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/compare-previews.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/cross-mark-on-a-black-circle-background-colored.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/cross-mark-on-a-black-circle-background-colored.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/custom_home_star.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/custom_home_star.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/delete.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/delete.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/dependencies.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/dependencies.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/download.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/download.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/downloadable.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/downloadable.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/duplicate.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/duplicate.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/edit-blank.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/edit-blank.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/edit-lock-green.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/edit-lock-green.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/edit-lock-red.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/edit-lock-red.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/error.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/error.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/exchange.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/exchange.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/exclamation-sign-colored.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/exclamation-sign-colored.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/fbx.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/fbx.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/firefox.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/firefox.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/hide.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/hide.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/history.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/history.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/illustrator.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/illustrator.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/json.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/json.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/jsx.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/jsx.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_done.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_done.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_oklodv.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_oklodv.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_omit.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_omit.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_retake.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_retake.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_todo.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_todo.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_wfa.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_wfa.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/kitsu_status_wip.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/kitsu_status_wip.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/krita.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/krita.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/lock-green.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/lock-green.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/lock-red.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/lock-red.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/log_out.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/log_out.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/multi-share-option.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/multi-share-option.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/nuke.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/nuke.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/origin-site.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/origin-site.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/padlock.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/padlock.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/padlock_green.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/padlock_green.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/padlock_red.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/padlock_red.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/publish-ae.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/publish-ae.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/publish-blender.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/publish-blender.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/publish.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/publish.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/quicktime.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/quicktime.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/refresh.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/refresh.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/request.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/request.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/requestable.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/requestable.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/run.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/run.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/show.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/show.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/stop.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/stop.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/sync.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/sync.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/sync_arrow.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/sync_arrow.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/time_format.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/time_format.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/unavailable.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/unavailable.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/upload.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/upload.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/vscodium.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/vscodium.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/waiting.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/waiting.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/warning.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/warning.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/libreflow/watch.png` & `libreflow-2.4.3/src/libreflow/resources/icons/libreflow/watch.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/done.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/done.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/err.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/err.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/inv.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/inv.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/none.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/none.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/nys.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/nys.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/oop.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/oop.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/rtk.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/rtk.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/rvw.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/rvw.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/wait.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/wait.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/warn.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/warn.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/status/wip.png` & `libreflow-2.4.3/src/libreflow/resources/icons/status/wip.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/animation.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/animation.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/clean.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/clean.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/colo.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/colo.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/compositing.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/compositing.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/design.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/design.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/layout.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/layout.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/lighting.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/lighting.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/modeling.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/modeling.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/rigging.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/rigging.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/icons/tasks/shading.svg` & `libreflow-2.4.3/src/libreflow/resources/icons/tasks/shading.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/mark_sequence/fields/default.json` & `libreflow-2.4.3/src/libreflow/resources/mark_sequence/fields/default.json`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/mark_sequence/fonts/LiberationMono-Regular.ttf` & `libreflow-2.4.3/src/libreflow/resources/mark_sequence/fonts/LiberationMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/scripts/blender/disable_save_keymap.py` & `libreflow-2.4.3/src/libreflow/resources/scripts/blender/disable_save_keymap.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/styles/lfs_tech/__init__.py` & `libreflow-2.4.3/src/libreflow/resources/styles/lfs_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css` & `libreflow-2.4.3/src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/scripts/mark_sequence.py` & `libreflow-2.4.3/src/libreflow/scripts/mark_sequence.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/scripts/session_worker.py` & `libreflow-2.4.3/src/libreflow/scripts/session_worker.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/session.py` & `libreflow-2.4.3/src/libreflow/session.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/sync.py` & `libreflow-2.4.3/src/libreflow/sync.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/sync_jobs_cleaner.py` & `libreflow-2.4.3/src/libreflow/sync_jobs_cleaner.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/flow/action_values.py` & `libreflow-2.4.3/src/libreflow/utils/flow/action_values.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/flow/context_values.py` & `libreflow-2.4.3/src/libreflow/utils/flow/context_values.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/flow/entities.py` & `libreflow-2.4.3/src/libreflow/utils/flow/entities.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/flow/file_processing.py` & `libreflow-2.4.3/src/libreflow/utils/flow/file_processing.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/flow/import_files.py` & `libreflow-2.4.3/src/libreflow/utils/flow/import_files.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/flow/process_files.py` & `libreflow-2.4.3/src/libreflow/utils/flow/process_files.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/flow/values.py` & `libreflow-2.4.3/src/libreflow/utils/flow/values.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/flow_entities/entities.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/flow_entities/entities.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/demo_flow.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/demo_flow.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_actor.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_actor.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_flow.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_flow.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_flow_worker.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_flow_worker.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_node.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_node.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/jobs/jobs_view.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/jobs/jobs_view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/actor/__init__.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/flow/__init__.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/runner_factory.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/runner_factory.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/subprocess_manager/views/subprocess_view.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/subprocess_manager/views/subprocess_view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/ui/flow_view.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/ui/flow_view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/ui/main_window.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/ui/navigation_control.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/ui/navigation_control.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/kabaret/ui/widget_view.py` & `libreflow-2.4.3/src/libreflow/utils/kabaret/ui/widget_view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/os.py` & `libreflow-2.4.3/src/libreflow/utils/os.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/actor.py` & `libreflow-2.4.3/src/libreflow/utils/search/actor.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/export.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/export.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/filter-disabled.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/filter-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/filter-enabled.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/filter-enabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/import.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/import.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/magn-glass.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/magn-glass.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/minus-button.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/minus-button.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/plus-button.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/plus-button.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/remove.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/remove.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/data/icons/run-button.png` & `libreflow-2.4.3/src/libreflow/utils/search/data/icons/run-button.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/search/view.py` & `libreflow-2.4.3/src/libreflow/utils/search/view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow/utils/ui/file_processing.py` & `libreflow-2.4.3/src/libreflow/utils/ui/file_processing.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/src/libreflow.egg-info/PKG-INFO` & `libreflow-2.4.3/src/libreflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow
-Version: 2.4.2
+Version: 2.4.3
 Summary: An example flow for kabaret
 Home-page: https://gitlab.com/lfs.coop/libreflow
 Author: Flavio Perez
 Author-email: flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -47,14 +47,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.4.3] - 2024-05-16
+
+### Changed
+
+* Activate the filter (search bar) on the assets and asset families map.
+
 ## [2.4.2] - 2024-05-03
 
 ### Added
 
 * mrViewer added in runners list for playback movies.
 
 ## [2.4.1] - 2024-04-27
```

### Comparing `libreflow-2.4.2/src/libreflow.egg-info/SOURCES.txt` & `libreflow-2.4.3/src/libreflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow-2.4.2/versioneer.py` & `libreflow-2.4.3/versioneer.py`

 * *Files identical despite different names*

