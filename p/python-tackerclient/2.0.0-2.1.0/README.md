# Comparing `tmp/python-tackerclient-2.0.0.tar.gz` & `tmp/python-tackerclient-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-tackerclient-2.0.0.tar", last modified: Wed Jan 10 17:08:27 2024, max compression
+gzip compressed data, was "python-tackerclient-2.1.0.tar", last modified: Thu May 16 13:04:02 2024, max compression
```

## Comparing `python-tackerclient-2.0.0.tar` & `python-tackerclient-2.1.0.tar`

### file list

```diff
@@ -1,256 +1,258 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.302683 python-tackerclient-2.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4725 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16971 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2024-01-10 17:08:27.302683 python-tackerclient-2.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.238680 python-tackerclient-2.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.238680 python-tackerclient-2.0.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.242680 python-tackerclient-2.0.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6704 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/cli/commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/cli/vim_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/cli/vnf_package_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/cli/vnffm_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/cli/vnflcm_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/cli/vnfpm_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2921 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.242680 python-tackerclient-2.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/contributor/developing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.242680 python-tackerclient-2.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1641 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.242680 python-tackerclient-2.0.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.246681 python-tackerclient-2.0.0/python_tackerclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/python_tackerclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9564 2024-01-10 17:08:27.000000 python-tackerclient-2.0.0/python_tackerclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/python_tackerclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5421 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/python_tackerclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/python_tackerclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/python_tackerclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/python_tackerclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-01-10 17:08:26.000000 python-tackerclient-2.0.0/python_tackerclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.226680 python-tackerclient-2.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.254681 python-tackerclient-2.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/add-creating-ns-vnffg-from-template-213eee7f1820aa0c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/add-vnffg-and-vnf-ids-to-ns-list-commands-9d462efc103f8ecb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/bug-1750865-04c3ebd0c3f8af29.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/bug-1754556-53268d3081fa18d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/bug-1754793-54446bcd0a4e84aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/bug-1754926-06ac4d7ffd17b5ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/clustering-service-cli-e15cc6627de293fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/del-project_and_user_id-e9dd396f83a162d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/deprecate-direct-yaml-cli-input-812564bab1b99b4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/deprecate-infra-mgmt-driver-attributes-e371624c50accee8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/deprecate-legacy-apis-excluding-vim-debaa69507f73179.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/deprecated-tacker-command-29121558bd748082.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/drop-py-2-7-b2052825c4b92b52.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/multi-delete-support-in-tacker-acd4a7e86114f0be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/network-services-descriptor-06f6abe90adb40f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/new-commmand-vnf-resource-list-d5422ab917f0892f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/obsolete-legacy-apis-excluding-vim-43d8dd73c3768fbb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/remove-passing-mgmt-and-infra-driver-from-client-c9135f84480b2cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/tacker-support-python-openstackclient-b88b20b80b872229.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/update-vim-without-config-c3b637741889eff6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/vnf-inline-template-25f6a0b66f7407a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/vnfd-vnf-vim-name-mandatory-in-tacker-cli-dfe802af6de5c80e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/notes/vnffg-client-abd7d7f06860b91d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.258681 python-tackerclient-2.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.258681 python-tackerclient-2.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.258681 python-tackerclient-2.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8504 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6490 2024-01-10 17:08:27.306683 python-tackerclient-2.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.262681 python-tackerclient-2.0.0/tackerclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14816 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.266681 python-tackerclient-2.0.0/tackerclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3785 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/clientmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5118 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3825 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/serializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5806 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/common/validators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.266681 python-tackerclient-2.0.0/tackerclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.266681 python-tackerclient-2.0.0/tackerclient/osc/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.266681 python-tackerclient-2.0.0/tackerclient/osc/common/vnflcm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/common/vnflcm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/common/vnflcm/vnflcm_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4348 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/sdk_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8674 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.266681 python-tackerclient-2.0.0/tackerclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.266681 python-tackerclient-2.0.0/tackerclient/osc/v1/nfvo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/nfvo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9931 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/nfvo/vim.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.270681 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.270681 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/change_ext_conn_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4071 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/create_lccn_subscription_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/heal_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2517 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/instantiate_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/scale_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/update_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21954 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/vnflcm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11909 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/vnflcm_op_occs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6366 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/vnflcm_subsc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.270681 python-tackerclient-2.0.0/tackerclient/osc/v1/vnfpkgm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnfpkgm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19486 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v1/vnfpkgm/vnf_package.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.270681 python-tackerclient-2.0.0/tackerclient/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.274682 python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.274682 python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/samples/create_vnf_fm_subscription_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6462 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/vnffm_alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5743 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/vnffm_sub.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.230680 python-tackerclient-2.0.0/tackerclient/osc/v2/vnflcm/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.274682 python-tackerclient-2.0.0/tackerclient/osc/v2/vnflcm/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnflcm/samples/change_vnfpkg_vnf_instance_param_sample.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.274682 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.278682 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/samples/create_vnf_pm_job_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/samples/create_vnf_pm_threshold_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/samples/update_vnf_pm_job_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/samples/update_vnf_pm_threshold_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10858 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/vnfpm_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/vnfpm_report.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7787 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/vnfpm_threshold.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31096 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.278682 python-tackerclient-2.0.0/tackerclient/tacker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tacker/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2556 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tacker/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.278682 python-tackerclient-2.0.0/tackerclient/tacker/v1_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26548 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tacker/v1_0/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.278682 python-tackerclient-2.0.0/tackerclient/tacker/v1_0/nfvo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tacker/v1_0/nfvo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tacker/v1_0/nfvo/vim.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tacker/v1_0/nfvo/vim_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.278682 python-tackerclient-2.0.0/tackerclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.282682 python-tackerclient-2.0.0/tackerclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.282682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.282682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/common/test_vnflcm_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.286682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.286682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.230680 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.290682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9191 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_common_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67244 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_vnfd_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7726 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_df_simple.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_top.vnfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_types.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.290682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/TOSCA-Metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/TOSCA-Metadata/TOSCA.meta
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.230680 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.290682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_common_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67211 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_vnfd_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7726 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_df_simple.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_top.vnfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_types.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.290682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Scripts/install.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.290682 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/TOSCA-Metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/TOSCA-Metadata/TOSCA.meta
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35875 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/test_vnf_package.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40067 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/test_vnflcm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23955 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/test_vnflcm_op_occs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10394 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/test_vnflcm_subsc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6767 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/vnf_package_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5735 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/vnflcm_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3373 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/vnflcm_op_occs_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6957 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/vnflcm_subsc_fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.298683 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11348 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnffm_alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12108 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnffm_sub.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6083 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnflcm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18727 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnfpm_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4842 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnfpm_report.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15811 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnfpm_threshold.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnffm_alarm_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3880 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnffm_sub_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4203 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnfpm_job_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnfpm_report_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3572 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnfpm_threshold_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14453 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_casual_args.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31529 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_cli10.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1317 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_command_meta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7144 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3116 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_ssl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5090 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4099 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.298683 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.302683 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/samples/vim_config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/samples/vim_config_with_false_cert_verify.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/samples/vim_config_without_auth_url.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/samples/vim_k8s_bearer_token.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/samples/vim_k8s_bearer_token_without_auth_url.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/samples/vim_k8s_config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/samples/vim_k8s_config_without_auth_url.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/test_cli10_vim.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7011 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6970 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s_with_bearer_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8180 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/tests/unit/vm/test_vim_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.302683 python-tackerclient-2.0.0/tackerclient/v1_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/v1_0/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40253 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/v1_0/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tackerclient/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-10 17:08:27.302683 python-tackerclient-2.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tools/tacker.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-01-10 17:07:55.000000 python-tackerclient-2.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.754619 python-tackerclient-2.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4765 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17324 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2024-05-16 13:04:02.754619 python-tackerclient-2.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.722619 python-tackerclient-2.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.722619 python-tackerclient-2.1.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.722619 python-tackerclient-2.1.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6704 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/cli/commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/cli/vim_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/cli/vnf_package_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/cli/vnffm_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/cli/vnflcm_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/cli/vnfpm_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2921 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.722619 python-tackerclient-2.1.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/contributor/developing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.722619 python-tackerclient-2.1.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1641 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.722619 python-tackerclient-2.1.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.726619 python-tackerclient-2.1.0/python_tackerclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/python_tackerclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9626 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/python_tackerclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/python_tackerclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5421 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/python_tackerclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/python_tackerclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/python_tackerclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/python_tackerclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-05-16 13:04:02.000000 python-tackerclient-2.1.0/python_tackerclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.714619 python-tackerclient-2.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.730620 python-tackerclient-2.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/add-creating-ns-vnffg-from-template-213eee7f1820aa0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/add-vnffg-and-vnf-ids-to-ns-list-commands-9d462efc103f8ecb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/bug-1750865-04c3ebd0c3f8af29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/bug-1754556-53268d3081fa18d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/bug-1754793-54446bcd0a4e84aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/bug-1754926-06ac4d7ffd17b5ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/clustering-service-cli-e15cc6627de293fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/del-project_and_user_id-e9dd396f83a162d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/deprecate-direct-yaml-cli-input-812564bab1b99b4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/deprecate-infra-mgmt-driver-attributes-e371624c50accee8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/deprecate-legacy-apis-excluding-vim-debaa69507f73179.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/deprecated-tacker-command-29121558bd748082.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/drop-py-2-7-b2052825c4b92b52.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/multi-delete-support-in-tacker-acd4a7e86114f0be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/network-services-descriptor-06f6abe90adb40f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/new-commmand-vnf-resource-list-d5422ab917f0892f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/obsolete-legacy-apis-excluding-vim-43d8dd73c3768fbb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/remove-passing-mgmt-and-infra-driver-from-client-c9135f84480b2cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/tacker-support-python-openstackclient-b88b20b80b872229.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/update-vim-without-config-c3b637741889eff6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/vnf-inline-template-25f6a0b66f7407a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/vnfd-vnf-vim-name-mandatory-in-tacker-cli-dfe802af6de5c80e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/notes/vnffg-client-abd7d7f06860b91d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.730620 python-tackerclient-2.1.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.730620 python-tackerclient-2.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.730620 python-tackerclient-2.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8504 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6490 2024-05-16 13:04:02.758619 python-tackerclient-2.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.734619 python-tackerclient-2.1.0/tackerclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14912 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.734619 python-tackerclient-2.1.0/tackerclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3785 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/clientmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5118 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3825 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/serializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5806 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/common/validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.734619 python-tackerclient-2.1.0/tackerclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.734619 python-tackerclient-2.1.0/tackerclient/osc/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.734619 python-tackerclient-2.1.0/tackerclient/osc/common/vnflcm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/common/vnflcm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/common/vnflcm/vnflcm_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4348 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/sdk_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8674 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.734619 python-tackerclient-2.1.0/tackerclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.738619 python-tackerclient-2.1.0/tackerclient/osc/v1/nfvo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/nfvo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9931 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/nfvo/vim.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.738619 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.738619 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/change_ext_conn_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4071 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/create_lccn_subscription_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/heal_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2517 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/instantiate_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/scale_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/update_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21954 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/vnflcm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11909 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/vnflcm_op_occs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6366 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/vnflcm_subsc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.738619 python-tackerclient-2.1.0/tackerclient/osc/v1/vnfpkgm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnfpkgm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19486 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v1/vnfpkgm/vnf_package.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.738619 python-tackerclient-2.1.0/tackerclient/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.738619 python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.738619 python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/samples/create_vnf_fm_subscription_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6462 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/vnffm_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5743 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/vnffm_sub.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.714619 python-tackerclient-2.1.0/tackerclient/osc/v2/vnflcm/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.738619 python-tackerclient-2.1.0/tackerclient/osc/v2/vnflcm/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnflcm/samples/change_vnfpkg_vnf_instance_param_sample.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.742619 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.742619 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/samples/create_vnf_pm_job_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/samples/create_vnf_pm_threshold_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/samples/update_vnf_pm_job_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/samples/update_vnf_pm_threshold_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10678 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/vnfpm_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/vnfpm_report.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7787 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/vnfpm_threshold.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31096 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.742619 python-tackerclient-2.1.0/tackerclient/tacker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tacker/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2556 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tacker/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.742619 python-tackerclient-2.1.0/tackerclient/tacker/v1_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26548 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tacker/v1_0/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.742619 python-tackerclient-2.1.0/tackerclient/tacker/v1_0/nfvo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tacker/v1_0/nfvo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tacker/v1_0/nfvo/vim.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tacker/v1_0/nfvo/vim_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.742619 python-tackerclient-2.1.0/tackerclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.746620 python-tackerclient-2.1.0/tackerclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.746620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.746620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/common/test_vnflcm_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.746620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.746620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.718619 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.750620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9191 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_common_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67244 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_vnfd_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7726 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_df_simple.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_top.vnfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_types.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.750620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/TOSCA-Metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/TOSCA-Metadata/TOSCA.meta
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.718619 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.750620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_common_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67211 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_vnfd_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7726 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_df_simple.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_top.vnfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_types.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.750620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Scripts/install.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.750620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/TOSCA-Metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/TOSCA-Metadata/TOSCA.meta
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35875 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/test_vnf_package.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40067 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/test_vnflcm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23955 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/test_vnflcm_op_occs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10394 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/test_vnflcm_subsc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6767 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/vnf_package_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5735 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/vnflcm_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3373 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/vnflcm_op_occs_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6957 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/vnflcm_subsc_fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.750620 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11348 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnffm_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12108 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnffm_sub.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6083 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnflcm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18709 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnfpm_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4842 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnfpm_report.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15811 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnfpm_threshold.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnffm_alarm_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3880 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnffm_sub_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3668 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnfpm_job_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnfpm_report_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3572 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnfpm_threshold_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14680 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_casual_args.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32211 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_cli10.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1317 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_command_meta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7144 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3116 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_ssl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5090 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4099 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.754619 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.754619 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/samples/vim_config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/samples/vim_config_with_false_cert_verify.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/samples/vim_config_without_auth_url.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/samples/vim_k8s_bearer_token.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/samples/vim_k8s_bearer_token_without_auth_url.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/samples/vim_k8s_config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/samples/vim_k8s_config_without_auth_url.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/test_cli10_vim.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7011 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6970 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s_with_bearer_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8180 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/tests/unit/vm/test_vim_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.754619 python-tackerclient-2.1.0/tackerclient/v1_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/v1_0/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40253 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/v1_0/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tackerclient/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:04:02.754619 python-tackerclient-2.1.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tools/tacker.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-05-16 13:03:09.000000 python-tackerclient-2.1.0/tox.ini
```

### Comparing `python-tackerclient-2.0.0/.pylintrc` & `python-tackerclient-2.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/AUTHORS` & `python-tackerclient-2.1.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 Janki Chhatbar <jchhatba@redhat.com>
 Janonymous <janonymous.codevulture@gmail.com>
 Javier Pena <jpena@redhat.com>
 Jeremy Stanley <fungi@yuggoth.org>
 Joel Capitao <jcapitao@redhat.com>
 KLuka <luka.krajger@gmail.com>
 Kanagaraj Manickam <mkr1481@gmail.com>
