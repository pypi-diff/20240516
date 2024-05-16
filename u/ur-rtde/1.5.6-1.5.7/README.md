# Comparing `tmp/ur_rtde-1.5.6.tar.gz` & `tmp/ur_rtde-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ur_rtde-1.5.6.tar", last modified: Tue Apr 11 21:57:43 2023, max compression
+gzip compressed data, was "ur_rtde-1.5.7.tar", last modified: Tue Sep 19 15:30:58 2023, max compression
```

## Comparing `ur_rtde-1.5.6.tar` & `ur_rtde-1.5.7.tar`

### file list

```diff
@@ -1,164 +1,170 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/.clang-format
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-04-11 19:51:54.000000 ur_rtde-1.5.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/.gitmodules
--rw-rw-rw-   0 root         (0) root         (0)    25756 2023-04-11 19:38:36.000000 ur_rtde-1.5.6/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-11 19:38:36.000000 ur_rtde-1.5.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5642 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5090 2023-03-23 09:59:42.000000 ur_rtde-1.5.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/ci/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.366021 ur_rtde-1.5.6/ci/.vol/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/ci/.vol/cb-series/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/ci/.vol/cb-series/.urcontrol/
--rw-rw-rw-   0 root         (0) root         (0)     2723 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/.vol/cb-series/.urcontrol/safety.conf.UR5
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/.vol/cb-series/default.installation
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/.vol/cb-series/default.variables
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/.vol/cb-series/programs.UR5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/ci/.vol/e-series/
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/.vol/e-series/default.installation
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/.vol/e-series/default.variables
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/.vol/e-series/programs.UR5
--rwxrwxrwx   0 root         (0) root         (0)      390 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/build-boost.sh
--rwxrwxrwx   0 root         (0) root         (0)     1484 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/build-wheels.sh
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/gitlab-ci-common.yml
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/gitlab-ci-linux.yml
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/gitlab-ci-mac.yml
--rw-rw-rw-   0 root         (0) root         (0)     1280 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/gitlab-ci-windows.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/ci/platforms/
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/platforms/mac-catalina.yml
--rw-rw-rw-   0 root         (0) root         (0)      450 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/platforms/ubuntu1804.yml
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-04-11 19:59:57.000000 ur_rtde-1.5.6/ci/platforms/ubuntu2004.yml
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/ci/platforms/ubuntu2204.yml
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-04-11 19:59:57.000000 ur_rtde-1.5.6/ci/platforms/windows10-vs16.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/cmake/
--rw-rw-rw-   0 root         (0) root         (0)     2995 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/cmake/FindEigen3.cmake
--rw-rw-rw-   0 root         (0) root         (0)     8383 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/cmake/FindPythonLibsNew.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1630 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/cmake/find_python_module.cmake
--rw-rw-rw-   0 root         (0) root         (0)     3223 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/cmake/pybind11Config.cmake
--rw-rw-rw-   0 root         (0) root         (0)     9582 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/cmake/pybind11Tools.cmake
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/cmake/ur_rtdeBuildConfig.cmake.in
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/cmake/ur_rtdeConfig.cmake
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/conanfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/debian/
--rw-rw-rw-   0 root         (0) root         (0)    13800 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        3 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/control
--rw-rw-rw-   0 root         (0) root         (0)     1342 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/copyright
--rw-rw-rw-   0 root         (0) root         (0)     2418 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/how_to_setup.md
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/librtde-dev.install
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/librtde.install
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/librtde.lintian-overrides
--rwxrwxrwx   0 root         (0) root         (0)      785 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/rules
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/debian/source/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/source/format
--rwxrwxrwx   0 root         (0) root         (0)     4691 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/debian/ur_rtde_build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.370021 ur_rtde-1.5.6/doc/
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.374021 ur_rtde-1.5.6/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)     7057 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/boost-logo.svg
--rw-rw-rw-   0 root         (0) root         (0)   275190 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/force_mode_example.gif
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/googled5bfdc1684e49924.html
--rw-rw-rw-   0 root         (0) root         (0)  1429269 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/move_circle_example.gif
--rw-rw-rw-   0 root         (0) root         (0)   177131 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/movel_path_blend.gif
--rw-rw-rw-   0 root         (0) root         (0)    52984 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/movep_circle.jpg
--rw-rw-rw-   0 root         (0) root         (0)    19601 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/open_cmake_project.png
--rw-rw-rw-   0 root         (0) root         (0)    58510 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/pybind11-logo.png
--rw-rw-rw-   0 root         (0) root         (0)    13243 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/robotiq_gripper.py
--rw-rw-rw-   0 root         (0) root         (0)     2676 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/robotiq_gripper_control.py
--rw-rw-rw-   0 root         (0) root         (0)    46852 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/robotiq_preamble.py
--rw-rw-rw-   0 root         (0) root         (0)    76571 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/robots.png
--rw-rw-rw-   0 root         (0) root         (0)   228095 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/servoj_example.gif
--rw-rw-rw-   0 root         (0) root         (0)   206770 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/speedj_example.gif
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/theme_overrides.css
--rw-rw-rw-   0 root         (0) root         (0)    19833 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/ur_rtde_diagram.png
--rw-rw-rw-   0 root         (0) root         (0)   300103 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/ur_rtde_logo.png
--rw-rw-rw-   0 root         (0) root         (0)  4287054 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/_static/ur_rtde_manual_program.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.378021 ur_rtde-1.5.6/doc/api/
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/api/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     6691 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/conf.py.in
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/doxyfile.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.378021 ur_rtde-1.5.6/doc/examples/
--rw-rw-rw-   0 root         (0) root         (0)    40103 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/examples/examples.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.378021 ur_rtde-1.5.6/doc/faq/
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/faq/faq.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.378021 ur_rtde-1.5.6/doc/guides/
--rw-rw-rw-   0 root         (0) root         (0)    26495 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/guides/guides.rst
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.378021 ur_rtde-1.5.6/doc/installation/
--rw-rw-rw-   0 root         (0) root         (0)     7285 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/installation/installation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.378021 ur_rtde-1.5.6/doc/introduction/
--rw-rw-rw-   0 root         (0) root         (0)     1815 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/doc/introduction/introduction.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.366021 ur_rtde-1.5.6/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.378021 ur_rtde-1.5.6/examples/cpp/
--rw-rw-rw-   0 root         (0) root         (0)     1249 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/forcemode_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/io_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1961 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/jog_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1753 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/move_async_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/move_path_async_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/move_until_contact.cpp
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/movej_path_with_blend_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2511 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/realtime_control_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2122 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/record_data_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3697 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/robotiq_gripper_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/servoj_example.cpp
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/cpp/speedj_example.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.378021 ur_rtde-1.5.6/examples/py/
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/forcemode_example.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/io_example.py
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/move_async_example.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/move_path_async_example.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/move_until_contact.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/movel_path_with_blend_example.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/realtime_control_example.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/record_data_example.py
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/servoj_example.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/examples/py/speedj_example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.366021 ur_rtde-1.5.6/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/include/ur_rtde/
--rw-rw-rw-   0 root         (0) root         (0)     5580 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/dashboard_client.h
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/dashboard_enums.h
--rw-rw-rw-   0 root         (0) root         (0)     5069 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/robot_state.h
--rw-rw-rw-   0 root         (0) root         (0)    16424 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/robotiq_gripper.h
--rw-rw-rw-   0 root         (0) root         (0)     6521 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/rtde.h
--rw-rw-rw-   0 root         (0) root         (0)    48606 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/rtde_control_interface.h
--rw-rw-rw-   0 root         (0) root         (0)    29143 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/rtde_control_interface_doc.h
--rw-rw-rw-   0 root         (0) root         (0)     4323 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/rtde_io_interface.h
--rw-rw-rw-   0 root         (0) root         (0)     4473 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/rtde_io_interface_doc.h
--rw-rw-rw-   0 root         (0) root         (0)    14509 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/rtde_receive_interface.h
--rw-rw-rw-   0 root         (0) root         (0)    10260 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/rtde_receive_interface_doc.h
--rw-rw-rw-   0 root         (0) root         (0)    14789 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/rtde_utility.h
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/ur_rtde/script_client.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/include/urcl/
--rw-rw-rw-   0 root         (0) root         (0)     3577 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/urcl/script_sender.h
--rw-rw-rw-   0 root         (0) root         (0)     2976 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/urcl/server.h
--rw-rw-rw-   0 root         (0) root         (0)     3800 2023-04-11 21:57:19.000000 ur_rtde-1.5.6/include/urcl/tcp_socket.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/scripts/
--rw-rw-rw-   0 root         (0) root         (0)    37000 2023-04-11 19:22:24.000000 ur_rtde-1.5.6/scripts/rtde_control.script
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4707 2023-04-11 19:38:36.000000 ur_rtde-1.5.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/src/
--rw-rw-rw-   0 root         (0) root         (0)    11568 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/src/dashboard_client.cpp
--rw-rw-rw-   0 root         (0) root         (0)     7803 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/src/dashboard_enums.cpp
--rw-rw-rw-   0 root         (0) root         (0)     7625 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/src/robot_state.cpp
--rw-rw-rw-   0 root         (0) root         (0)    14536 2023-03-15 12:40:47.000000 ur_rtde-1.5.6/src/robotiq_gripper.cpp
--rw-rw-rw-   0 root         (0) root         (0)    24949 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/src/rtde.cpp
--rw-rw-rw-   0 root         (0) root         (0)    77104 2023-04-11 19:22:24.000000 ur_rtde-1.5.6/src/rtde_control_interface.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12462 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/src/rtde_io_interface.cpp
--rw-rw-rw-   0 root         (0) root         (0)    34744 2023-04-11 19:22:24.000000 ur_rtde-1.5.6/src/rtde_python_bindings.cpp
--rw-rw-rw-   0 root         (0) root         (0)    28637 2023-02-02 14:30:05.000000 ur_rtde-1.5.6/src/rtde_receive_interface.cpp
--rw-rw-rw-   0 root         (0) root         (0)     9581 2023-04-11 19:22:24.000000 ur_rtde-1.5.6/src/script_client.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/src/urcl/
--rw-rw-rw-   0 root         (0) root         (0)     3341 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/src/urcl/server.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5442 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/src/urcl/tcp_socket.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/test/
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/test/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)   299373 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/test/doctest.h
--rw-rw-rw-   0 root         (0) root         (0)     9841 2023-01-17 19:31:57.000000 ur_rtde-1.5.6/test/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:57:43.382022 ur_rtde-1.5.6/ur_rtde.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5642 2023-04-11 21:57:43.000000 ur_rtde-1.5.6/ur_rtde.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3730 2023-04-11 21:57:43.000000 ur_rtde-1.5.6/ur_rtde.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 21:57:43.000000 ur_rtde-1.5.6/ur_rtde.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 21:57:43.000000 ur_rtde-1.5.6/ur_rtde.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 21:57:43.000000 ur_rtde-1.5.6/ur_rtde.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.629027 ur_rtde-1.5.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/.clang-format
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/.gitmodules
+-rw-rw-rw-   0 root         (0) root         (0)    26296 2023-09-19 07:54:50.000000 ur_rtde-1.5.7/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5642 2023-09-19 15:30:58.629027 ur_rtde-1.5.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5090 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.501027 ur_rtde-1.5.7/ci/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.469027 ur_rtde-1.5.7/ci/.vol/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.505027 ur_rtde-1.5.7/ci/.vol/cb-series/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.505027 ur_rtde-1.5.7/ci/.vol/cb-series/.urcontrol/
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/.vol/cb-series/.urcontrol/safety.conf.UR5
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/.vol/cb-series/default.installation
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/.vol/cb-series/default.variables
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/.vol/cb-series/programs.UR5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.505027 ur_rtde-1.5.7/ci/.vol/e-series/
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/.vol/e-series/default.installation
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/.vol/e-series/default.variables
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/.vol/e-series/programs.UR5
+-rwxrwxrwx   0 root         (0) root         (0)      390 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/build-boost.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1484 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/build-wheels.sh
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/gitlab-ci-common.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2023-09-01 12:45:06.000000 ur_rtde-1.5.7/ci/gitlab-ci-linux.yml
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/gitlab-ci-mac.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/gitlab-ci-windows.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.505027 ur_rtde-1.5.7/ci/platforms/
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/platforms/mac-catalina.yml
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/platforms/ubuntu1804.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-09-01 12:45:06.000000 ur_rtde-1.5.7/ci/platforms/ubuntu2004.yml
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/platforms/ubuntu2204.yml
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/ci/platforms/windows10-vs16.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.505027 ur_rtde-1.5.7/cmake/
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/cmake/FindEigen3.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     8383 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/cmake/FindPythonLibsNew.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/cmake/find_python_module.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/cmake/pybind11Config.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     9582 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/cmake/pybind11Tools.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/cmake/ur_rtdeBuildConfig.cmake.in
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/cmake/ur_rtdeConfig.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/conanfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.509027 ur_rtde-1.5.7/debian/
+-rw-rw-rw-   0 root         (0) root         (0)    13800 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        3 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/copyright
+-rw-rw-rw-   0 root         (0) root         (0)     2418 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/how_to_setup.md
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/librtde-dev.install
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/librtde.install
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/librtde.lintian-overrides
+-rwxrwxrwx   0 root         (0) root         (0)      785 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/rules
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.509027 ur_rtde-1.5.7/debian/source/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/source/format
+-rwxrwxrwx   0 root         (0) root         (0)     4691 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/debian/ur_rtde_build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.509027 ur_rtde-1.5.7/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.513027 ur_rtde-1.5.7/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     7057 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/boost-logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)   275190 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/force_mode_example.gif
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/googled5bfdc1684e49924.html
+-rw-rw-rw-   0 root         (0) root         (0)  1429269 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/move_circle_example.gif
+-rw-rw-rw-   0 root         (0) root         (0)   177131 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/movel_path_blend.gif
+-rw-rw-rw-   0 root         (0) root         (0)    52984 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/movep_circle.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    19601 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/open_cmake_project.png
+-rw-rw-rw-   0 root         (0) root         (0)    58510 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/pybind11-logo.png
+-rw-rw-rw-   0 root         (0) root         (0)    13243 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/robotiq_gripper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2676 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/robotiq_gripper_control.py
+-rw-rw-rw-   0 root         (0) root         (0)    46852 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/robotiq_preamble.py
+-rw-rw-rw-   0 root         (0) root         (0)    76571 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/robots.png
+-rw-rw-rw-   0 root         (0) root         (0)   228095 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/servoj_example.gif
+-rw-rw-rw-   0 root         (0) root         (0)   206770 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/speedj_example.gif
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/theme_overrides.css
+-rw-rw-rw-   0 root         (0) root         (0)    19833 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/ur_rtde_diagram.png
+-rw-rw-rw-   0 root         (0) root         (0)   300103 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/ur_rtde_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)  4287054 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/_static/ur_rtde_manual_program.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.517027 ur_rtde-1.5.7/doc/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/api/api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6691 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/conf.py.in
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/doxyfile.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.517027 ur_rtde-1.5.7/doc/examples/
+-rw-rw-rw-   0 root         (0) root         (0)    40103 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/examples/examples.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.517027 ur_rtde-1.5.7/doc/faq/
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/faq/faq.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.517027 ur_rtde-1.5.7/doc/guides/
+-rw-rw-rw-   0 root         (0) root         (0)    26495 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/guides/guides.rst
+-rw-rw-rw-   0 root         (0) root         (0)      756 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.517027 ur_rtde-1.5.7/doc/installation/
+-rw-rw-rw-   0 root         (0) root         (0)     7285 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/installation/installation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.517027 ur_rtde-1.5.7/doc/introduction/
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/doc/introduction/introduction.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.473027 ur_rtde-1.5.7/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.573027 ur_rtde-1.5.7/examples/cpp/
+-rw-rw-rw-   0 root         (0) root         (0)     1392 2023-06-30 08:04:24.000000 ur_rtde-1.5.7/examples/cpp/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2108 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/contact_detection_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/forcemode_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/io_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1961 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/jog_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/move_async_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/move_path_async_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/move_until_contact.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/movej_path_with_blend_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2511 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/realtime_control_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/record_data_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3697 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/robotiq_gripper_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/servoj_example.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/cpp/speedj_example.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.577027 ur_rtde-1.5.7/examples/py/
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/forcemode_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/io_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/move_async_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/move_path_async_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/move_until_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/movel_path_with_blend_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/realtime_control_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/record_data_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/servoj_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/examples/py/speedj_example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.473027 ur_rtde-1.5.7/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.577027 ur_rtde-1.5.7/include/ur_rtde/
+-rw-rw-rw-   0 root         (0) root         (0)     5580 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/dashboard_client.h
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/dashboard_enums.h
+-rw-rw-rw-   0 root         (0) root         (0)     5069 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/robot_state.h
+-rw-rw-rw-   0 root         (0) root         (0)    16424 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/robotiq_gripper.h
+-rw-rw-rw-   0 root         (0) root         (0)     6627 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/rtde.h
+-rw-rw-rw-   0 root         (0) root         (0)    51283 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/rtde_control_interface.h
+-rw-rw-rw-   0 root         (0) root         (0)    29589 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/rtde_control_interface_doc.h
+-rw-rw-rw-   0 root         (0) root         (0)     4323 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/rtde_io_interface.h
+-rw-rw-rw-   0 root         (0) root         (0)     4473 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/rtde_io_interface_doc.h
+-rw-rw-rw-   0 root         (0) root         (0)    14509 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/rtde_receive_interface.h
+-rw-rw-rw-   0 root         (0) root         (0)    10260 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/rtde_receive_interface_doc.h
+-rw-rw-rw-   0 root         (0) root         (0)    14813 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/rtde_utility.h
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/ur_rtde/script_client.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.581027 ur_rtde-1.5.7/include/urcl/
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/urcl/default_log_handler.h
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/urcl/log.h
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/urcl/script_sender.h
+-rw-rw-rw-   0 root         (0) root         (0)     5453 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/urcl/tcp_server.h
+-rw-rw-rw-   0 root         (0) root         (0)     4027 2023-09-19 15:30:20.000000 ur_rtde-1.5.7/include/urcl/tcp_socket.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.581027 ur_rtde-1.5.7/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    40472 2023-09-19 07:54:50.000000 ur_rtde-1.5.7/scripts/rtde_control.script
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-19 15:30:58.629027 ur_rtde-1.5.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2023-09-19 07:54:50.000000 ur_rtde-1.5.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.581027 ur_rtde-1.5.7/src/
+-rw-rw-rw-   0 root         (0) root         (0)    11568 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/src/dashboard_client.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     7803 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/src/dashboard_enums.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     7625 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/src/robot_state.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    14869 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/src/robotiq_gripper.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    24949 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/src/rtde.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    78338 2023-09-19 07:54:50.000000 ur_rtde-1.5.7/src/rtde_control_interface.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    12462 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/src/rtde_io_interface.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    35910 2023-09-19 07:54:50.000000 ur_rtde-1.5.7/src/rtde_python_bindings.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    28642 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/src/rtde_receive_interface.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     9581 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/src/script_client.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.581027 ur_rtde-1.5.7/src/urcl/
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2023-09-01 12:45:06.000000 ur_rtde-1.5.7/src/urcl/default_log_handler.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2023-09-01 12:45:06.000000 ur_rtde-1.5.7/src/urcl/log.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2023-09-01 12:45:06.000000 ur_rtde-1.5.7/src/urcl/script_sender.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     8444 2023-09-01 12:45:06.000000 ur_rtde-1.5.7/src/urcl/tcp_server.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     5460 2023-09-01 12:45:06.000000 ur_rtde-1.5.7/src/urcl/tcp_socket.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.625027 ur_rtde-1.5.7/test/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/test/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)   299373 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/test/doctest.h
+-rw-rw-rw-   0 root         (0) root         (0)     9841 2023-06-29 08:30:28.000000 ur_rtde-1.5.7/test/main.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 15:30:58.629027 ur_rtde-1.5.7/ur_rtde.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5642 2023-09-19 15:30:58.000000 ur_rtde-1.5.7/ur_rtde.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3912 2023-09-19 15:30:58.000000 ur_rtde-1.5.7/ur_rtde.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 15:30:58.000000 ur_rtde-1.5.7/ur_rtde.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 15:30:58.000000 ur_rtde-1.5.7/ur_rtde.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-19 15:30:58.000000 ur_rtde-1.5.7/ur_rtde.egg-info/top_level.txt
```

### Comparing `ur_rtde-1.5.6/.clang-format` & `ur_rtde-1.5.7/.clang-format`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/.gitlab-ci.yml` & `ur_rtde-1.5.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/CMakeLists.txt` & `ur_rtde-1.5.7/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 	if(DEFINED WIN32)
 		ADD_DEFINITIONS(-D_WIN32_WINNT=0x0A00)
 		ADD_DEFINITIONS(-DBOOST_ALL_NO_LIB)
 	endif()
 
 endif()
 
-project(ur_rtde VERSION 1.5.6 LANGUAGES ${PROJECT_LANGUAGES})
+project(ur_rtde VERSION 1.5.7 LANGUAGES ${PROJECT_LANGUAGES})
 set(PROJECT_VERSION_SUFFIX "") # alpha/beta/rc, e.g. "-rc0"
 set(PROJECT_VERSION "${PROJECT_VERSION}${PROJECT_VERSION_SUFFIX}")
 set(PROJECT_AUTHOR "Anders Prier Lindvig")
 set(PROJECT_COPYRIGHT "2023")
 set(PROJECT_MAIL "anpl@mmmi.sdu.dk")
 
 if(${CODE})
@@ -67,15 +67,15 @@
 	find_package(Threads)
 
 	if(${PYTHON_BINDINGS})
 		# This is required to find python site-packages for installation of ur_rtde python bindings.
 		if(NOT PYBIND11_PYTHON_VERSION)
 			set(PYBIND11_PYTHON_VERSION "" CACHE STRING "Python version to use for compiling modules")
 		endif()
-		set(Python_ADDITIONAL_VERSIONS 3.10 3.9 3.8 3.7 3.6 3.5 3.4)
+		set(Python_ADDITIONAL_VERSIONS 3.11 3.10 3.9 3.8 3.7 3.6 3.5 3.4)
 		find_package(PythonLibsNew ${PYBIND11_PYTHON_VERSION} REQUIRED)
 
 		if(${CMAKE_VERSION} VERSION_LESS 3.11)
 			# pybind11 must be found from submodule
 			add_subdirectory(pybind11)
 		else()
 			# Get pybind11 with FetchContent
@@ -134,16 +134,19 @@
 			src/dashboard_client.cpp
 			src/dashboard_enums.cpp
 			src/script_client.cpp
 			src/rtde_control_interface.cpp
 			src/rtde_receive_interface.cpp
 			src/rtde_io_interface.cpp
 			src/robotiq_gripper.cpp
-			src/urcl/server.cpp
-			src/urcl/tcp_socket.cpp)
+			src/urcl/script_sender.cpp
+			src/urcl/tcp_server.cpp
+			src/urcl/log.cpp
+			src/urcl/default_log_handler.cpp
+            )
 
 	set(LIB_HEADER_FILES
 			include/ur_rtde/rtde.h
 			include/ur_rtde/rtde_utility.h
 			include/ur_rtde/dashboard_enums.h
 			include/ur_rtde/dashboard_client.h
 			include/ur_rtde/robot_state.h
@@ -153,16 +156,18 @@
 			include/ur_rtde/rtde_receive_interface.h
 			include/ur_rtde/rtde_receive_interface_doc.h
 			include/ur_rtde/rtde_io_interface.h
 			include/ur_rtde/rtde_io_interface_doc.h
 			include/ur_rtde/robotiq_gripper.h)
 
 	set(LIB_URCL_HEADER_FILES
+			include/urcl/log.h
+			include/urcl/default_log_handler.h
 			include/urcl/script_sender.h
-			include/urcl/server.h
+			include/urcl/tcp_server.h
 			include/urcl/tcp_socket.h)
 
 endif()
 
 if(NOT DOC STREQUAL "OFF")
 	add_subdirectory(doc)
 endif()
@@ -313,29 +318,33 @@
 		target_include_directories(record_data_example PUBLIC ${Boost_INCLUDE_DIRS} $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include> $<INSTALL_INTERFACE:include>)
 		target_link_libraries(record_data_example PRIVATE rtde ${Boost_SYSTEM_LIBRARY} ${Boost_THREAD_LIBRARY} ${Boost_PROGRAM_OPTIONS_LIBRARY})
 
 		add_executable(realtime_control_example examples/cpp/realtime_control_example.cpp)
 		target_include_directories(realtime_control_example PUBLIC ${Boost_INCLUDE_DIRS} $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include> $<INSTALL_INTERFACE:include>)
 		target_link_libraries(realtime_control_example PRIVATE rtde ${Boost_SYSTEM_LIBRARY} ${Boost_THREAD_LIBRARY} ${Boost_PROGRAM_OPTIONS_LIBRARY})
 
+		add_executable(contact_detection_example examples/cpp/contact_detection_example.cpp)
+		target_include_directories(contact_detection_example PUBLIC ${Boost_INCLUDE_DIRS} $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include> $<INSTALL_INTERFACE:include>)
+		target_link_libraries(contact_detection_example PRIVATE rtde ${Boost_SYSTEM_LIBRARY} ${Boost_THREAD_LIBRARY})
+
 		if (UNIX)
 			find_package(Curses)
 			if(Curses_FOUND)
 				add_executable(jog_example examples/cpp/jog_example.cpp)
 				target_include_directories(jog_example PUBLIC ${CURSES_INCLUDE_DIR} ${Boost_INCLUDE_DIRS} $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include> $<INSTALL_INTERFACE:include>)
 				target_link_libraries(jog_example PRIVATE rtde ${CURSES_LIBRARY} ${Boost_SYSTEM_LIBRARY} ${Boost_THREAD_LIBRARY})
 				set_target_properties(jog_example
 					PROPERTIES
 					RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_SOURCE_DIR}/bin"
 					)
 				add_executable(ur_rtde::jog_example ALIAS jog_example)
 			endif()
 		endif (UNIX)
 
-		set_target_properties(servoj_example forcemode_example speedj_example movej_path_with_blend_example io_example move_async_example move_path_async_example robotiq_gripper_example move_until_contact_example record_data_example realtime_control_example
+		set_target_properties(servoj_example forcemode_example speedj_example movej_path_with_blend_example io_example move_async_example move_path_async_example robotiq_gripper_example move_until_contact_example record_data_example realtime_control_example contact_detection_example
 				PROPERTIES
 				RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_SOURCE_DIR}/bin"
 				)
 	endif()
 
 	generate_export_header(rtde EXPORT_FILE_NAME ${CMAKE_CURRENT_SOURCE_DIR}/include/ur_rtde/rtde_export.h)
```

