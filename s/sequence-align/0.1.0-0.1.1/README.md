# Comparing `tmp/sequence_align-0.1.0-cp37-abi3-win_amd64.whl.zip` & `tmp/sequence_align-0.1.1-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 115771 bytes, number of entries: 10
--rw-r--r--  4.6 unx     7414 b- defN 23-Apr-05 19:34 sequence_align-0.1.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-05 19:34 sequence_align-0.1.0.dist-info/WHEEL
--rw-r--r--  4.6 unx    11566 b- defN 23-Apr-05 19:34 sequence_align-0.1.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    11566 b- defN 23-Apr-05 19:34 sequence_align-0.1.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx       59 b- defN 23-Apr-05 19:34 sequence_align-0.1.0.dist-info/license_files/AUTHORS.md
--rw-r--r--  4.6 unx     6792 b- defN 23-Apr-05 19:34 sequence_align/pairwise.py
--rw-r--r--  4.6 unx        0 b- defN 23-Apr-05 19:34 sequence_align/py.typed
--rw-r--r--  4.6 unx        0 b- defN 23-Apr-05 19:34 sequence_align/__init__.py
--rwxr-xr-x  4.6 unx   209408 b- defN 23-Apr-05 19:34 sequence_align/_sequence_align.pyd
--rw-r--r--  4.6 unx      890 b- defN 23-Apr-05 19:34 sequence_align-0.1.0.dist-info/RECORD
-10 files, 247791 bytes uncompressed, 114229 bytes compressed:  53.9%
+Zip file size: 110645 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     7495 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11566 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    11566 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx       59 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/license_files/AUTHORS.md
+-rw-r--r--  4.6 unx     6792 b- defN 24-May-02 14:46 sequence_align/pairwise.py
+-rw-r--r--  4.6 unx        0 b- defN 24-May-02 14:46 sequence_align/py.typed
+-rw-r--r--  4.6 unx        0 b- defN 24-May-02 14:46 sequence_align/__init__.py
+-rwxr-xr-x  4.6 unx   195072 b- defN 24-May-02 14:46 sequence_align/sequence_align.pyd
+-rw-r--r--  4.6 unx      889 b- defN 24-May-02 14:46 sequence_align-0.1.1.dist-info/RECORD
+10 files, 233533 bytes uncompressed, 109105 bytes compressed:  53.3%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: sequence_align-0.1.0.dist-info/METADATA
+Filename: sequence_align-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sequence_align-0.1.0.dist-info/WHEEL
+Filename: sequence_align-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sequence_align-0.1.0.dist-info/license_files/LICENSE
+Filename: sequence_align-0.1.1.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: sequence_align-0.1.0.dist-info/license_files/LICENSE
+Filename: sequence_align-0.1.1.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: sequence_align-0.1.0.dist-info/license_files/AUTHORS.md
+Filename: sequence_align-0.1.1.dist-info/license_files/AUTHORS.md
 Comment: 
 
 Filename: sequence_align/pairwise.py
 Comment: 
 
 Filename: sequence_align/py.typed
 Comment: 
 
 Filename: sequence_align/__init__.py
 Comment: 
 
-Filename: sequence_align/_sequence_align.pyd
+Filename: sequence_align/sequence_align.pyd
 Comment: 
 
-Filename: sequence_align-0.1.0.dist-info/RECORD
+Filename: sequence_align-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sequence_align-0.1.0.dist-info/METADATA` & `sequence_align-0.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sequence_align
-Version: 0.1.0
-Classifier: License :: OSI Approved :: Apache Software License
+Version: 0.1.1
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Typing :: Typed
-Requires-Dist: bandit; extra == 'dev'
-Requires-Dist: black; extra == 'dev'
-Requires-Dist: codecov; extra == 'dev'
-Requires-Dist: flake8; extra == 'dev'
-Requires-Dist: isort>=5.0.0,<6; extra == 'dev'
-Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: pydocstyle; extra == 'dev'
-Requires-Dist: pylint; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: bandit ; extra == 'dev'
+Requires-Dist: black ; extra == 'dev'
+Requires-Dist: flake8 ; extra == 'dev'
+Requires-Dist: isort >=5.0.0, <6 ; extra == 'dev'
+Requires-Dist: mypy ; extra == 'dev'
+Requires-Dist: psutil ; extra == 'dev'
+Requires-Dist: pydocstyle ; extra == 'dev'
+Requires-Dist: pylint ; extra == 'dev'
+Requires-Dist: pytest ; extra == 'dev'
+Requires-Dist: pytest-cov ; extra == 'dev'
+Requires-Dist: pyyaml ; extra == 'dev'
+Requires-Dist: types-psutil ; extra == 'dev'
+Requires-Dist: types-pyyaml ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 License-File: LICENSE
 License-File: AUTHORS.md
 Summary: Efficient implementations of Needleman-Wunsch and other sequence alignment algorithms in Rust with Python bindings.