+Kaori Mitani <mitani.kaori@fujitsu.com>
 Kawaguchi Kentaro <ken-kawaguchi@vt.jp.nec.com>
 Koichi Edagawa <edagawa.kc@nec.com>
 Koji Shimizu <shimizu.koji@fujitsu.com>
 LiangLu <lu.liang@jp.fujitsu.com>
 LongKB <longkb@bka.vn>
 Lu lei <lei.lu@easystack.cn>
 Luka Krajger <luka.krajger@gmail.com>
```

### Comparing `python-tackerclient-2.0.0/CONTRIBUTING.rst` & `python-tackerclient-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/ChangeLog` & `python-tackerclient-2.1.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 CHANGES
 =======
 
+2.1.0
+-----
+
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+* Fix output regarding PM Job response
+* Fix the handling of content-type in HTTPClient
+* reno: Update master for unmaintained/yoga
+
 2.0.0
 -----
 
 * Obsolete Legacy APIs excluding VIM feature
 * Fix unit test error caused by cliff upgrade
 * Remove legacy documentation
+* Update master for stable/2023.2
 
 1.14.0
 ------
 
 * Update metadata in setup.cfg
 * Update master for stable/2023.1
```

### Comparing `python-tackerclient-2.0.0/HACKING.rst` & `python-tackerclient-2.1.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/LICENSE` & `python-tackerclient-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/PKG-INFO` & `python-tackerclient-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-tackerclient
-Version: 2.0.0
+Version: 2.1.0
 Summary: CLI and Client Library for OpenStack Tacker
 Home-page: https://docs.openstack.org/python-tackerclient/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: CLI and Client Library for OpenStack Tacker
 Platform: UNKNOWN