### Comparing `ur_rtde-1.5.6/LICENSE` & `ur_rtde-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/PKG-INFO` & `ur_rtde-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ur_rtde
-Version: 1.5.6
+Version: 1.5.7
 Summary: A Python interface for controlling and receiving data from a UR robot using the Real-Time Data Exchange (RTDE) interface of the robot. 
 Home-page: https://gitlab.com/sdurobotics/ur_rtde
 Author: Anders Prier Lindvig
 Author-email: anpl@mmmi.sdu.dk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ur_rtde-1.5.6/README.md` & `ur_rtde-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/ci/.vol/cb-series/.urcontrol/safety.conf.UR5` & `ur_rtde-1.5.7/ci/.vol/cb-series/.urcontrol/safety.conf.UR5`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/ci/.vol/cb-series/default.installation` & `ur_rtde-1.5.7/ci/.vol/cb-series/default.installation`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/ci/.vol/e-series/default.installation` & `ur_rtde-1.5.7/ci/.vol/e-series/default.installation`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/ci/build-wheels.sh` & `ur_rtde-1.5.7/ci/build-wheels.sh`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/ci/gitlab-ci-linux.yml` & `ur_rtde-1.5.7/ci/gitlab-ci-linux.yml`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 .linux-polyscopetest:
   extends: .CI-common-linux
   before_script:
     - 'export DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"'
     - echo "Using " $DIR
     - docker network create --subnet=192.168.56.0/24 static_test_net
-    - docker login -u gitlab-ci-token -p $CI_BUILD_TOKEN $CI_REGISTRY
+    - docker login -u $CI_REGISTRY_USER -p $CI_JOB_TOKEN $CI_REGISTRY
     - docker run --rm -d --net static_test_net --ip 192.168.56.101 -p 5900:5900 -p 29999:29999 -p 30001-30004:30001-30004 -v "${DIR}/ci/.vol/${POLYSCOPE_TYPE}":/ursim/programs --privileged ${POLYSCOPE_IMAGE}
   script:
     - echo "Preparing tests"
     - cd test
     - mkdir build
     - cd build
     - cmake ..
```

