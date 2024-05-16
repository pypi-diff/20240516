# Comparing `tmp/pyecm-0.0.1.tar.gz` & `tmp/pyecm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecm-0.0.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyecm-0.0.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyecm-0.0.1.tar` & `pyecm-0.0.2.tar`

### file list

```diff
@@ -1,372 +1,373 @@
--rw-r--r--   0        0        0     1304 2022-11-09 12:37:21.000000 pyecm-0.0.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 pyecm-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 pyecm-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 pyecm-0.0.1/.gitignore
--rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 pyecm-0.0.1/.gitmodules
--rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 pyecm-0.0.1/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     3732 2022-11-09 12:37:21.000000 pyecm-0.0.1/CMakeLists.txt
--rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 pyecm-0.0.1/Dockerfile.dev
--rw-r--r--   0        0        0     1063 2022-11-09 12:37:21.000000 pyecm-0.0.1/LICENSE
--rw-r--r--   0        0        0      972 2022-11-09 12:37:21.000000 pyecm-0.0.1/README.md
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 pyecm-0.0.1/example.py
--rw-r--r--   0        0        0       36 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/.git
--rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/.gitattributes
--rw-r--r--   0        0        0      716 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/.github/workflows/build.yml
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/.gitignore
--rw-r--r--   0        0        0     3765 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/CMakeLists.txt
--rw-r--r--   0        0        0     3954 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/ChangeLog
--rw-r--r--   0        0        0    79469 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/Doxyfile
--rw-r--r--   0        0        0     1740 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/LICENSE
--rw-r--r--   0        0        0     1133 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/README.md
--rw-r--r--   0        0        0      329 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/cmake/Modules/Platform/rt-kernel-C.cmake
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/cmake/Modules/Platform/rt-kernel-gcc-bfin.cmake
--rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/cmake/Modules/Platform/rt-kernel-gcc-kinetis.cmake
--rw-r--r--   0        0        0      556 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/cmake/Modules/Platform/rt-kernel-gcc.cmake
--rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/cmake/Modules/Platform/rt-kernel.cmake
--rw-r--r--   0        0        0      583 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/cmake/Modules/Platform/rtems.cmake
--rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/cmake/Toolchains/rt-kernel-bfin.cmake
--rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/cmake/Toolchains/rt-kernel-kinetis.cmake
--rw-r--r--   0        0        0    25053 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/doc/images/legacy_iomap.png
--rw-r--r--   0        0        0    14665 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/doc/images/memory_layout.png
--rw-r--r--   0        0        0    28169 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/doc/images/overlapping_iomap.png
--rw-r--r--   0        0        0     7890 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/doc/soem.dox
--rw-r--r--   0        0        0    15550 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/doc/tutorial.txt
--rw-r--r--   0        0        0      142 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/drvcomment.txt
--rw-r--r--   0        0        0     2473 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/erika/osal.c
--rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/erika/osal_defs.h
--rw-r--r--   0        0        0     2071 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/intime/osal.c
--rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/intime/osal_defs.h
--rw-r--r--   0        0        0     3610 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/linux/osal.c
--rw-r--r--   0        0        0      649 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/linux/osal_defs.h
--rw-r--r--   0        0        0     3578 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/macosx/osal.c
--rw-r--r--   0        0        0      649 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/macosx/osal_defs.h
--rw-r--r--   0        0        0     1473 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/osal.h
--rw-r--r--   0        0        0     3578 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/rtems/osal.c
--rw-r--r--   0        0        0      649 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/rtems/osal_defs.h
--rw-r--r--   0        0        0     3946 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/rtk/osal.c
--rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/rtk/osal_defs.h
--rw-r--r--   0        0        0     5615 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/vxworks/osal.c
--rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/vxworks/osal_defs.h
--rw-r--r--   0        0        0     7995 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/win32/inttypes.h
--rw-r--r--   0        0        0     3902 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/win32/osal.c
--rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/win32/osal_defs.h
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/win32/osal_win32.h
--rw-r--r--   0        0        0     7719 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/osal/win32/stdint.h
--rw-r--r--   0        0        0    18697 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/erika/nicdrv.c
--rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/erika/nicdrv.h
--rw-r--r--   0        0        0     1811 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/erika/oshw.c
--rw-r--r--   0        0        0      556 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/erika/oshw.h
--rw-r--r--   0        0        0    22518 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/intime/nicdrv.c
--rw-r--r--   0        0        0     3168 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/intime/nicdrv.h
--rw-r--r--   0        0        0     1096 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/intime/oshw.c
--rw-r--r--   0        0        0      553 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/intime/oshw.h
--rw-r--r--   0        0        0    20915 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/linux/nicdrv.c
--rw-r--r--   0        0        0     3067 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/linux/nicdrv.h
--rw-r--r--   0        0        0     2791 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/linux/oshw.c
--rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/linux/oshw.h
--rw-r--r--   0        0        0    20209 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/macosx/nicdrv.c
--rw-r--r--   0        0        0     3072 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/macosx/nicdrv.h
--rw-r--r--   0        0        0     2774 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/macosx/oshw.c
--rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/macosx/oshw.h
--rw-r--r--   0        0        0    21720 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtems/nicdrv.c
--rw-r--r--   0        0        0     3067 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtems/nicdrv.h
--rw-r--r--   0        0        0     2773 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtems/oshw.c
--rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtems/oshw.h
--rw-r--r--   0        0        0    25509 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtk/fec/fec_ecat.c
--rw-r--r--   0        0        0     1701 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtk/fec/fec_ecat.h
--rw-r--r--   0        0        0    15762 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtk/lw_mac/lw_emac.c
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtk/lw_mac/lw_emac.h
--rw-r--r--   0        0        0    19556 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtk/nicdrv.c
--rw-r--r--   0        0        0     2966 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtk/nicdrv.h
--rw-r--r--   0        0        0     1209 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtk/oshw.c
--rw-r--r--   0        0        0      559 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/rtk/oshw.h
--rw-r--r--   0        0        0    29615 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/vxworks/nicdrv.c
--rw-r--r--   0        0        0     3456 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/vxworks/nicdrv.h
--rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/vxworks/oshw.c
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/vxworks/oshw.h
--rw-r--r--   0        0        0    20408 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/nicdrv.c
--rw-r--r--   0        0        0     3113 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/nicdrv.h
--rw-r--r--   0        0        0     2931 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/oshw.c
--rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/oshw.h
--rw-r--r--   0        0        0    16556 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/Packet32.h
--rw-r--r--   0        0        0     3914 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/Win32-Extensions.h
--rw-r--r--   0        0        0     3925 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/bittypes.h
--rw-r--r--   0        0        0     5756 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/ip6_misc.h
--rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/bluetooth.h
--rw-r--r--   0        0        0    29101 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/bpf.h
--rw-r--r--   0        0        0     3421 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/namedb.h
--rw-r--r--   0        0        0    14057 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/pcap.h
--rw-r--r--   0        0        0     5567 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/sll.h
--rw-r--r--   0        0        0     2921 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/usb.h
--rw-r--r--   0        0        0     2155 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/vlan.h
--rw-r--r--   0        0        0     2392 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap-bpf.h
--rw-r--r--   0        0        0     2125 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap-namedb.h
--rw-r--r--   0        0        0     2865 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap-stdinc.h
--rw-r--r--   0        0        0     2320 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap.h
--rw-r--r--   0        0        0    14450 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/remote-ext.h
--rw-r--r--   0        0        0     8450 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/Packet.lib
--rw-r--r--   0        0        0    20814 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/libpacket.a
--rw-r--r--   0        0        0    54276 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/libwpcap.a
--rw-r--r--   0        0        0    19320 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/wpcap.lib
--rw-r--r--   0        0        0     8290 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/x64/Packet.lib
--rw-r--r--   0        0        0    18892 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/x64/wpcap.lib
--rw-r--r--   0        0        0      570 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercat.h
--rw-r--r--   0        0        0    21826 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatbase.c
--rw-r--r--   0        0        0     3424 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatbase.h
--rw-r--r--   0        0        0    56499 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatcoe.c
--rw-r--r--   0        0        0     3752 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatcoe.h
--rw-r--r--   0        0        0    64858 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatconfig.c
--rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatconfig.h
--rw-r--r--   0        0        0     5717 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatconfiglist.h
--rw-r--r--   0        0        0    15651 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatdc.c
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatdc.h
--rw-r--r--   0        0        0    20334 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercateoe.c
--rw-r--r--   0        0        0     6797 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercateoe.h
--rw-r--r--   0        0        0    13056 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatfoe.c
--rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatfoe.h
--rw-r--r--   0        0        0    76429 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatmain.c
--rw-r--r--   0        0        0    17346 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatmain.h
--rw-r--r--   0        0        0    13275 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatprint.c
--rw-r--r--   0        0        0      669 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatprint.h
--rw-r--r--   0        0        0    13811 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatsoe.c
--rw-r--r--   0        0        0     3460 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercatsoe.h
--rw-r--r--   0        0        0    16115 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/soem/ethercattype.h
--rw-r--r--   0        0        0    14144 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/intime/ec_master/ec_master.c
--rw-r--r--   0        0        0    12340 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/aliastool.c
--rw-r--r--   0        0        0    11074 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/ebox/ebox.c
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/eepromtool/CMakeLists.txt
--rw-r--r--   0        0        0    13684 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/eepromtool/eepromtool.c
--rw-r--r--   0        0        0    13109 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/eoe_test/eoe_test.c
--rw-r--r--   0        0        0     4679 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/firm_update/firm_update.c
--rw-r--r--   0        0        0    10691 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/red_test/red_test.c
--rw-r--r--   0        0        0      152 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/simple_test/CMakeLists.txt
--rw-r--r--   0        0        0     8425 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/simple_test/simple_test.c
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/slaveinfo/CMakeLists.txt
--rw-r--r--   0        0        0    25211 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/linux/slaveinfo/slaveinfo.c
--rw-r--r--   0        0        0    15726 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/rtk/main.c
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/rtk/schedule.tt
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/simple_ng/CMakeLists.txt
--rw-r--r--   0        0        0     9847 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/simple_ng/simple_ng.c
--rw-r--r--   0        0        0    11137 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/win32/ebox/ebox.c
--rw-r--r--   0        0        0    11254 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/win32/eepromtool/eepromtool.c
--rw-r--r--   0        0        0     4567 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/win32/firm_update/firm_update.c
--rw-r--r--   0        0        0     7383 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/win32/red_test/red_test.c
--rw-r--r--   0        0        0    12410 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/win32/simple_test/simple_test.c
--rw-r--r--   0        0        0    22856 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/SOEM/test/win32/slaveinfo/slaveinfo.c
--rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/.git
--rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/.github/ISSUE_TEMPLATE/all-other.yml
--rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1724 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/.github/workflows/ci.yml
--rw-r--r--   0        0        0      490 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/.gitignore
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/.gitmodules
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/.readthedocs.yaml
--rw-r--r--   0        0        0     5341 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/CMakeLists.txt
--rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/LICENSE
--rw-r--r--   0        0        0     2972 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/README.md
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/cmake/collect-symbols-pypy.py
--rw-r--r--   0        0        0     1386 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/cmake/collect-symbols.py
--rw-r--r--   0        0        0    21656 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/cmake/darwin-ld-cpython.sym
--rw-r--r--   0        0        0    24687 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/cmake/darwin-ld-pypy.sym
--rw-r--r--   0        0        0    14995 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/cmake/nanobind-config.cmake
--rw-r--r--   0        0        0    19418 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/api_cmake.rst
--rw-r--r--   0        0        0   105744 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/api_core.rst
--rw-r--r--   0        0        0    48244 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/api_extra.rst
--rw-r--r--   0        0        0    14897 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/basics.rst
--rw-r--r--   0        0        0     7853 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/benchmark.rst
--rw-r--r--   0        0        0     4515 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/building.rst
--rw-r--r--   0        0        0    54431 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/changelog.rst
--rw-r--r--   0        0        0    34488 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/classes.rst
--rw-r--r--   0        0        0     8130 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/conf.py
--rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/cppyy.h
--rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/eigen.rst
--rw-r--r--   0        0        0    10941 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/exceptions.rst
--rw-r--r--   0        0        0    13969 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/exchanging.rst
--rw-r--r--   0        0        0    16796 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/faq.rst
--rw-r--r--   0        0        0    17459 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/functions.rst
--rw-r--r--   0        0        0    20461 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/binding-dark.svg
--rw-r--r--   0        0        0    20183 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/binding-light.svg
--rw-r--r--   0        0        0    18165 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/caster-dark.svg
--rw-r--r--   0        0        0    17829 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/caster-light.svg
--rw-r--r--   0        0        0   426666 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/logo.jpg
--rw-r--r--   0        0        0    56614 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/perf.svg
--rw-r--r--   0        0        0    53541 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/sizes.svg
--rw-r--r--   0        0        0    52665 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/times.svg
--rw-r--r--   0        0        0    14221 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/wrapper-dark.svg
--rw-r--r--   0        0        0    13943 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/images/wrapper-light.svg
--rw-r--r--   0        0        0     3445 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/index.rst
--rw-r--r--   0        0        0     1565 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/installing.rst
--rw-r--r--   0        0        0    11200 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/lowlevel.rst
--rw-r--r--   0        0        0    17077 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/microbenchmark.ipynb
--rw-r--r--   0        0        0    21588 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/ndarray.rst
--rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/ndarray_index.rst
--rw-r--r--   0        0        0    15750 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/ownership.rst
--rw-r--r--   0        0        0    17463 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/ownership_adv.rst
--rw-r--r--   0        0        0    12130 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/packaging.rst
--rw-r--r--   0        0        0    14481 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/porting.rst
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/pypy.rst
--rw-r--r--   0        0        0      700 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/release.rst
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/requirements.txt
--rw-r--r--   0        0        0     7114 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/typeslots.rst
--rw-r--r--   0        0        0    23602 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/typing.rst
--rw-r--r--   0        0        0     1671 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/utilities.rst
--rw-r--r--   0        0        0    11854 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/docs/why.rst
--rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/.clang-format
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/.codecov.yml
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/.git
--rw-r--r--   0        0        0     4725 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3397 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/CMakeLists.txt
--rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/LICENSE
--rw-r--r--   0        0        0    23256 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/README.md
--rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/cmake/tsl-robin-mapConfig.cmake.in
--rw-r--r--   0        0        0   108206 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/doxygen.conf
--rw-r--r--   0        0        0    12181 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/include/tsl/robin_growth_policy.h
--rw-r--r--   0        0        0    54606 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/include/tsl/robin_hash.h
--rw-r--r--   0        0        0    28770 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/include/tsl/robin_map.h
--rw-r--r--   0        0        0    23947 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/include/tsl/robin_set.h
--rw-r--r--   0        0        0     1141 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/CMakeLists.txt
--rw-r--r--   0        0        0     3875 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/custom_allocator_tests.cpp
--rw-r--r--   0        0        0     1247 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/main.cpp
--rw-r--r--   0        0        0     3351 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/policy_tests.cpp
--rw-r--r--   0        0        0    46146 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/robin_map_tests.cpp
--rw-r--r--   0        0        0     5980 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/robin_set_tests.cpp
--rw-r--r--   0        0        0    12624 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/utils.h
--rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/ext/robin_map/tsl-robin-map.natvis
--rw-r--r--   0        0        0    17958 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/eigen/dense.h
--rw-r--r--   0        0        0     6503 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/eigen/sparse.h
--rw-r--r--   0        0        0     1939 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/eval.h
--rw-r--r--   0        0        0     8884 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/intrusive/counter.h
--rw-r--r--   0        0        0     4874 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/intrusive/counter.inl
--rw-r--r--   0        0        0     4860 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/intrusive/ref.h
--rw-r--r--   0        0        0     6365 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/make_iterator.h
--rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nanobind.h
--rw-r--r--   0        0        0     6228 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_accessor.h
--rw-r--r--   0        0        0    10641 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_attr.h
--rw-r--r--   0        0        0     5472 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_call.h
--rw-r--r--   0        0        0    21039 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_cast.h
--rw-r--r--   0        0        0    27926 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_class.h
--rw-r--r--   0        0        0     6837 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_defs.h
--rw-r--r--   0        0        0     5130 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_descr.h
--rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_enums.h
--rw-r--r--   0        0        0     5207 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_error.h
--rw-r--r--   0        0        0    15280 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_func.h
--rw-r--r--   0        0        0    21889 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_lib.h
--rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_misc.h
--rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_python.h
--rw-r--r--   0        0        0     8923 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_traits.h
--rw-r--r--   0        0        0     2468 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_tuple.h
--rw-r--r--   0        0        0    29717 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/nb_types.h
--rw-r--r--   0        0        0    20407 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/ndarray.h
--rw-r--r--   0        0        0     7449 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/operators.h
--rw-r--r--   0        0        0      535 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/array.h
--rw-r--r--   0        0        0     5924 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/bind_map.h
--rw-r--r--   0        0        0     7384 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/bind_vector.h
--rw-r--r--   0        0        0     8673 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/chrono.h
--rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/complex.h
--rw-r--r--   0        0        0    10571 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/chrono.h
--rw-r--r--   0        0        0     1859 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/nb_array.h
--rw-r--r--   0        0        0     2961 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/nb_dict.h
--rw-r--r--   0        0        0     2308 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/nb_list.h
--rw-r--r--   0        0        0     2125 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/nb_set.h
--rw-r--r--   0        0        0     3219 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/traits.h
--rw-r--r--   0        0        0     2884 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/filesystem.h
--rw-r--r--   0        0        0     2488 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/function.h
--rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/list.h
--rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/map.h
--rw-r--r--   0        0        0     2084 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/optional.h
--rw-r--r--   0        0        0     2772 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/pair.h
--rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/set.h
--rw-r--r--   0        0        0     4820 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/shared_ptr.h
--rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/string.h
--rw-r--r--   0        0        0     1062 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/string_view.h
--rw-r--r--   0        0        0     3304 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/tuple.h
--rw-r--r--   0        0        0     4389 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/unique_ptr.h
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/unordered_map.h
--rw-r--r--   0        0        0      652 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/unordered_set.h
--rw-r--r--   0        0        0     2750 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/variant.h
--rw-r--r--   0        0        0      537 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/stl/vector.h
--rw-r--r--   0        0        0     2975 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/trampoline.h
--rw-r--r--   0        0        0      753 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/include/nanobind/typing.h
--rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/pyproject.toml
--rw-r--r--   0        0        0     3225 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/setup.py
--rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/__init__.py
--rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/__main__.py
--rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/buffer.h
--rw-r--r--   0        0        0    31127 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/common.cpp
--rw-r--r--   0        0        0     8851 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/error.cpp
--rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/hash.h
--rw-r--r--   0        0        0     2350 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/implicit.cpp
--rw-r--r--   0        0        0     3908 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/nb_combined.cpp
--rw-r--r--   0        0        0     6947 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/nb_enum.cpp
--rw-r--r--   0        0        0    47578 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/nb_func.cpp
--rw-r--r--   0        0        0    16440 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/nb_internals.cpp
--rw-r--r--   0        0        0    11159 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/nb_internals.h
--rw-r--r--   0        0        0    24227 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/nb_ndarray.cpp
--rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/nb_static_property.cpp
--rw-r--r--   0        0        0    62105 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/nb_type.cpp
--rwxr-xr-x   0        0        0    50599 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/stubgen.py
--rw-r--r--   0        0        0     5144 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/src/trampoline.cpp
--rw-r--r--   0        0        0     4803 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/CMakeLists.txt
--rw-r--r--   0        0        0      484 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/common.py
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/inter_module.cpp
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/inter_module.h
--rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/object_py.h
--rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/pattern_file.nb
--rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/py_stub_test.py
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/py_stub_test.pyi
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/py_stub_test.pyi.ref
--rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_chrono.cpp
--rw-r--r--   0        0        0    10852 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_chrono.py
--rw-r--r--   0        0        0    20146 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_classes.cpp
--rw-r--r--   0        0        0    22086 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_classes.py
--rw-r--r--   0        0        0     6254 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_classes_ext.pyi.ref
--rw-r--r--   0        0        0     9576 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_eigen.cpp
--rw-r--r--   0        0        0    12097 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_eigen.py
--rw-r--r--   0        0        0     1492 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_enum.cpp
--rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_enum.py
--rw-r--r--   0        0        0      831 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_enum_ext.pyi.ref
--rw-r--r--   0        0        0     2342 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_eval.cpp
--rw-r--r--   0        0        0      893 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_eval.py
--rw-r--r--   0        0        0     2579 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_exception.cpp
--rw-r--r--   0        0        0     3301 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_exception.py
--rw-r--r--   0        0        0    12057 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_functions.cpp
--rw-r--r--   0        0        0    16239 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_functions.py
--rw-r--r--   0        0        0     4301 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_functions_ext.pyi.ref
--rw-r--r--   0        0        0     9373 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_holders.cpp
--rw-r--r--   0        0        0    11149 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_holders.py
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_inter_module.py
--rw-r--r--   0        0        0      170 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_inter_module_1.cpp
--rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_inter_module_2.cpp
--rw-r--r--   0        0        0     1884 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_intrusive.cpp
--rw-r--r--   0        0        0     1281 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_intrusive.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_intrusive_impl.cpp
--rw-r--r--   0        0        0     1845 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_issue.cpp
--rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_issue.py
--rw-r--r--   0        0        0     3526 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_make_iterator.cpp
--rw-r--r--   0        0        0     1036 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_make_iterator.py
--rw-r--r--   0        0        0      698 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_make_iterator_ext.pyi.ref
--rw-r--r--   0        0        0    11983 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_ndarray.cpp
--rw-r--r--   0        0        0    20060 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_ndarray.py
--rw-r--r--   0        0        0     5158 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_ndarray_ext.pyi.ref
--rw-r--r--   0        0        0    15951 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_stl.cpp
--rw-r--r--   0        0        0    23123 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_stl.py
--rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_stl_bind_map.cpp
--rw-r--r--   0        0        0     4076 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_stl_bind_map.py
--rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_stl_bind_vector.cpp
--rw-r--r--   0        0        0     4288 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_stl_bind_vector.py
--rw-r--r--   0        0        0     6239 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_stl_ext.pyi.ref
--rw-r--r--   0        0        0     1842 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_stubs.py
--rw-r--r--   0        0        0     3353 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_typing.cpp
--rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_typing.py
--rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyecm-0.0.1/ext/nanobind/tests/test_typing_ext.pyi.ref
--rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 pyecm-0.0.1/pyecm/__init__.py
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 pyecm-0.0.1/pyecm/soem/__init__.py
--rw-r--r--   0        0        0    13467 2022-11-09 12:37:21.000000 pyecm-0.0.1/pyecm/soem/soem_ext.pyi
--rw-r--r--   0        0        0    12210 2022-11-09 12:37:21.000000 pyecm-0.0.1/pyecm/soem_ext.cpp
--rw-r--r--   0        0        0     1289 2022-11-09 12:37:21.000000 pyecm-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pyecm-0.0.1/requirements.dev
--rw-r--r--   0        0        0     5772 2022-11-09 12:37:21.000000 pyecm-0.0.1/tests/environments/basic/test_basic_env.py
--rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 pyecm-0.0.1/tests/test_ethercatmain.py
--rw-r--r--   0        0        0      370 2022-11-09 12:37:21.000000 pyecm-0.0.1/tests/test_ethercattype.py
--rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 pyecm-0.0.1/tests/test_init.py
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 pyecm-0.0.1/tests/test_soem_add.py
--rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 pyecm-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1407 2022-11-09 12:37:21.000000 pyecm-0.0.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 pyecm-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2249 2022-11-09 12:37:21.000000 pyecm-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 pyecm-0.0.2/.gitignore
+-rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 pyecm-0.0.2/.gitmodules
+-rw-r--r--   0        0        0     2333 2022-11-09 12:37:21.000000 pyecm-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0     3227 2022-11-09 12:37:21.000000 pyecm-0.0.2/CMakeLists.txt
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 pyecm-0.0.2/Dockerfile.dev
+-rw-r--r--   0        0        0     1063 2022-11-09 12:37:21.000000 pyecm-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2836 2022-11-09 12:37:21.000000 pyecm-0.0.2/README.md
+-rw-r--r--   0        0        0     8435 2022-11-09 12:37:21.000000 pyecm-0.0.2/examples/soem/simple_test.py
+-rw-r--r--   0        0        0       36 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/.git
+-rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/.gitattributes
+-rw-r--r--   0        0        0      716 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/.github/workflows/build.yml
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/.gitignore
+-rw-r--r--   0        0        0     3765 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/CMakeLists.txt
+-rw-r--r--   0        0        0     3954 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/ChangeLog
+-rw-r--r--   0        0        0    79469 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/Doxyfile
+-rw-r--r--   0        0        0     1740 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/LICENSE
+-rw-r--r--   0        0        0     1133 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/README.md
+-rw-r--r--   0        0        0      329 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/cmake/Modules/Platform/rt-kernel-C.cmake
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/cmake/Modules/Platform/rt-kernel-gcc-bfin.cmake
+-rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/cmake/Modules/Platform/rt-kernel-gcc-kinetis.cmake
+-rw-r--r--   0        0        0      556 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/cmake/Modules/Platform/rt-kernel-gcc.cmake
+-rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/cmake/Modules/Platform/rt-kernel.cmake
+-rw-r--r--   0        0        0      583 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/cmake/Modules/Platform/rtems.cmake
+-rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/cmake/Toolchains/rt-kernel-bfin.cmake
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/cmake/Toolchains/rt-kernel-kinetis.cmake
+-rw-r--r--   0        0        0    25053 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/doc/images/legacy_iomap.png
+-rw-r--r--   0        0        0    14665 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/doc/images/memory_layout.png
+-rw-r--r--   0        0        0    28169 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/doc/images/overlapping_iomap.png
+-rw-r--r--   0        0        0     7890 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/doc/soem.dox
+-rw-r--r--   0        0        0    15550 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/doc/tutorial.txt
+-rw-r--r--   0        0        0      142 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/drvcomment.txt
+-rw-r--r--   0        0        0     2473 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/erika/osal.c
+-rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/erika/osal_defs.h
+-rw-r--r--   0        0        0     2071 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/intime/osal.c
+-rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/intime/osal_defs.h
+-rw-r--r--   0        0        0     3610 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/linux/osal.c
+-rw-r--r--   0        0        0      649 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/linux/osal_defs.h
+-rw-r--r--   0        0        0     3578 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/macosx/osal.c
+-rw-r--r--   0        0        0      649 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/macosx/osal_defs.h
+-rw-r--r--   0        0        0     1473 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/osal.h
+-rw-r--r--   0        0        0     3578 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/rtems/osal.c
+-rw-r--r--   0        0        0      649 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/rtems/osal_defs.h
+-rw-r--r--   0        0        0     3946 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/rtk/osal.c
+-rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/rtk/osal_defs.h
+-rw-r--r--   0        0        0     5615 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/vxworks/osal.c
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/vxworks/osal_defs.h
+-rw-r--r--   0        0        0     7995 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/win32/inttypes.h
+-rw-r--r--   0        0        0     3902 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/win32/osal.c
+-rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/win32/osal_defs.h
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/win32/osal_win32.h
+-rw-r--r--   0        0        0     7719 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/osal/win32/stdint.h
+-rw-r--r--   0        0        0    18697 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/erika/nicdrv.c
+-rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/erika/nicdrv.h
+-rw-r--r--   0        0        0     1811 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/erika/oshw.c
+-rw-r--r--   0        0        0      556 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/erika/oshw.h
+-rw-r--r--   0        0        0    22518 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/intime/nicdrv.c
+-rw-r--r--   0        0        0     3168 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/intime/nicdrv.h
+-rw-r--r--   0        0        0     1096 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/intime/oshw.c
+-rw-r--r--   0        0        0      553 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/intime/oshw.h
+-rw-r--r--   0        0        0    20915 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/linux/nicdrv.c
+-rw-r--r--   0        0        0     3067 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/linux/nicdrv.h
+-rw-r--r--   0        0        0     2791 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/linux/oshw.c
+-rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/linux/oshw.h
+-rw-r--r--   0        0        0    20209 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/macosx/nicdrv.c
+-rw-r--r--   0        0        0     3072 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/macosx/nicdrv.h
+-rw-r--r--   0        0        0     2774 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/macosx/oshw.c
+-rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/macosx/oshw.h
+-rw-r--r--   0        0        0    21720 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtems/nicdrv.c
+-rw-r--r--   0        0        0     3067 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtems/nicdrv.h
+-rw-r--r--   0        0        0     2773 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtems/oshw.c
+-rw-r--r--   0        0        0      557 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtems/oshw.h
+-rw-r--r--   0        0        0    25509 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtk/fec/fec_ecat.c
+-rw-r--r--   0        0        0     1701 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtk/fec/fec_ecat.h
+-rw-r--r--   0        0        0    15762 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtk/lw_mac/lw_emac.c
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtk/lw_mac/lw_emac.h
+-rw-r--r--   0        0        0    19556 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtk/nicdrv.c
+-rw-r--r--   0        0        0     2966 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtk/nicdrv.h
+-rw-r--r--   0        0        0     1209 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtk/oshw.c
+-rw-r--r--   0        0        0      559 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/rtk/oshw.h
+-rw-r--r--   0        0        0    29615 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/vxworks/nicdrv.c
+-rw-r--r--   0        0        0     3456 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/vxworks/nicdrv.h
+-rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/vxworks/oshw.c
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/vxworks/oshw.h
+-rw-r--r--   0        0        0    20408 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/nicdrv.c
+-rw-r--r--   0        0        0     3113 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/nicdrv.h
+-rw-r--r--   0        0        0     2931 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/oshw.c
+-rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/oshw.h
+-rw-r--r--   0        0        0    16556 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/Packet32.h
+-rw-r--r--   0        0        0     3914 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/Win32-Extensions.h
+-rw-r--r--   0        0        0     3925 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/bittypes.h
+-rw-r--r--   0        0        0     5756 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/ip6_misc.h
+-rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/bluetooth.h
+-rw-r--r--   0        0        0    29101 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/bpf.h
+-rw-r--r--   0        0        0     3421 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/namedb.h
+-rw-r--r--   0        0        0    14057 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/pcap.h
+-rw-r--r--   0        0        0     5567 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/sll.h
+-rw-r--r--   0        0        0     2921 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/usb.h
+-rw-r--r--   0        0        0     2155 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/vlan.h
+-rw-r--r--   0        0        0     2392 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap-bpf.h
+-rw-r--r--   0        0        0     2125 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap-namedb.h
+-rw-r--r--   0        0        0     2865 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap-stdinc.h
+-rw-r--r--   0        0        0     2320 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap.h
+-rw-r--r--   0        0        0    14450 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/remote-ext.h
+-rw-r--r--   0        0        0     8450 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/Packet.lib
+-rw-r--r--   0        0        0    20814 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/libpacket.a
+-rw-r--r--   0        0        0    54276 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/libwpcap.a
+-rw-r--r--   0        0        0    19320 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/wpcap.lib
+-rw-r--r--   0        0        0     8290 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/x64/Packet.lib
+-rw-r--r--   0        0        0    18892 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/x64/wpcap.lib
+-rw-r--r--   0        0        0      570 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercat.h
+-rw-r--r--   0        0        0    21826 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatbase.c
+-rw-r--r--   0        0        0     3424 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatbase.h
+-rw-r--r--   0        0        0    56499 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatcoe.c
+-rw-r--r--   0        0        0     3752 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatcoe.h
+-rw-r--r--   0        0        0    64858 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatconfig.c
+-rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatconfig.h
+-rw-r--r--   0        0        0     5717 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatconfiglist.h
+-rw-r--r--   0        0        0    15651 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatdc.c
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatdc.h
+-rw-r--r--   0        0        0    20334 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercateoe.c
+-rw-r--r--   0        0        0     6797 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercateoe.h
+-rw-r--r--   0        0        0    13056 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatfoe.c
+-rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatfoe.h
+-rw-r--r--   0        0        0    76429 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatmain.c
+-rw-r--r--   0        0        0    17346 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatmain.h
+-rw-r--r--   0        0        0    13275 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatprint.c
+-rw-r--r--   0        0        0      669 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatprint.h
+-rw-r--r--   0        0        0    13811 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatsoe.c
+-rw-r--r--   0        0        0     3460 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercatsoe.h
+-rw-r--r--   0        0        0    16115 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/soem/ethercattype.h
+-rw-r--r--   0        0        0    14144 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/intime/ec_master/ec_master.c
+-rw-r--r--   0        0        0    12340 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/aliastool.c
+-rw-r--r--   0        0        0    11074 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/ebox/ebox.c
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/eepromtool/CMakeLists.txt
+-rw-r--r--   0        0        0    13684 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/eepromtool/eepromtool.c
+-rw-r--r--   0        0        0    13109 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/eoe_test/eoe_test.c
+-rw-r--r--   0        0        0     4679 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/firm_update/firm_update.c
+-rw-r--r--   0        0        0    10691 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/red_test/red_test.c
+-rw-r--r--   0        0        0      152 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/simple_test/CMakeLists.txt
+-rw-r--r--   0        0        0     8425 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/simple_test/simple_test.c
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/slaveinfo/CMakeLists.txt
+-rw-r--r--   0        0        0    25211 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/linux/slaveinfo/slaveinfo.c
+-rw-r--r--   0        0        0    15726 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/rtk/main.c
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/rtk/schedule.tt
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/simple_ng/CMakeLists.txt
+-rw-r--r--   0        0        0     9847 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/simple_ng/simple_ng.c
+-rw-r--r--   0        0        0    11137 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/win32/ebox/ebox.c
+-rw-r--r--   0        0        0    11254 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/win32/eepromtool/eepromtool.c
+-rw-r--r--   0        0        0     4567 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/win32/firm_update/firm_update.c
+-rw-r--r--   0        0        0     7383 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/win32/red_test/red_test.c
+-rw-r--r--   0        0        0    12410 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/win32/simple_test/simple_test.c
+-rw-r--r--   0        0        0    22856 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/SOEM/test/win32/slaveinfo/slaveinfo.c
+-rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/.git
+-rw-r--r--   0        0        0      927 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/.github/ISSUE_TEMPLATE/all-other.yml
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1724 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      490 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/.gitignore
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/.gitmodules
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/.readthedocs.yaml
+-rw-r--r--   0        0        0     5341 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/LICENSE
+-rw-r--r--   0        0        0     2972 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/README.md
+-rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/cmake/collect-symbols-pypy.py
+-rw-r--r--   0        0        0     1386 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/cmake/collect-symbols.py
+-rw-r--r--   0        0        0    21656 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/cmake/darwin-ld-cpython.sym
+-rw-r--r--   0        0        0    24687 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/cmake/darwin-ld-pypy.sym
+-rw-r--r--   0        0        0    14995 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/cmake/nanobind-config.cmake
+-rw-r--r--   0        0        0    19418 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/api_cmake.rst
+-rw-r--r--   0        0        0   105744 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/api_core.rst
+-rw-r--r--   0        0        0    48244 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/api_extra.rst
+-rw-r--r--   0        0        0    14897 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/basics.rst
+-rw-r--r--   0        0        0     7853 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/benchmark.rst
+-rw-r--r--   0        0        0     4515 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/building.rst
+-rw-r--r--   0        0        0    54431 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/changelog.rst
+-rw-r--r--   0        0        0    34488 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/classes.rst
+-rw-r--r--   0        0        0     8130 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/conf.py
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/cppyy.h
+-rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/eigen.rst
+-rw-r--r--   0        0        0    10941 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/exceptions.rst
+-rw-r--r--   0        0        0    13969 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/exchanging.rst
+-rw-r--r--   0        0        0    16796 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/faq.rst
+-rw-r--r--   0        0        0    17459 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/functions.rst
+-rw-r--r--   0        0        0    20461 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/binding-dark.svg
+-rw-r--r--   0        0        0    20183 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/binding-light.svg
+-rw-r--r--   0        0        0    18165 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/caster-dark.svg
+-rw-r--r--   0        0        0    17829 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/caster-light.svg
+-rw-r--r--   0        0        0   426666 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/logo.jpg
+-rw-r--r--   0        0        0    56614 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/perf.svg
+-rw-r--r--   0        0        0    53541 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/sizes.svg
+-rw-r--r--   0        0        0    52665 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/times.svg
+-rw-r--r--   0        0        0    14221 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/wrapper-dark.svg
+-rw-r--r--   0        0        0    13943 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/images/wrapper-light.svg
+-rw-r--r--   0        0        0     3445 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/index.rst
+-rw-r--r--   0        0        0     1565 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/installing.rst
+-rw-r--r--   0        0        0    11200 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/lowlevel.rst
+-rw-r--r--   0        0        0    17077 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/microbenchmark.ipynb
+-rw-r--r--   0        0        0    21588 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/ndarray.rst
+-rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/ndarray_index.rst
+-rw-r--r--   0        0        0    15750 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/ownership.rst
+-rw-r--r--   0        0        0    17463 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/ownership_adv.rst
+-rw-r--r--   0        0        0    12130 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/packaging.rst
+-rw-r--r--   0        0        0    14481 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/porting.rst
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/pypy.rst
+-rw-r--r--   0        0        0      700 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/release.rst
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/requirements.txt
+-rw-r--r--   0        0        0     7114 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/typeslots.rst
+-rw-r--r--   0        0        0    23602 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/typing.rst
+-rw-r--r--   0        0        0     1671 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/utilities.rst
+-rw-r--r--   0        0        0    11854 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/docs/why.rst
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/.clang-format
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/.codecov.yml
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/.git
+-rw-r--r--   0        0        0     4725 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3397 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/CMakeLists.txt
+-rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/LICENSE
+-rw-r--r--   0        0        0    23256 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/README.md
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/cmake/tsl-robin-mapConfig.cmake.in
+-rw-r--r--   0        0        0   108206 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/doxygen.conf
+-rw-r--r--   0        0        0    12181 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/include/tsl/robin_growth_policy.h
+-rw-r--r--   0        0        0    54606 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/include/tsl/robin_hash.h
+-rw-r--r--   0        0        0    28770 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/include/tsl/robin_map.h
+-rw-r--r--   0        0        0    23947 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/include/tsl/robin_set.h
+-rw-r--r--   0        0        0     1141 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     3875 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/custom_allocator_tests.cpp
+-rw-r--r--   0        0        0     1247 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/main.cpp
+-rw-r--r--   0        0        0     3351 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/policy_tests.cpp
+-rw-r--r--   0        0        0    46146 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/robin_map_tests.cpp
+-rw-r--r--   0        0        0     5980 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/robin_set_tests.cpp
+-rw-r--r--   0        0        0    12624 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/utils.h
+-rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/ext/robin_map/tsl-robin-map.natvis
+-rw-r--r--   0        0        0    17958 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/eigen/dense.h
+-rw-r--r--   0        0        0     6503 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/eigen/sparse.h
+-rw-r--r--   0        0        0     1939 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/eval.h
+-rw-r--r--   0        0        0     8884 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/intrusive/counter.h
+-rw-r--r--   0        0        0     4874 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/intrusive/counter.inl
+-rw-r--r--   0        0        0     4860 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/intrusive/ref.h
+-rw-r--r--   0        0        0     6365 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/make_iterator.h
+-rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nanobind.h
+-rw-r--r--   0        0        0     6228 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_accessor.h
+-rw-r--r--   0        0        0    10641 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_attr.h
+-rw-r--r--   0        0        0     5472 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_call.h
+-rw-r--r--   0        0        0    21039 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_cast.h
+-rw-r--r--   0        0        0    27926 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_class.h
+-rw-r--r--   0        0        0     6837 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_defs.h
+-rw-r--r--   0        0        0     5130 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_descr.h
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_enums.h
+-rw-r--r--   0        0        0     5207 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_error.h
+-rw-r--r--   0        0        0    15280 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_func.h
+-rw-r--r--   0        0        0    21889 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_lib.h
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_misc.h
+-rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_python.h
+-rw-r--r--   0        0        0     8923 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_traits.h
+-rw-r--r--   0        0        0     2468 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_tuple.h
+-rw-r--r--   0        0        0    29717 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/nb_types.h
+-rw-r--r--   0        0        0    20407 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/ndarray.h
+-rw-r--r--   0        0        0     7449 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/operators.h
+-rw-r--r--   0        0        0      535 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/array.h
+-rw-r--r--   0        0        0     5924 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/bind_map.h
+-rw-r--r--   0        0        0     7384 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/bind_vector.h
+-rw-r--r--   0        0        0     8673 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/chrono.h
+-rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/complex.h
+-rw-r--r--   0        0        0    10571 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/chrono.h
+-rw-r--r--   0        0        0     1859 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/nb_array.h
+-rw-r--r--   0        0        0     2961 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/nb_dict.h
+-rw-r--r--   0        0        0     2308 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/nb_list.h
+-rw-r--r--   0        0        0     2125 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/nb_set.h
+-rw-r--r--   0        0        0     3219 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/traits.h
+-rw-r--r--   0        0        0     2884 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/filesystem.h
+-rw-r--r--   0        0        0     2488 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/function.h
+-rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/list.h
+-rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/map.h
+-rw-r--r--   0        0        0     2084 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/optional.h
+-rw-r--r--   0        0        0     2772 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/pair.h
+-rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/set.h
+-rw-r--r--   0        0        0     4820 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/shared_ptr.h
+-rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/string.h
+-rw-r--r--   0        0        0     1062 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/string_view.h
+-rw-r--r--   0        0        0     3304 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/tuple.h
+-rw-r--r--   0        0        0     4389 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/unique_ptr.h
+-rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/unordered_map.h
+-rw-r--r--   0        0        0      652 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/unordered_set.h
+-rw-r--r--   0        0        0     2750 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/variant.h
+-rw-r--r--   0        0        0      537 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/stl/vector.h
+-rw-r--r--   0        0        0     2975 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/trampoline.h
+-rw-r--r--   0        0        0      753 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/include/nanobind/typing.h
+-rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/pyproject.toml
+-rw-r--r--   0        0        0     3225 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/setup.py
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/__init__.py
+-rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/__main__.py
+-rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/buffer.h
+-rw-r--r--   0        0        0    31127 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/common.cpp
+-rw-r--r--   0        0        0     8851 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/error.cpp
+-rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/hash.h
+-rw-r--r--   0        0        0     2350 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/implicit.cpp
+-rw-r--r--   0        0        0     3908 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/nb_combined.cpp
+-rw-r--r--   0        0        0     6947 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/nb_enum.cpp
+-rw-r--r--   0        0        0    47578 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/nb_func.cpp
+-rw-r--r--   0        0        0    16440 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/nb_internals.cpp
+-rw-r--r--   0        0        0    11159 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/nb_internals.h
+-rw-r--r--   0        0        0    24227 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/nb_ndarray.cpp
+-rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/nb_static_property.cpp
+-rw-r--r--   0        0        0    62105 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/nb_type.cpp
+-rwxr-xr-x   0        0        0    50599 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/stubgen.py
+-rw-r--r--   0        0        0     5144 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/src/trampoline.cpp
+-rw-r--r--   0        0        0     4803 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      484 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/common.py
+-rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/inter_module.cpp
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/inter_module.h
+-rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/object_py.h
+-rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/pattern_file.nb
+-rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/py_stub_test.py
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/py_stub_test.pyi
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/py_stub_test.pyi.ref
+-rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_chrono.cpp
+-rw-r--r--   0        0        0    10852 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_chrono.py
+-rw-r--r--   0        0        0    20146 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_classes.cpp
+-rw-r--r--   0        0        0    22086 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_classes.py
+-rw-r--r--   0        0        0     6254 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_classes_ext.pyi.ref
+-rw-r--r--   0        0        0     9576 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_eigen.cpp
+-rw-r--r--   0        0        0    12097 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_eigen.py
+-rw-r--r--   0        0        0     1492 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_enum.cpp
+-rw-r--r--   0        0        0     4769 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_enum.py
+-rw-r--r--   0        0        0      831 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_enum_ext.pyi.ref
+-rw-r--r--   0        0        0     2342 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_eval.cpp
+-rw-r--r--   0        0        0      893 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_eval.py
+-rw-r--r--   0        0        0     2579 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_exception.cpp
+-rw-r--r--   0        0        0     3301 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_exception.py
+-rw-r--r--   0        0        0    12057 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_functions.cpp
+-rw-r--r--   0        0        0    16239 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_functions.py
+-rw-r--r--   0        0        0     4301 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_functions_ext.pyi.ref
+-rw-r--r--   0        0        0     9373 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_holders.cpp
+-rw-r--r--   0        0        0    11149 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_holders.py
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_inter_module.py
+-rw-r--r--   0        0        0      170 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_inter_module_1.cpp
+-rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_inter_module_2.cpp
+-rw-r--r--   0        0        0     1884 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_intrusive.cpp
+-rw-r--r--   0        0        0     1281 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_intrusive.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_intrusive_impl.cpp
+-rw-r--r--   0        0        0     1845 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_issue.cpp
+-rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_issue.py
+-rw-r--r--   0        0        0     3526 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_make_iterator.cpp
+-rw-r--r--   0        0        0     1036 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_make_iterator.py
+-rw-r--r--   0        0        0      698 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_make_iterator_ext.pyi.ref
+-rw-r--r--   0        0        0    11983 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_ndarray.cpp
+-rw-r--r--   0        0        0    20060 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_ndarray.py
+-rw-r--r--   0        0        0     5158 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_ndarray_ext.pyi.ref
+-rw-r--r--   0        0        0    15951 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_stl.cpp
+-rw-r--r--   0        0        0    23123 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_stl.py
+-rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_stl_bind_map.cpp
+-rw-r--r--   0        0        0     4076 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_stl_bind_map.py
+-rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_stl_bind_vector.cpp
+-rw-r--r--   0        0        0     4288 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_stl_bind_vector.py
+-rw-r--r--   0        0        0     6239 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_stl_ext.pyi.ref
+-rw-r--r--   0        0        0     1842 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_stubs.py
+-rw-r--r--   0        0        0     3353 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_typing.cpp
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_typing.py
+-rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyecm-0.0.2/ext/nanobind/tests/test_typing_ext.pyi.ref
+-rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 pyecm-0.0.2/pyecm/__init__.py
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 pyecm-0.0.2/pyecm/soem/__init__.py
+-rw-r--r--   0        0        0    21082 2022-11-09 12:37:21.000000 pyecm-0.0.2/pyecm/soem/soem_ext.pyi
+-rw-r--r--   0        0        0    19048 2022-11-09 12:37:21.000000 pyecm-0.0.2/pyecm/soem_ext.cpp
+-rw-r--r--   0        0        0     1421 2022-11-09 12:37:21.000000 pyecm-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pyecm-0.0.2/requirements.dev
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 pyecm-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0    16328 2022-11-09 12:37:21.000000 pyecm-0.0.2/tests/environments/basic/test_basic_env.py
+-rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 pyecm-0.0.2/tests/test_ethercatmain.py
+-rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 pyecm-0.0.2/tests/test_ethercattype.py
+-rw-r--r--   0        0        0     6067 2022-11-09 12:37:21.000000 pyecm-0.0.2/tests/test_soem.py
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 pyecm-0.0.2/tests/test_soem_add.py
+-rw-r--r--   0        0        0     3321 2022-11-09 12:37:21.000000 pyecm-0.0.2/PKG-INFO
```