-Author-email: Kensho Technologies LLC. <sequence-align-maintainer@kensho.com>
-Maintainer-email: Kensho Technologies LLC. <sequence-align-maintainer@kensho.com>
+Author-email: "Kensho Technologies LLC." <sequence-align-maintainer@kensho.com>
+Maintainer-email: "Kensho Technologies LLC." <sequence-align-maintainer@kensho.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: source, https://github.com/kensho-technologies/sequence_align
 Project-URL: Homepage, https://github.com/kensho-technologies/sequence_align
 Project-URL: Bug Tracker, https://github.com/kensho-technologies/sequence_align/issues
-Project-URL: source, https://github.com/kensho-technologies/sequence_align
 
   <a href="https://github.com/kensho-technologies/sequence_align/actions?query=workflow%3A%22Tests+and+lint%22"><img src="https://github.com/kensho-technologies/sequence_align/workflows/Tests%20and%20lint/badge.svg" /></a>
   <a href="https://codecov.io/gh/kensho-technologies/sequence_align"><img src="https://codecov.io/gh/kensho-technologies/sequence_align/branch/main/graph/badge.svg" /></a>
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" /></a>
   <a href="http://www.repostatus.org/#active"><img src="http://www.repostatus.org/badges/latest/active.svg" /></a>
   <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
```

### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: sequence_align Version: 0.1.0 Classifier: License
-:: OSI Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language :: Rust
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Classifier:
-Typing :: Typed Requires-Dist: bandit; extra == 'dev' Requires-Dist: black;
-extra == 'dev' Requires-Dist: codecov; extra == 'dev' Requires-Dist: flake8;
-extra == 'dev' Requires-Dist: isort>=5.0.0,<6; extra == 'dev' Requires-Dist:
-mypy; extra == 'dev' Requires-Dist: pydocstyle; extra == 'dev' Requires-Dist:
-pylint; extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist:
-pytest-cov; extra == 'dev' Provides-Extra: dev License-File: LICENSE License-
-File: LICENSE License-File: AUTHORS.md Summary: Efficient implementations of
+Metadata-Version: 2.3 Name: sequence_align Version: 0.1.1 Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Rust Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Typing :: Typed Requires-Dist: bandit ; extra == 'dev' Requires-
+Dist: black ; extra == 'dev' Requires-Dist: flake8 ; extra == 'dev' Requires-
+Dist: isort >=5.0.0, <6 ; extra == 'dev' Requires-Dist: mypy ; extra == 'dev'
+Requires-Dist: psutil ; extra == 'dev' Requires-Dist: pydocstyle ; extra ==
+'dev' Requires-Dist: pylint ; extra == 'dev' Requires-Dist: pytest ; extra ==
+'dev' Requires-Dist: pytest-cov ; extra == 'dev' Requires-Dist: pyyaml ; extra
+== 'dev' Requires-Dist: types-psutil ; extra == 'dev' Requires-Dist: types-
+pyyaml ; extra == 'dev' Provides-Extra: dev License-File: LICENSE License-File:
+LICENSE License-File: AUTHORS.md Summary: Efficient implementations of
 Needleman-Wunsch and other sequence alignment algorithms in Rust with Python
-bindings. Author-email: Kensho Technologies LLC.
-kensho.com> Maintainer-email: Kensho Technologies LLC.
+bindings. Author-email: "Kensho Technologies LLC."
+kensho.com> Maintainer-email: "Kensho Technologies LLC."
 kensho.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Homepage, https://github.com/kensho-
+charset=UTF-8; variant=GFM Project-URL: source, https://github.com/kensho-
+technologies/sequence_align Project-URL: Homepage, https://github.com/kensho-
 technologies/sequence_align Project-URL: Bug Tracker, https://github.com/
-kensho-technologies/sequence_align/issues Project-URL: source, https://
-github.com/kensho-technologies/sequence_align _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_k_e_n_s_h_o_-
+kensho-technologies/sequence_align/issues _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_k_e_n_s_h_o_-
 _t_e_c_h_n_o_l_o_g_i_e_s_/_s_e_q_u_e_n_c_e___a_l_i_g_n_/_w_o_r_k_f_l_o_w_s_/_T_e_s_t_s_%_2_0_a_n_d_%_2_0_l_i_n_t_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
 _c_o_d_e_c_o_v_._i_o_/_g_h_/_k_e_n_s_h_o_-_t_e_c_h_n_o_l_o_g_i_e_s_/_s_e_q_u_e_n_c_e___a_l_i_g_n_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_:_/_/
 _w_w_w_._r_e_p_o_s_t_a_t_u_s_._o_r_g_/_b_a_d_g_e_s_/_l_a_t_e_s_t_/_a_c_t_i_v_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
 _c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]# sequence_align Efficient implementations of
 [Needleman-Wunsch](https://en.wikipedia.org/wiki/
 Needleman%E2%80%93Wunsch_algorithm) and other sequence alignment algorithms
```