### Comparing `ur_rtde-1.5.6/ci/gitlab-ci-windows.yml` & `ur_rtde-1.5.7/ci/gitlab-ci-windows.yml`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/ci/platforms/ubuntu2004.yml` & `ur_rtde-1.5.7/ci/platforms/ubuntu2004.yml`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/cmake/FindEigen3.cmake` & `ur_rtde-1.5.7/cmake/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/cmake/FindPythonLibsNew.cmake` & `ur_rtde-1.5.7/cmake/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/cmake/find_python_module.cmake` & `ur_rtde-1.5.7/cmake/find_python_module.cmake`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/cmake/pybind11Config.cmake` & `ur_rtde-1.5.7/cmake/pybind11Config.cmake`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/cmake/pybind11Tools.cmake` & `ur_rtde-1.5.7/cmake/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/cmake/ur_rtdeBuildConfig.cmake.in` & `ur_rtde-1.5.7/cmake/ur_rtdeBuildConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/cmake/ur_rtdeConfig.cmake` & `ur_rtde-1.5.7/cmake/ur_rtdeConfig.cmake`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/debian/changelog` & `ur_rtde-1.5.7/debian/changelog`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/debian/control` & `ur_rtde-1.5.7/debian/control`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Source: ur-rtde
 Priority: optional
 Maintainer: Anders Prier Lindvig <anpl@mmmi.sdu.dk>
 Build-Depends: 
-  debhelper (>= 10), 
+  debhelper (>= 9),
   cmake(>= 3.5), 
-  libboost-system-dev (>= 1.54), 
+  libboost-system-dev (>= 1.54),
+  libboost-program-options-dev (>= 1.54),
   libboost-thread-dev (>= 1.54), 
 Standards-Version: 4.1.2
 Section: libs
 Homepage: https://sdurobotics.gitlab.io/ur_rtde/
 Vcs-Git: https://gitlab.com/sdurobotics/ur_rtde.git
 Vcs-Browser: https://gitlab.com/sdurobotics/ur_rtde
```

### Comparing `ur_rtde-1.5.6/debian/copyright` & `ur_rtde-1.5.7/debian/copyright`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/debian/how_to_setup.md` & `ur_rtde-1.5.7/debian/how_to_setup.md`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/debian/rules` & `ur_rtde-1.5.7/debian/rules`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/debian/ur_rtde_build.sh` & `ur_rtde-1.5.7/debian/ur_rtde_build.sh`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/CMakeLists.txt` & `ur_rtde-1.5.7/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/boost-logo.svg` & `ur_rtde-1.5.7/doc/_static/boost-logo.svg`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/force_mode_example.gif` & `ur_rtde-1.5.7/doc/_static/force_mode_example.gif`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/move_circle_example.gif` & `ur_rtde-1.5.7/doc/_static/move_circle_example.gif`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/movel_path_blend.gif` & `ur_rtde-1.5.7/doc/_static/movel_path_blend.gif`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/movep_circle.jpg` & `ur_rtde-1.5.7/doc/_static/movep_circle.jpg`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/open_cmake_project.png` & `ur_rtde-1.5.7/doc/_static/open_cmake_project.png`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/pybind11-logo.png` & `ur_rtde-1.5.7/doc/_static/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/robotiq_gripper.py` & `ur_rtde-1.5.7/doc/_static/robotiq_gripper.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/robotiq_gripper_control.py` & `ur_rtde-1.5.7/doc/_static/robotiq_gripper_control.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/robotiq_preamble.py` & `ur_rtde-1.5.7/doc/_static/robotiq_preamble.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/robots.png` & `ur_rtde-1.5.7/doc/_static/robots.png`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/servoj_example.gif` & `ur_rtde-1.5.7/doc/_static/servoj_example.gif`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/speedj_example.gif` & `ur_rtde-1.5.7/doc/_static/speedj_example.gif`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/ur_rtde_diagram.png` & `ur_rtde-1.5.7/doc/_static/ur_rtde_diagram.png`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/ur_rtde_logo.png` & `ur_rtde-1.5.7/doc/_static/ur_rtde_logo.png`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/_static/ur_rtde_manual_program.png` & `ur_rtde-1.5.7/doc/_static/ur_rtde_manual_program.png`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/api/api.rst` & `ur_rtde-1.5.7/doc/api/api.rst`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/conf.py.in` & `ur_rtde-1.5.7/doc/conf.py.in`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/doxyfile.in` & `ur_rtde-1.5.7/doc/doxyfile.in`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/examples/examples.rst` & `ur_rtde-1.5.7/doc/examples/examples.rst`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/faq/faq.rst` & `ur_rtde-1.5.7/doc/faq/faq.rst`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/guides/guides.rst` & `ur_rtde-1.5.7/doc/guides/guides.rst`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/index.rst` & `ur_rtde-1.5.7/doc/index.rst`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/installation/installation.rst` & `ur_rtde-1.5.7/doc/installation/installation.rst`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/doc/introduction/introduction.rst` & `ur_rtde-1.5.7/doc/introduction/introduction.rst`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/CMakeLists.txt` & `ur_rtde-1.5.7/examples/cpp/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,8 +26,11 @@
 add_executable(speedj speedj_example.cpp)
 target_link_libraries(speedj PUBLIC ur_rtde::rtde)
 
 add_executable(move_async move_async_example.cpp)
 target_link_libraries(move_async PUBLIC ur_rtde::rtde)
 
 add_executable(robotiq_gripper_example robotiq_gripper_example.cpp)
-target_link_libraries(robotiq_gripper_example PUBLIC ur_rtde::rtde)
+target_link_libraries(robotiq_gripper_example PUBLIC ur_rtde::rtde)
+
+add_executable(contact_detection_example contact_detection_example.cpp)
+target_link_libraries(contact_detection_example PUBLIC ur_rtde::rtde)
```