### Comparing `pyecm-0.0.1/.devcontainer/devcontainer.json` & `pyecm-0.0.2/.devcontainer/devcontainer.json`

 * *Files 20% similar despite different names*

```diff
@@ -11,31 +11,28 @@
 	"customizations": {
 		"vscode": {
 			"extensions": [
 				"ms-python.python",
 				"ms-azuretools.vscode-docker",
 				"ms-vscode.cpptools-extension-pack",
 				"tamasfe.even-better-toml",
-				"charliermarsh.ruff"
+				"charliermarsh.ruff",
+				"ms-python.black-formatter",
+				"usernamehw.errorlens"
 			]
-		}
+		},
+		"python.analysis.typeCheckingMode": "standard"
 	},
 	"runArgs": [
 		"--network=host"
 	]
-	
-
 	// Features to add to the dev container. More info: https://containers.dev/features.
 	// "features": {},
-
 	// Use 'forwardPorts' to make a list of ports inside the container available locally.
 	// "forwardPorts": [],
-
 	// Uncomment the next line to run commands after the container is created.
 	// "postCreateCommand": "cat /etc/os-release",
-
 	// Configure tool-specific properties.
 	// "customizations": {},
-
 	// Uncomment to connect as an existing user other than the container default. More info: https://aka.ms/dev-containers-non-root.
 	// "remoteUser": "devcontainer"
-}
+}
```