## Comparing `sequence_align-0.1.0.dist-info/license_files/LICENSE` & `sequence_align-0.1.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `sequence_align-0.1.0.dist-info/RECORD` & `sequence_align-0.1.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-sequence_align-0.1.0.dist-info/METADATA,sha256=v_CSWOUOJo-mU9IzQNJY20bZvQWqtD692FY62zVmGMY,7414
-sequence_align-0.1.0.dist-info/WHEEL,sha256=Rr1U4WCl0doeAIMYogh8nyAkPDjFceOWTG2inGYI8Eo,96
-sequence_align-0.1.0.dist-info/license_files/LICENSE,sha256=j9q0KoZXpK8fT1GXnUEV0DfgbGQv8XIn35OREXVn920,11566
-sequence_align-0.1.0.dist-info/license_files/LICENSE,sha256=j9q0KoZXpK8fT1GXnUEV0DfgbGQv8XIn35OREXVn920,11566
-sequence_align-0.1.0.dist-info/license_files/AUTHORS.md,sha256=zgfGnnTADSip5x0UBLZc4zlz8y5MHAa7c40hrPBddqE,59
+sequence_align-0.1.1.dist-info/METADATA,sha256=NUkXPf4LKZ4o8QoZ6f1XDBTjD8YNY2zbX6lN9nod_JI,7495
+sequence_align-0.1.1.dist-info/WHEEL,sha256=2KdwICnFEHl2ghwQAXqeXd9gNxeAiTvogEqUIMDbYbo,94
+sequence_align-0.1.1.dist-info/license_files/LICENSE,sha256=j9q0KoZXpK8fT1GXnUEV0DfgbGQv8XIn35OREXVn920,11566
+sequence_align-0.1.1.dist-info/license_files/LICENSE,sha256=j9q0KoZXpK8fT1GXnUEV0DfgbGQv8XIn35OREXVn920,11566
+sequence_align-0.1.1.dist-info/license_files/AUTHORS.md,sha256=zgfGnnTADSip5x0UBLZc4zlz8y5MHAa7c40hrPBddqE,59
 sequence_align/pairwise.py,sha256=Mji0Easoy3nQpWD5BAwOwHnnlRu95SLjy9Cvb2IMV98,6792
 sequence_align/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sequence_align/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sequence_align/_sequence_align.pyd,sha256=3g-NnsaiV4JNxV6k_jvdWHJ-HsFo5h05rB_YhAg0pHA,209408
-sequence_align-0.1.0.dist-info/RECORD,,
+sequence_align/sequence_align.pyd,sha256=HjlBz3kMHLjOtez02mRElgrTzwYHUYT807mQvlQ_MKE,195072
+sequence_align-0.1.1.dist-info/RECORD,,
```