### Comparing `ur_rtde-1.5.6/examples/cpp/forcemode_example.cpp` & `ur_rtde-1.5.7/examples/cpp/forcemode_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/io_example.cpp` & `ur_rtde-1.5.7/examples/cpp/io_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/jog_example.cpp` & `ur_rtde-1.5.7/examples/cpp/jog_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/move_async_example.cpp` & `ur_rtde-1.5.7/examples/cpp/move_async_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/move_path_async_example.cpp` & `ur_rtde-1.5.7/examples/cpp/move_path_async_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/movej_path_with_blend_example.cpp` & `ur_rtde-1.5.7/examples/cpp/movej_path_with_blend_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/realtime_control_example.cpp` & `ur_rtde-1.5.7/examples/cpp/realtime_control_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/record_data_example.cpp` & `ur_rtde-1.5.7/examples/cpp/record_data_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/robotiq_gripper_example.cpp` & `ur_rtde-1.5.7/examples/cpp/robotiq_gripper_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/servoj_example.cpp` & `ur_rtde-1.5.7/examples/cpp/servoj_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/cpp/speedj_example.cpp` & `ur_rtde-1.5.7/examples/cpp/speedj_example.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/py/forcemode_example.py` & `ur_rtde-1.5.7/examples/py/forcemode_example.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/py/io_example.py` & `ur_rtde-1.5.7/examples/py/io_example.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/py/move_async_example.py` & `ur_rtde-1.5.7/examples/py/move_async_example.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/py/move_path_async_example.py` & `ur_rtde-1.5.7/examples/py/move_path_async_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 print("Path finished!")
 
 # Now move given path asynchronously
 print("Move path asynchronously with progress feedback...")
 rtde_c.movePath(path, True)
 
 # Wait for start of asynchronous operation
-while rtde_c.getAsyncOperationProgress() < 0:
+while not rtde_c.getAsyncOperationProgressEx().isAsyncOperationRunning():
     time.sleep(0.010)
 print("Async path started.. ")
 
 # Wait for end of asynchronous operation
 waypoint = -1
-while rtde_c.getAsyncOperationProgress() >= 0:
+while rtde_c.getAsyncOperationProgressEx().isAsyncOperationRunning():
     time.sleep(0.2)
     new_waypoint = rtde_c.getAsyncOperationProgress()
     if new_waypoint != waypoint:
         waypoint = new_waypoint
         print("Moving to path waypoint ")
 
 print("Async path finished...\n\n")
```

### Comparing `ur_rtde-1.5.6/examples/py/movel_path_with_blend_example.py` & `ur_rtde-1.5.7/examples/py/movel_path_with_blend_example.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/py/realtime_control_example.py` & `ur_rtde-1.5.7/examples/py/realtime_control_example.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/py/record_data_example.py` & `ur_rtde-1.5.7/examples/py/record_data_example.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/py/servoj_example.py` & `ur_rtde-1.5.7/examples/py/servoj_example.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/examples/py/speedj_example.py` & `ur_rtde-1.5.7/examples/py/speedj_example.py`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/dashboard_client.h` & `ur_rtde-1.5.7/include/ur_rtde/dashboard_client.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/dashboard_enums.h` & `ur_rtde-1.5.7/include/ur_rtde/dashboard_enums.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/robot_state.h` & `ur_rtde-1.5.7/include/ur_rtde/robot_state.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/robotiq_gripper.h` & `ur_rtde-1.5.7/include/ur_rtde/robotiq_gripper.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/rtde.h` & `ur_rtde-1.5.7/include/ur_rtde/rtde.h`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,17 @@
       SET_EXTERNAL_FORCE_TORQUE = 55,
       FT_RTDE_INPUT_ENABLE = 56,
       ENABLE_EXTERNAL_FT_SENSOR = 57,
       GET_ACTUAL_TOOL_FLANGE_POSE = 58,
       SET_GRAVITY = 59,
       GET_INVERSE_KINEMATICS_HAS_SOLUTION_DEFAULT = 60,
       GET_INVERSE_KINEMATICS_HAS_SOLUTION_ARGS = 61,
+      START_CONTACT_DETECTION = 62,
+      STOP_CONTACT_DETECTION = 63,
+      READ_CONTACT_DETECTION = 64,
       WATCHDOG = 99,
       STOP_SCRIPT = 255
     };
 
     enum Recipe
     {
       RECIPE_1 = 1,
```

### Comparing `ur_rtde-1.5.6/include/ur_rtde/rtde_control_interface.h` & `ur_rtde-1.5.7/include/ur_rtde/rtde_control_interface.h`

 * *Files 3% similar despite different names*

```diff
@@ -89,24 +89,24 @@
    | Bit 31 | Bit 30 - 24 | Bit 23 | Bit 9 - 22     | Bit 15  | Bit 14 - 0 |
     +--------+-------------+--------+----------------+---------+------------+
    | rsv    | async_op_id | rsv    | async_wr_count | running | progress   |
 
    running: 1 - async op. running, 0 - async op. finished
    progress: progress of running async. operation.
  */
-class CAsyncOperationStatus
+class AsyncOperationStatus
 {
  private:
   uint32_t status_;  // the status word received from robot
 
  public:
   /**
    * Create status object from received status word
    */
-  CAsyncOperationStatus(int Value = 0) : status_(Value)
+  AsyncOperationStatus(int Value = 0) : status_(Value)
   {
   }
 
   /**
    * Access the raw status value
    */
   uint32_t value() const
@@ -163,15 +163,15 @@
       return -1;  // -1 indicates no async operation running
     }
   }
 
   /**
    * Test, if async operation progress changed
    */
-  bool equals(const CAsyncOperationStatus &other) const
+  bool equals(const AsyncOperationStatus &other) const
   {
     return this->status_ == other.status_;
   }
 };
 
 /**
  * This class provides the interface to control the robot and to execute robot
@@ -522,18 +522,20 @@
    * vectors if the user moves the joystick or the Space Navigator cap.
    * @param speed Speed vector for translation and rotation. Translation values
    * are given in mm / s and rotation values in rad / s.
    * @param feature Configures to move to move with respect to base frame
    * (FEATURE_BASE), tool frame (FEATURE_TOOL) or custom frame (FEATURE_CUSTOM)
    * If the feature is FEATURE_CUSTOM then the custom_frame parameter needs to
    * be a valid pose.
+   * @param acc Acceleration value. If you need to manually jog items that
+   *        require a lower acceleration, then you can provide a custom value here.
    * @param custom_frame The custom_frame given as pose if the selected feature
    * is FEATURE_CUSTOM
    */
