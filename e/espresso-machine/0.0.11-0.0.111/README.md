# Comparing `tmp/espresso_machine-0.0.11.tar.gz` & `tmp/espresso_machine-0.0.111.tar.gz`

## Comparing `espresso_machine-0.0.11.tar` & `espresso_machine-0.0.111.tar`

### file list

```diff
@@ -1,220 +1,220 @@
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/FeO.ipynb
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/MaterialsProject.ipynb
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/MnPS3-yaml.ipynb
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/MnPS3.ipynb
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/NbSe2.ipynb
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Notebook.ipynb
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Si_parameter_test.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/config.json
--rw-r--r--   0        0        0   403768 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/plot.ipynb
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/requirements.txt
--rw-r--r--   0        0        0    47832 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/test.ipynb
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Structures/Al.poscar
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Structures/C.poscar
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Structures/Fe.poscar
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Structures/FeO.poscar
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Structures/MnPS3.poscar
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Structures/NbSe2.poscar
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Structures/Si.poscar
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Structures/UTe2.poscar
--rw-r--r--   0        0        0    84382 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/1-Si-Band.ipynb
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/2-Si-DOS.ipynb
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/3-Si-PDOS.ipynb
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/4-Si-KDOS.ipynb
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/5-Al-PDOS.ipynb
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/5-Fe-DOS.ipynb
--rw-r--r--   0        0        0   286684 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/6-Fe-Band.ipynb
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/C_electron_band.ipynb
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/Tutorials/C_phonon_band.ipynb
--rw-r--r--   0        0        0    90193 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/NC/Al.UPF
--rw-r--r--   0        0        0    90153 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/NC/C.UPF
--rw-r--r--   0        0        0   115566 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/NC/Nb.UPF
--rw-r--r--   0        0        0   115528 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/NC/Se.UPF
--rw-r--r--   0        0        0    90193 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/NC/Si.UPF
--rw-r--r--   0        0        0  1308566 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/US/Al.UPF
--rw-r--r--   0        0        0   606527 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/US/Co.UPF
--rw-r--r--   0        0        0  1431019 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/US/Fe.UPF
--rw-r--r--   0        0        0  1426269 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/US/Mn.UPF
--rw-r--r--   0        0        0   376736 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/US/O.UPF
--rw-r--r--   0        0        0  1322288 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/US/P.UPF
--rw-r--r--   0        0        0  1326847 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/US/S.UPF
--rw-r--r--   0        0        0  1315428 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pseudos/US/Si.UPF
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/__init__.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/adiabatic.sh
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/check.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/compute.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/generate.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/kpoints.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/ph.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/ph_plot.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/plot_band.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/plot_sigma_energy.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/plots.py
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/project.py
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/reads.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/run.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/scaffold.py
--rw-r--r--   0        0        0    11762 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/structure.py
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/utils.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/writes.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/__init__.py
--rw-r--r--   0        0        0    26349 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/getpaths.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/brillouinzone/__init__.py
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py
--rw-r--r--   0        0        0    21490 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/__init__.py
--rw-r--r--   0        0        0     9666 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/spg_db.py
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/spg_mapping.py
--rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/tools.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/POSCAR_inversion
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/k_vector_parameters.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/path.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/points.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/k_vector_parameters.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/path.txt
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/points.txt
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/k_vector_parameters.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/path.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/points.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/k_vector_parameters.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/path.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/points.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/k_vector_parameters.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/path.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/points.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/path.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/points.txt
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/POSCAR_inversion
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/k_vector_parameters.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/path.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/points.txt
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/path.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/points.txt
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/POSCAR_inversion
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/k_vector_parameters.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/path.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/points.txt
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/k_vector_parameters.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/path.txt
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/points.txt
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/k_vector_parameters.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/path.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/points.txt
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/k_vector_parameters.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/path.txt
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/points.txt
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/k_vector_parameters.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/path.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/points.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/k_vector_parameters.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/path.txt
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/points.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_inversion
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/path.txt
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/points.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/k_vector_parameters.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/path.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/points.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/k_vector_parameters.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/path.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/points.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/POSCAR_inversion
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/k_vector_parameters.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/path.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/points.txt
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/k_vector_parameters.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/path.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/points.txt
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/k_vector_parameters.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/path.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/points.txt
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/k_vector_parameters.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/path.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/points.txt
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/k_vector_parameters.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/path.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/points.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/k_vector_parameters.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/path.txt
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/points.txt
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/k_vector_parameters.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/path.txt
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/points.txt
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion_alternate
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/k_vector_parameters.txt
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/path.txt
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/points.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/POSCAR_inversion
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/path.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/points.txt
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/k_vector_parameters.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/path.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/points.txt
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/POSCAR_inversion
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/POSCAR_noinversion
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/k_vector_parameters.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/path.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/points.txt
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/POSCAR_inversion
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/POSCAR_noinversion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/k_vector_parameters.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/path.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/points.txt
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/LICENSE
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/pyproject.toml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 espresso_machine-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/FeO.ipynb
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/MaterialsProject.ipynb
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/MnPS3-yaml.ipynb
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/MnPS3.ipynb
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/NbSe2.ipynb
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Notebook.ipynb
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Si_parameter_test.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/config.json
+-rw-r--r--   0        0        0   403768 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/plot.ipynb
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/requirements.txt
+-rw-r--r--   0        0        0    47832 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/test.ipynb
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Structures/Al.poscar
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Structures/C.poscar
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Structures/Fe.poscar
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Structures/FeO.poscar
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Structures/MnPS3.poscar
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Structures/NbSe2.poscar
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Structures/Si.poscar
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Structures/UTe2.poscar
+-rw-r--r--   0        0        0    84382 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/1-Si-Band.ipynb
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/2-Si-DOS.ipynb
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/3-Si-PDOS.ipynb
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/4-Si-KDOS.ipynb
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/5-Al-PDOS.ipynb
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/5-Fe-DOS.ipynb
+-rw-r--r--   0        0        0   286684 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/6-Fe-Band.ipynb
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/C_electron_band.ipynb
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/Tutorials/C_phonon_band.ipynb
+-rw-r--r--   0        0        0    90193 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/NC/Al.UPF
+-rw-r--r--   0        0        0    90153 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/NC/C.UPF
+-rw-r--r--   0        0        0   115566 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/NC/Nb.UPF
+-rw-r--r--   0        0        0   115528 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/NC/Se.UPF
+-rw-r--r--   0        0        0    90193 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/NC/Si.UPF
+-rw-r--r--   0        0        0  1308566 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/US/Al.UPF
+-rw-r--r--   0        0        0   606527 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/US/Co.UPF
+-rw-r--r--   0        0        0  1431019 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/US/Fe.UPF
+-rw-r--r--   0        0        0  1426269 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/US/Mn.UPF
+-rw-r--r--   0        0        0   376736 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/US/O.UPF
+-rw-r--r--   0        0        0  1322288 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/US/P.UPF
+-rw-r--r--   0        0        0  1326847 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/US/S.UPF
+-rw-r--r--   0        0        0  1315428 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pseudos/US/Si.UPF
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/__init__.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/adiabatic.sh
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/check.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/compute.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/generate.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/kpoints.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/ph.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/ph_plot.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/plot_band.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/plot_sigma_energy.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/plots.py
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/project.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/reads.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/run.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/scaffold.py
+-rw-r--r--   0        0        0    11762 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/structure.py
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/utils.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/writes.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/__init__.py
+-rw-r--r--   0        0        0    26349 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/getpaths.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/brillouinzone/__init__.py
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py
+-rw-r--r--   0        0        0    21490 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/__init__.py
+-rw-r--r--   0        0        0     9666 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/spg_db.py
+-rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/spg_mapping.py
+-rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/tools.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/POSCAR_inversion
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/path.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP2/points.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/k_vector_parameters.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/path.txt
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/points.txt
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/path.txt
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/points.txt
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/path.txt
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/points.txt
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/path.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/points.txt
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/path.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/points.txt
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/POSCAR_inversion
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/path.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/points.txt
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/path.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/points.txt
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/POSCAR_inversion
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/path.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP2/points.txt
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/path.txt
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/points.txt
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/path.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/points.txt
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/path.txt
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/points.txt
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/path.txt
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/points.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/k_vector_parameters.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/path.txt
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/points.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_inversion
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/path.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/points.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/path.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/points.txt
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/path.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/points.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/POSCAR_inversion
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/path.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/points.txt
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/path.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/points.txt
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/path.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/points.txt
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/path.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/points.txt
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/k_vector_parameters.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/path.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/points.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/path.txt
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/points.txt
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/path.txt
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/points.txt
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion_alternate
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/k_vector_parameters.txt
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/path.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/points.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/POSCAR_inversion
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/path.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oP1/points.txt
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/path.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/points.txt
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/POSCAR_inversion
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/POSCAR_noinversion
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/k_vector_parameters.txt
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/path.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI2/points.txt
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/POSCAR_inversion
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/POSCAR_noinversion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/k_vector_parameters.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/path.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tP1/points.txt
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/LICENSE
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/README.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/pyproject.toml
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 espresso_machine-0.0.111/PKG-INFO
```