### Comparing `pyecm-0.0.1/.gitignore` & `pyecm-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/CMakeLists.txt` & `pyecm-0.0.2/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -35,35 +35,20 @@
 find_package(nanobind CONFIG REQUIRED)
 
 # who knows that pos ind code is but this fixes an error:
 # relocation R_X86_64_PC32 against symbol `secMAC' can not be used when making a shared object; recompile with -fPIC
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
 
 
-add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/ext/SOEM) # soem is installed as a submodule
+add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/ext/SOEM EXCLUDE_FROM_ALL) # soem is installed as a submodule
 
-# We are now ready to compile the actual extension module
 nanobind_add_module(
-  # Name of the extension
   soem_ext
-
-  # Target the stable ABI for Python 3.12+, which reduces
-  # the number of binary wheels that must be built. This
-  # does nothing on older Python versions
-  STABLE_ABI
-
-  # Build libnanobind statically and merge it into the
-  # extension (which itself remains a shared library)
-  #
-  # If your project builds multiple extensions, you can
-  # replace this flag by NB_SHARED to conserve space by
-  # reusing a shared libnanobind across libraries
+  STABLE_ABI 
   NB_STATIC
-
-  # Source code goes here
   pyecm/soem_ext.cpp
 )
 target_link_libraries(soem_ext PUBLIC soem)
 
 if(WIN32)
   # Add the directory containing pcap.h to the include directories
   # this is a hack to temporarily fix https://github.com/OpenEtherCATsociety/SOEM/issues/785