-  RTDE_EXPORT bool jogStart(const std::vector<double> &speeds, int feature = FEATURE_BASE,
+  RTDE_EXPORT bool jogStart(const std::vector<double> &speeds, int feature = FEATURE_BASE, double acc = 0.5,
                             const std::vector<double> &custom_frame = {});
 
   /**
    * Stops jogging that has been started start_jog
    */
   RTDE_EXPORT bool jogStop();
 
@@ -727,18 +729,18 @@
   RTDE_EXPORT int getAsyncOperationProgress();
 
   /**
    * Returns extended async operation progress information for asynchronous
    * operations that supports progress feedback (such as movePath).
    * It also returns the status of any async operation such as moveJ, moveL,
    * stopJ or stopL.
-   * @see CAsyncOperationStatus for a detailed description of the progress
+   * @see AsyncOperationStatus class for a detailed description of the progress
    *      status.
    */
-  RTDE_EXPORT CAsyncOperationStatus getAsyncOperationProgressEx();
+  RTDE_EXPORT AsyncOperationStatus getAsyncOperationProgressEx();
 
   /**
    * @brief Enable a watchdog for the communication with a specified minimum frequency for which an input update is
    * expected to arrive. The watchdog is useful for safety critical realtime applications eg. servoing. The default
    * action taken is to shutdown the control, if the watchdog is not kicked with the minimum frequency.
    *
    * Preferably you would call this function right after the RTDEControlInterface has been constructed.
@@ -828,14 +830,15 @@
    * @param xd tool speed [m/s] (spatial vector)
    * @param direction List of six floats. The first three elements are interpreted as a 3D vector
    * (in the robot base coordinate system) giving the direction in which contacts should be detected. If all elements
    * of the list are zero, contacts from all directions are considered. You can also set
    * direction=get_target_tcp_speed() in which case it will detect contacts in the direction of the TCP movement.
    * @param acceleration tool position acceleration [m/s^2]
    * @returns True once the robot is in contact.
+   * @see startContactDetection() function for async contact detection
    */
   RTDE_EXPORT bool moveUntilContact(const std::vector<double> &xd,
                                     const std::vector<double> &direction = {0.0, 0.0, 0.0, 0.0, 0.0, 0.0},
                                     double acceleration = 0.5);
 
   /**
    * @brief Set robot in freedrive mode. In this mode the robot can be moved around by hand in the same way
@@ -992,14 +995,69 @@
    * @param maxOrientationError the maximum allowed orientationerror (Optional)
    * @returns true if getInverseKin has a solution, false otherwise (bool)
    */
   RTDE_EXPORT bool getInverseKinematicsHasSolution(const std::vector<double> &x, const std::vector<double> &qnear = {},
                                                    double max_position_error = 1e-10,
                                                    double max_orientation_error = 1e-10);
 
+  /**
+   * @brief Starts async contact detection thread
+   *
+   * Move the robot until contact, with specified speed and contact detection direction.
+   * The robot will automatically retract to the initial point of contact.
+   *
+   * Contact monitoring should get started after a async move command has been
+   * started. That means, there should be no async move commands after this
+   * command because async move commands may cause a reupload of the script
+   * which in turn kills the contact monitoring thread. If a contact is detected,
+   * the contact monitoring thread is stopped, the robot is stopped and then
+   * retracted to the initial point of contact.
+   *
+   * \code
+   *  rtde_control.moveL(target, 0.25, 0.5, true);
+   *  rtde_control.startContactDetection(); // detect contact in direction of TCP movement
+   *
+   *  // now wait until the robot stops - it either stops if it has reached
+   *  // the target pose or if a contact has been detected
+   *  // you can use the readContactDetection() function, to check if a contact
+   *  // has been detected.
+   *  bool contact_detected = rtde_control.readContactDetection();
+   *
+   *
+   *  contact_detected = rtde_control.stopContactDetection();
+   * \endcode
+   *
+   * @param direction List of six floats.
+   * The first three elements are interpreted as a 3D vector
+   * (in the robot base coordinate system) giving the direction in which contacts should be detected.
+   * If all elements of the list are zero, direction will be set to
+   * direction=get_target_tcp_speed() in which case it will detect contacts in
+   * the direction of the TCP movement.
+   *
+   * @return Returns true, if a contact has been detected
+   */
+  RTDE_EXPORT bool startContactDetection(const std::vector<double> &direction = {0.0, 0.0, 0.0, 0.0, 0.0, 0.0});
+
+  /**
+   * Reads the current async contact detection state.
+   * The function returns true, when a contact between the tool and an object
+   * has been detected.
+   */
+  RTDE_EXPORT bool readContactDetection();
+
+  /**
+   * @brief Stop contact monitoring
+   * This function stops contact monitoring and returns true, if a contact has
+   * been detected. Normally the contact
+   * detection is stopped, as soon as a contact ha been detected. If you would
+   * like to stop the contact detection manually, i.e. because of a timeout,
+   * the you can use this function.
+   */
+  RTDE_EXPORT bool stopContactDetection();
+
   // Unlocks a protective stop via the dashboard client.
   void unlockProtectiveStop();
 
   // Returns the version numbers of the robot.
   const Versions &versions() const
   {
     return versions_;
@@ -1085,19 +1143,19 @@
   std::shared_ptr<RTDE> rtde_;
   std::atomic<bool> stop_thread_{false};
   std::shared_ptr<boost::thread> th_;
   std::shared_ptr<DashboardClient> db_client_;
   std::shared_ptr<ScriptClient> script_client_;
   std::shared_ptr<RobotState> robot_state_;
 #if !defined(_WIN32) && !defined(__APPLE__)
-  std::unique_ptr<urcl::comm::ScriptSender> urcl_script_sender_;
+  std::unique_ptr<urcl::control::ScriptSender> urcl_script_sender_;
 #endif
   std::vector<std::string> state_names_;
   // major, minor, bugfix, build numbers.
-  Versions versions_;
+  Versions versions_{};
   std::string serial_number_;
   size_t no_bytes_avail_cnt_;
 };
 
 /**
  * Single path entry in a move path
  */
```

### Comparing `ur_rtde-1.5.6/include/ur_rtde/rtde_control_interface_doc.h` & `ur_rtde-1.5.7/include/ur_rtde/rtde_control_interface_doc.h`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,23 @@
 returned by this function is less than 0 and is different from that
 last value returned by this function, then a new async operation has
 finished. @retval 0 Indicates that an async operation has started -
 progress 0 @retval >= 0 Indicates the progress of an async operation.
 For example, if an operation has 3 steps, the progress ranges from 0 -
 2. The progress value is updated, before a step is executed. When the
 last step has been executed, the value will change to -1 to indicate
-the end of the async operation.)doc";
+the end of the async operation. @deprecated The function is deprecated and only
+here for backward compatibility. Use getAsyncOperationProgressEx() instead.)doc";
+
+
+static const char *__doc_ur_rtde_RTDEControlInterface_getAsyncOperationProgressEx =
+R"doc(Returns extended async operation progress information for asynchronous
+operations that supports progress feedback (such as movePath).
+@see AsyncOperationStatus documentation for a detailed description of the
+returned status.)doc";
 
 
 static const char *__doc_ur_rtde_RTDEControlInterface_getRobotStatus =
 R"doc(Returns:
     Robot status Bits 0-3: Is power on | Is program running | Is teach
     button pressed | Is power button pressed
     There is a synchronization gap between the three interfaces RTDE Control
@@ -68,15 +76,14 @@
     RTDE Control already reports program running.
     \note If you work with RTDE control and receive interface and you need to
     read the robot status or program running state, then you should always
     use the getRobotStatus() function from RTDE Control if you need a status
     that is in sync with the program uploading or reuploading of this object.)doc";
 
 
-
 static const char *__doc_ur_rtde_RTDEControlInterface_forceMode =
 R"doc(Set robot to be controlled in force mode
 
 Parameter ``task_frame``:
     A pose vector that defines the force frame relative to the base
     frame.
```

### Comparing `ur_rtde-1.5.6/include/ur_rtde/rtde_io_interface.h` & `ur_rtde-1.5.7/include/ur_rtde/rtde_io_interface.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/rtde_io_interface_doc.h` & `ur_rtde-1.5.7/include/ur_rtde/rtde_io_interface_doc.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/rtde_receive_interface.h` & `ur_rtde-1.5.7/include/ur_rtde/rtde_receive_interface.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/rtde_receive_interface_doc.h` & `ur_rtde-1.5.7/include/ur_rtde/rtde_receive_interface_doc.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/ur_rtde/rtde_utility.h` & `ur_rtde-1.5.7/include/ur_rtde/rtde_utility.h`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 #include <ratio>
 #include <ctime>
 #include <cerrno>
 #include <cassert>
 
 #if defined(WIN32) || defined(_WIN32) || defined(__WIN32__) || defined(__NT__)
 #define WIN32_LEAN_AND_MEAN
+#ifndef NOMINMAX
 #define NOMINMAX
+#endif
 #include <windows.h>
 #else
 #include <pthread.h>
 #include <fstream>
 #endif
 
 #define SLACK_TIME_IN_MICROS 300UL
```

### Comparing `ur_rtde-1.5.6/include/ur_rtde/script_client.h` & `ur_rtde-1.5.7/include/ur_rtde/script_client.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/include/urcl/tcp_socket.h` & `ur_rtde-1.5.7/include/urcl/tcp_socket.h`

 * *Files 9% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 #pragma once
 #ifndef URCL_TCP_SOCKET_H
 #define URCL_TCP_SOCKET_H
 
 #include <netdb.h>
 #include <sys/socket.h>
 #include <sys/types.h>
-
 #include <atomic>
-#include <memory>
 #include <mutex>
 #include <string>
+#include <memory>
 
 namespace urcl
 {
 namespace comm
 {
 /*!
  * \brief State the socket can be in
@@ -50,17 +49,17 @@
 
 /*!
  * \brief Class for TCP socket abstraction
  */
 class TCPSocket
 {
  private:
-  bool verbose_;
   std::atomic<int> socket_fd_;
   std::atomic<SocketState> state_;
+  std::chrono::seconds reconnection_time_;
 
  protected:
   virtual bool open(int socket_fd, struct sockaddr* address, size_t address_len)
   {
     return false;
   }
   virtual void setOptions(int socket_fd);
@@ -69,15 +68,15 @@
 
   std::unique_ptr<timeval> recv_timeout_;
 
  public:
   /*!
    * \brief Creates a TCPSocket object
    */
-  TCPSocket(bool verbose = false);
+  TCPSocket();
   virtual ~TCPSocket();
 
   /*!
    * \brief Getter for the state of the socket.
    *
    * \returns Returns the current state of the socket
    */
@@ -91,27 +90,19 @@
    *
    * \returns The file descriptor of the socket
    */
   int getSocketFD()
   {
     return socket_fd_;
   }
-  /*!
-   * \brief Setter for the file descriptor of the socket.
-   *
-   * \param socket_fd The new value
-   *
-   * \returns False, if the socket is in state connected
-   */
-  bool setSocketFD(int socket_fd);
 
   /*!
-   * \brief Determines the IP address of the local machine
+   * \brief Determines the local IP address of the currently configured socket
    *
-   * \returns The IP address of the local machine.
+   * \returns The local IP address of the socket associated to the current file descriptor
    */
   std::string getIP() const;
 
   /*!
    * \brief Reads one byte from the socket
    *
    * \param[out] character Target buffer
@@ -149,12 +140,23 @@
 
   /*!
    * \brief Setup Receive timeout used for this socket.
    *
    * \param timeout Timeout used for setting things up
    */
   void setReceiveTimeout(const timeval& timeout);
+
+  /*!
+   * \brief Set reconnection time, if the server is unavailable during connection this will set the time before
+   * trying connect to the server again.
+   *
+   * \param reconnection_time time in between connection attempts to the server
+   */
+  void setReconnectionTime(std::chrono::seconds reconnection_time)
+  {
+    reconnection_time_ = reconnection_time;
+  }
 };
 }  // namespace comm
 }  // namespace urcl
 
 #endif  // URCL_TCP_SOCKET_H
```

### Comparing `ur_rtde-1.5.6/scripts/rtde_control.script` & `ur_rtde-1.5.7/scripts/rtde_control.script`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,20 @@
     global speed_thrd = 0
     global force_thrd = 0
 
     global jog_feature = 0 # 0 - base, 1 - tool, 2 - custom
     global jog_speed_pose = p[0, 0, 0, 0, 0, 0]
     global jog_custom_feature = p[0, 0, 0, 0, 0, 0]
     global jog_thrd = 0
+    global jog_acc = 0.5
+
+    global contact_direction = p[0, 0, 0, 0, 0, 0]
+    global contact_step_back = 0
+    global contact_thrd = 0
+    global internal_cmd = 0
     
     def read_input_float_reg(register_index):
         return read_input_float_register(register_index + reg_offset_float)
     end
 
     def read_input_integer_reg(register_index):
         return read_input_integer_register(register_index + reg_offset_int)
@@ -128,15 +134,15 @@
         write_async_progress_register(-1) # negative values indicate operation finished
       end
   
       def reset_async_progress():
         signal_async_operation_finished()
       end
 
-      # asynchronous stop thread
+    # asynchronous stop thread
     # stopping a move with a low deceleration may take quite some time, so
     # async execution may prevent blocking the caller
     thread stop_thread():
       textmsg("stop_thread started")
       signal_async_operation_started()
       while (True):
           if stop_type == 0:
@@ -274,14 +280,57 @@
 
     thread servoc_thread():
         while (True):
             servoc(servoc_target, a=servoc_acceleration, v=servoc_velocity, r=servoc_blend)
         end
     end
 
+    thread contact_thread():
+      textmsg("contact_thread started")
+      enter_critical
+      contact_step_back = 0
+      dir = contact_direction
+      exit_critical
+
+      textmsg("direction:", dir)
+      use_speed_vector = pose_is_null(dir)
+      if use_speed_vector:
+          textmsg("Using speed vector")
+      end
+
+      step_back = 1
+      # First we wait until there is not contact
+$5.4  while step_back > 0:
+$5.4      if use_speed_vector:
+$5.4          step_back = tool_contact(direction=get_target_tcp_speed())
+$5.4      else:
+$5.4          step_back = tool_contact(direction=dir)
+$5.4      end
+$5.4      sync()
+$5.4  end
+
+      # Now we can wait for a contact
+$5.4  while step_back == 0:
+$5.4      if use_speed_vector:
+$5.4          step_back = tool_contact(direction=get_target_tcp_speed())
+$5.4      else:
+$5.4          step_back = tool_contact(direction=dir)
+$5.4      end
+$5.4      sync()
+$5.4  end
+      textmsg("step_back:", step_back)
+      textmsg("target_tcp_speed: ", get_target_tcp_speed())
+      enter_critical
+      contact_thrd = 0
+      contact_step_back = step_back
+      internal_cmd = 254 # delegate processing of contact detection to main thread
+      exit_critical
+      textmsg("contact_thread finished")
+    end
+
     def q_from_input_float_registers(register_index):
       q = [0, 0, 0, 0, 0, 0]
       q[0] = read_input_float_reg(register_index + 0)
       q[1] = read_input_float_reg(register_index + 1)
       q[2] = read_input_float_reg(register_index + 2)
       q[3] = read_input_float_reg(register_index + 3)
       q[4] = read_input_float_reg(register_index + 4)
@@ -335,14 +384,19 @@
       p[2] = p[2] * factor
       p[3] = p[3] * factor
       p[4] = p[4] * factor
       p[5] = p[5] * factor
       return p
     end
 
+    def pose_is_null(p):
+      sum = p[0] + p[1] + p[2] + p[3] + p[4] + p[5]
+      return (sum < 0.0000000001)
+    end
+
     # convert tool_speed expressed in the frame_wrt_base in the robot base frame
     # examples :
     # speed_wrt_base([0.020, 0.020,0,0,0,0], plane_1)
     # speedl(get_speed_wrt_base([0,0,0.02,0,0,1.57], get_actual_tcp_pose()),a=1,t=0.5,aRot=4))
   
     #### input arguments
     # tool_speed : [Tx, Ty, Tz, Rx, Ry, Rz] spatial vector list - Txyz [m/s]), Rxyz [rad/s]
@@ -392,33 +446,40 @@
       end
 
       while (True):
         enter_critical
         speed_pose = jog_speed_pose
         exit_critical
         speed_wrt_base = get_speed_wrt_base(speed_pose, frame_wrt_base)
-        speedl(speed_wrt_base, 0.5)
+        speedl(speed_wrt_base, jog_acc)
       end
     end
 
     def signal_ready():
         write_output_integer_reg(0, 1)
     end
 
     def signal_done_with_cmd():
         write_output_integer_reg(0, 2)
     end
 
     def rtde_cmd():
-        return read_input_integer_reg(0)
+      cmd = read_input_integer_reg(0)
+      # only if command is 0 - that means we are idle, we process internal
+      # commands
+      if cmd == 0:
+          enter_critical
+          cmd = internal_cmd
+          internal_cmd = 0
+          exit_critical
+      end
+      return cmd
     end
 
-    def process_cmd():
-        cmd = read_input_integer_reg(0)
-
+    def process_cmd(cmd):
         if cmd == 1:
             textmsg("movej")
             q = q_from_input_float_registers(0)
             velocity = read_input_float_reg(6)
             acceleration = read_input_float_reg(7)
             async = read_input_integer_reg(1)
             textmsg("Target q:")
@@ -786,21 +847,23 @@
 $3.6        pose_to_output_float_registers(0, tcp_offset)
             textmsg("get_tcp_offset done")
         elif cmd == 41:
               textmsg("start_jog")
               enter_critical
               jog_speed_pose = pose_from_input_float_registers(0)
               jog_feature = read_input_float_reg(6)
-              jog_custom_feature = pose_from_input_float_registers(7)
+              jog_acc = read_input_float_reg(7)
+              jog_custom_feature = pose_from_input_float_registers(8)
               if jog_thrd == 0:
                 jog_thrd = run jog_speed_thread()
               end
               exit_critical
               textmsg("jog_feature: ", jog_feature)
               textmsg("jog_custom_feature: ", jog_custom_feature)
+              textmsg("jog_acc: ", jog_acc)
               textmsg("start_jog done")
         elif cmd == 42:
               textmsg("stop_jog")
               enter_critical
               if jog_thrd != 0:
                 textmsg("stopping jogging - killing jog_thrd")
                 kill jog_thrd
@@ -969,14 +1032,54 @@
 $5.10|3.15    has_solution = get_inverse_kin_has_solution(x, qnear, maxPositionError, maxOrientationError)
 $5.10|3.15    if has_solution == True:
 $5.10|3.15        write_output_integer_reg(1, 1)
 $5.10|3.15    else:
 $5.10|3.15        write_output_integer_reg(1, 0)
 $5.10|3.15    end
               textmsg("get_inverse_kin_has_solution_args done")
+            elif cmd == 62:
+              textmsg("start_contact_detection")
+              enter_critical
+              if contact_thrd != 0:
+                  textmsg("killing contact_thrd")
+                  kill contact_thrd
+                  contact_thrd = 0
+              end
+              exit_critical
+              contact_direction = pose_from_input_float_registers(0)
+              contact_thrd = run contact_thread()
+              textmsg("start_contact_detection done")
+          elif cmd == 63:
+              textmsg("stop_contact_detection")
+              enter_critical
+              if contact_thrd != 0:
+                  textmsg("killing contact_thrd")
+                  kill contact_thrd
+                  contact_thrd = 0
+              end
+              exit_critical
+              write_output_integer_reg(1, contact_step_back)
+              textmsg("stop_contact_detection done")
+          elif cmd == 64:
+              textmsg("read_contact_detection")
+              enter_critical
+              step_back = contact_step_back
+              exit_critical
+              write_output_integer_reg(1, step_back)
+              textmsg("read_contact_detection done")
+          elif cmd == 254: # internal command
+              textmsg("cmd == 254 - contact detected") 
+$5.4          stop_async_move()
+$5.4          # Get q for when the contact was first seen
+$5.4          q = get_actual_joint_positions_history(contact_step_back)
+$5.4          # Stop the movement
+$5.4          stopl(3)
+$5.4          # Move to the initial contact point
+$5.4          movel(q)
+$5.4          textmsg("cmd == 254 - contact detected done")
         elif cmd == 255:
               textmsg("Received stop script!")
         end
 
         if cmd != 255:
               signal_done_with_cmd()
         end
@@ -987,40 +1090,39 @@
 # HEADER_END
 
 # NODE_CONTROL_LOOP_BEGINS
 
         ###################################
         # RTDE Control script - Main loop #
         ###################################
-
-        textmsg("RTDE Control Script Loaded (06.03.2023-15:00)")
+        textmsg("RTDE Control Script Loaded (06.06.2023-13:52)")
 
         # Initialize gain and damping for force mode to a more stable default
 $5.0    force_mode_set_gain_scaling(0.5)
 $3.5    force_mode_set_damping(0.025)
 
         keep_running = True
         executing_cmd = False
         reset_async_progress()
         signal_ready()
 
         while keep_running:
             cmd = rtde_cmd()
             if cmd == 24 or cmd == 11 or cmd == 9 or cmd == 10 or cmd == 6 or cmd == 25 or cmd == 26 or cmd == 27 or cmd == 38 or cmd == 58:
                 # for realtime commands simply process and signal ready.
-                keep_running = process_cmd()
+                keep_running = process_cmd(cmd)
                 signal_ready()
             else:
                 # regular mode
                 if cmd == 0:
                     executing_cmd = False
                     signal_ready()
                 else:
                     if not executing_cmd:
-                        keep_running = process_cmd()
+                        keep_running = process_cmd(cmd)
                     end
                     executing_cmd = True
                 end
             end
 
             sync()
         end
```

### Comparing `ur_rtde-1.5.6/setup.py` & `ur_rtde-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     def __str__(self):
         import pybind11
         return pybind11.get_include(self.user)
 
 
 setup(
     name="ur_rtde",
-    version="1.5.6",
+    version="1.5.7",
     author="Anders Prier Lindvig",
     author_email="anpl@mmmi.sdu.dk",
     description="A Python interface for controlling and receiving data from a UR robot using the Real-Time Data Exchange (RTDE) interface of the robot. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[CMakeExtension('ur_rtde')],
     cmdclass=dict(build_ext=CMakeBuild),
```

### Comparing `ur_rtde-1.5.6/src/dashboard_client.cpp` & `ur_rtde-1.5.7/src/dashboard_client.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/src/dashboard_enums.cpp` & `ur_rtde-1.5.7/src/dashboard_enums.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/src/robot_state.cpp` & `ur_rtde-1.5.7/src/robot_state.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/src/robotiq_gripper.cpp` & `ur_rtde-1.5.7/src/robotiq_gripper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,28 @@
   // atomic commands send/rcv
   std::string rx_string;
   {
     const std::lock_guard<std::mutex> lock(mutex_);
     send(cmd);
     rx_string = receive();
   }
+
+  // In case of connection loss we may get empty string here and need to catch
+  // this in order to avoid a crash
+  if (rx_string.empty())
+  {
+	 throw std::logic_error("Empty response");
+  }
+
   auto data = split(rx_string);
+  if (data.empty())
+  {
+	  throw std::logic_error("Invalid or empty response data");
+  }
+
   if (data[0] != var)
   {
     throw std::logic_error("Unexpected response: data " + data[0] + " does not match " + var);
   }
   // if emergency stop is active, then reading a variable does not return a value
   // but a questionmark
   if (data[1][0] == '?')
@@ -512,14 +525,15 @@
   if (deadline_.expires_at() <= boost::asio::deadline_timer::traits_type::now())
   {
     // The deadline has passed. The socket is closed so that any outstanding
     // asynchronous operations are cancelled. This allows the blocked
     // connect(), read_line() or write_line() functions to return.
     boost::system::error_code ignored_ec;
     socket_->close(ignored_ec);
+    conn_state_ = ConnectionState::DISCONNECTED;
 
     // There is no longer an active deadline. The expiry is set to positive
     // infinity so that the actor takes no action until a new deadline is set.
     deadline_.expires_at(boost::posix_time::pos_infin);
   }
 
   // Put the actor back to sleep.
```

### Comparing `ur_rtde-1.5.6/src/rtde.cpp` & `ur_rtde-1.5.7/src/rtde.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/src/rtde_control_interface.cpp` & `ur_rtde-1.5.7/src/rtde_control_interface.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -208,16 +208,15 @@
   }
 
 #if !defined(_WIN32) && !defined(__APPLE__)
   // When the user wants to use ur_rtde with the ExternalControl UR Cap
   if (!upload_script_ && use_external_control_ur_cap_)
   {
     // Create a connection to the ExternalControl UR cap for sending scripts to the cap
-    urcl_script_sender_.reset(new urcl::comm::ScriptSender(ur_cap_port_, script_client_->getScript(), false));
-    urcl_script_sender_->start();
+    urcl_script_sender_.reset(new urcl::control::ScriptSender(ur_cap_port_, script_client_->getScript()));
 
     if (!no_wait_)
     {
       if (!isProgramRunning())
       {
         start_time = std::chrono::high_resolution_clock::now();
         std::cout << "Waiting for RTDE control program to be running on the controller" << std::endl;
@@ -294,25 +293,25 @@
   auto AsyncStatus = getAsyncOperationProgressEx();
   if (AsyncStatus.isAsyncOperationRunning())
   {
 	  return AsyncStatus.progress();
   }
   else
   {
-	  return 0 - (AsyncStatus.operationId() % 2); // toggle between -1 and -2 to mimic the old progress info scheme
+	  return (AsyncStatus.operationId() % 2) - 2; // toggle between -1 and -2 to mimic the old progress info scheme
   }
 }
 
 
-CAsyncOperationStatus RTDEControlInterface::getAsyncOperationProgressEx()
+AsyncOperationStatus RTDEControlInterface::getAsyncOperationProgressEx()
 {
   std::string output_int_register_key = "output_int_register_" + std::to_string(2+register_offset_);
   int32_t output_int_register_val;
   if (robot_state_->getStateData(output_int_register_key, output_int_register_val))
-    return CAsyncOperationStatus(output_int_register_val);
+    return AsyncOperationStatus(output_int_register_val);
   else
     throw std::runtime_error("unable to get state data for specified key: " + output_int_register_key);
 }
 
 
 void RTDEControlInterface::waitForProgramRunning()
 {
@@ -476,16 +475,15 @@
   }
 
 #if !defined(_WIN32) && !defined(__APPLE__)
   // When the user wants to use ur_rtde with the ExternalControl UR Cap
   if (!upload_script_ && use_external_control_ur_cap_)
   {
     // Create a connection to the ExternalControl UR cap for sending scripts to the cap
-    urcl_script_sender_.reset(new urcl::comm::ScriptSender(ur_cap_port_, script_client_->getScript(), false));
-    urcl_script_sender_->start();
+    urcl_script_sender_.reset(new urcl::control::ScriptSender(ur_cap_port_, script_client_->getScript()));
 
     if (!no_wait_)
     {
       if (!isProgramRunning())
       {
         start_time = std::chrono::high_resolution_clock::now();
         std::cout << "Waiting for RTDE control program to be running on the controller" << std::endl;
@@ -669,15 +667,15 @@
                                          inDoubleReg(4), inDoubleReg(5), inDoubleReg(6), inDoubleReg(7)};
   rtde_->sendInputSetup(setp_input);
 
   // Recipe 14
   std::vector<std::string> jog_input = {inIntReg(0),     inDoubleReg(0), inDoubleReg(1), inDoubleReg(2),
                                         inDoubleReg(3),  inDoubleReg(4), inDoubleReg(5), inDoubleReg(6),
                                         inDoubleReg(7),  inDoubleReg(8), inDoubleReg(9), inDoubleReg(10),
-                                        inDoubleReg(11), inDoubleReg(12)};
+                                        inDoubleReg(11), inDoubleReg(12), inDoubleReg(13)};
   rtde_->sendInputSetup(jog_input);
 
   // Recipe 15
   std::vector<std::string> async_path_input = {inIntReg(0), inIntReg(1)};
   rtde_->sendInputSetup(async_path_input);
 
   // Recipe 16
@@ -1155,21 +1153,22 @@
   robot_cmd.val_ = transform;
   robot_cmd.val_.push_back(speed);
   robot_cmd.val_.push_back(acceleration);
   return sendCommand(robot_cmd);
 }
 
 bool RTDEControlInterface::jogStart(const std::vector<double> &speeds, int feature,
-                                    const std::vector<double> &custom_frame)
+	double acc, const std::vector<double> &custom_frame)
 {
   RTDE::RobotCommand robot_cmd;
   robot_cmd.type_ = RTDE::RobotCommand::Type::JOG_START;
   robot_cmd.recipe_id_ = RTDE::RobotCommand::Recipe::RECIPE_14;
   robot_cmd.val_ = speeds;
   robot_cmd.val_.push_back(feature);
+  robot_cmd.val_.push_back(acc);
   if (!custom_frame.empty())
   {
     for (const auto &val : custom_frame)
       robot_cmd.val_.push_back(val);
   }
   else
   {
@@ -1720,14 +1719,73 @@
   }
   else
   {
     return false;
   }
 }
 
+
+bool RTDEControlInterface::startContactDetection(const std::vector<double> &direction)
+{
+  RTDE::RobotCommand robot_cmd;
+  robot_cmd.type_ = RTDE::RobotCommand::Type::START_CONTACT_DETECTION;
+  robot_cmd.recipe_id_ = RTDE::RobotCommand::Recipe::RECIPE_6;
+  robot_cmd.val_ = direction;
+  return sendCommand(robot_cmd);
+}
+
+
+bool RTDEControlInterface::stopContactDetection()
+{
+  RTDE::RobotCommand robot_cmd;
+  robot_cmd.type_ = RTDE::RobotCommand::Type::STOP_CONTACT_DETECTION;
+  robot_cmd.recipe_id_ = RTDE::RobotCommand::Recipe::RECIPE_4;
+
+  if (sendCommand(robot_cmd))
+  {
+    if (robot_state_ != nullptr)
+    {
+      return getOutputIntReg(1) != 0;
+    }
+    else
+    {
+      throw std::logic_error("Please initialize the RobotState, before using it!");
+    }
+  }
+  else
+  {
+    return false;
+  }
+}
+
+
+bool RTDEControlInterface::readContactDetection()
+{
+  RTDE::RobotCommand robot_cmd;
+  robot_cmd.type_ = RTDE::RobotCommand::Type::READ_CONTACT_DETECTION;
+  robot_cmd.recipe_id_ = RTDE::RobotCommand::Recipe::RECIPE_4;
+
+  if (sendCommand(robot_cmd))
+  {
+    if (robot_state_ != nullptr)
+    {
+      return getOutputIntReg(1) != 0;
+    }
+    else
+    {
+      throw std::logic_error("Please initialize the RobotState, before using it!");
+    }
+  }
+  else
+  {
+    return false;
+  }
+}
+
+
 bool RTDEControlInterface::isJointsWithinSafetyLimits(const std::vector<double> &q)
 {
   RTDE::RobotCommand robot_cmd;
   robot_cmd.type_ = RTDE::RobotCommand::Type::IS_JOINTS_WITHIN_SAFETY_LIMITS;
   robot_cmd.recipe_id_ = RTDE::RobotCommand::Recipe::RECIPE_6;
   robot_cmd.val_ = q;
```

### Comparing `ur_rtde-1.5.6/src/rtde_io_interface.cpp` & `ur_rtde-1.5.7/src/rtde_io_interface.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/src/rtde_python_bindings.cpp` & `ur_rtde-1.5.7/src/rtde_python_bindings.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,24 @@
       .def("size", &Path::size, "", py::call_guard<py::gil_scoped_release>())
       .def("waypoints", &Path::waypoints, "", py::call_guard<py::gil_scoped_release>())
       .def("appendMovelPath", &Path::appendMovelPath, "", py::arg("path"), py::call_guard<py::gil_scoped_release>())
       .def("appendMovejPath", &Path::appendMovejPath, "", py::arg("path"), py::call_guard<py::gil_scoped_release>())
       .def("toScriptCode", &Path::toScriptCode, "", py::call_guard<py::gil_scoped_release>())
       .def("__repr__", [](const Path &a) { return "<rtde_control.Path>"; });
 
+  py::class_<AsyncOperationStatus>(m, "AsyncOperationStatus")
+	.def(py::init<int>())
+	.def("value", &AsyncOperationStatus::value, "", py::call_guard<py::gil_scoped_release>())
+	.def("isAsyncOperationRunning", &AsyncOperationStatus::isAsyncOperationRunning, "", py::call_guard<py::gil_scoped_release>())
+	.def("operationId", &AsyncOperationStatus::operationId, "", py::call_guard<py::gil_scoped_release>())
+	.def("changeCount", &AsyncOperationStatus::changeCount, "", py::call_guard<py::gil_scoped_release>())
+	.def("progress", &AsyncOperationStatus::progress, "", py::call_guard<py::gil_scoped_release>())
+	.def("equals", &AsyncOperationStatus::equals, py::arg("other"), py::call_guard<py::gil_scoped_release>())
+	.def("__repr__", [](const AsyncOperationStatus &a) { return "<rtde_control.AsyncOperationStatus>"; });
+
 
   py::class_<RTDEControlInterface> control(m, "RTDEControlInterface");
   py::enum_<RTDEControlInterface::Flags>(control, "Flags", py::arithmetic())
       .value("FLAG_UPLOAD_SCRIPT", RTDEControlInterface::Flags::FLAG_UPLOAD_SCRIPT)
       .value("FLAG_USE_EXT_UR_CAP", RTDEControlInterface::Flags::FLAG_USE_EXT_UR_CAP)
       .value("FLAG_VERBOSE", RTDEControlInterface::Flags::FLAG_VERBOSE)
       .value("FLAG_UPPER_RANGE_REGISTERS", RTDEControlInterface::Flags::FLAG_UPPER_RANGE_REGISTERS)
@@ -158,17 +168,17 @@
            py::call_guard<py::gil_scoped_release>());
   control.def("poseTrans", &RTDEControlInterface::poseTrans,
            DOC(ur_rtde, RTDEControlInterface, poseTrans), py::arg("p_from"), py::arg("p_from_to"),
            py::call_guard<py::gil_scoped_release>());
   control.def("triggerProtectiveStop", &RTDEControlInterface::triggerProtectiveStop,
            DOC(ur_rtde, RTDEControlInterface, triggerProtectiveStop), py::call_guard<py::gil_scoped_release>());
   control.def("stopL", &RTDEControlInterface::stopL,
-           DOC(ur_rtde, RTDEControlInterface, stopL), py::call_guard<py::gil_scoped_release>());
+           DOC(ur_rtde, RTDEControlInterface, stopL), py::arg("a") = 10.0, py::arg("asynchronous") = false, py::call_guard<py::gil_scoped_release>());
   control.def("stopJ", &RTDEControlInterface::stopJ,
-           DOC(ur_rtde, RTDEControlInterface, stopJ), py::call_guard<py::gil_scoped_release>());
+           DOC(ur_rtde, RTDEControlInterface, stopJ), py::arg("a") = 2.0, py::arg("asynchronous") = false, py::call_guard<py::gil_scoped_release>());
   control.def("setWatchdog", &RTDEControlInterface::setWatchdog,
            DOC(ur_rtde, RTDEControlInterface, setWatchdog), py::arg("min_frequency") = 10.0,
            py::call_guard<py::gil_scoped_release>());
   control.def("kickWatchdog", &RTDEControlInterface::kickWatchdog,
            DOC(ur_rtde, RTDEControlInterface, kickWatchdog), py::call_guard<py::gil_scoped_release>());
   control.def("isPoseWithinSafetyLimits", &RTDEControlInterface::isPoseWithinSafetyLimits,
            DOC(ur_rtde, RTDEControlInterface, isPoseWithinSafetyLimits), py::call_guard<py::gil_scoped_release>());