### Comparing `espresso_machine-0.0.11/FeO.ipynb` & `espresso_machine-0.0.111/FeO.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/MaterialsProject.ipynb` & `espresso_machine-0.0.111/MaterialsProject.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/MnPS3-yaml.ipynb` & `espresso_machine-0.0.111/MnPS3-yaml.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/MnPS3.ipynb` & `espresso_machine-0.0.111/MnPS3.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/NbSe2.ipynb` & `espresso_machine-0.0.111/NbSe2.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Notebook.ipynb` & `espresso_machine-0.0.111/Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Si_parameter_test.ipynb` & `espresso_machine-0.0.111/Si_parameter_test.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/config.json` & `espresso_machine-0.0.111/config.json`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/plot.ipynb` & `espresso_machine-0.0.111/plot.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/requirements.txt` & `espresso_machine-0.0.111/requirements.txt`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/test.ipynb` & `espresso_machine-0.0.111/test.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Structures/MnPS3.poscar` & `espresso_machine-0.0.111/Structures/MnPS3.poscar`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Structures/NbSe2.poscar` & `espresso_machine-0.0.111/Structures/NbSe2.poscar`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Structures/Si.poscar` & `espresso_machine-0.0.111/Structures/Si.poscar`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Structures/UTe2.poscar` & `espresso_machine-0.0.111/Structures/UTe2.poscar`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/1-Si-Band.ipynb` & `espresso_machine-0.0.111/Tutorials/1-Si-Band.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/2-Si-DOS.ipynb` & `espresso_machine-0.0.111/Tutorials/2-Si-DOS.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/3-Si-PDOS.ipynb` & `espresso_machine-0.0.111/Tutorials/3-Si-PDOS.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/4-Si-KDOS.ipynb` & `espresso_machine-0.0.111/Tutorials/4-Si-KDOS.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/5-Al-PDOS.ipynb` & `espresso_machine-0.0.111/Tutorials/5-Al-PDOS.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/5-Fe-DOS.ipynb` & `espresso_machine-0.0.111/Tutorials/5-Fe-DOS.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/6-Fe-Band.ipynb` & `espresso_machine-0.0.111/Tutorials/6-Fe-Band.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/C_electron_band.ipynb` & `espresso_machine-0.0.111/Tutorials/C_electron_band.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/Tutorials/C_phonon_band.ipynb` & `espresso_machine-0.0.111/Tutorials/C_phonon_band.ipynb`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/NC/Al.UPF` & `espresso_machine-0.0.111/pseudos/NC/Al.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/NC/C.UPF` & `espresso_machine-0.0.111/pseudos/NC/C.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/NC/Nb.UPF` & `espresso_machine-0.0.111/pseudos/NC/Nb.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/NC/Se.UPF` & `espresso_machine-0.0.111/pseudos/NC/Se.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/NC/Si.UPF` & `espresso_machine-0.0.111/pseudos/NC/Si.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/US/Al.UPF` & `espresso_machine-0.0.111/pseudos/US/Al.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/US/Co.UPF` & `espresso_machine-0.0.111/pseudos/US/Co.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/US/Fe.UPF` & `espresso_machine-0.0.111/pseudos/US/Fe.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/US/Mn.UPF` & `espresso_machine-0.0.111/pseudos/US/Mn.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/US/O.UPF` & `espresso_machine-0.0.111/pseudos/US/O.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/US/P.UPF` & `espresso_machine-0.0.111/pseudos/US/P.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/US/S.UPF` & `espresso_machine-0.0.111/pseudos/US/S.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pseudos/US/Si.UPF` & `espresso_machine-0.0.111/pseudos/US/Si.UPF`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/adiabatic.sh` & `espresso_machine-0.0.111/src/espresso_machine/adiabatic.sh`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/compute.py` & `espresso_machine-0.0.111/src/espresso_machine/compute.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/generate.py` & `espresso_machine-0.0.111/src/espresso_machine/generate.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/kpoints.py` & `espresso_machine-0.0.111/src/espresso_machine/kpoints.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/ph.py` & `espresso_machine-0.0.111/src/espresso_machine/ph.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/ph_plot.py` & `espresso_machine-0.0.111/src/espresso_machine/ph_plot.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/plot_band.py` & `espresso_machine-0.0.111/src/espresso_machine/plot_band.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/plot_sigma_energy.py` & `espresso_machine-0.0.111/src/espresso_machine/plot_sigma_energy.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/plots.py` & `espresso_machine-0.0.111/src/espresso_machine/plots.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/project.py` & `espresso_machine-0.0.111/src/espresso_machine/project.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/reads.py` & `espresso_machine-0.0.111/src/espresso_machine/reads.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/run.py` & `espresso_machine-0.0.111/src/espresso_machine/run.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/scaffold.py` & `espresso_machine-0.0.111/src/espresso_machine/scaffold.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/structure.py` & `espresso_machine-0.0.111/src/espresso_machine/structure.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/utils.py` & `espresso_machine-0.0.111/src/espresso_machine/utils.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/writes.py` & `espresso_machine-0.0.111/src/espresso_machine/writes.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/__init__.py` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/__init__.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/getpaths.py` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/getpaths.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/util.py` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/util.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/__init__.py` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/__init__.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/spg_db.py` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/spg_db.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/spg_mapping.py` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/spg_mapping.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/tools.py` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/tools.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion` & `espresso_machine-0.0.111/src/espresso_machine/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/.gitignore` & `espresso_machine-0.0.111/.gitignore`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/LICENSE` & `espresso_machine-0.0.111/LICENSE`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.11/pyproject.toml` & `espresso_machine-0.0.111/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "espresso-machine"
-version = "0.0.11"
+version = "0.0.111"
 authors = [
   { name="Susy Exists", email="susy@selectron.me" },
 ]
 description = "Quantum Espresso automation tool"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-  "numpy","matplotlib"
+  "numpy","matplotlib","pandas"
 ]
 
 [project.urls]
 Homepage = "https://github.com/susyexstsi/espresso-machine"
```

### Comparing `espresso_machine-0.0.11/PKG-INFO` & `espresso_machine-0.0.111/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: espresso-machine
-Version: 0.0.11
+Version: 0.0.111
 Summary: Quantum Espresso automation tool
 Project-URL: Homepage, https://github.com/susyexstsi/espresso-machine
 Author-email: Susy Exists <susy@selectron.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: pandas
 Description-Content-Type: text/markdown
 
 # Espresso Machine
 Automation library for Quantum Espresso via python
 
 # Start by executing adiabatic.sh
 Edit parameters in the file for local environment. Such as HPC parameters, python, MPI, Quantum Espresso directories
```