```

### Comparing `python-tackerclient-2.0.0/README.rst` & `python-tackerclient-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/cli/commands.rst` & `python-tackerclient-2.1.0/doc/source/cli/commands.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/cli/index.rst` & `python-tackerclient-2.1.0/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/cli/vim_commands.rst` & `python-tackerclient-2.1.0/doc/source/cli/vim_commands.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/cli/vnf_package_commands.rst` & `python-tackerclient-2.1.0/doc/source/cli/vnf_package_commands.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/cli/vnffm_commands.rst` & `python-tackerclient-2.1.0/doc/source/cli/vnffm_commands.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/cli/vnflcm_commands.rst` & `python-tackerclient-2.1.0/doc/source/cli/vnflcm_commands.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/cli/vnfpm_commands.rst` & `python-tackerclient-2.1.0/doc/source/cli/vnfpm_commands.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/conf.py` & `python-tackerclient-2.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/contributor/contributing.rst` & `python-tackerclient-2.1.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/contributor/developing.rst` & `python-tackerclient-2.1.0/doc/source/contributor/developing.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/contributor/index.rst` & `python-tackerclient-2.1.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/index.rst` & `python-tackerclient-2.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/install/index.rst` & `python-tackerclient-2.1.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/doc/source/reference/index.rst` & `python-tackerclient-2.1.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/python_tackerclient.egg-info/PKG-INFO` & `python-tackerclient-2.1.0/python_tackerclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-tackerclient
-Version: 2.0.0
+Version: 2.1.0
 Summary: CLI and Client Library for OpenStack Tacker
 Home-page: https://docs.openstack.org/python-tackerclient/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: CLI and Client Library for OpenStack Tacker
 Platform: UNKNOWN