@@ -183,14 +193,15 @@
                   py::call_guard<py::gil_scoped_release>());
   control.def("isSteady", &RTDEControlInterface::isSteady, DOC(ur_rtde, RTDEControlInterface, isSteady), py::call_guard<py::gil_scoped_release>());
   control.def("moveUntilContact", &RTDEControlInterface::moveUntilContact, DOC(ur_rtde, RTDEControlInterface, moveUntilContact), py::arg("xd"),
               py::arg("direction") = std::vector<double>{0, 0, 0, 0, 0, 0}, py::arg("acceleration") = 1.2,
               py::call_guard<py::gil_scoped_release>());
   control.def("jogStart", &RTDEControlInterface::jogStart, DOC(ur_rtde, RTDEControlInterface, jogStart), py::arg("speeds"),
               py::arg("feature") = RTDEControlInterface::Feature::FEATURE_BASE,
+              py::arg("acc") = 0.5,
               py::arg("custom_frame") = std::vector<double>{0, 0, 0, 0, 0, 0},
               py::call_guard<py::gil_scoped_release>());
   control.def("jogStop", &RTDEControlInterface::jogStop, DOC(ur_rtde, RTDEControlInterface, jogStop), py::call_guard<py::gil_scoped_release>());
   control.def("freedriveMode", &RTDEControlInterface::freedriveMode, py::arg("free_axes") = std::vector<int>{1, 1, 1, 1, 1, 1},
               py::arg("feature") = std::vector<double>{0, 0, 0, 0, 0, 0}, py::call_guard<py::gil_scoped_release>());
   control.def("endFreedriveMode", &RTDEControlInterface::endFreedriveMode, py::call_guard<py::gil_scoped_release>());
   control.def("getFreedriveStatus", &RTDEControlInterface::getFreedriveStatus, py::call_guard<py::gil_scoped_release>());