@@ -71,24 +56,24 @@
     ${CMAKE_CURRENT_LIST_DIR}/ext/SOEM/oshw/win32/wpcap/Include
   )
   if(CMAKE_SIZEOF_VOID_P EQUAL 8)
     target_link_directories(soem_ext PUBLIC ${CMAKE_CURRENT_LIST_DIR}/ext/SOEM/oshw/win32/wpcap/Lib/x64)
   elseif(CMAKE_SIZEOF_VOID_P EQUAL 4)
     target_link_directories(soem_ext PUBLIC ${CMAKE_CURRENT_LIST_DIR}/ext/SOEM/oshw/win32/wpcap/Lib)
   endif()
-  
 endif()
 
-
 nanobind_add_stub(
   soem_ext_stub
   MODULE soem_ext
   OUTPUT "${CMAKE_SOURCE_DIR}/pyecm/soem/soem_ext.pyi"
-  PYTHON_PATH $<TARGET_FILE_DIR:soem_ext>
+  PYTHON_PATH $<SHELL_PATH:$<TARGET_FILE_DIR:soem_ext>>
   DEPENDS soem_ext
   MARKER_FILE py.typed
+  VERBOSE
 )
 # Install directive for scikit-build-core
 
 install(TARGETS soem_ext LIBRARY DESTINATION "pyecm/soem")
 install(FILES "${CMAKE_SOURCE_DIR}/pyecm/soem/soem_ext.pyi" DESTINATION "pyecm/soem")