```

### Comparing `python-tackerclient-2.0.0/python_tackerclient.egg-info/SOURCES.txt` & `python-tackerclient-2.1.0/python_tackerclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 releasenotes/notes/remove-passing-mgmt-and-infra-driver-from-client-c9135f84480b2cae.yaml
 releasenotes/notes/tacker-support-python-openstackclient-b88b20b80b872229.yaml
 releasenotes/notes/update-vim-without-config-c3b637741889eff6.yaml
 releasenotes/notes/vnf-inline-template-25f6a0b66f7407a1.yaml
 releasenotes/notes/vnfd-vnf-vim-name-mandatory-in-tacker-cli-dfe802af6de5c80e.yaml
 releasenotes/notes/vnffg-client-abd7d7f06860b91d.yaml
 releasenotes/source/2023.1.rst
+releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
```

### Comparing `python-tackerclient-2.0.0/python_tackerclient.egg-info/entry_points.txt` & `python-tackerclient-2.1.0/python_tackerclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/releasenotes/source/conf.py` & `python-tackerclient-2.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/requirements.txt` & `python-tackerclient-2.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/setup.cfg` & `python-tackerclient-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/setup.py` & `python-tackerclient-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/client.py` & `python-tackerclient-2.1.0/tackerclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
     def _cs_request(self, *args, **kwargs):
         kargs = {}
         kargs.setdefault('headers', kwargs.get('headers', {}))
         kargs['headers']['User-Agent'] = self.USER_AGENT
 
         if 'body' in kwargs:
             kargs['body'] = kwargs['body']
+        if 'content_type' in kwargs:
+            kargs['content_type'] = kwargs['content_type']
 
         if self.log_credentials:
             log_kargs = kargs
         else:
             log_kargs = self._strip_credentials(kargs)
 
         utils.http_log_req(_logger, args, log_kargs)