@@ -202,14 +213,15 @@
   control.def("enableExternalFtSensor", &RTDEControlInterface::enableExternalFtSensor, py::arg("enable"),
               py::arg("sensor_mass") = 0.0,
               py::arg("sensor_measuring_offset") = std::vector<double>{0.0, 0.0, 0.0},
               py::arg("sensor_cog") = std::vector<double>{0.0, 0.0, 0.0},
               py::call_guard<py::gil_scoped_release>());
   control.def("setExternalForceTorque", &RTDEControlInterface::setExternalForceTorque, py::call_guard<py::gil_scoped_release>());
   control.def("getAsyncOperationProgress", &RTDEControlInterface::getAsyncOperationProgress, DOC(ur_rtde, RTDEControlInterface, getAsyncOperationProgress), py::call_guard<py::gil_scoped_release>());
+  control.def("getAsyncOperationProgressEx", &RTDEControlInterface::getAsyncOperationProgressEx, DOC(ur_rtde, RTDEControlInterface, getAsyncOperationProgressEx), py::call_guard<py::gil_scoped_release>());
   control.def("getRobotStatus", &RTDEControlInterface::getRobotStatus, DOC(ur_rtde, RTDEControlInterface, getRobotStatus), py::call_guard<py::gil_scoped_release>());
   control.def("getActualToolFlangePose", &RTDEControlInterface::getActualToolFlangePose, py::call_guard<py::gil_scoped_release>());
   control.def("setGravity", &RTDEControlInterface::setGravity, py::call_guard<py::gil_scoped_release>());
   control.def("initPeriod", &RTDEControlInterface::initPeriod, py::call_guard<py::gil_scoped_release>());
   control.def("waitPeriod", &RTDEControlInterface::waitPeriod, py::call_guard<py::gil_scoped_release>());
   control.def("getInverseKinematicsHasSolution", &RTDEControlInterface::getInverseKinematicsHasSolution,
               py::arg("x"), py::arg("qnear") = std::vector<double>(),
```

### Comparing `ur_rtde-1.5.6/src/rtde_receive_interface.cpp` & `ur_rtde-1.5.7/src/rtde_receive_interface.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         }
 
 #if defined(__linux__) || defined(__APPLE__)
         // Data not available on socket yet, yield to other threads and sleep before trying to receive data again.
         std::this_thread::yield();
         std::this_thread::sleep_for(std::chrono::microseconds(100));
 #endif
