# Comparing `tmp/simevopy-0.1.1.tar.gz` & `tmp/simevopy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simevopy-0.1.1.tar", last modified: Thu May 16 17:21:06 2024, max compression
+gzip compressed data, was "simevopy-0.1.2.tar", last modified: Thu May 16 19:02:30 2024, max compression
```

## Comparing `simevopy-0.1.1.tar` & `simevopy-0.1.2.tar`

### file list

```diff
@@ -1,109 +1,57 @@
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.269194 simevopy-0.1.1/
--rw-r--r--   0 yjack      (501) staff       (20)      195 2024-05-16 13:29:37.000000 simevopy-0.1.1/.clang-format
--rw-r--r--   0 yjack      (501) staff       (20)      318 2024-05-16 16:43:54.000000 simevopy-0.1.1/.clangd
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.245175 simevopy-0.1.1/.github/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.248265 simevopy-0.1.1/.github/workflows/
--rw-r--r--   0 yjack      (501) staff       (20)     1504 2024-05-16 15:38:02.000000 simevopy-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 yjack      (501) staff       (20)       37 2024-05-16 16:58:00.000000 simevopy-0.1.1/.gitignore
--rw-r--r--   0 yjack      (501) staff       (20)      686 2024-05-16 16:42:22.000000 simevopy-0.1.1/CMakeLists.txt
--rw-r--r--   0 yjack      (501) staff       (20)     9354 2024-05-16 17:21:06.268904 simevopy-0.1.1/PKG-INFO
--rw-r--r--   0 yjack      (501) staff       (20)     9110 2024-05-16 15:57:16.000000 simevopy-0.1.1/README.md
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.245308 simevopy-0.1.1/_skbuild/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.245362 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.245867 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.245668 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.251328 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/
--rw-r--r--   0 yjack      (501) staff       (20)    87851 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock-actions.h
--rw-r--r--   0 yjack      (501) staff       (20)     6102 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock-cardinalities.h
--rw-r--r--   0 yjack      (501) staff       (20)    25450 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock-function-mocker.h
--rw-r--r--   0 yjack      (501) staff       (20)   209838 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock-matchers.h
--rw-r--r--   0 yjack      (501) staff       (20)    38299 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock-more-actions.h
--rw-r--r--   0 yjack      (501) staff       (20)     4416 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock-more-matchers.h
--rw-r--r--   0 yjack      (501) staff       (20)    10840 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock-nice-strict.h
--rw-r--r--   0 yjack      (501) staff       (20)    79815 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock-spec-builders.h
--rw-r--r--   0 yjack      (501) staff       (20)     3723 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/gmock.h
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.251935 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.252845 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/custom/
--rw-r--r--   0 yjack      (501) staff       (20)      510 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/custom/README.md
--rw-r--r--   0 yjack      (501) staff       (20)      314 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/custom/gmock-generated-actions.h
--rw-r--r--   0 yjack      (501) staff       (20)     1918 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/custom/gmock-matchers.h
--rw-r--r--   0 yjack      (501) staff       (20)     1953 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/custom/gmock-port.h
--rw-r--r--   0 yjack      (501) staff       (20)    18576 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/gmock-internal-utils.h
--rw-r--r--   0 yjack      (501) staff       (20)     6064 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/gmock-port.h
--rw-r--r--   0 yjack      (501) staff       (20)    13491 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gmock/internal/gmock-pp.h
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.256180 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/
--rw-r--r--   0 yjack      (501) staff       (20)     8502 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-assertion-result.h
--rw-r--r--   0 yjack      (501) staff       (20)    14886 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-death-test.h
--rw-r--r--   0 yjack      (501) staff       (20)    33614 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-matchers.h
--rw-r--r--   0 yjack      (501) staff       (20)     8109 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-message.h
--rw-r--r--   0 yjack      (501) staff       (20)    23926 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-param-test.h
--rw-r--r--   0 yjack      (501) staff       (20)    36840 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-printers.h
--rw-r--r--   0 yjack      (501) staff       (20)    12824 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-spi.h
--rw-r--r--   0 yjack      (501) staff       (20)     7111 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-test-part.h
--rw-r--r--   0 yjack      (501) staff       (20)    15921 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest-typed-test.h
--rw-r--r--   0 yjack      (501) staff       (20)    90156 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest.h
--rw-r--r--   0 yjack      (501) staff       (20)    12783 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest_pred_impl.h
--rw-r--r--   0 yjack      (501) staff       (20)     2502 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/gtest_prod.h
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.259090 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.260143 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/custom/
--rw-r--r--   0 yjack      (501) staff       (20)     1269 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/custom/README.md
--rw-r--r--   0 yjack      (501) staff       (20)     1873 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/custom/gtest-port.h
--rw-r--r--   0 yjack      (501) staff       (20)     2094 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/custom/gtest-printers.h
--rw-r--r--   0 yjack      (501) staff       (20)     1858 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/custom/gtest.h
--rw-r--r--   0 yjack      (501) staff       (20)    13916 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/gtest-death-test-internal.h
--rw-r--r--   0 yjack      (501) staff       (20)    10220 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/gtest-filepath.h
--rw-r--r--   0 yjack      (501) staff       (20)    63753 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/gtest-internal.h
--rw-r--r--   0 yjack      (501) staff       (20)    38054 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/gtest-param-util.h
--rw-r--r--   0 yjack      (501) staff       (20)     4178 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/gtest-port-arch.h
--rw-r--r--   0 yjack      (501) staff       (20)    87997 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/gtest-port.h
--rw-r--r--   0 yjack      (501) staff       (20)     7301 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/gtest-string.h
--rw-r--r--   0 yjack      (501) staff       (20)     6247 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/include/gtest/internal/gtest-type-util.h
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.261927 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.246034 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/cmake/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.262695 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/cmake/GTest/
--rw-r--r--   0 yjack      (501) staff       (20)     1073 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/cmake/GTest/GTestConfig.cmake
--rw-r--r--   0 yjack      (501) staff       (20)     1978 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/cmake/GTest/GTestConfigVersion.cmake
--rw-r--r--   0 yjack      (501) staff       (20)     2260 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/cmake/GTest/GTestTargets-release.cmake
--rw-r--r--   0 yjack      (501) staff       (20)     5330 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/cmake/GTest/GTestTargets.cmake
--rw-r--r--   0 yjack      (501) staff       (20)   126576 2024-05-16 17:21:06.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/libgmock.a
--rw-r--r--   0 yjack      (501) staff       (20)     5056 2024-05-16 17:21:06.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/libgmock_main.a
--rw-r--r--   0 yjack      (501) staff       (20)   637704 2024-05-16 17:21:06.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/libgtest.a
--rw-r--r--   0 yjack      (501) staff       (20)     1336 2024-05-16 17:21:06.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/libgtest_main.a
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.263381 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/pkgconfig/
--rw-r--r--   0 yjack      (501) staff       (20)      393 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/pkgconfig/gmock.pc
--rw-r--r--   0 yjack      (501) staff       (20)      400 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/pkgconfig/gmock_main.pc
--rw-r--r--   0 yjack      (501) staff       (20)      368 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/pkgconfig/gtest.pc
--rw-r--r--   0 yjack      (501) staff       (20)      400 2024-05-16 16:52:35.000000 simevopy-0.1.1/_skbuild/macosx-14.0-arm64-3.9/cmake-install/lib/pkgconfig/gtest_main.pc
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.263669 simevopy-0.1.1/examples/
--rw-r--r--   0 yjack      (501) staff       (20)        0 2024-05-16 15:57:10.000000 simevopy-0.1.1/examples/size_awareness.py
--rw-r--r--   0 yjack      (501) staff       (20)      667 2024-05-16 15:57:10.000000 simevopy-0.1.1/examples/speed_food.py
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.246458 simevopy-0.1.1/include/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.264668 simevopy-0.1.1/include/core/
--rw-r--r--   0 yjack      (501) staff       (20)      595 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/core/Environment.hpp
--rw-r--r--   0 yjack      (501) staff       (20)      143 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/core/Food.hpp
--rw-r--r--   0 yjack      (501) staff       (20)      435 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/core/Genes.hpp
--rw-r--r--   0 yjack      (501) staff       (20)      617 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/core/Organism.hpp
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.265552 simevopy-0.1.1/include/index/
--rw-r--r--   0 yjack      (501) staff       (20)      435 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/index/ISpatialIndex.hpp
--rw-r--r--   0 yjack      (501) staff       (20)      208 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/index/ISpatialObject.hpp
--rw-r--r--   0 yjack      (501) staff       (20)     1108 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/index/SpatialIndex.hpp
--rw-r--r--   0 yjack      (501) staff       (20)      521 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/index/SpatialObjectWrapper.hpp
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.266087 simevopy-0.1.1/include/test/
--rw-r--r--   0 yjack      (501) staff       (20)      119 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/test/Dummy.hpp
--rw-r--r--   0 yjack      (501) staff       (20)      684 2024-05-16 15:57:11.000000 simevopy-0.1.1/include/test/SpatialIndexTest.hpp
--rw-r--r--   0 yjack      (501) staff       (20)       38 2024-05-16 17:21:06.269243 simevopy-0.1.1/setup.cfg
--rw-r--r--   0 yjack      (501) staff       (20)      527 2024-05-16 17:19:51.000000 simevopy-0.1.1/setup.py
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.268593 simevopy-0.1.1/simevopy.egg-info/
--rw-r--r--   0 yjack      (501) staff       (20)     9354 2024-05-16 17:21:06.000000 simevopy-0.1.1/simevopy.egg-info/PKG-INFO
--rw-r--r--   0 yjack      (501) staff       (20)     4859 2024-05-16 17:21:06.000000 simevopy-0.1.1/simevopy.egg-info/SOURCES.txt
--rw-r--r--   0 yjack      (501) staff       (20)        1 2024-05-16 17:21:06.000000 simevopy-0.1.1/simevopy.egg-info/dependency_links.txt
--rw-r--r--   0 yjack      (501) staff       (20)        1 2024-05-16 17:16:58.000000 simevopy-0.1.1/simevopy.egg-info/not-zip-safe
--rw-r--r--   0 yjack      (501) staff       (20)        1 2024-05-16 17:21:06.000000 simevopy-0.1.1/simevopy.egg-info/top_level.txt
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.246708 simevopy-0.1.1/src/
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.267747 simevopy-0.1.1/src/core/
--rw-r--r--   0 yjack      (501) staff       (20)     1027 2024-05-16 15:57:12.000000 simevopy-0.1.1/src/core/Environment.cpp
--rw-r--r--   0 yjack      (501) staff       (20)      600 2024-05-16 15:57:12.000000 simevopy-0.1.1/src/core/Genes.cpp
--rw-r--r--   0 yjack      (501) staff       (20)      640 2024-05-16 15:57:12.000000 simevopy-0.1.1/src/core/Organism.cpp
-drwxr-xr-x   0 yjack      (501) staff       (20)        0 2024-05-16 17:21:06.268242 simevopy-0.1.1/src/index/
--rw-r--r--   0 yjack      (501) staff       (20)      683 2024-05-16 15:57:12.000000 simevopy-0.1.1/src/index/DefaultSpatialIndex.cpp
--rw-r--r--   0 yjack      (501) staff       (20)     2155 2024-05-16 15:57:12.000000 simevopy-0.1.1/src/index/OptimizedSpatialIndex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.765354 simevopy-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 19:02:15.000000 simevopy-0.1.2/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 19:02:15.000000 simevopy-0.1.2/.clangd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.757354 simevopy-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-16 19:02:15.000000 simevopy-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 19:02:15.000000 simevopy-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-16 19:02:15.000000 simevopy-0.1.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 19:02:15.000000 simevopy-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-05-16 19:02:30.765354 simevopy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-05-16 19:02:15.000000 simevopy-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-16 19:02:15.000000 simevopy-0.1.2/bindings/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/bindings/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-16 19:02:15.000000 simevopy-0.1.2/bindings/core/genes_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-16 19:02:15.000000 simevopy-0.1.2/bindings/core/organism_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 19:02:15.000000 simevopy-0.1.2/bindings/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 19:02:15.000000 simevopy-0.1.2/bindings/python_bindings.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      853 2024-05-16 19:02:15.000000 simevopy-0.1.2/bump_version.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:15.000000 simevopy-0.1.2/examples/size_awareness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 19:02:15.000000 simevopy-0.1.2/examples/speed_food.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.757354 simevopy-0.1.2/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/include/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/core/Environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/core/Food.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/core/Genes.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/core/Organism.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/include/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/index/ISpatialIndex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/index/ISpatialObject.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/index/SpatialIndex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/index/SpatialObjectWrapper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/include/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/test/Dummy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-16 19:02:15.000000 simevopy-0.1.2/include/test/SpatialIndexTest.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:02:30.765354 simevopy-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-16 19:02:30.000000 simevopy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/simevopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-05-16 19:02:30.000000 simevopy-0.1.2/simevopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 19:02:30.000000 simevopy-0.1.2/simevopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:02:30.000000 simevopy-0.1.2/simevopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:02:30.000000 simevopy-0.1.2/simevopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.761354 simevopy-0.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-16 19:02:15.000000 simevopy-0.1.2/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.765354 simevopy-0.1.2/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-16 19:02:15.000000 simevopy-0.1.2/src/core/Environment.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 19:02:15.000000 simevopy-0.1.2/src/core/Genes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 19:02:15.000000 simevopy-0.1.2/src/core/Organism.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.765354 simevopy-0.1.2/src/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-16 19:02:15.000000 simevopy-0.1.2/src/index/DefaultSpatialIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-16 19:02:15.000000 simevopy-0.1.2/src/index/OptimizedSpatialIndex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.757354 simevopy-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:02:30.765354 simevopy-0.1.2/tests/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-16 19:02:15.000000 simevopy-0.1.2/tests/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-16 19:02:15.000000 simevopy-0.1.2/tests/cpp/SpatialIndexTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-16 19:02:15.000000 simevopy-0.1.2/tests/cpp/gtest.cmake
```

### Comparing `simevopy-0.1.1/CMakeLists.txt` & `simevopy-0.1.2/CMakeLists.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 cmake_minimum_required(VERSION 3.24)
 project(SimEvo)
 