-install(FILES "${CMAKE_CURRENT_BINARY_DIR}/py.typed" DESTINATION "pyecm/soem")
+install(FILES "${CMAKE_CURRENT_BINARY_DIR}/py.typed" DESTINATION "pyecm/soem")
+
```

### Comparing `pyecm-0.0.1/LICENSE` & `pyecm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/.github/workflows/build.yml` & `pyecm-0.0.2/ext/SOEM/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/CMakeLists.txt` & `pyecm-0.0.2/ext/SOEM/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/ChangeLog` & `pyecm-0.0.2/ext/SOEM/ChangeLog`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/Doxyfile` & `pyecm-0.0.2/ext/SOEM/Doxyfile`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/LICENSE` & `pyecm-0.0.2/ext/SOEM/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/README.md` & `pyecm-0.0.2/ext/SOEM/README.md`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/cmake/Modules/Platform/rt-kernel-gcc.cmake` & `pyecm-0.0.2/ext/SOEM/cmake/Modules/Platform/rt-kernel-gcc.cmake`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/cmake/Modules/Platform/rtems.cmake` & `pyecm-0.0.2/ext/SOEM/cmake/Modules/Platform/rtems.cmake`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/doc/images/legacy_iomap.png` & `pyecm-0.0.2/ext/SOEM/doc/images/legacy_iomap.png`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/doc/images/memory_layout.png` & `pyecm-0.0.2/ext/SOEM/doc/images/memory_layout.png`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/doc/images/overlapping_iomap.png` & `pyecm-0.0.2/ext/SOEM/doc/images/overlapping_iomap.png`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/doc/soem.dox` & `pyecm-0.0.2/ext/SOEM/doc/soem.dox`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/doc/tutorial.txt` & `pyecm-0.0.2/ext/SOEM/doc/tutorial.txt`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/erika/osal.c` & `pyecm-0.0.2/ext/SOEM/osal/erika/osal.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/erika/osal_defs.h` & `pyecm-0.0.2/ext/SOEM/osal/erika/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/intime/osal.c` & `pyecm-0.0.2/ext/SOEM/osal/intime/osal.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/intime/osal_defs.h` & `pyecm-0.0.2/ext/SOEM/osal/intime/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/linux/osal.c` & `pyecm-0.0.2/ext/SOEM/osal/linux/osal.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/linux/osal_defs.h` & `pyecm-0.0.2/ext/SOEM/osal/linux/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/macosx/osal.c` & `pyecm-0.0.2/ext/SOEM/osal/macosx/osal.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/macosx/osal_defs.h` & `pyecm-0.0.2/ext/SOEM/osal/macosx/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/osal.h` & `pyecm-0.0.2/ext/SOEM/osal/osal.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/rtems/osal.c` & `pyecm-0.0.2/ext/SOEM/osal/rtems/osal.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/rtems/osal_defs.h` & `pyecm-0.0.2/ext/SOEM/osal/rtems/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/rtk/osal.c` & `pyecm-0.0.2/ext/SOEM/osal/rtk/osal.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/rtk/osal_defs.h` & `pyecm-0.0.2/ext/SOEM/osal/rtk/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/vxworks/osal.c` & `pyecm-0.0.2/ext/SOEM/osal/vxworks/osal.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/vxworks/osal_defs.h` & `pyecm-0.0.2/ext/SOEM/osal/vxworks/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/win32/inttypes.h` & `pyecm-0.0.2/ext/SOEM/osal/win32/inttypes.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/win32/osal.c` & `pyecm-0.0.2/ext/SOEM/osal/win32/osal.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/win32/osal_defs.h` & `pyecm-0.0.2/ext/SOEM/osal/win32/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/win32/osal_win32.h` & `pyecm-0.0.2/ext/SOEM/osal/win32/osal_win32.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/osal/win32/stdint.h` & `pyecm-0.0.2/ext/SOEM/osal/win32/stdint.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/erika/nicdrv.c` & `pyecm-0.0.2/ext/SOEM/oshw/erika/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/erika/nicdrv.h` & `pyecm-0.0.2/ext/SOEM/oshw/erika/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/erika/oshw.c` & `pyecm-0.0.2/ext/SOEM/oshw/erika/oshw.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/erika/oshw.h` & `pyecm-0.0.2/ext/SOEM/oshw/erika/oshw.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/intime/nicdrv.c` & `pyecm-0.0.2/ext/SOEM/oshw/intime/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/intime/nicdrv.h` & `pyecm-0.0.2/ext/SOEM/oshw/intime/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/intime/oshw.c` & `pyecm-0.0.2/ext/SOEM/oshw/intime/oshw.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/intime/oshw.h` & `pyecm-0.0.2/ext/SOEM/oshw/intime/oshw.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/linux/nicdrv.c` & `pyecm-0.0.2/ext/SOEM/oshw/linux/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/linux/nicdrv.h` & `pyecm-0.0.2/ext/SOEM/oshw/linux/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/linux/oshw.c` & `pyecm-0.0.2/ext/SOEM/oshw/linux/oshw.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/linux/oshw.h` & `pyecm-0.0.2/ext/SOEM/oshw/linux/oshw.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/macosx/nicdrv.c` & `pyecm-0.0.2/ext/SOEM/oshw/macosx/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/macosx/nicdrv.h` & `pyecm-0.0.2/ext/SOEM/oshw/macosx/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/macosx/oshw.c` & `pyecm-0.0.2/ext/SOEM/oshw/macosx/oshw.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/macosx/oshw.h` & `pyecm-0.0.2/ext/SOEM/oshw/macosx/oshw.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtems/nicdrv.c` & `pyecm-0.0.2/ext/SOEM/oshw/rtems/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtems/nicdrv.h` & `pyecm-0.0.2/ext/SOEM/oshw/rtems/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtems/oshw.c` & `pyecm-0.0.2/ext/SOEM/oshw/rtems/oshw.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtems/oshw.h` & `pyecm-0.0.2/ext/SOEM/oshw/rtems/oshw.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtk/fec/fec_ecat.c` & `pyecm-0.0.2/ext/SOEM/oshw/rtk/fec/fec_ecat.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtk/fec/fec_ecat.h` & `pyecm-0.0.2/ext/SOEM/oshw/rtk/fec/fec_ecat.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtk/lw_mac/lw_emac.c` & `pyecm-0.0.2/ext/SOEM/oshw/rtk/lw_mac/lw_emac.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtk/nicdrv.c` & `pyecm-0.0.2/ext/SOEM/oshw/rtk/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtk/nicdrv.h` & `pyecm-0.0.2/ext/SOEM/oshw/rtk/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtk/oshw.c` & `pyecm-0.0.2/ext/SOEM/oshw/rtk/oshw.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/rtk/oshw.h` & `pyecm-0.0.2/ext/SOEM/oshw/rtk/oshw.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/vxworks/nicdrv.c` & `pyecm-0.0.2/ext/SOEM/oshw/vxworks/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/vxworks/nicdrv.h` & `pyecm-0.0.2/ext/SOEM/oshw/vxworks/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/vxworks/oshw.c` & `pyecm-0.0.2/ext/SOEM/oshw/vxworks/oshw.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/nicdrv.c` & `pyecm-0.0.2/ext/SOEM/oshw/win32/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/nicdrv.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/oshw.c` & `pyecm-0.0.2/ext/SOEM/oshw/win32/oshw.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/oshw.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/oshw.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/Packet32.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/Packet32.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/Win32-Extensions.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/Win32-Extensions.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/bittypes.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/bittypes.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/ip6_misc.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/ip6_misc.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/bluetooth.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/bluetooth.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/bpf.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/bpf.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/namedb.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/namedb.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/pcap.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/pcap.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/sll.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/sll.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/usb.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/usb.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap/vlan.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap/vlan.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap-bpf.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap-bpf.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap-namedb.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap-namedb.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap-stdinc.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap-stdinc.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/pcap.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/pcap.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Include/remote-ext.h` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Include/remote-ext.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/Packet.lib` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/Packet.lib`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/libpacket.a` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/libpacket.a`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/libwpcap.a` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/libwpcap.a`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/wpcap.lib` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/wpcap.lib`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/x64/Packet.lib` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/x64/Packet.lib`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/oshw/win32/wpcap/Lib/x64/wpcap.lib` & `pyecm-0.0.2/ext/SOEM/oshw/win32/wpcap/Lib/x64/wpcap.lib`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercat.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercat.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatbase.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercatbase.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatbase.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatbase.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatcoe.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercatcoe.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatcoe.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatcoe.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatconfig.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercatconfig.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatconfig.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatconfig.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatconfiglist.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatconfiglist.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatdc.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercatdc.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatdc.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatdc.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercateoe.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercateoe.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercateoe.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercateoe.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatfoe.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercatfoe.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatfoe.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatfoe.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatmain.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercatmain.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatmain.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatmain.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatprint.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercatprint.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatprint.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatprint.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatsoe.c` & `pyecm-0.0.2/ext/SOEM/soem/ethercatsoe.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercatsoe.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercatsoe.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/soem/ethercattype.h` & `pyecm-0.0.2/ext/SOEM/soem/ethercattype.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/intime/ec_master/ec_master.c` & `pyecm-0.0.2/ext/SOEM/test/intime/ec_master/ec_master.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/linux/aliastool.c` & `pyecm-0.0.2/ext/SOEM/test/linux/aliastool.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/linux/ebox/ebox.c` & `pyecm-0.0.2/ext/SOEM/test/linux/ebox/ebox.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/linux/eepromtool/eepromtool.c` & `pyecm-0.0.2/ext/SOEM/test/linux/eepromtool/eepromtool.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/linux/eoe_test/eoe_test.c` & `pyecm-0.0.2/ext/SOEM/test/linux/eoe_test/eoe_test.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/linux/firm_update/firm_update.c` & `pyecm-0.0.2/ext/SOEM/test/linux/firm_update/firm_update.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/linux/red_test/red_test.c` & `pyecm-0.0.2/ext/SOEM/test/linux/red_test/red_test.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/linux/simple_test/simple_test.c` & `pyecm-0.0.2/ext/SOEM/test/linux/simple_test/simple_test.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/linux/slaveinfo/slaveinfo.c` & `pyecm-0.0.2/ext/SOEM/test/linux/slaveinfo/slaveinfo.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/rtk/main.c` & `pyecm-0.0.2/ext/SOEM/test/rtk/main.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/simple_ng/simple_ng.c` & `pyecm-0.0.2/ext/SOEM/test/simple_ng/simple_ng.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/win32/ebox/ebox.c` & `pyecm-0.0.2/ext/SOEM/test/win32/ebox/ebox.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/win32/eepromtool/eepromtool.c` & `pyecm-0.0.2/ext/SOEM/test/win32/eepromtool/eepromtool.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/win32/firm_update/firm_update.c` & `pyecm-0.0.2/ext/SOEM/test/win32/firm_update/firm_update.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/win32/red_test/red_test.c` & `pyecm-0.0.2/ext/SOEM/test/win32/red_test/red_test.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/win32/simple_test/simple_test.c` & `pyecm-0.0.2/ext/SOEM/test/win32/simple_test/simple_test.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/SOEM/test/win32/slaveinfo/slaveinfo.c` & `pyecm-0.0.2/ext/SOEM/test/win32/slaveinfo/slaveinfo.c`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/.github/ISSUE_TEMPLATE/all-other.yml` & `pyecm-0.0.2/ext/nanobind/.github/ISSUE_TEMPLATE/all-other.yml`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/.github/ISSUE_TEMPLATE/bug-report.yml` & `pyecm-0.0.2/ext/nanobind/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/.github/workflows/ci.yml` & `pyecm-0.0.2/ext/nanobind/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/CMakeLists.txt` & `pyecm-0.0.2/ext/nanobind/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/LICENSE` & `pyecm-0.0.2/ext/nanobind/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/README.md` & `pyecm-0.0.2/ext/nanobind/README.md`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/cmake/collect-symbols-pypy.py` & `pyecm-0.0.2/ext/nanobind/cmake/collect-symbols-pypy.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/cmake/collect-symbols.py` & `pyecm-0.0.2/ext/nanobind/cmake/collect-symbols.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/cmake/darwin-ld-cpython.sym` & `pyecm-0.0.2/ext/nanobind/cmake/darwin-ld-cpython.sym`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/cmake/darwin-ld-pypy.sym` & `pyecm-0.0.2/ext/nanobind/cmake/darwin-ld-pypy.sym`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/cmake/nanobind-config.cmake` & `pyecm-0.0.2/ext/nanobind/cmake/nanobind-config.cmake`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/api_cmake.rst` & `pyecm-0.0.2/ext/nanobind/docs/api_cmake.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/api_core.rst` & `pyecm-0.0.2/ext/nanobind/docs/api_core.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/api_extra.rst` & `pyecm-0.0.2/ext/nanobind/docs/api_extra.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/basics.rst` & `pyecm-0.0.2/ext/nanobind/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/benchmark.rst` & `pyecm-0.0.2/ext/nanobind/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/building.rst` & `pyecm-0.0.2/ext/nanobind/docs/building.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/changelog.rst` & `pyecm-0.0.2/ext/nanobind/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/classes.rst` & `pyecm-0.0.2/ext/nanobind/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/conf.py` & `pyecm-0.0.2/ext/nanobind/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/eigen.rst` & `pyecm-0.0.2/ext/nanobind/docs/eigen.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/exceptions.rst` & `pyecm-0.0.2/ext/nanobind/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/exchanging.rst` & `pyecm-0.0.2/ext/nanobind/docs/exchanging.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/faq.rst` & `pyecm-0.0.2/ext/nanobind/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/functions.rst` & `pyecm-0.0.2/ext/nanobind/docs/functions.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/binding-dark.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/binding-dark.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/binding-light.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/binding-light.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/caster-dark.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/caster-dark.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/caster-light.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/caster-light.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/logo.jpg` & `pyecm-0.0.2/ext/nanobind/docs/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/perf.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/perf.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/sizes.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/sizes.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/times.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/times.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/wrapper-dark.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/wrapper-dark.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/images/wrapper-light.svg` & `pyecm-0.0.2/ext/nanobind/docs/images/wrapper-light.svg`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/index.rst` & `pyecm-0.0.2/ext/nanobind/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/installing.rst` & `pyecm-0.0.2/ext/nanobind/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/lowlevel.rst` & `pyecm-0.0.2/ext/nanobind/docs/lowlevel.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/microbenchmark.ipynb` & `pyecm-0.0.2/ext/nanobind/docs/microbenchmark.ipynb`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/ndarray.rst` & `pyecm-0.0.2/ext/nanobind/docs/ndarray.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/ownership.rst` & `pyecm-0.0.2/ext/nanobind/docs/ownership.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/ownership_adv.rst` & `pyecm-0.0.2/ext/nanobind/docs/ownership_adv.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/packaging.rst` & `pyecm-0.0.2/ext/nanobind/docs/packaging.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/porting.rst` & `pyecm-0.0.2/ext/nanobind/docs/porting.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/pypy.rst` & `pyecm-0.0.2/ext/nanobind/docs/pypy.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/release.rst` & `pyecm-0.0.2/ext/nanobind/docs/release.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/typeslots.rst` & `pyecm-0.0.2/ext/nanobind/docs/typeslots.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/typing.rst` & `pyecm-0.0.2/ext/nanobind/docs/typing.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/utilities.rst` & `pyecm-0.0.2/ext/nanobind/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/docs/why.rst` & `pyecm-0.0.2/ext/nanobind/docs/why.rst`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/.github/workflows/ci.yml` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/CMakeLists.txt` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/LICENSE` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/README.md` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/README.md`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/doxygen.conf` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/doxygen.conf`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/include/tsl/robin_growth_policy.h` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/include/tsl/robin_growth_policy.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/include/tsl/robin_hash.h` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/include/tsl/robin_hash.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/include/tsl/robin_map.h` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/include/tsl/robin_map.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/include/tsl/robin_set.h` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/include/tsl/robin_set.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/CMakeLists.txt` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/custom_allocator_tests.cpp` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/custom_allocator_tests.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/main.cpp` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/main.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/policy_tests.cpp` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/policy_tests.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/robin_map_tests.cpp` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/robin_map_tests.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/robin_set_tests.cpp` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/robin_set_tests.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/tests/utils.h` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/tests/utils.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/ext/robin_map/tsl-robin-map.natvis` & `pyecm-0.0.2/ext/nanobind/ext/robin_map/tsl-robin-map.natvis`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/eigen/dense.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/eigen/dense.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/eigen/sparse.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/eigen/sparse.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/eval.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/eval.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/intrusive/counter.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/intrusive/counter.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/intrusive/counter.inl` & `pyecm-0.0.2/ext/nanobind/include/nanobind/intrusive/counter.inl`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/intrusive/ref.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/intrusive/ref.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/make_iterator.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/make_iterator.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nanobind.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nanobind.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_accessor.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_accessor.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_attr.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_attr.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_call.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_call.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_cast.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_cast.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_class.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_class.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_defs.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_defs.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_descr.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_descr.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_enums.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_enums.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_error.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_error.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_func.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_func.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_lib.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_lib.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_misc.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_misc.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_python.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_python.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_traits.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_traits.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_tuple.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_tuple.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/nb_types.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/nb_types.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/ndarray.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/ndarray.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/operators.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/operators.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/array.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/array.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/bind_map.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/bind_map.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/bind_vector.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/bind_vector.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/chrono.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/chrono.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/complex.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/complex.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/chrono.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/chrono.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/nb_array.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/nb_array.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/nb_dict.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/nb_dict.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/nb_list.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/nb_list.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/nb_set.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/nb_set.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/detail/traits.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/detail/traits.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/filesystem.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/function.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/function.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/list.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/list.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/map.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/map.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/optional.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/optional.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/pair.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/pair.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/set.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/set.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/shared_ptr.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/shared_ptr.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/string.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/string.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/string_view.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/string_view.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/tuple.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/tuple.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/unique_ptr.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/unique_ptr.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/unordered_map.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/unordered_map.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/unordered_set.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/unordered_set.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/variant.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/variant.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/stl/vector.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/stl/vector.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/trampoline.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/trampoline.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/include/nanobind/typing.h` & `pyecm-0.0.2/ext/nanobind/include/nanobind/typing.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/setup.py` & `pyecm-0.0.2/ext/nanobind/setup.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/__init__.py` & `pyecm-0.0.2/ext/nanobind/src/__init__.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/__main__.py` & `pyecm-0.0.2/ext/nanobind/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/buffer.h` & `pyecm-0.0.2/ext/nanobind/src/buffer.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/common.cpp` & `pyecm-0.0.2/ext/nanobind/src/common.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/error.cpp` & `pyecm-0.0.2/ext/nanobind/src/error.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/hash.h` & `pyecm-0.0.2/ext/nanobind/src/hash.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/implicit.cpp` & `pyecm-0.0.2/ext/nanobind/src/implicit.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/nb_combined.cpp` & `pyecm-0.0.2/ext/nanobind/src/nb_combined.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/nb_enum.cpp` & `pyecm-0.0.2/ext/nanobind/src/nb_enum.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/nb_func.cpp` & `pyecm-0.0.2/ext/nanobind/src/nb_func.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/nb_internals.cpp` & `pyecm-0.0.2/ext/nanobind/src/nb_internals.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/nb_internals.h` & `pyecm-0.0.2/ext/nanobind/src/nb_internals.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/nb_ndarray.cpp` & `pyecm-0.0.2/ext/nanobind/src/nb_ndarray.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/nb_static_property.cpp` & `pyecm-0.0.2/ext/nanobind/src/nb_static_property.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/nb_type.cpp` & `pyecm-0.0.2/ext/nanobind/src/nb_type.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/stubgen.py` & `pyecm-0.0.2/ext/nanobind/src/stubgen.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/src/trampoline.cpp` & `pyecm-0.0.2/ext/nanobind/src/trampoline.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/CMakeLists.txt` & `pyecm-0.0.2/ext/nanobind/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/object_py.h` & `pyecm-0.0.2/ext/nanobind/tests/object_py.h`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/py_stub_test.py` & `pyecm-0.0.2/ext/nanobind/tests/py_stub_test.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/py_stub_test.pyi` & `pyecm-0.0.2/ext/nanobind/tests/py_stub_test.pyi`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/py_stub_test.pyi.ref` & `pyecm-0.0.2/ext/nanobind/tests/py_stub_test.pyi.ref`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_chrono.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_chrono.py` & `pyecm-0.0.2/ext/nanobind/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_classes.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_classes.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_classes.py` & `pyecm-0.0.2/ext/nanobind/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_classes_ext.pyi.ref` & `pyecm-0.0.2/ext/nanobind/tests/test_classes_ext.pyi.ref`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_eigen.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_eigen.py` & `pyecm-0.0.2/ext/nanobind/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_enum.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_enum.py` & `pyecm-0.0.2/ext/nanobind/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_enum_ext.pyi.ref` & `pyecm-0.0.2/ext/nanobind/tests/test_enum_ext.pyi.ref`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_eval.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_eval.py` & `pyecm-0.0.2/ext/nanobind/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_exception.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_exception.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_exception.py` & `pyecm-0.0.2/ext/nanobind/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_functions.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_functions.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_functions.py` & `pyecm-0.0.2/ext/nanobind/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_functions_ext.pyi.ref` & `pyecm-0.0.2/ext/nanobind/tests/test_functions_ext.pyi.ref`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_holders.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_holders.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_holders.py` & `pyecm-0.0.2/ext/nanobind/tests/test_holders.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_intrusive.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_intrusive.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_intrusive.py` & `pyecm-0.0.2/ext/nanobind/tests/test_intrusive.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_issue.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_issue.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_issue.py` & `pyecm-0.0.2/ext/nanobind/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_make_iterator.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_make_iterator.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_make_iterator.py` & `pyecm-0.0.2/ext/nanobind/tests/test_make_iterator.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_make_iterator_ext.pyi.ref` & `pyecm-0.0.2/ext/nanobind/tests/test_make_iterator_ext.pyi.ref`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_ndarray.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_ndarray.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_ndarray.py` & `pyecm-0.0.2/ext/nanobind/tests/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_ndarray_ext.pyi.ref` & `pyecm-0.0.2/ext/nanobind/tests/test_ndarray_ext.pyi.ref`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_stl.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_stl.py` & `pyecm-0.0.2/ext/nanobind/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_stl_bind_map.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_stl_bind_map.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_stl_bind_map.py` & `pyecm-0.0.2/ext/nanobind/tests/test_stl_bind_map.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_stl_bind_vector.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_stl_bind_vector.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_stl_bind_vector.py` & `pyecm-0.0.2/ext/nanobind/tests/test_stl_bind_vector.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_stl_ext.pyi.ref` & `pyecm-0.0.2/ext/nanobind/tests/test_stl_ext.pyi.ref`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_stubs.py` & `pyecm-0.0.2/ext/nanobind/tests/test_stubs.py`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_typing.cpp` & `pyecm-0.0.2/ext/nanobind/tests/test_typing.cpp`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/ext/nanobind/tests/test_typing_ext.pyi.ref` & `pyecm-0.0.2/ext/nanobind/tests/test_typing_ext.pyi.ref`

 * *Files identical despite different names*

### Comparing `pyecm-0.0.1/pyproject.toml` & `pyecm-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [project]
 name = "pyecm"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jeff Anderson", email="kj4tmp@gmail.com" },
 ]
 description = "An EtherCAT MainDevice in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = ["numpy"]
 
 [build-system]
 requires = ["scikit-build-core >=0.9.1", "typing_extensions"]
 build-backend = "scikit_build_core.build"
 
 [tool.scikit-build]
 # Protect the configuration against future changes in scikit-build-core
 minimum-version = "0.9"