-      }
+      }     
     }
     catch (std::exception& e)
     {
       std::cerr << "RTDEReceiveInterface Exception: " << e.what() << std::endl;
       if (rtde_->isConnected())
         rtde_->disconnect();
       stop_receive_thread = true;
```

### Comparing `ur_rtde-1.5.6/src/script_client.cpp` & `ur_rtde-1.5.7/src/script_client.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/src/urcl/tcp_socket.cpp` & `ur_rtde-1.5.7/src/urcl/tcp_socket.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 2021 SDU - Anders Prier Lindvig anpl@mmmi.sdu.dk (refactor)
+ * Copyright 2023, SDU - Anders Prier Lindvig anpl@mmmi.sdu.dk (refactor)
  *
  * Copyright 2019, FZI Forschungszentrum Informatik (refactor)
  *
  * Copyright 2017, 2018 Jarek Potiuk (low bandwidth trajectory follower)
  *
  * Copyright 2017, 2018 Simon Rasmussen (refactor)
  *
@@ -19,109 +19,104 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include <arpa/inet.h>
+#include <endian.h>
 #include <netinet/tcp.h>
 #include <unistd.h>
-#include <urcl/tcp_socket.h>
-
 #include <cstring>
-#include <iostream>
+#include <sstream>
+#include <thread>
+
+#include <urcl/log.h>
+#include <urcl/tcp_socket.h>
 
 namespace urcl
 {
 namespace comm
 {
-TCPSocket::TCPSocket(bool verbose) : verbose_(verbose), socket_fd_(-1), state_(SocketState::Invalid)
+TCPSocket::TCPSocket() : socket_fd_(-1), state_(SocketState::Invalid), reconnection_time_(std::chrono::seconds(10))
 {
 }
 TCPSocket::~TCPSocket()
 {
   close();
 }
 
 void TCPSocket::setOptions(int socket_fd)
 {
   int flag = 1;
   setsockopt(socket_fd, IPPROTO_TCP, TCP_NODELAY, &flag, sizeof(int));
-#if defined(__linux) || defined(linux) || defined(__linux__)
   setsockopt(socket_fd, IPPROTO_TCP, TCP_QUICKACK, &flag, sizeof(int));
-#endif
+
   if (recv_timeout_ != nullptr)
   {
     setsockopt(socket_fd, SOL_SOCKET, SO_RCVTIMEO, recv_timeout_.get(), sizeof(timeval));
   }
 }
 
 bool TCPSocket::setup(std::string& host, int port)
 {
   if (state_ == SocketState::Connected)
     return false;
 
-  if (verbose_)
-    std::cout << "Setting up connection: " << host.c_str() << ":" << port << std::endl;
+  UR_RTDE_LOG_DEBUG("Setting up connection: %s:%d", host.c_str(), port);
 
   // gethostbyname() is deprecated so use getadderinfo() as described in:
-  // http://www.beej.us/guide/bgnet/output/html/multipage/syscalls.html#getaddrinfo
+  // https://beej.us/guide/bgnet/html/#getaddrinfoprepare-to-launch
 
   const char* host_name = host.empty() ? nullptr : host.c_str();
   std::string service = std::to_string(port);
   struct addrinfo hints, *result;
   std::memset(&hints, 0, sizeof(hints));
 
   hints.ai_family = AF_UNSPEC;
   hints.ai_socktype = SOCK_STREAM;
   hints.ai_flags = AI_PASSIVE;
 
-  if (getaddrinfo(host_name, service.c_str(), &hints, &result) != 0)
-  {
-    std::cerr << "Failed to get address for " << host.c_str() << ":" << port << std::endl;
-    return false;
-  }
-
   bool connected = false;
-  // loop through the list of addresses untill we find one that's connectable
-  for (struct addrinfo* p = result; p != nullptr; p = p->ai_next)
+  while (!connected)
   {
-    socket_fd_ = ::socket(p->ai_family, p->ai_socktype, p->ai_protocol);
-
-    if (socket_fd_ != -1 && open(socket_fd_, p->ai_addr, p->ai_addrlen))
+    if (getaddrinfo(host_name, service.c_str(), &hints, &result) != 0)
     {
-      connected = true;
-      break;
+      UR_RTDE_LOG_ERROR("Failed to get address for %s:%d", host.c_str(), port);
+      return false;
+    }
+    // loop through the list of addresses untill we find one that's connectable
+    for (struct addrinfo* p = result; p != nullptr; p = p->ai_next)
+    {
+      socket_fd_ = ::socket(p->ai_family, p->ai_socktype, p->ai_protocol);
+
+      if (socket_fd_ != -1 && open(socket_fd_, p->ai_addr, p->ai_addrlen))
+      {
+        connected = true;
+        break;
+      }
     }
-  }
 
-  freeaddrinfo(result);
+    freeaddrinfo(result);
 
-  if (!connected)
-  {
-    state_ = SocketState::Invalid;
-    std::cerr << "Connection setup failed for " << host.c_str() << ":" << port << std::endl;
-  }
-  else
-  {
-    setOptions(socket_fd_);
-    state_ = SocketState::Connected;
-    if (verbose_)
-      std::cout << "Connection established for " << host.c_str() << ":" << port << std::endl;
+    if (!connected)
+    {
+      state_ = SocketState::Invalid;
+      std::stringstream ss;
+      ss << "Failed to connect to robot on IP " << host_name
+         << ". Please check that the robot is booted and reachable on " << host_name << ". Retrying in "
+         << reconnection_time_.count() << " seconds";
+      UR_RTDE_LOG_ERROR("%s", ss.str().c_str());
+      std::this_thread::sleep_for(reconnection_time_);
+    }
   }
-  return connected;
-}
-
-bool TCPSocket::setSocketFD(int socket_fd)
-{
-  if (state_ == SocketState::Connected)
-    return false;
-  socket_fd_ = socket_fd;
+  setOptions(socket_fd_);
   state_ = SocketState::Connected;
-  return true;
+  UR_RTDE_LOG_DEBUG("Connection established for %s:%d", host.c_str(), port);
+  return connected;
 }
 
 void TCPSocket::close()
 {
   if (socket_fd_ >= 0)
   {
     state_ = SocketState::Closed;
@@ -134,15 +129,15 @@
 {
   sockaddr_in name;
   socklen_t len = sizeof(name);
   int res = ::getsockname(socket_fd_, (sockaddr*)&name, &len);
 
   if (res < 0)
   {
-    std::cerr << "Could not get local IP" << std::endl;
+    UR_RTDE_LOG_ERROR("Could not get local IP");
     return std::string();
   }
 
   char buf[128];
   inet_ntop(AF_INET, &name.sin_addr, buf, sizeof(buf));
   return std::string(buf);
 }
@@ -179,28 +174,28 @@
 
 bool TCPSocket::write(const uint8_t* buf, const size_t buf_len, size_t& written)
 {
   written = 0;
 
   if (state_ != SocketState::Connected)
   {
-    std::cerr << "Attempt to write on a non-connected socket" << std::endl;
+    UR_RTDE_LOG_ERROR("Attempt to write on a non-connected socket");
     return false;
   }
 
   size_t remaining = buf_len;
 
   // handle partial sends
   while (written < buf_len)
   {
     ssize_t sent = ::send(socket_fd_, buf + written, remaining, 0);
 
     if (sent <= 0)
     {
-      std::cerr << "Sending data through socket failed." << std::endl;
+      UR_RTDE_LOG_ERROR("Sending data through socket failed.");
       return false;
     }
 
     written += sent;
     remaining -= sent;
   }
```

### Comparing `ur_rtde-1.5.6/test/doctest.h` & `ur_rtde-1.5.7/test/doctest.h`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/test/main.cpp` & `ur_rtde-1.5.7/test/main.cpp`

 * *Files identical despite different names*

### Comparing `ur_rtde-1.5.6/ur_rtde.egg-info/PKG-INFO` & `ur_rtde-1.5.7/ur_rtde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ur-rtde
-Version: 1.5.6
+Version: 1.5.7
 Summary: A Python interface for controlling and receiving data from a UR robot using the Real-Time Data Exchange (RTDE) interface of the robot. 
 Home-page: https://gitlab.com/sdurobotics/ur_rtde
 Author: Anders Prier Lindvig
 Author-email: anpl@mmmi.sdu.dk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ur_rtde-1.5.6/ur_rtde.egg-info/SOURCES.txt` & `ur_rtde-1.5.7/ur_rtde.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 doc/api/api.rst
 doc/examples/examples.rst
 doc/faq/faq.rst
 doc/guides/guides.rst
 doc/installation/installation.rst
 doc/introduction/introduction.rst
 examples/cpp/CMakeLists.txt
+examples/cpp/contact_detection_example.cpp
 examples/cpp/forcemode_example.cpp
 examples/cpp/io_example.cpp
 examples/cpp/jog_example.cpp
 examples/cpp/move_async_example.cpp
 examples/cpp/move_path_async_example.cpp
 examples/cpp/move_until_contact.cpp
 examples/cpp/movej_path_with_blend_example.cpp
@@ -103,29 +104,34 @@
 include/ur_rtde/rtde_control_interface_doc.h
 include/ur_rtde/rtde_io_interface.h
 include/ur_rtde/rtde_io_interface_doc.h
 include/ur_rtde/rtde_receive_interface.h
 include/ur_rtde/rtde_receive_interface_doc.h
 include/ur_rtde/rtde_utility.h
 include/ur_rtde/script_client.h
+include/urcl/default_log_handler.h
+include/urcl/log.h
 include/urcl/script_sender.h
-include/urcl/server.h
+include/urcl/tcp_server.h
 include/urcl/tcp_socket.h
 scripts/rtde_control.script
 src/dashboard_client.cpp
 src/dashboard_enums.cpp
 src/robot_state.cpp
 src/robotiq_gripper.cpp
 src/rtde.cpp
 src/rtde_control_interface.cpp
 src/rtde_io_interface.cpp
 src/rtde_python_bindings.cpp
 src/rtde_receive_interface.cpp
 src/script_client.cpp
-src/urcl/server.cpp
+src/urcl/default_log_handler.cpp
+src/urcl/log.cpp
+src/urcl/script_sender.cpp
+src/urcl/tcp_server.cpp
 src/urcl/tcp_socket.cpp
 test/CMakeLists.txt
 test/doctest.h
 test/main.cpp
 ur_rtde.egg-info/PKG-INFO
 ur_rtde.egg-info/SOURCES.txt
 ur_rtde.egg-info/dependency_links.txt
```