+set(CMAKE_POSITION_INDEPENDENT_CODE ON)
+
 # check if the compiler supports C++20
 include(CheckCXXCompilerFlag)
 check_cxx_compiler_flag("-std=c++20" COMPILER_SUPPORTS_CXX20)
 
 if(COMPILER_SUPPORTS_CXX20)
   set(CMAKE_CXX_STANDARD 20)
   set(CMAKE_CXX_STANDARD_REQUIRED True)
@@ -14,15 +16,20 @@
 endif()
 
 # include the headers
 include_directories(include)
 
 # add the subdirectories
 add_subdirectory(src)
-add_subdirectory(bindings)
 
-## using BUILD_TESTS to enable/disable the tests
+# using BUILD_BINDINGS to enable/disable the python bindings
+option(BUILD_BINDINGS "Build Python bindings" ON)
+if(BUILD_BINDINGS)
+  add_subdirectory(bindings)
+endif()
+
+# using BUILD_TESTS to enable/disable the tests
 option(BUILD_TESTS "Build the test programs" ON)
 if(BUILD_TESTS)
   enable_testing()
   add_subdirectory(tests/cpp)
 endif()
```

### Comparing `simevopy-0.1.1/PKG-INFO` & `simevopy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: simevopy
-Version: 0.1.1
+Version: 0.1.2
 Summary: SimEvo Python bindings
 Home-page: https://github.com/YJack0000/SimEvo
 Author: YJack0000
 Author-email: yjack0000.cs12@nycu.edu.tw
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 SimEvo: A Simple Python Library for Simulations of Natural Selection
 ---
 
 ## Basic Information
 
 > **Project Overview:** Simulating Natural Selection in Ecosystems using C++ and Python