-
 # Setuptools-style build caching in a local directory
 build-dir = "build/{wheel_tag}"
 
 # Build stable ABI wheels for CPython 3.12+
 wheel.py-api = "cp312"
 
 [project.urls]
@@ -32,20 +32,22 @@
 Issues = "https://github.com/kj4tmp/pyecm/issues"
 
 [tool.cibuildwheel]
 # Necessary to see build output from the actual compilation
 build-verbosity = 1
 
 # Optional: run pytest to ensure that the package was correctly built
-# test-command = "pytest {project}/tests"
-# test-requires = "pytest"
+test-command = "pytest {project}/tests"
+test-requires = "pytest==8.1.1"
 
 # Needed for full C++17 support on macOS
 [tool.cibuildwheel.macos.environment]
 MACOSX_DEPLOYMENT_TARGET = "10.14"
 
+[tool.cibuildwheel.windows]
+archs = ["auto64"] # skip 32-bit on windows since stub generation is broken
 
 # pyproject.toml
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
-]
+]
```

### Comparing `pyecm-0.0.1/tests/environments/basic/test_basic_env.py` & `pyecm-0.0.2/tests/test_soem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,20 @@
-'''
-
-run using command:
-
-pip install . && pytest --log-cli-level=INFO -s tests/environments/basic/test_basic_env.py 
-'''
 import logging
 