```

### Comparing `python-tackerclient-2.0.0/tackerclient/common/_i18n.py` & `python-tackerclient-2.1.0/tackerclient/common/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/common/clientmanager.py` & `python-tackerclient-2.1.0/tackerclient/common/clientmanager.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/common/command.py` & `python-tackerclient-2.1.0/tackerclient/common/command.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/common/constants.py` & `python-tackerclient-2.1.0/tackerclient/common/constants.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/common/exceptions.py` & `python-tackerclient-2.1.0/tackerclient/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/common/extension.py` & `python-tackerclient-2.1.0/tackerclient/common/extension.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/common/serializer.py` & `python-tackerclient-2.1.0/tackerclient/common/serializer.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/common/utils.py` & `python-tackerclient-2.1.0/tackerclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/common/validators.py` & `python-tackerclient-2.1.0/tackerclient/common/validators.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/i18n.py` & `python-tackerclient-2.1.0/tackerclient/i18n.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/common/vnflcm/vnflcm_versions.py` & `python-tackerclient-2.1.0/tackerclient/osc/common/vnflcm/vnflcm_versions.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/plugin.py` & `python-tackerclient-2.1.0/tackerclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/sdk_utils.py` & `python-tackerclient-2.1.0/tackerclient/osc/sdk_utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/utils.py` & `python-tackerclient-2.1.0/tackerclient/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v1/nfvo/vim.py` & `python-tackerclient-2.1.0/tackerclient/osc/v1/nfvo/vim.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/change_ext_conn_vnf_instance_param_sample.json` & `python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/change_ext_conn_vnf_instance_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/create_lccn_subscription_param_sample.json` & `python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/create_lccn_subscription_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/samples/instantiate_vnf_instance_param_sample.json` & `python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/samples/instantiate_vnf_instance_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/vnflcm.py` & `python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/vnflcm.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/vnflcm_op_occs.py` & `python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/vnflcm_op_occs.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v1/vnflcm/vnflcm_subsc.py` & `python-tackerclient-2.1.0/tackerclient/osc/v1/vnflcm/vnflcm_subsc.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v1/vnfpkgm/vnf_package.py` & `python-tackerclient-2.1.0/tackerclient/osc/v1/vnfpkgm/vnf_package.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/samples/create_vnf_fm_subscription_param_sample.json` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/samples/create_vnf_fm_subscription_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/vnffm_alarm.py` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/vnffm_alarm.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnffm/vnffm_sub.py` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnffm/vnffm_sub.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnflcm/samples/change_vnfpkg_vnf_instance_param_sample.json` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnflcm/samples/change_vnfpkg_vnf_instance_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/samples/create_vnf_pm_job_param_sample.json` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/samples/create_vnf_pm_job_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/samples/create_vnf_pm_threshold_param_sample.json` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/samples/create_vnf_pm_threshold_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/samples/update_vnf_pm_threshold_param_sample.json` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/samples/update_vnf_pm_threshold_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/vnfpm_job.py` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/vnfpm_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,34 +30,29 @@
     'objectInstanceIds': tacker_osc_utils.FormatComplexDataColumn,
     'subObjectInstanceIds': tacker_osc_utils.FormatComplexDataColumn,
     'criteria': tacker_osc_utils.FormatComplexDataColumn,
     'reports': tacker_osc_utils.FormatComplexDataColumn,
     '_links': tacker_osc_utils.FormatComplexDataColumn
 }
 