@@ -164,7 +166,9 @@
 - Create documentation and update example scripts.
 
 Week 7 (5/20):
 - Prepare for the paper presentation.
 
 Week 8 (5/27):
 - Designate as flexible time for any overflow tasks or final adjustments.
+
+
```

### Comparing `simevopy-0.1.1/README.md` & `simevopy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/examples/speed_food.py` & `simevopy-0.1.2/examples/speed_food.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/include/core/Environment.hpp` & `simevopy-0.1.2/include/core/Environment.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/include/core/Organism.hpp` & `simevopy-0.1.2/include/core/Organism.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/include/index/SpatialIndex.hpp` & `simevopy-0.1.2/include/index/SpatialIndex.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/include/index/SpatialObjectWrapper.hpp` & `simevopy-0.1.2/include/index/SpatialObjectWrapper.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/include/test/SpatialIndexTest.hpp` & `simevopy-0.1.2/include/test/SpatialIndexTest.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/setup.py` & `simevopy-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="simevopy",
-    version="0.1.1",
+    version='0.1.2',
     description="SimEvo Python bindings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     cmake_source_dir=".",
     url='https://github.com/YJack0000/SimEvo',
     author='YJack0000',
```

### Comparing `simevopy-0.1.1/simevopy.egg-info/PKG-INFO` & `simevopy-0.1.2/simevopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: simevopy
-Version: 0.1.1
+Version: 0.1.2
 Summary: SimEvo Python bindings
 Home-page: https://github.com/YJack0000/SimEvo
 Author: YJack0000
 Author-email: yjack0000.cs12@nycu.edu.tw
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 SimEvo: A Simple Python Library for Simulations of Natural Selection
 ---
 
 ## Basic Information
 
 > **Project Overview:** Simulating Natural Selection in Ecosystems using C++ and Python