-import pyecm
 import pytest
 
+import pyecm
+from pyecm.soem import SOEM, ec_eepromFMMUt, ec_eepromSMt, ec_slavet
+
 _logger = logging.getLogger(__name__)
 
-@pytest.fixture(scope='module')
-def basic_environment():
-    # info about this environment
-    USE_REDUNDANCY = True
-    NETWORK_ADAPTER_NAME = 'enp0s20f0u1'
-    RED_NETWORK_ADAPTER_NAME = 'enp0s20f0u3'
-    NUM_SUBDEVICES = 5
-
-
-    adapters = pyecm.soem.ec_find_adapters()
-    adapter_names = [adapter.name.decode() for adapter in adapters]
-    
-    assert NETWORK_ADAPTER_NAME in adapter_names
-
-    if USE_REDUNDANCY:
-        assert RED_NETWORK_ADAPTER_NAME in adapter_names
-    
-    ctx = pyecm.soem.ecx_contextt()
-
-    if USE_REDUNDANCY:
-        red_port = pyecm.soem.ecx_redportt()
-        assert pyecm.soem.ecx_init_redundant(ctx, red_port, NETWORK_ADAPTER_NAME, RED_NETWORK_ADAPTER_NAME) > 0
-    else:
-        assert pyecm.soem.ecx_init(ctx, NETWORK_ADAPTER_NAME) > 0
-    
-
-    # i don't know why but this fails frequently unless the subdevices are power cycled
-    assert  pyecm.soem.ecx_config_init(ctx, False) == NUM_SUBDEVICES
-    assert  ctx.slavecount == NUM_SUBDEVICES
-    
-    _logger.info('test starting')
-    log_context(ctx)
-    yield ctx
-    _logger.info('test finished')
-    log_context(ctx)
-    pyecm.soem.ecx_close(ctx)
 