-_FORMATTERS_UPDATE = {
-    'authentication': tacker_osc_utils.FormatComplexDataColumn
-}
-
 _MIXED_CASE_FIELDS = (
     'objectType', 'objectInstanceIds', 'subObjectInstanceIds', 'callbackUri'
 )
 
 _MIXED_CASE_FIELDS_UPDATE = (
     'callbackUri'
 )
 
 _VNF_PM_JOB_ID = 'vnf_pm_job_id'
 
 
 def _get_columns(vnfpm_job_obj, action=None):
     if action == 'update':
         column_map = {
-            'callbackUri': 'Callback Uri',
-            'authentication': 'Authentication'
+            'callbackUri': 'Callback Uri'
         }
     else:
         column_map = {
             'id': 'ID',
             'objectType': 'Object Type',
             'objectInstanceIds': 'Object Instance Ids',
             'subObjectInstanceIds': 'Sub Object Instance Ids',
@@ -255,16 +250,15 @@
     def take_action(self, parsed_args):
         client = self.app.client_manager.tackerclient
         updated_values = client.update_vnf_pm_job(
             parsed_args.vnf_pm_job_id,
             tacker_osc_utils.jsonfile2body(parsed_args.request_file))
         display_columns, columns = _get_columns(updated_values, 'update')
         data = utils.get_item_properties(
-            sdk_utils.DictModel(updated_values),
-            columns, formatters=_FORMATTERS_UPDATE,
+            sdk_utils.DictModel(updated_values), columns,
             mixed_case_fields=_MIXED_CASE_FIELDS_UPDATE)
         return (display_columns, data)
 
 
 class DeleteVnfPmJob(command.Command):
     _description = _("Delete VNF PM job")
```

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/vnfpm_report.py` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/vnfpm_report.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/osc/v2/vnfpm/vnfpm_threshold.py` & `python-tackerclient-2.1.0/tackerclient/osc/v2/vnfpm/vnfpm_threshold.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/shell.py` & `python-tackerclient-2.1.0/tackerclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tacker/client.py` & `python-tackerclient-2.1.0/tackerclient/tacker/client.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tacker/v1_0/__init__.py` & `python-tackerclient-2.1.0/tackerclient/tacker/v1_0/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tacker/v1_0/nfvo/vim.py` & `python-tackerclient-2.1.0/tackerclient/tacker/v1_0/nfvo/vim.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tacker/v1_0/nfvo/vim_utils.py` & `python-tackerclient-2.1.0/tackerclient/tacker/v1_0/nfvo/vim_utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/base.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/base.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/common/test_vnflcm_versions.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/common/test_vnflcm_versions.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/client.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/client.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_common_types.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_common_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_vnfd_types.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_vnfd_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_df_simple.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_df_simple.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_top.vnfd.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_top.vnfd.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_types.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_common_types.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_common_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_vnfd_types.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_vnfd_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_df_simple.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_df_simple.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_top.vnfd.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_top.vnfd.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_types.yaml` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/test_vnf_package.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/test_vnf_package.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/test_vnflcm.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/test_vnflcm.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/test_vnflcm_op_occs.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/test_vnflcm_op_occs.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/test_vnflcm_subsc.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/test_vnflcm_subsc.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/vnf_package_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/vnf_package_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/vnflcm_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/vnflcm_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/vnflcm_op_occs_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/vnflcm_op_occs_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v1/vnflcm_subsc_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v1/vnflcm_subsc_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnffm_alarm.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnffm_alarm.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnffm_sub.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnffm_sub.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnflcm.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnflcm.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnfpm_job.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnfpm_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.app_args = mock.Mock()
         self.client_manager = self.cs
         self.app.client_manager.tackerclient = self.client_manager
 
 
 def _get_columns_vnfpm_job(action=None):
     if action == 'update':
-        columns = ['Callback Uri', 'Authentication']
+        columns = ['Callback Uri']
     else:
         columns = ['ID', 'Object Type', 'Object Instance Ids',
                    'Sub Object Instance Ids', 'Criteria', 'Callback Uri',
                    'Reports', 'Links']
     if action == 'list':
         columns = [
             ele for ele in columns if ele not in [
```

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnfpm_report.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnfpm_report.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/test_vnfpm_threshold.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/test_vnfpm_threshold.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnffm_alarm_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnffm_alarm_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnffm_sub_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnffm_sub_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnfpm_job_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnfpm_job_fakes.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,30 +39,15 @@
     :param Dictionary attrs:
         A dictionary with all attributes
     :return:
         A pm job dict
     """
     if action == 'update':
         fake_vnf_pm_job = {
-            "callbackUri": "/nfvo/notify/job",
-            "authentication": {
-                "authType": [
-                    "BASIC",
-                    "OAUTH2_CLIENT_CREDENTIALS"
-                ],
-                "paramsBasic": {
-                    "userName": "nfvo",
-                    "password": "nfvopwd"
-                },
-                "paramsOauth2ClientCredentials": {
-                    "clientId": "auth_user_name",
-                    "clientPassword": "auth_password",
-                    "tokenEndpoint": "token_endpoint"
-                }
-            }
+            "callbackUri": "/nfvo/notify/job"
         }
         return fake_vnf_pm_job
 
     attrs = attrs or {}
     # Set default attributes.
     fake_vnf_pm_job = {
         "id": "2bb72d78-b1d9-48fe-8c64-332654ffeb5d",
```

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnfpm_report_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnfpm_report_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/osc/v2/vnfpm_threshold_fakes.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/osc/v2/vnfpm_threshold_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_auth.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,16 @@
 
         mock_request.return_value = (resp_200, '')
         self.client.do_request('/resource', 'GET',
                                headers=headers)
         mock_request.assert_called_once_with(
             ENDPOINT_URL + '/resource',
             'GET',
-            headers=headers)
+            headers=headers,
+            content_type=None)
         self.assertEqual(self.client.endpoint_url, ENDPOINT_URL)
 
 
 class CLITestAuthKeystone(testtools.TestCase):
 
     # Auth Body expected
     auth_body = ('{"auth": {"tenantName": "testtenant", '
@@ -149,15 +150,15 @@
     @mock.patch('tackerclient.client.HTTPClient.request')
     def test_get_token(self, mock_request):
 
         mock_request.return_value = (resp_200, json.dumps(KS_TOKEN_RESULT))
         self.client.do_request('/resource', 'GET')
         mock_request.assert_called_with(
             ENDPOINT_URL + '/resource', 'GET',
-            headers=expected_headers)
+            headers=expected_headers, content_type=None)
         self.assertEqual(self.client.endpoint_url, ENDPOINT_URL)
         self.assertEqual(self.client.auth_token, TOKEN)
 
     @mock.patch('tackerclient.client.HTTPClient.request')
     def test_refresh_token(self, mock_request):
 
         self.client.auth_token = TOKEN
@@ -170,15 +171,15 @@
                           '/resource',
                           'GET')
 
         mock_request.return_value = (resp_200, json.dumps(KS_TOKEN_RESULT))
         self.client.do_request('/resource', 'GET')
         mock_request.assert_called_with(
             ENDPOINT_URL + '/resource', 'GET',
-            headers=expected_headers)
+            headers=expected_headers, content_type=None)
 
     @mock.patch('tackerclient.client.HTTPClient.request')
     def test_refresh_token_no_auth_url(self, mock_request):
 
         self.client.auth_url = None
 
         self.client.auth_token = TOKEN
@@ -188,15 +189,16 @@
         mock_request.return_value = (resp_401, '')
         self.assertRaises(exceptions.NoAuthURLProvided,
                           self.client.do_request,
                           '/resource',
                           'GET')
         expected_url = ENDPOINT_URL + '/resource'
         mock_request.assert_called_with(expected_url, 'GET',
-                                        headers=expected_headers)
+                                        headers=expected_headers,
+                                        content_type=None)
 
     def test_get_endpoint_url_with_invalid_auth_url(self):
         # Handle the case when auth_url is not provided
         self.client.auth_url = None
         self.assertRaises(exceptions.NoAuthURLProvided,
                           self.client._get_endpoint_url)
 
@@ -205,22 +207,22 @@
 
         self.client.auth_token = TOKEN
 
         mock_request.return_value = (resp_200, json.dumps(ENDPOINTS_RESULT))
         self.client.do_request('/resource', 'GET')
         mock_request.assert_called_with(
             ENDPOINT_URL + '/resource', 'GET',
-            headers=expected_headers)
+            headers=expected_headers, content_type=None)
 
         mock_request.return_value = (resp_200, '')
         self.client.do_request('/resource', 'GET',
                                headers=headers)
         mock_request.assert_called_with(
             ENDPOINT_URL + '/resource', 'GET',
-            headers=headers)
+            headers=headers, content_type=None)
 
     @mock.patch('tackerclient.client.HTTPClient.request')
     def test_use_given_endpoint_url(self, mock_request):
         self.client = client.HTTPClient(
             username=USERNAME, tenant_name=TENANT_NAME, password=PASSWORD,
             auth_url=AUTH_URL, region_name=REGION,
             endpoint_url=ENDPOINT_OVERRIDE)
@@ -229,15 +231,15 @@
         self.client.auth_token = TOKEN
         mock_request.return_value = (resp_200, '')
 
         self.client.do_request('/resource', 'GET',
                                headers=headers)
         mock_request.assert_called_with(
             ENDPOINT_OVERRIDE + '/resource', 'GET',
-            headers=headers)
+            headers=headers, content_type=None)
         self.assertEqual(self.client.endpoint_url, ENDPOINT_OVERRIDE)
 
     @mock.patch('tackerclient.client.HTTPClient.request')
     def test_get_endpoint_url_other(self, mock_request):
         self.client = client.HTTPClient(
             username=USERNAME, tenant_name=TENANT_NAME, password=PASSWORD,
             auth_url=AUTH_URL, region_name=REGION, endpoint_type='otherURL')
@@ -320,15 +322,16 @@
 
         body = ('{"auth": {"tenantId": "testtenant_id",'
                 '"passwordCredentials": {"password": "password",'
                 '"userId": "testuser_id"}}}')
         expected_body = ('{"auth": {"tenantId": "testtenant_id",'
                          '"REDACTEDCredentials": {"REDACTED": "REDACTED",'
                          '"userId": "testuser_id"}}}')
-        _headers = {'headers': expected_headers, 'body': expected_body}
+        _headers = {'headers': expected_headers, 'body': expected_body,
+                    'content_type': None}
 
         mock_request.return_value = (resp_200, json.dumps(KS_TOKEN_RESULT))
         self.client.do_request('/resource', 'GET', body=body)
 
         args, kwargs = mock_http_log_req.call_args
         # Check that credentials are stripped while logging.
         self.assertEqual(_headers, args[2])
```

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_casual_args.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_casual_args.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_cli10.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_cli10.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,25 +235,28 @@
         resource_plural = tackerV1_0._get_resource_plural(resource,
                                                           self.client)
         path = getattr(self.client, resource_plural + "_path")
         # Work around for LP #1217791. XML deserializer called from
         # MyComparator does not decodes XML string correctly.
         if self.format == 'json':
             _body = MyComparator(body, self.client)
+            _content_type = 'application/json'
         else:
             _body = self.client.serialize(body)
+            _content_type = 'application/zip'
         with mock.patch.object(self.client.httpclient, 'request') as mock_req:
             mock_req.return_value = (MyResp(200), resstr)
             args.extend(['--request-format', self.format])
             cmd_parser = cmd.get_parser('create_' + resource)
             shell.run_command(cmd, cmd_parser, args)
             mock_req.assert_called_once_with(
                 end_url(path, format=self.format), 'POST',
                 body=_body,
-                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                content_type=_content_type)
         self.assertEqual(get_client_called_count, mock_get.call_count)
         _str = self.fake_stdout.make_string()
         self.assertIn(myid, _str)
         if name:
             self.assertIn(name, _str)
 
     @mock.patch.object(TackerCommand, 'get_client')
@@ -269,15 +272,16 @@
             mock_req.return_value = (MyResp(200), resstr)
             args.extend(['--request-format', self.format])
             cmd_parser = cmd.get_parser("list_" + resources_collection)
             shell.run_command(cmd, cmd_parser, args)
             mock_req.assert_called_once_with(
                 end_url(path, format=self.format), 'GET',
                 body=None,
-                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                content_type='application/json')
         mock_get.assert_called_once_with()
 
     def _test_list_resources(self, resources, cmd, detail=False, tags=[],
                              fields_1=[], fields_2=[], page_size=None,
                              sort_key=[], sort_dir=[], response_contents=None,
                              base_args=None, path=None,
                              template_source=None):
@@ -364,15 +368,16 @@
                 cmd_parser = cmd.get_parser("list_" + resources)
                 shell.run_command(cmd, cmd_parser, args)
                 mock_req.assert_called_once_with(
                     MyUrlComparator(end_url(path, query, format=self.format),
                                     self.client),
                     'GET',
                     body=None,
-                    headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                    headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                    content_type='application/json')
         _str = self.fake_stdout.make_string()
         if response_contents is None:
             self.assertIn('myid1', _str)
         return _str
 
     @mock.patch.object(TackerCommand, 'get_client')
     def _test_list_sub_resources(self, resources, api_resource, cmd, myid,
@@ -461,15 +466,16 @@
                 self.client)
             args.extend(['--request-format', self.format])
             cmd_parser = cmd.get_parser("list_" + resources)
             shell.run_command(cmd, cmd_parser, args)
             mock_req.assert_called_once_with(
                 comparator, 'GET',
                 body=None,
-                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                content_type='application/json')
         _str = self.fake_stdout.make_string()
         if response_contents is None:
             self.assertIn('myid1', _str)
         return _str
 
     # TODO(gongysh) add pagination unit test BUG 1633255
     # def _test_list_sub_resources_with_pagination(
@@ -547,28 +553,31 @@
         body = {resource: extrafields}
         path = getattr(self.client, resource + "_path")
         self.client.format = self.format
         # Work around for LP #1217791. XML deserializer called from
         # MyComparator does not decodes XML string correctly.
         if self.format == 'json':
             _body = MyComparator(body, self.client)
+            _content_type = 'application/json'
         else:
             _body = self.client.serialize(body)
+            _content_type = 'application/zip'
         with mock.patch.object(self.client.httpclient, 'request') as mock_req:
             comparator = MyUrlComparator(
                 end_url(path % myid, format=self.format), self.client)
             mock_req.return_value = (MyResp(204), None)
             args.extend(['--request-format', self.format])
             cmd_parser = cmd.get_parser("update_" + resource)
             shell.run_command(cmd, cmd_parser, args)
             mock_req.assert_called_once_with(
                 comparator,
                 'PUT',
                 body=_body,
-                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                content_type=_content_type)
 
         self.assertEqual(get_client_called_count, mock_get.call_count)
         _str = self.fake_stdout.make_string()
         self.assertIn(myid, _str)
 
     def _test_show_resource(self, resource, cmd, myid, args, fields=[]):
         with mock.patch.object(cmd, 'get_client') as mock_get:
@@ -585,15 +594,16 @@
                 mock_req.return_value = (MyResp(200), resstr)
                 args.extend(['--request-format', self.format])
                 cmd_parser = cmd.get_parser("show_" + resource)
                 shell.run_command(cmd, cmd_parser, args)
                 mock_req.assert_called_once_with(
                     end_url(path % myid, query, format=self.format), 'GET',
                     body=None,
-                    headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                    headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                    content_type='application/json')
             _str = self.fake_stdout.make_string()
             mock_get.assert_called_once_with()
             self.assertIn(myid, _str)
             self.assertIn('myname', _str)
 
     @mock.patch.object(TackerCommand, 'get_client')
     def _test_delete_resource(self, resource, cmd, myid, args, mock_get):
@@ -607,20 +617,22 @@
             shell.run_command(cmd, cmd_parser, args)
             if '--force' in args:
                 body_str = '{"' + resource + \
                            '": {"attributes": {"force": true}}}'
                 mock_req.assert_called_once_with(
                     end_url(path % myid, format=self.format), 'DELETE',
                     body=body_str,
-                    headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                    headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                    content_type='application/json')
             else:
                 mock_req.assert_called_once_with(
                     end_url(path % myid, format=self.format), 'DELETE',
                     body=None,
-                    headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                    headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                    content_type='application/json')
         mock_get.assert_called_once_with()
         _str = self.fake_stdout.make_string()
         msg = 'All specified %(resource)s(s) %(msg)s successfully\n' % {
             'msg': deleted_msg.get(resource, 'deleted'),
             'resource': resource}
         self.assertEqual(msg, _str)
 
@@ -634,15 +646,16 @@
             mock_req.return_value = (MyResp(204), retval)
             args.extend(['--request-format', self.format])
             cmd_parser = cmd.get_parser("delete_" + resource)
             shell.run_command(cmd, cmd_parser, args)
             mock_req.assert_called_once_with(
                 end_url(path % path_action, format=self.format), 'PUT',
                 body=MyComparator(body, self.client),
-                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN))
+                headers=test_utils.ContainsKeyValue('X-Auth-Token', TOKEN),
+                content_type='application/json')
         _str = self.fake_stdout.make_string()
         self.assertIn(myid, _str)
 
 
 class ClientV1TestJson(CLITestV10Base):
     def test_do_request_unicode(self):
         self.client.format = self.format
@@ -656,15 +669,16 @@
             mock_req.return_value = (MyResp(200), expect_body)
             res_body = self.client.do_request('PUT', action, body=body,
                                               params=params)
             expected_uri = 'localurl/v1.0/test.json?test=%E7%BD%91%E7%BB%9C'
             mock_req.assert_called_with(
                 expected_uri, 'PUT', body=expect_body,
                 headers={'X-Auth-Token': unicode_text,
-                         'User-Agent': 'python-tackerclient'})
+                         'User-Agent': 'python-tackerclient'},
+                content_type='application/json')
         # test response with unicode
         self.assertEqual(res_body, body)
 
     def test_do_request_error_without_response_body(self):
         self.client.format = self.format
         params = {'test': 'value'}
         expect_query = urlparse.urlencode(params)
```

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_command_meta.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_command_meta.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_http.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_http.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_shell.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_ssl.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_ssl.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_utils.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/test_validators.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/vm/test_cli10_vim.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/vm/test_cli10_vim.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s_with_bearer_token.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s_with_bearer_token.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/tests/unit/vm/test_vim_utils.py` & `python-tackerclient-2.1.0/tackerclient/tests/unit/vm/test_vim_utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/v1_0/client.py` & `python-tackerclient-2.1.0/tackerclient/v1_0/client.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tackerclient/version.py` & `python-tackerclient-2.1.0/tackerclient/version.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tools/tacker.bash_completion` & `python-tackerclient-2.1.0/tools/tacker.bash_completion`

 * *Files identical despite different names*

### Comparing `python-tackerclient-2.0.0/tox.ini` & `python-tackerclient-2.1.0/tox.ini`

 * *Files identical despite different names*