@@ -164,7 +166,9 @@
 - Create documentation and update example scripts.
 
 Week 7 (5/20):
 - Prepare for the paper presentation.
 
 Week 8 (5/27):
 - Designate as flexible time for any overflow tasks or final adjustments.
+
+
```

### Comparing `simevopy-0.1.1/src/core/Environment.cpp` & `simevopy-0.1.2/src/core/Environment.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/src/core/Genes.cpp` & `simevopy-0.1.2/src/core/Genes.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #include <core/Genes.hpp>
+#include <cstring>
+#include <ctime>
 #include <cstdlib>
 
 Genes::Genes(const char *dnaStr, MutationFunction customMutationLogic = nullptr)
     : mutationLogic(customMutationLogic ? customMutationLogic
                                         : defaultMutationLogic) {
     std::memcpy(dna, dnaStr, 4);
 }
```

### Comparing `simevopy-0.1.1/src/core/Organism.cpp` & `simevopy-0.1.2/src/core/Organism.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/src/index/DefaultSpatialIndex.cpp` & `simevopy-0.1.2/src/index/DefaultSpatialIndex.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.1/src/index/OptimizedSpatialIndex.cpp` & `simevopy-0.1.2/src/index/OptimizedSpatialIndex.cpp`

 * *Files identical despite different names*