-def log_subdevices(subdevices: list[pyecm.soem.ec_slavet]):
+def log_subdevices(subdevices: pyecm.soem.ECSlaveTVector):
     for i, subdevice in enumerate(subdevices):
-        if i ==0:
+        if i == 0:
             _logger.info("MainDevice:")
         else:
             _logger.info(f"SubDevice: {i-1}")
         _logger.info(f"    {subdevice.state=}")
         _logger.info(f"    {subdevice.ALstatuscode=}")
         _logger.info(f"    {subdevice.configadr=}")
         _logger.info(f"    {subdevice.aliasadr=}")
@@ -118,50 +78,99 @@
     # _logger.info(f"{subdevice.FMMUunused=}")
     # _logger.info(f"{subdevice.islost=}")
     # _logger.info(f"{subdevice.PO2SOconfig=}")
     # _logger.info(f"{subdevice.PO2SOconfigx=}")
     # _logger.info(f"{subdevice.name=}")
 
 
-def log_context(ctx: pyecm.soem.ecx_contextt):
+def log_context(ctx: pyecm.soem.SOEM):
     _logger.info(f"{ctx.port=}")
     _logger.info(f"{ctx.slavelist=}")
     _logger.info(f"{ctx.slavecount=}")
     _logger.info(f"{ctx.maxslave=}")
     _logger.info(f"{ctx.grouplist=}")
     _logger.info(f"{ctx.maxgroup=}")
-    _logger.info(f"{ctx.esibuf=}")
-    _logger.info(f"{ctx.esimap=}")
-    _logger.info(f"{ctx.esislave=}")
+    # _logger.info(f"{ctx.esibuf=}")
+    # _logger.info(f"{ctx.esimap=}")
+    # _logger.info(f"{ctx.esislave=}")
     _logger.info(f"{ctx.elist=}")
     _logger.info(f"{ctx.idxstack=}")
     _logger.info(f"{ctx.ecaterror=}")
     _logger.info(f"{ctx.DCtime=}")
     _logger.info(f"{ctx.SMcommtype=}")
     _logger.info(f"{ctx.PDOassign=}")
     _logger.info(f"{ctx.PDOdesc=}")
     _logger.info(f"{ctx.eepSM=}")
     _logger.info(f"{ctx.eepFMMU=}")
-    _logger.info(f"{ctx.manualstatechange=}")
-    _logger.info(f"{ctx.userdata=}")
+    # _logger.info(f"{ctx.manualstatechange=}")
+    # _logger.info(f"{ctx.userdata=}")
     log_subdevices(ctx.slavelist)
 
-    
-def test_correct_subdevices(basic_environment: pyecm.soem.ecx_contextt):
-
-    ctx = basic_environment
-
-    assert ctx.slavelist[1].name == 'EK1100'
-    assert ctx.slavelist[2].name == 'EL3314'
-    assert ctx.slavelist[3].name == 'EL2088'
-    assert ctx.slavelist[4].name == 'EL3681'
-    assert ctx.slavelist[5].name == 'EL3204'
-    pass
-
-def test_process_data():
-    pass
-
-
-
-
-
 
+@pytest.mark.parametrize(
+    ("maxslave", "maxgroup"),
+    [[12345456, 12], [12, 12345], [-1, 23], [23, -1], [123456, 123456]],
+)
+def test_SOEM_incompatible_arguments(maxslave, maxgroup):
+    """context init should raise when args are too big / negative"""
+    with pytest.raises(TypeError):
+        SOEM(maxslave, maxgroup, 1)
+
+
+@pytest.mark.parametrize(
+    ("maxslave", "maxgroup", "iomap_size_bytes"), [[0, 1, 1], [1, 0, 1], [1, 1, 0]]
+)
+def test_SOEM_value_errors(maxslave, maxgroup, iomap_size_bytes):
+    with pytest.raises(ValueError):
+        SOEM(maxslave, maxgroup, iomap_size_bytes)
+
+
+@pytest.mark.parametrize(
+    ("maxslave", "maxgroup", "iomap_size_bytes"),
+    [
+        [12, 12, 1],
+        [1345, 1, 12345],
+    ],
+)
+def test_SOEM_compatible_arguments(maxslave, maxgroup, iomap_size_bytes):
+    SOEM(maxslave, maxgroup, iomap_size_bytes)
+
+
+def test_ec_eepromFMMUt():
+    t = ec_eepromFMMUt()
+    t.FMMU0 = 23
+    t.FMMU1 = 234
+    t.FMMU2 = 0
+    t.FMMU3 = 34
+    t.nFMMU = 2
+    with pytest.raises(TypeError):
+        t.FMMU0 = 12345
+
+
+def test_ec_eepromSM():
+    t = ec_eepromSMt()
+    t.nSM = 23
+    with pytest.raises(TypeError):
+        t.Creg = 12345
+
+
+# TODO: this fails due to nanobind copy return value policy for vector __getitem__
+# def test_slavelist():
+#     context = SOEM(maxslave=2, maxgroup=2)
+#     context.slavelist[0].state = 13
+#     assert context.slavelist[0].state == 13
+
+
+def test_slavelist2():
+    context = SOEM(maxslave=2, maxgroup=2, iomap_size_bytes=1)
+    new_slave = ec_slavet()
+    new_slave.state = 13
+    context.slavelist[0] = new_slave
+    assert context.slavelist[0].state == 13
+
+
+def test_slavelist3():
+    context = SOEM(maxslave=2, maxgroup=2, iomap_size_bytes=1)
+    new_slave = context.slavelist[0]
+    new_slave.state = 13
+    context.slavelist[0] = new_slave
+    assert context.slavelist[0].state == 13
```

