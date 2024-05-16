# Comparing `tmp/pyLIQTR-1.0.1.tar.gz` & `tmp/pyliqtr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLIQTR-1.0.1.tar", last modified: Fri Mar  1 19:25:52 2024, max compression
+gzip compressed data, was "pyliqtr-1.2.0.tar", last modified: Thu May 16 21:17:49 2024, max compression
```

## Comparing `pyLIQTR-1.0.1.tar` & `pyliqtr-1.2.0.tar`

### file list

```diff
@@ -1,166 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.815991 pyLIQTR-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-03-01 19:25:52.815991 pyLIQTR-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 19:25:52.815991 pyLIQTR-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.787991 pyLIQTR-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.791991 pyLIQTR-1.0.1/src/pyLIQTR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.791991 pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/BlockEncoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/LinearT.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/PauliStringLCU.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/fermi_hubbard_square_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/getEncoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.795991 pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/pe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/pe_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/pe_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.795991 pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.795991 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/ChemicalHamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/ElectronicStructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/LatticeInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/MatrixInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/ProblemInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/fermionic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/getInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/spin_models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.795991 pyLIQTR-1.0.1/src/pyLIQTR/circuits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.799991 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/AddMod.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/hamiltonian_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/multiCZ.py
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)    16549 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/prepare_LinearT.py
--rw-r--r--   0 runner    (1001) docker     (127)    21153 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/prepare_oracle_pauli_lcu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/reflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/selectV.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/selectVutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/select_LinearT.py
--rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/select_oracle_pauli_lcu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/select_prepare_pauli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.799991 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/test_hamiltonian_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/test_multiCZ.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/test_reflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/test_selectV.py
--rw-r--r--   0 runner    (1001) docker     (127)    15966 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/pyLCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/pyLOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/qsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.799991 pyLIQTR-1.0.1/src/pyLIQTR/circuits/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/tests/test_pyLCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/circuits/tests/test_pyLOperator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.803991 pyLIQTR-1.0.1/src/pyLIQTR/clam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/atomic_lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/cell_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/lattice_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.803991 pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/burgers_nonlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)    15832 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/linearization_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/multilinear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/vlasov_spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/multilinear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/operator_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)    21948 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/operator_lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/operator_sims.py
--rw-r--r--   0 runner    (1001) docker     (127)    18995 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/operator_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/physical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/simqsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/tensor_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.803991 pyLIQTR-1.0.1/src/pyLIQTR/clam/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/time_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/clam/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.807991 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26557 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/cirq_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/clifford_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/exact_decomp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/gate_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/grid_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    25862 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/point_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/rings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/rotation_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/solve_diophantine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.807991 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    25311 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_cirq_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_exact_decomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    20825 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_point_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_solve_diophantine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.807991 pyLIQTR-1.0.1/src/pyLIQTR/pest_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/pest_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/pest_interface/pest_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.811991 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/angler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.811991 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/fourier_response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/fourier_response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/fourier_response/fourier_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/named_factors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.811991 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/ChebyshevPoly.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19912 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/angler_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/expander.py
--rw-r--r--   0 runner    (1001) docker     (127)    16141 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/fitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/phase_factors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.811991 pyLIQTR-1.0.1/src/pyLIQTR/qubitization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/qubitization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/qubitization/phase_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19346 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/qubitization/qsvt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/qubitization/qsvt_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/qubitization/qubitized_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.811991 pyLIQTR-1.0.1/src/pyLIQTR/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/tests/test_cirq_ft_resource_analyze_multiple_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/tests/test_cirq_ft_resource_analyze_single_gate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.815991 pyLIQTR-1.0.1/src/pyLIQTR/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/Hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/circuit_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/get_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/pauli_string_manip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/plot_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/qsp_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/resource_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.815991 pyLIQTR-1.0.1/src/pyLIQTR/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/tests/test_resoure_analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-03-01 19:25:39.000000 pyLIQTR-1.0.1/src/pyLIQTR/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 19:25:52.815991 pyLIQTR-1.0.1/src/pyLIQTR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-03-01 19:25:52.000000 pyLIQTR-1.0.1/src/pyLIQTR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-01 19:25:52.000000 pyLIQTR-1.0.1/src/pyLIQTR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 19:25:52.000000 pyLIQTR-1.0.1/src/pyLIQTR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-01 19:25:52.000000 pyLIQTR-1.0.1/src/pyLIQTR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-01 19:25:52.000000 pyLIQTR-1.0.1/src/pyLIQTR.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.560864 pyliqtr-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-05-16 21:17:49.560864 pyliqtr-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:17:49.560864 pyliqtr-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.528864 pyliqtr-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.532863 pyliqtr-1.2.0/src/pyLIQTR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.536863 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/BlockEncoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14114 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/CarlemanLinearization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22071 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/DoubleFactorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/LinearT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/PauliStringLCU.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/fermi_hubbard_square_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/getEncoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.536863 pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/pe_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/pe_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.536863 pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.536863 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/
+-rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/ChemicalHamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/ElectronicStructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/LatticeInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/MatrixInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/NonlinearODE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/ProblemInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/fermionic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/getInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/spin_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.536863 pyliqtr-1.2.0/src/pyLIQTR/circuits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.544864 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/AddMod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/BinaryToUnary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/BitwiseZRotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/ControlledUniformSuperposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/DF_InnerPrepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/DF_OuterPrepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/DF_RotationsBlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/ExampleFMatrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/FixupTableQROM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/FlaggedPrepareUniformSuperposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/PhaseGradientRotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/ProductPauliExponentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/QROMwithMeasurementUncompute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/RotationsQROM.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/cascading_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/cyclic_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/diagonal_bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/hamiltonian_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/multiCZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17036 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/prepare_LinearT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21153 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/prepare_oracle_pauli_lcu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/reflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/selectV.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/selectVutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/select_LinearT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/select_oracle_pauli_lcu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/select_prepare_pauli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/swap_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.544864 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_BinaryToUnary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_DataAndKeyCondition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_PhaseGradientRotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_ProductPauliExponentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_QROMwithMeasurementUncompute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_RotationsQROM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_cyclic_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_diagonal_bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_hamiltonian_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_multiCZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_qtAdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_reflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_selectV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15984 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/pyLCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/pyLOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/qsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.544864 pyliqtr-1.2.0/src/pyLIQTR/circuits/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/tests/test_pyLCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/circuits/tests/test_pyLOperator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.548864 pyliqtr-1.2.0/src/pyLIQTR/clam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/atomic_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/cell_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/lattice_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.548864 pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/burgers_nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15832 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/linearization_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/multilinear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/vlasov_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/multilinear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/operator_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21948 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/operator_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/operator_sims.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18995 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/operator_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/physical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/simqsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/tensor_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.548864 pyliqtr-1.2.0/src/pyLIQTR/clam/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/time_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/clam/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.552864 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26557 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/cirq_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/clifford_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/exact_decomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/gate_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/grid_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25862 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/point_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/rings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/rotation_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/solve_diophantine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.552864 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25311 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_cirq_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_exact_decomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20825 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_point_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_solve_diophantine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.552864 pyliqtr-1.2.0/src/pyLIQTR/pest_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/pest_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/pest_interface/pest_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.552864 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/angler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.552864 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/fourier_response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/fourier_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/fourier_response/fourier_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/named_factors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.556864 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/ChebyshevPoly.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19912 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/angler_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/expander.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16141 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/fitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/phase_factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/phase_factors/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.556864 pyliqtr-1.2.0/src/pyLIQTR/qubitization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/qubitization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-16 21:17:35.000000 pyliqtr-1.2.0/src/pyLIQTR/qubitization/phase_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/qubitization/qsvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/qubitization/qsvt_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13596 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/qubitization/qubitized_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.556864 pyliqtr-1.2.0/src/pyLIQTR/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/tests/test_qualtran_resource_analyze_multiple_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/tests/test_qualtran_resource_analyze_single_gate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.556864 pyliqtr-1.2.0/src/pyLIQTR/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/Hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/circuit_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/df_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/get_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/global_ancilla_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/pauli_string_manip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/qsp_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/resource_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.556864 pyliqtr-1.2.0/src/pyLIQTR/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/tests/test_resoure_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-16 21:17:36.000000 pyliqtr-1.2.0/src/pyLIQTR/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:17:49.556864 pyliqtr-1.2.0/src/pyLIQTR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-05-16 21:17:49.000000 pyliqtr-1.2.0/src/pyLIQTR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-05-16 21:17:49.000000 pyliqtr-1.2.0/src/pyLIQTR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:17:49.000000 pyliqtr-1.2.0/src/pyLIQTR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-16 21:17:49.000000 pyliqtr-1.2.0/src/pyLIQTR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 21:17:49.000000 pyliqtr-1.2.0/src/pyLIQTR.egg-info/top_level.txt
```

### Comparing `pyLIQTR-1.0.1/LICENSE.txt` & `pyliqtr-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/PKG-INFO` & `pyliqtr-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pyLIQTR
-Version: 1.0.1
+Version: 1.2.0
 Summary: A python package for generating quantum circuits using quantum algorithms.
 Author: Kevin Obenland, Justin Elenewski, Arthur Kurlej,  Joe Belarge, John Blue, and Robert Rood
 Author-email: Kevin.Obenland@ll.mit.edu
 License: BDS-2
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: cirq-core==1.3.0.dev20231102230836
-Requires-Dist: cirq-ft==1.3.0.dev20231102230836
-Requires-Dist: cirq-google==1.3.0.dev20231102230836
+Requires-Dist: cirq-core==1.3.0.dev20231018023458
+Requires-Dist: qualtran==0.2.0
+Requires-Dist: ipykernel
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: scipy
+Requires-Dist: scipy<1.13.0
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: openfermion
 Requires-Dist: portalocker
 Requires-Dist: ply
 Requires-Dist: gmpy2
 Requires-Dist: networkx
+Requires-Dist: juliacall
+Requires-Dist: juliapkg
 Provides-Extra: dev
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: jupyterlab; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
@@ -35,121 +37,142 @@
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: pypandoc; extra == "dev"
 Requires-Dist: recommonmark; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 
 # pyLIQTR
-_Kevin Obenland, Justin Elenewski, Kaitlyn Morrell, Rylee Neumann, Arthur Kurlej, Robert Rood, John Blue, Joe Belarge & Parker Kuklinski_
+
+_Kevin Obenland, Justin Elenewski, Kaitlyn Morrell, Rylee Stuart Neumann, Arthur Kurlej, Robert Rood, John Blue, Joe Belarge, Benjamin Rempfer & Parker Kuklinski_
 
 ---
+
 ## Description
-`pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms and generating Clifford+T resource estimates. 
 
-This package is built extensively atop `cirq` & the recent release of `cirq-ft`. 
+`pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms and generating Clifford+T resource estimates.
+
+This package is built extensively atop `cirq` & the recent release of `qualtran`.
 
 pyLIQTR is primarily structured as:
+
 - pyLIQTR.ProblemInstances
-    - A set of code that provides an easy interface (through `pyLIQTR.ProblemInstances.getInstance`) to generate Hamiltonians that capture various physical models of interest.
+  - A set of code that provides an easy interface (through `pyLIQTR.ProblemInstances.getInstance`) to generate Hamiltonians that capture various physical models of interest.
 - pyLIQTR.BlockEncodings
-    - A set of codes that provides an easy interface (through `pyLIQTR.BlockEncodings.getEncoding`) to generate BlockEncodings that encode the action of a ProblemInstance through various different encodings.
+  - A set of codes that provides an easy interface (through `pyLIQTR.BlockEncodings.getEncoding`) to generate BlockEncodings that encode the action of a ProblemInstance through various different encodings.
 - pyLIQTR.clam
-    - A set of code that provides various classical utilities supporting:
-        - Integration of classical ODE’s (following application problems)
-        - Conversion of spin / fermionic Hamiltonians to classical numerics
-        - Simulation of quantum dynamics
-        - Quadratic / Integrable Hamiltonians (fast; polynomial scaling)
-        - General Hamiltonians (exponentially scaling)
-        - Source / Notebooks: This is scattered diffusely throughout the examples (Vlasov, Nonequilibrium, Heisenberg / Hubbard).
+  - A set of code that provides various classical utilities supporting:
+    - Integration of classical ODE’s (following application problems)
+    - Conversion of spin / fermionic Hamiltonians to classical numerics
+    - Simulation of quantum dynamics
+    - Quadratic / Integrable Hamiltonians (fast; polynomial scaling)
+    - General Hamiltonians (exponentially scaling)
+    - Source / Notebooks: This is scattered diffusely throughout the examples (Vlasov, Nonequilibrium, Heisenberg / Hubbard).
 - pyLIQTR.qubitization
-    - A set of code that provides ways of building QSP/QSVT circuits in the context of the pyLIQTR package.
+  - A set of code that provides ways of building QSP/QSVT circuits in the context of the pyLIQTR package.
 - pyLIQTR.phase_factors
-    - A set of code that calculates the angles required for a given QSP/QSVT sequence
+  - A set of code that calculates the angles required for a given QSP/QSVT sequence
 - pyLIQTR.circuits
-    - A set of pyLIQTR cirq circuits/gates used in our implementation of block encodings and algorithms.
+  - A set of pyLIQTR cirq circuits/gates used in our implementation of block encodings and algorithms.
 - pyLIQTR.gate_decomp
-    - A set of code that performs gate synthesis (converting rotations to Clifford+T gates) for a specified precision.
+  - A set of code that performs gate synthesis (converting rotations to Clifford+T gates) for a specified precision.
 - pyLIQTR.pest_interface
-    - A pythonic interface to the PEST Julia package.
+  - A pythonic interface to the PEST Julia package.
 - pyLIQTR.utils
-    - A set of various utility functions. 
-    - `pyLIQTR.utils.resource_analysis.estimate_resources` (adds robust estimation in addition to `cirq_ft.t_complexity`) can be used to determine the Clifford+T cost of any circuit generated with pyLIQTR
-    - `pyLIQTR.utils.circuit_decomposition.circuit_decompose_multi` (adds robust decomposition in addition to `cirq`'s decomposition functions) can be used to decompose circuits to 1+2QB gates
+  - A set of various utility functions.
+  - `pyLIQTR.utils.resource_analysis.estimate_resources` (adds robust estimation in addition to `qualtran.t_complexity`) can be used to determine the Clifford+T cost of any circuit generated with pyLIQTR
+  - `pyLIQTR.utils.circuit_decomposition.circuit_decompose_multi` (adds robust decomposition in addition to `cirq`'s decomposition functions) can be used to decompose circuits to 1+2QB gates
 
 In addition, a seperate Julia package for generating electronic structure hamiltonians (root/PEST) is included with pyLIQTR.
 
 pyLIQTR is a work-in-progress, as time goes on, we hope to provide better and more extensive documentation and examples in addition to new features. Please reach out to us if anything is unclear, so we can prioritize the documentation of the aspects that are most frequently used or most unclear.
 
 ---
+
 ## Features
-The features of this package are described in detail in [FEATURES.md](FEATURES.md). This includes not only descriptions, but also source files and example notebooks.
+
+The features of this package are described in detail in [FEATURES.md](Features.md). This includes not only descriptions, but also source files and example notebooks.
 
 ---
 
 ## Installation and Environment Setup
-It is recommended that conda be used to manage the environment. A setup.py file is included to facilitate this.
+
+- You can install the latest public tagged release from [PYPI](https://pypi.org/project/pyLIQTR/) using pip:
+
+        pip install pyLIQTR
+
+- You can install the latest state of the main branch:
+
+        pip install git+https://github.com/isi-usc-edu/pyLIQTR.git
+
+If you are going to be activelty developing the pyLIQTR source code, it is recommended that conda be used to manage the environment. A setup.py file is included to facilitate this.
 Change directory to the location of setup.py, then perform the following commands.
 
 - Create and activate the environment:
 
         on Windows use:
         conda create -n <Environment Name> "python>=3.8,<=3.11.5"
         on Mac use:
         conda create -n <Environment Name> python'>=3.8,<=3.11.5'
 
         conda activate <Environment Name>
-        
+
 - Install the package
 
         pip install .
 
-- Or, as a developer (for all platforms and shells):
+- If you are working as a developer (for all platforms and shells):
 
+        on Windows use:
+        pip install -e .[dev]
+        on Mac use:
         pip install -e ."[dev]"
-        
+
+<a id="optional-installs"></a>
 ### Optional Installs
-- Install MPSolve polynomial solver, which is used in the angle generation algorithm. Instructions for installation can be found here: https://numpi.dm.unipi.it/software/mpsolve
+
+- Install openfermionpyscf, which is used for the DoubleFactorized block encoding.
+    pip install openfermionpyscf
 - If not installed, then scipy will be used to calculate valid angles. Angle generation using scipy will generally take longer than angle generation using mpsolve.
 Effort is underway to deprecate the existing angle generation in favor of a more portable and efficient method.
-- Install openfermion & pyscf. 
-    - Openfermion is used for the implementation of Suzuki-Trotter and as the input to our implementation of GSE. This is required to use the GSE implementation.
-    - pyscf is used in conjunction with openfermion in order to generate new problem instances as input into our GSE implementation.
+- Install pyscf.
+  - pyscf is used in conjunction with openfermion in order to generate new problem instances as input into our GSE and Double Factorization implementation.
+    pip install pyscf
 
 ---
 
 ## Overview of Examples Included as Jupyter Notebooks
 
 Notebooks showcasing features are organized as follows in the /Examples directory.
+
 - Algorithm_and_Infrastructure
-    - A set of notebooks that go over the ProblemInstance and BlockEncoding infrastructure, in addition to a QSVT/QSP overview. Note that these are still being drafted.
+  - A set of notebooks that go over the ProblemInstance and BlockEncoding infrastructure, in addition to a QSVT/QSP overview. Note that these are still being drafted.
 - AngleGeneration
-    - Contains three notebooks describing the reworked angle generation features
+  - Contains three notebooks describing the reworked angle generation features
 - ApplicationInstances
-    - Contains four directories showing different types of physical models and how one may use the pyLIQTR package to generate circuits and provide resource estimates.
+  - Contains four directories showing different types of physical models and how one may use the pyLIQTR package to generate circuits and provide resource estimates.
 - PEST
-    - An introduction to the generating electronic structure hamiltonians using the PEST package.
+  - An introduction to the generating electronic structure hamiltonians using the PEST package.
+
 ---
 
 ## Citation
-To be populated once code is posted. Cannot create DOI on zenodo without link to repo.
 
-Should generally also include citations of cirq.
+Please use this DOI number reference, published on [Zenodo](https://zenodo.org), when citing the software:
+
+![DOI](image.png)
 
 ---
 
 ## Disclaimer
 
 DISTRIBUTION STATEMENT A. Approved for public release: distribution unlimited.
 
 © 2023 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
-    
+
     Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014)
     SPDX-License-Identifier: BSD-2-Clause
-    
+
 This material is based upon work supported by the Under Secretary of Defense for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Under Secretary of Defense for Research and Engineering.
 
 A portion of this research was sponsored by the United States Air Force Research Laboratory and the United States Air Force Artificial Intelligence Accelerator and was accomplished under Cooperative Agreement Number FA8750-19-2-1000. The views and conclusions contained in this document are those of the authors and should not be interpreted as representing the official policies, either expressed or implied, of the United States Air Force or the U.S. Government. The U.S. Government is authorized to reproduce and distribute reprints for Government purposes notwithstanding any copyright notation herein.
 
 The software/firmware is provided to you on an As-Is basis
-
-
-
```

### Comparing `pyLIQTR-1.0.1/README.md` & `pyliqtr-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,115 +1,136 @@
 # pyLIQTR
-_Kevin Obenland, Justin Elenewski, Kaitlyn Morrell, Rylee Neumann, Arthur Kurlej, Robert Rood, John Blue, Joe Belarge & Parker Kuklinski_
+
+_Kevin Obenland, Justin Elenewski, Kaitlyn Morrell, Rylee Stuart Neumann, Arthur Kurlej, Robert Rood, John Blue, Joe Belarge, Benjamin Rempfer & Parker Kuklinski_
 
 ---
+
 ## Description
-`pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms and generating Clifford+T resource estimates. 
 
-This package is built extensively atop `cirq` & the recent release of `cirq-ft`. 
+`pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms and generating Clifford+T resource estimates.
+
+This package is built extensively atop `cirq` & the recent release of `qualtran`.
 
 pyLIQTR is primarily structured as:
+
 - pyLIQTR.ProblemInstances
-    - A set of code that provides an easy interface (through `pyLIQTR.ProblemInstances.getInstance`) to generate Hamiltonians that capture various physical models of interest.
+  - A set of code that provides an easy interface (through `pyLIQTR.ProblemInstances.getInstance`) to generate Hamiltonians that capture various physical models of interest.
 - pyLIQTR.BlockEncodings
-    - A set of codes that provides an easy interface (through `pyLIQTR.BlockEncodings.getEncoding`) to generate BlockEncodings that encode the action of a ProblemInstance through various different encodings.
+  - A set of codes that provides an easy interface (through `pyLIQTR.BlockEncodings.getEncoding`) to generate BlockEncodings that encode the action of a ProblemInstance through various different encodings.
 - pyLIQTR.clam
-    - A set of code that provides various classical utilities supporting:
-        - Integration of classical ODE’s (following application problems)
-        - Conversion of spin / fermionic Hamiltonians to classical numerics
-        - Simulation of quantum dynamics
-        - Quadratic / Integrable Hamiltonians (fast; polynomial scaling)
-        - General Hamiltonians (exponentially scaling)
-        - Source / Notebooks: This is scattered diffusely throughout the examples (Vlasov, Nonequilibrium, Heisenberg / Hubbard).
+  - A set of code that provides various classical utilities supporting:
+    - Integration of classical ODE’s (following application problems)
+    - Conversion of spin / fermionic Hamiltonians to classical numerics
+    - Simulation of quantum dynamics
+    - Quadratic / Integrable Hamiltonians (fast; polynomial scaling)
+    - General Hamiltonians (exponentially scaling)
+    - Source / Notebooks: This is scattered diffusely throughout the examples (Vlasov, Nonequilibrium, Heisenberg / Hubbard).
 - pyLIQTR.qubitization
-    - A set of code that provides ways of building QSP/QSVT circuits in the context of the pyLIQTR package.
+  - A set of code that provides ways of building QSP/QSVT circuits in the context of the pyLIQTR package.
 - pyLIQTR.phase_factors
-    - A set of code that calculates the angles required for a given QSP/QSVT sequence
+  - A set of code that calculates the angles required for a given QSP/QSVT sequence
 - pyLIQTR.circuits
-    - A set of pyLIQTR cirq circuits/gates used in our implementation of block encodings and algorithms.
+  - A set of pyLIQTR cirq circuits/gates used in our implementation of block encodings and algorithms.
 - pyLIQTR.gate_decomp
-    - A set of code that performs gate synthesis (converting rotations to Clifford+T gates) for a specified precision.
+  - A set of code that performs gate synthesis (converting rotations to Clifford+T gates) for a specified precision.
 - pyLIQTR.pest_interface
-    - A pythonic interface to the PEST Julia package.
+  - A pythonic interface to the PEST Julia package.
 - pyLIQTR.utils
-    - A set of various utility functions. 
-    - `pyLIQTR.utils.resource_analysis.estimate_resources` (adds robust estimation in addition to `cirq_ft.t_complexity`) can be used to determine the Clifford+T cost of any circuit generated with pyLIQTR
-    - `pyLIQTR.utils.circuit_decomposition.circuit_decompose_multi` (adds robust decomposition in addition to `cirq`'s decomposition functions) can be used to decompose circuits to 1+2QB gates
+  - A set of various utility functions.
+  - `pyLIQTR.utils.resource_analysis.estimate_resources` (adds robust estimation in addition to `qualtran.t_complexity`) can be used to determine the Clifford+T cost of any circuit generated with pyLIQTR
+  - `pyLIQTR.utils.circuit_decomposition.circuit_decompose_multi` (adds robust decomposition in addition to `cirq`'s decomposition functions) can be used to decompose circuits to 1+2QB gates
 
 In addition, a seperate Julia package for generating electronic structure hamiltonians (root/PEST) is included with pyLIQTR.
 
 pyLIQTR is a work-in-progress, as time goes on, we hope to provide better and more extensive documentation and examples in addition to new features. Please reach out to us if anything is unclear, so we can prioritize the documentation of the aspects that are most frequently used or most unclear.
 
 ---
+
 ## Features
-The features of this package are described in detail in [FEATURES.md](FEATURES.md). This includes not only descriptions, but also source files and example notebooks.
+
+The features of this package are described in detail in [FEATURES.md](Features.md). This includes not only descriptions, but also source files and example notebooks.
 
 ---
 
 ## Installation and Environment Setup
-It is recommended that conda be used to manage the environment. A setup.py file is included to facilitate this.
+
+- You can install the latest public tagged release from [PYPI](https://pypi.org/project/pyLIQTR/) using pip:
+
+        pip install pyLIQTR
+
+- You can install the latest state of the main branch:
+
+        pip install git+https://github.com/isi-usc-edu/pyLIQTR.git
+
+If you are going to be activelty developing the pyLIQTR source code, it is recommended that conda be used to manage the environment. A setup.py file is included to facilitate this.
 Change directory to the location of setup.py, then perform the following commands.
 
 - Create and activate the environment:
 
         on Windows use:
         conda create -n <Environment Name> "python>=3.8,<=3.11.5"
         on Mac use:
         conda create -n <Environment Name> python'>=3.8,<=3.11.5'
 
         conda activate <Environment Name>
-        
+
 - Install the package
 
         pip install .
 
-- Or, as a developer (for all platforms and shells):
+- If you are working as a developer (for all platforms and shells):
 
+        on Windows use:
+        pip install -e .[dev]
+        on Mac use:
         pip install -e ."[dev]"
-        
+
+<a id="optional-installs"></a>
 ### Optional Installs
-- Install MPSolve polynomial solver, which is used in the angle generation algorithm. Instructions for installation can be found here: https://numpi.dm.unipi.it/software/mpsolve
+
+- Install openfermionpyscf, which is used for the DoubleFactorized block encoding.
+    pip install openfermionpyscf
 - If not installed, then scipy will be used to calculate valid angles. Angle generation using scipy will generally take longer than angle generation using mpsolve.
 Effort is underway to deprecate the existing angle generation in favor of a more portable and efficient method.
-- Install openfermion & pyscf. 
-    - Openfermion is used for the implementation of Suzuki-Trotter and as the input to our implementation of GSE. This is required to use the GSE implementation.
-    - pyscf is used in conjunction with openfermion in order to generate new problem instances as input into our GSE implementation.
+- Install pyscf.
+  - pyscf is used in conjunction with openfermion in order to generate new problem instances as input into our GSE and Double Factorization implementation.
+    pip install pyscf
 
 ---
 
 ## Overview of Examples Included as Jupyter Notebooks
 
 Notebooks showcasing features are organized as follows in the /Examples directory.
+
 - Algorithm_and_Infrastructure
-    - A set of notebooks that go over the ProblemInstance and BlockEncoding infrastructure, in addition to a QSVT/QSP overview. Note that these are still being drafted.
+  - A set of notebooks that go over the ProblemInstance and BlockEncoding infrastructure, in addition to a QSVT/QSP overview. Note that these are still being drafted.
 - AngleGeneration
-    - Contains three notebooks describing the reworked angle generation features
+  - Contains three notebooks describing the reworked angle generation features
 - ApplicationInstances
-    - Contains four directories showing different types of physical models and how one may use the pyLIQTR package to generate circuits and provide resource estimates.
+  - Contains four directories showing different types of physical models and how one may use the pyLIQTR package to generate circuits and provide resource estimates.
 - PEST
-    - An introduction to the generating electronic structure hamiltonians using the PEST package.
+  - An introduction to the generating electronic structure hamiltonians using the PEST package.
+
 ---
 
 ## Citation
-To be populated once code is posted. Cannot create DOI on zenodo without link to repo.
 
-Should generally also include citations of cirq.
+Please use this DOI number reference, published on [Zenodo](https://zenodo.org), when citing the software:
+
+![DOI](image.png)
 
 ---
 
 ## Disclaimer
 
 DISTRIBUTION STATEMENT A. Approved for public release: distribution unlimited.
 
 © 2023 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
-    
+
     Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014)
     SPDX-License-Identifier: BSD-2-Clause
-    
+
 This material is based upon work supported by the Under Secretary of Defense for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Under Secretary of Defense for Research and Engineering.
 
 A portion of this research was sponsored by the United States Air Force Research Laboratory and the United States Air Force Artificial Intelligence Accelerator and was accomplished under Cooperative Agreement Number FA8750-19-2-1000. The views and conclusions contained in this document are those of the authors and should not be interpreted as representing the official policies, either expressed or implied, of the United States Air Force or the U.S. Government. The U.S. Government is authorized to reproduce and distribute reprints for Government purposes notwithstanding any copyright notation herein.
 
 The software/firmware is provided to you on an As-Is basis
-
-
-
```

### Comparing `pyLIQTR-1.0.1/setup.py` & `pyliqtr-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 AUTHOR_EMAIL = "Kevin.Obenland@ll.mit.edu"
 DESCRIPTION = (
     "A python package for generating quantum circuits using quantum algorithms."
 )
 THIS_DIRECTORY = Path(__file__).parent
 LONG_DESCRIPTION = (THIS_DIRECTORY / "README.md").read_text()
 
-REQUIREMENTS = (THIS_DIRECTORY / "requirements.txt").read_text().splitlines()
+REQUIREMENTS = open(THIS_DIRECTORY / "requirements.txt").readlines()
 REQUIREMENTS = [r.strip() for r in REQUIREMENTS]
 
-REQUIREMENTS_DEV = (THIS_DIRECTORY / "requirements-dev.txt").read_text().splitlines()
+REQUIREMENTS_DEV = open(THIS_DIRECTORY / "requirements-dev.txt").readlines()
 REQUIREMENTS_DEV = [r.strip() for r in REQUIREMENTS_DEV]
 
 __version__ = ""
 exec(open("src/pyLIQTR/_version.py").read())
 
 setup(
     name=DISTNAME,
@@ -63,11 +63,11 @@
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     packages=find_packages(where="src"),
     package_dir={"": "src"},
-    python_requires=">=3.8",
+    python_requires=">=3.8,<=3.12",
     install_requires=REQUIREMENTS,
     extras_require={"dev": REQUIREMENTS_DEV},
 )
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/BlockEncoding.py` & `pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/BlockEncoding.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
 import  numpy                  as  np
 import  cirq                   as  cirq
-import  cirq_ft                as  cirq_ft
-import  cirq_ft.infra.testing  as  cirq_test
+import  qualtran               as  qt
+import  qualtran.cirq_interop.testing  as  qt_test
  
 from    pyLIQTR.utils.pauli_string_manip  import  convert_to_dense_pauli_string
 
 import abc
 from   typing import Tuple
 
 
 
 
-class BlockEncoding(cirq_ft.GateWithRegisters):
+class BlockEncoding(qt._infra.gate_with_registers.GateWithRegisters):
     
     def __init__(self,ProblemInstance,control_val=None,**kwargs):
 
         self.PI                 =  ProblemInstance
 
         self._encoding_type     =  None
 
@@ -43,48 +43,48 @@
 
         if (self._control_val is not None):
             self._controlled    =  True
 
 
     @property
     @abc.abstractmethod
-    def control_registers(self) -> Tuple[cirq_ft.infra.Register, ...]:
+    def control_registers(self) -> Tuple[qt._infra.registers.Register, ...]:
         ...
 
     @property
     @abc.abstractmethod
-    def selection_registers(self) -> Tuple[cirq_ft.infra.SelectionRegister, ...]:
+    def selection_registers(self) -> Tuple[qt._infra.registers.SelectionRegister, ...]:
         ...
 
     @property
     @abc.abstractmethod
-    def target_registers(self) -> Tuple[cirq_ft.infra.Register, ...]:
+    def target_registers(self) -> Tuple[qt._infra.registers.Register, ...]:
         ...
 
 
     @property
     @abc.abstractmethod
-    def signature(self) -> cirq_ft.infra.Signature:
+    def signature(self) -> qt._infra.registers.Signature:
         ...
 
 
     @property
     def alpha(self):
         return (self.PI.alpha)
 
 
     @property
     def all_qubits(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.all_qubits)
 
 
     @property
     def circuit(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.circuit)  
 
 
 
 
 
 class BlockEncoding_select_prepare(BlockEncoding):
@@ -125,25 +125,25 @@
             return(self._prepare_gate.junk_registers)
         else:
             return( () )
 
 
     @property
     def signature(self):
-        return cirq_ft.Signature(
+        return qt._infra.registers.Signature(
             [*self.control_registers, *self.selection_registers, 
              *self.target_registers, *self.junk_registers] )
  #       return( self._get_common_signature( [self._select_gate,self._prepare_gate] ) )
 
 
 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
 
-        prepare_cost  =  cirq_ft.t_complexity(self._prepare_gate)
-        select_cost   =  cirq_ft.t_complexity(self._select_gate)
+        prepare_cost  =  qt.cirq_interop.t_complexity_protocol.t_complexity(self._prepare_gate)
+        select_cost   =  qt.cirq_interop.t_complexity_protocol.t_complexity(self._select_gate)
 
         if (self._do_prepare and self._do_prepare_inverse):
             total_cost = 2*prepare_cost + select_cost
         else:
             total_cost = prepare_cost + select_cost
 
         return (total_cost)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/LinearT.py` & `pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/LinearT.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
-import cirq_ft
+import qualtran  as  qt
 import cirq
 
 import numpy as np
 from functools import cached_property
 
 from pyLIQTR.BlockEncodings import *
 from pyLIQTR.BlockEncodings.BlockEncoding import BlockEncoding_select_prepare
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/PauliStringLCU.py` & `pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/PauliStringLCU.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,69 +16,77 @@
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
 import  numpy as np
 
 import  cirq
-import  cirq_ft                as  cirq_ft
-import  cirq_ft.infra.testing  as  cirq_cqt
+import  qualtran               as  qt
 
 # from  functools import cached_property 
 
 from pyLIQTR.BlockEncodings                 import   VALID_ENCODINGS
 #  from pyLIQTR.BlockEncodings.BlockEncoding   import   BlockEncoding
 from pyLIQTR.BlockEncodings.BlockEncoding   import   BlockEncoding_select_prepare
 
 
 from pyLIQTR.circuits.operators.prepare     import   Prepare
 from pyLIQTR.utils.pauli_string_manip       import   convert_sparse_term, convert_to_dense_pauli_string
 from pyLIQTR.utils.resource_analysis         import   legacy_resource_profile
 
 
 from pyLIQTR.circuits.operators.select_prepare_pauli  import  prepare_pauli_lcu
-
+from qualtran.bloqs.select_pauli_lcu import SelectPauliLCU
+from qualtran.bloqs.state_preparation import StatePreparationAliasSampling
 
 
 
 
 class PauliStringLCU(BlockEncoding_select_prepare):
 
 
-    def __init__(self,ProblemInstance, **kwargs):
+    def __init__(self,ProblemInstance, prepare_type=None, probability_eps=0.002, **kwargs):
 
         super().__init__(ProblemInstance,**kwargs)
 
         self._encoding_type     =  VALID_ENCODINGS.PauliLCU
 
         ##  n_terms   :   Number of problem terms
         ##  n_pad     :   Number of padding terms
         ##  n_tot     :   Total number of terms
         ##
         self.n_terms  =  self.PI.n_terms(encoding=self._encoding_type)
         self.n_pad    =  2**(int(np.ceil(np.log2(self.n_terms)))) - self.n_terms
         self.n_tot    =  self.n_terms + self.n_pad
 
-
         alphas        =  [np.sqrt(np.abs(t.coefficient)) for t in self.getTerms]
 
         selection_bitsize = int(np.ceil(np.log2(self.n_tot)))
 
-        self._select_gate          =  cirq_ft.GenericSelect( selection_bitsize=selection_bitsize,
+        self._select_gate          =  SelectPauliLCU( selection_bitsize=selection_bitsize,
                                                              target_bitsize=self.PI.n_qubits(),
                                                              select_unitaries=self.getTerms,
                                                              control_val=self._control_val )
 
-
-        self._prepare_gate         =  prepare_pauli_lcu(selection_bitsize=selection_bitsize,
+        if prepare_type is None:
+            self._prepare_gate         =  prepare_pauli_lcu(selection_bitsize=selection_bitsize,
                                                          alphas=alphas)
+        elif prepare_type=='AS':
+            for t in self.getTerms:
+                coeff = np.real(t.coefficient)
+                if coeff < 0:
+                    raise ValueError("Negative coefficients are not supported yet.")
+            
+            self._prepare_gate         =  StatePreparationAliasSampling.from_lcu_probs(
+                                                lcu_probabilities=[np.real(t.coefficient) for t in self.getTerms]
+                                                    , probability_epsilon=probability_eps)
 
 
     @property
     def getTerms(self):        
         terms    =  [convert_to_dense_pauli_string(term)
                         for term in self.PI.yield_PauliLCU_Info(do_pad=self.n_pad, return_as='strings')]    
         return terms
 
     @property
     def alpha(self):
-        return(self.PI.alpha)
+        return(self.PI.alpha)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/fermi_hubbard_square_encoding.py` & `pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/fermi_hubbard_square_encoding.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
 import  numpy as np
 
 import  cirq
-import  cirq_ft                      as  cirq_ft
-import  cirq_ft.infra.testing        as  cirq_cqt
+import  qualtran                     as  qt
+import  qualtran.cirq_interop.testing  as  qt_test
 
-import  cirq_ft.algos.hubbard_model          as  cirq_hm
+import  qualtran.bloqs.hubbard_model as  qt_hm
 
 
 from    pyLIQTR.BlockEncodings                 import   VALID_ENCODINGS
 from    pyLIQTR.BlockEncodings.BlockEncoding   import   BlockEncoding_select_prepare
 
 
 
@@ -43,26 +43,26 @@
         if (self.PI._model != 'Fermi-Hubbard Model - SquareLattice(regular)'):
             raise NotImplementedError
 
         self.dims = ProblemInstance.shape
 
         self._encoding_type  =  VALID_ENCODINGS.FermiHubbardSquare
 
-        self._select_gate    =  cirq_hm.SelectHubbard( x_dim=self.dims[0], 
+        self._select_gate    =  qt_hm.SelectHubbard( x_dim=self.dims[0], 
                                                        y_dim=self.dims[1], 
                                                        control_val=self._control_val )
    
-        self._prepare_gate   =  cirq_hm.PrepareHubbard( x_dim=self.dims[0], 
+        self._prepare_gate   =  qt_hm.PrepareHubbard( x_dim=self.dims[0], 
                                                         y_dim=self.dims[1], 
                                                         t=-ProblemInstance.J,
                                                         mu=ProblemInstance.U )
         
 
     @property
     def alpha(self):
-        N  =  np.prod(self.PI.shape)
+        N  =  2*np.prod(self.PI.shape)
         J  =  np.abs(self.PI.J)
         U  =  np.abs(self.PI.U)
         alpha = 2*N*J + U*N/2
         return (alpha)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/BlockEncodings/getEncoding.py` & `pyliqtr-1.2.0/src/pyLIQTR/BlockEncodings/getEncoding.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,31 +18,37 @@
 may violate any copyrights that exist in this work.
 """
 from pyLIQTR.ProblemInstances.ProblemInstance import ProblemInstance
 from pyLIQTR.BlockEncodings import VALID_ENCODINGS
 from pyLIQTR.BlockEncodings.PauliStringLCU import PauliStringLCU
 from pyLIQTR.BlockEncodings.fermi_hubbard_square_encoding import fermi_hubbard_square_encoding
 from pyLIQTR.BlockEncodings.LinearT import Fermionic_LinearT
+from pyLIQTR.BlockEncodings.DoubleFactorized import DoubleFactorized
 
 validEncodings = []
 
-def getEncoding(encoding : VALID_ENCODINGS, instance =  None,  **kwargs):
+def getEncoding(encoding : VALID_ENCODINGS, instance =  None, prepare_type = None, **kwargs):
 
     instantiate = True if (instance is not None) else False
 
     if (encoding == VALID_ENCODINGS.PauliLCU):
         if instantiate:
-            return PauliStringLCU(ProblemInstance=instance,**kwargs)
+            return PauliStringLCU(ProblemInstance=instance, prepare_type=prepare_type, **kwargs)
         else:
             return PauliStringLCU
     elif (encoding == VALID_ENCODINGS.FermiHubbardSquare):
         if instantiate:
             return fermi_hubbard_square_encoding(ProblemInstance=instance,**kwargs)
         else:
             return fermi_hubbard_square_encoding
     elif encoding == VALID_ENCODINGS.LinearT:
         if instantiate:
             return Fermionic_LinearT(ProblemInstance=instance,**kwargs)
         else:
             return Fermionic_LinearT
+    elif encoding == VALID_ENCODINGS.DoubleFactorized:
+        if instantiate:
+            return DoubleFactorized(ProblemInstance=instance,**kwargs)
+        else:
+            return DoubleFactorized
     else:
-        raise NotImplementedError("Sorry :'(")
+        raise NotImplementedError("Sorry :'(")
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/pe.py` & `pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/pe.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/pe_gates.py` & `pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/pe_gates.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/PhaseEstimation/pe_sim.py` & `pyliqtr-1.2.0/src/pyLIQTR/PhaseEstimation/pe_sim.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/ElectronicStructure.py` & `pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/ElectronicStructure.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
-import numpy       as np
+import numpy as np
 import pyLIQTR.pest_interface.pest_python as pp
-
+from functools import cached_property
+from pyLIQTR.clam.operator_strings import op_strings
 from pyLIQTR.ProblemInstances.ProblemInstance import ProblemInstance
 
 class ElectronicStructure(ProblemInstance):
     """
     This ProblemInstance represents periodic electronic structure Hamiltonians generated using PEST. The Hamiltoninas generally take on the form 
     $$ 
     H = \sum_{p,q,\sigma} T(p-q) a^\dagger_{p,\sigma}a_{q,\sigma} + \sum_{p,\sigma} U(p) n_{p,\sigma} + \sum_{(p,\alpha)\neq(q,\beta)} V(p-q)n_{p,\alpha}n_{q,\beta}
@@ -56,14 +57,58 @@
     def __str__(self):
         return f"{self._model}\r\n\tHamiltonian filename:{self._filenameH}\tGrid filename:{self._filenameG}\n\r\tN:{self._N}\tM_vals:{self._M_vals}"
 
     def n_qubits(self):
         # equal to number of basis functions including spin
         return int(2*self._N)
 
+    @cached_property
+    def _ops(self):
+        _ops = op_strings(N_qb=2*self._N)
+        spin_offset = self._N
+
+        for p in range(self._N):
+
+            # loop over q>p and include a factor of 2 since coeffs only depend on abs(p-q)
+            for q in range(p+1,self._N):
+
+                xx_str = 'X' + ('Z'*abs(p-q)) + 'X'
+                yy_str = 'Y' + ('Z'*abs(p-q)) + 'Y'
+                idx_set_up = tuple(np.arange(p,p+abs(p-q)+2,1))
+                idx_set_down = tuple(np.arange(p+spin_offset,p+spin_offset+abs(p-q)+2,1))
+                
+                # NOTE: returns only non zero coefficients
+                if self._H.c_xzx(p,q) != 0.0:
+                    # spin up
+                    _ops.append_tuple((idx_set_up, xx_str, 2*self._H.c_xzx(p,q))) # factor of 2 for q<p case
+                    _ops.append_tuple((idx_set_up, yy_str, 2*self._H.c_xzx(p,q)))
+                    # spin down
+                    _ops.append_tuple((idx_set_down, xx_str, 2*self._H.c_xzx(p,q))) # factor of 2 for q<p case
+                    _ops.append_tuple((idx_set_down, yy_str, 2*self._H.c_xzx(p,q)))
+                if self._H.c_zz(p,q) != 0.0:
+                    # alpha = beta = up, p \neq q
+                    _ops.append_tuple(((p,q), 'ZZ', 2*self._H.c_zz(p,q))) # factor of 2 for q<p case
+                    # alpha = beta = down, p \neq q
+                    _ops.append_tuple(((p+spin_offset,q+spin_offset), 'ZZ', 2*self._H.c_zz(p,q)))
+                    # alpha=up, beta=down, p \neq q
+                    _ops.append_tuple(((p,q+spin_offset), 'ZZ', 2*self._H.c_zz(p,q)))
+                    # alpha=down, beta=up, p \neq q
+                    _ops.append_tuple(((p+spin_offset,q), 'ZZ', 2*self._H.c_zz(p,q)))
+
+            if self._H.c_zz(p,p) != 0.0:
+                # alpha=up, beta=down, p = q
+                _ops.append_tuple(((p,p+spin_offset), 'ZZ', self._H.c_zz(p,p)))
+                # alpha=down, beta=up, p = q
+                _ops.append_tuple(((p+spin_offset,p), 'ZZ', self._H.c_zz(p,p)))
+
+            if self._H.c_z(p) != 0.0:
+                _ops.append_tuple(((p,),'Z',self._H.c_z(p)))
+
+        return _ops
+
     def get_alpha(self,encoding:str='LinearT'):
         # sum of the absolute value of the hamiltonian coefficients
         # TODO: can this be more efficient
         if encoding == 'LinearT':
             T_pq_mag_sum = 0
             V_pq_mag_sum = 0
             U_p_mag_sum = 0
@@ -71,43 +116,23 @@
                 U_p_mag_sum += abs(self._H.U(p))
                 for q in range(self._N):
                     T_pq_mag_sum += abs(self._H.T(p,q))
                     if p != q: # exclude p=q for V
                         V_pq_mag_sum += abs(self._H.V(p,q))    
             return T_pq_mag_sum + U_p_mag_sum + V_pq_mag_sum
 
-    def yield_PauliLCU_Info(self, do_pad=0,return_as='arrays'):
-
-        if return_as=='arrays':
-
-            if do_pad:
-                for __ in range(int(np.floor(do_pad/2))):
-                    yield ((),'I',0)
-
-            for p in range(self._N):
+    def yield_PauliLCU_Info(self,return_as='arrays',do_pad=0,pad_value=1.0):
 
-                for q in range(p+1,self._N):
+        if (return_as == 'arrays'):
+            terms = self._ops.terms(do_pad=do_pad,pad_value=pad_value)
+        elif (return_as == 'strings'):
+            terms = self._ops.strings(do_pad=do_pad,pad_value=pad_value)
 
-                    xx_str = 'X' + ('Z'*abs(p-q)) + 'X'
-                    yy_str = 'Y' + ('Z'*abs(p-q)) + 'Y'
-                    idx_set = tuple(np.arange(p,p+abs(p-q)+2,1))
-                    
-                    # NOTE: return only non zero coefficients?
-                    yield (idx_set, xx_str, self._H.c_xzx(p,q))
-                    yield (idx_set, yy_str, self._H.c_xzx(p,q))
-                    yield ((p,q), 'ZZ', self._H.c_zz(p,q))
-
-                yield ((p,),'Z',self._H.c_z(p))
-
-            if do_pad:
-                for __ in range(int(np.ceil(do_pad/2))):
-                    yield ((),'I',0)
-        else:
-            # TODO
-            raise NotImplementedError()
+        for term in terms:
+            yield term
 
     def yield_LinearT_Info(self,termSelect:str):
         
         if termSelect == 'T':
             # this corresponds to tilde(T)**2 in https://arxiv.org/pdf/1805.03662.pdf
             for p in range(self._N):
                 term = 2*self._H.c_xzx(p,0) # factor of 2 since coefficients occur for each xzx/yzy term only once depending on p<q or p>q
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/LatticeInstance.py` & `pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/LatticeInstance.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/MatrixInstance.py` & `pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/MatrixInstance.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/ProblemInstance.py` & `pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/ProblemInstance.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/fermionic_models.py` & `pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/fermionic_models.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/getInstance.py` & `pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/getInstance.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/ProblemInstances/spin_models.py` & `pyliqtr-1.2.0/src/pyLIQTR/ProblemInstances/spin_models.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/AddMod.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/AddMod.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
-import cirq_ft
 import cirq
 import numpy as np
-from cirq_ft import infra,algos
-from cirq_ft.algos import and_gate
+from qualtran.bloqs.arithmetic.addition import Add as qtAdd
+from qualtran.bloqs.arithmetic.addition import AddConstantMod as qtAddConstantMod
+from qualtran import bloqs
+from qualtran.bloqs import and_bloq
 from cirq._compat import cached_property
 from typing import List, Tuple, Sequence, Optional
 from numpy.typing import NDArray
 
 def two_complement(val,nb):
     if np.sign(val) >= 0:
         return format(val,"0{}b".format(nb))
@@ -43,15 +44,15 @@
 
     print("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~")
     print(name)
     print(circuit)
     print(cirq.Simulator().simulate(circuit,qubit_order=qord,initial_state=initial_state))
     print("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~")
 
-class Add(algos.AdditionGate):
+class Add(qtAdd):
     def _decompose_with_context_(
         self, qubits: Sequence[cirq.Qid], context: Optional[cirq.DecompositionContext] = None
     ) -> cirq.OP_TREE:
         if context is None:
             context = cirq.DecompositionContext(cirq.ops.SimpleQubitManager())
         input_bits = qubits[: self.bitsize][::-1]
         output_bits = qubits[self.bitsize :][::-1]
@@ -59,42 +60,42 @@
             assert(len(input_bits) == 1)
             assert(len(output_bits) == 1)
             #I dont love this because it drops the carry bit...
             yield cirq.CX(input_bits[0],output_bits[0])
         else:
             ancillas = context.qubit_manager.qalloc(self.bitsize - 1)[::-1]
             # Start off the addition by anding into the ancilla
-            yield and_gate.And().on(input_bits[0], output_bits[0], ancillas[0])
+            yield and_bloq.And().on(input_bits[0], output_bits[0], ancillas[0])
             # Left part of Fig.2
             yield from self._left_building_block(input_bits, output_bits, ancillas, 1)
             yield cirq.CX(ancillas[-1], output_bits[-1])
             yield cirq.CX(input_bits[-1], output_bits[-1])
             # right part of Fig.2
             yield from self._right_building_block(input_bits, output_bits, ancillas, self.bitsize - 2)
-            yield and_gate.And(adjoint=True).on(input_bits[0], output_bits[0], ancillas[0])
+            yield and_bloq.And(uncompute=True).on(input_bits[0], output_bits[0], ancillas[0])
             yield cirq.CX(input_bits[0], output_bits[0])
             context.qubit_manager.qfree(ancillas)
+        
 
-
-class AddMod(algos.AddMod):
+class AddMod(qtAddConstantMod):
     def _decompose_with_context_(
         self, qubits: Sequence[cirq.Qid], context: Optional[cirq.DecompositionContext] = None
     ) -> cirq.OP_TREE:
         #Following the construction in
         #https://journals.aps.org/pra/pdf/10.1103/PhysRevA.54.147
         #from Fig 4.
         tmpG = []
         if context is None:
             context = cirq.DecompositionContext(cirq.ops.SimpleQubitManager())
 
-        isControlled =  len(self.cv)>0
+        isControlled =  len(self.cvs)>0
         if isControlled:
-            ctlQubits = list(qubits[0:len(self.cv)])
+            ctlQubits = list(qubits[0:len(self.cvs)])
             targetQubit = context.qubit_manager.qalloc(1)
-            yield cirq_ft.MultiControlPauli(self.cv).on(*(ctlQubits+targetQubit))
+            yield bloqs.multi_control_multi_target_pauli.MultiControlPauli(self.cvs).on(*(ctlQubits+targetQubit))
         
         #MSB is first qubit
         #if the input register is A, with size a
         #then our tmp register B needs to be of size a+1
         MSB = 0
         
         #Cirq-ft add_mod is semiclassical (ie adds or subtracts a classical value)
@@ -123,16 +124,16 @@
         
         add = Add(bitsize=self.bitsize)
         sub = cirq.inverse(add)
         
         
         #Input qubits (qubits) should be of the correct size. We make no guarantee about 
         #overflow though...
-        assert(len(qubits)-len(self.cv)==self.bitsize)
-        A = list(qubits[len(self.cv)::])
+        assert(len(qubits)-len(self.cvs)==self.bitsize)
+        A = list(qubits[len(self.cvs)::])
         #SWITCH IN ORDER TO DO INPLACE
         tmpB = A
         A = B
         B = tmpB
 
         #A,B,N,|0> = tmp
         #|a>,|b> --> |a>,|a+b>
@@ -195,16 +196,16 @@
         for idx,c in enumerate(modVal):
             if c=='1':
                 #tmpG.append(cirq.X.on(N[idx]))
                 yield cirq.X.on(N[idx])
 
         #debugPrint("Reorder",tmpG)
         if isControlled:
-            ctlQubits = list(qubits[0:len(self.cv)])
-            yield cirq_ft.MultiControlPauli(self.cv).on(*(ctlQubits+targetQubit))
+            ctlQubits = list(qubits[0:len(self.cvs)])
+            yield bloqs.multi_control_multi_target_pauli.MultiControlPauli(self.cvs).on(*(ctlQubits+targetQubit))
         
 
         context.qubit_manager.qfree(A)
         context.qubit_manager.qfree(N)
         context.qubit_manager.qfree(t)
         if isControlled:
-            context.qubit_manager.qfree(targetQubit)
+            context.qubit_manager.qfree(targetQubit)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/hamiltonian_encodings.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/hamiltonian_encodings.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/multiCZ.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/multiCZ.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/prepare.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,16 @@
     def pp_com(self):
         return self.__pp_com
 
     def _decompose_(self, qubits):
         return self.disentangle_recursive(alt=False, flip=True, pp_tgt=self.pp_exp, pp_com=self.pp_com, pp_ctl=self.pp_ctl)
 
     def __eq__(self,other):
+        if not hasattr(other,'total_decomp'):
+            return False
         return (self.total_decomp == other.total_decomp) and (self.__class__ == other.__class__)
 
     def alpha_prep(self, flip: bool, alpha_pair:Tuple[float, float]):
         if flip:
             if alpha_pair[0] == 0:
                 return (0, alpha_pair[1])
             else:
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/prepare_LinearT.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/prepare_LinearT.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,49 +13,53 @@
 
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
-import cirq_ft
 import cirq
 import attr
 import warnings
 import numpy as np
-from cirq_ft import linalg,infra
-from cirq._compat import cached_property
+import qualtran as qt
+from functools import cached_property
 from typing import List, Tuple, Sequence
 from numpy.typing import NDArray
+from qualtran import _infra
+from qualtran.linalg.lcu_util import preprocess_lcu_coefficients_for_reversible_sampling
+from qualtran.bloqs.qrom import QROM
+from qualtran.bloqs.multi_control_multi_target_pauli import MultiControlPauli
+
 from pyLIQTR.circuits.operators.AddMod import Add
 
-class FermionicPrepare_LinearT(infra.GateWithRegisters):
+class FermionicPrepare_LinearT(_infra.gate_with_registers.GateWithRegisters):
     '''
-    Implements circuit from Fig. 16 of https://arxiv.org/pdf/1805.03662.pdf using cirq_ft gates.
+    Implements circuit from Fig. 16 of https://arxiv.org/pdf/1805.03662.pdf using qualtran gates.
 
     Initializes the sate 
         $$
         (\sum_{p,sigma} U(p) |theta_p> |1>_U |0>_V |p, sigma, p, sigma>  
         + \sum_{p!=q, sigma} T(p-q) |theta_{p-q}^0> |0>_U |0>_V |p, sigma, q, sigma> 
         + \sum_{(p,alpha)!=(q,beta)} V(p-q) |theta_{p-q}^1> |0>_U |1>_V  |p,alpha,q,beta>) |temp>
         $$
     where the coefficients U(d), T(d), and V(d) are mu-bit binary approximations to the true values. mu is set according to the condition approx_error <= 1/(2**mu N) where N is the total number of T,U, and V coefficients.
 
     Args:
         T_array: The (XZX + YZY) operator coefficients, equivalent to tilde(T)**2 in the reference. Formatted such that the ith coefficient, Ti, is given by T_array[i] = ((1-sign(Ti))/2,abs(Ti)).
         U_array: The (Z) operator coefficients, equivalent to tilde(U)**2 in the reference. Formatted the same as T_array.
         V_array: The (ZZ) operator coefficients, equivalent to tilde(V)**2 in the reference. Formatted the same as T_array.
         M_vals: Number of grid points (orbitals) along each spatial dimension.
-        approx_error: The desired accuracy to represent each coefficient which sets mu size and keep/alt integers). See `cirq_ft.linalg.lcu_util.preprocess_lcu_coefficients_for_reversible_sampling` for more information.
+        approx_error: The desired accuracy to represent each coefficient which sets mu size and keep/alt integers). See `qualtran.linalg.lcu_util.preprocess_lcu_coefficients_for_reversible_sampling` for more information.
     '''
 
     def __init__(self, T_array: List[Tuple[int,float]], U_array: List[Tuple[int,float]], V_array: List[Tuple[int,float]], M_vals: NDArray[np.int_], approx_error: float):
 
         if any(M_vals <= 2):
-            # cirq_ft AdditionGate doesn't decompose properly for bitsize (logM) of 1 so need this warning for now
+            # qualtran AdditionGate doesn't decompose properly for bitsize (logM) of 1 so need this warning for now
             warnings.warn(f"All M_vals must be greater than 2 for full circuit decomposition to work, currently M_vals={M_vals}", stacklevel=2)
 
         self.__T_array = T_array
         self.__U_array = U_array
         self.__V_array = V_array
         self.__M_vals = M_vals
         self.__approx_error = approx_error
@@ -68,47 +72,47 @@
         self.__mu = max(0, int(np.ceil(-np.log2(approx_error * num_coeffs))))
         if self.__mu == 0:
             warnings.warn(f"approx_error={approx_error} may be too large for given basis size {np.prod(self.__M_vals)}",stacklevel=2)
 
         super(FermionicPrepare_LinearT, self)
 
     @cached_property
-    def selection_registers(self) -> Tuple[infra.SelectionRegister]:
-        theta_reg = infra.SelectionRegister(name="theta",bitsize=1)
-        U_reg = infra.SelectionRegister(name="U",bitsize=1)
-        V_reg = infra.SelectionRegister(name="V",bitsize=1)
-        p_reg = infra.SelectionRegister(name="p",bitsize=self.__Np_bits)
-        a_reg = infra.SelectionRegister(name="a",bitsize=1)
-        q_reg = infra.SelectionRegister(name="q",bitsize=self.__Np_bits)
-        b_reg = infra.SelectionRegister(name="b",bitsize=1)
+    def selection_registers(self) -> Tuple[_infra.registers.SelectionRegister]:
+        theta_reg = _infra.registers.SelectionRegister(name="theta",bitsize=1)
+        U_reg = _infra.registers.SelectionRegister(name="U",bitsize=1)
+        V_reg = _infra.registers.SelectionRegister(name="V",bitsize=1)
+        p_reg = _infra.registers.SelectionRegister(name="p",bitsize=self.__Np_bits)
+        a_reg = _infra.registers.SelectionRegister(name="a",bitsize=1)
+        q_reg = _infra.registers.SelectionRegister(name="q",bitsize=self.__Np_bits)
+        b_reg = _infra.registers.SelectionRegister(name="b",bitsize=1)
         return (theta_reg,U_reg,V_reg,p_reg,a_reg,q_reg,b_reg)
 
     @cached_property
     def alternates_bitsize(self) -> int:
         # factor of 2 comes from U and V bits
         return int(sum(self.__logM_vals) + 2)
 
     @cached_property
     def keep_bitsize(self) -> int:
         return self.__mu
 
     @cached_property
-    def junk_registers(self) -> Tuple[infra.Register]:
+    def junk_registers(self) -> Tuple[_infra.registers.Register]:
         # These make up the temp register. They are not perfectly uncomputed due to entanglement with the selection register and so must be retained and passed to the next instance of Subprepare/prepare.
-        return ( infra.Signature.build(
+        return ( _infra.registers.Signature.build(
             sigma_mu=self.__mu,
             alt=self.alternates_bitsize,
             keep=self.keep_bitsize,
             theta_alt=1,
             less_than_equal=1,
         ) )
 
     @cached_property
-    def signature(self) -> infra.Signature:
-        return infra.Signature([*self.selection_registers, *self.junk_registers])
+    def signature(self) -> _infra.registers.Signature:
+        return _infra.registers.Signature([*self.selection_registers, *self.junk_registers])
    
     def __repr__(self) -> str:
         T_repr = cirq._compat.proper_repr(self.__T_array)
         U_repr = cirq._compat.proper_repr(self.__U_array)
         V_repr = cirq._compat.proper_repr(self.__V_array)
         return (
             f'pyLIQTR.FermionicPrepare_LinearT('
@@ -140,36 +144,36 @@
 
         subprepare = Subprepare_LinearT.from_TUV_arrays(T_array=self.__T_array, U_array=self.__U_array, V_array=self.__V_array, M_vals=self.__M_vals, approx_error=self.__approx_error)
 
         yield subprepare.on_registers(U=U,V=V,d=p,sigma_mu=sigma_mu,alt=alt,keep=keep,theta=theta,theta_alt=theta_alt,less_than_equal=less_than_equal)
 
         # prepare a uniform superposition over M for each dimension on the q register, zero-controlled on U
         for qi, q_reg in enumerate(q_regs):
-            yield cirq_ft.PrepareUniformSuperposition(int(self.__M_vals[qi]),cv=(0,)).on_registers(controls=U,target=q_reg)
+            yield qt.bloqs.prepare_uniform_superposition.PrepareUniformSuperposition(int(self.__M_vals[qi]),cvs=(0,)).on_registers(ctrl=U,target=q_reg)
 
         yield cirq.H.on(*a)
 
         yield cirq.H.on(*b).controlled_by(*V)
-        yield cirq.H.on(*b).controlled_by(*V,*p,control_values=(1,)+(0,)*self.__Np_bits)
-        yield cirq.X.on(*b).controlled_by(*V,*p,control_values=(1,)+(0,)*self.__Np_bits)
+        yield MultiControlPauli(cvs=(1,)+(0,)*self.__Np_bits,target_gate=cirq.H).on_registers(controls=list(V)+list(p),target=b)
+        yield MultiControlPauli(cvs=(1,)+(0,)*self.__Np_bits,target_gate=cirq.X).on_registers(controls=list(V)+list(p),target=b)
 
         yield cirq.CNOT(*a,*b)
 
-        yield cirq_ft.MultiTargetCSwap.make_on(control=U, target_x=q, target_y=p)
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(ctrl=U, x=q, y=p)
 
         for Mi,logM in enumerate(self.__logM_vals):
             yield Add(bitsize=logM).on(*q_regs[Mi],*p_regs[Mi])
 
 
 @cirq.value_equality()
 @attr.frozen
-class Subprepare_LinearT(infra.GateWithRegisters):
+class Subprepare_LinearT(_infra.gate_with_registers.GateWithRegisters):
 
     '''
-    Implements circuit from Fig. 15 of https://arxiv.org/pdf/1805.03662.pdf using cirq_ft gates. Code structure based on cirq_ft.StatePreparationAliasSampling. 
+    Implements circuit from Fig. 15 of https://arxiv.org/pdf/1805.03662.pdf using qualtran gates. Code structure based on qualtran.StatePreparationAliasSampling. 
 
     Initializes the sate 
         $$
         \sum_{d=0}^{N-1} ( U(d) |theta_d> |1>_U |0>_V  + T(d) |theta_d^0> |0>_U |0>_V  + V(d) |theta_d^1> |0>_U |1>_V ) |d> |temp_d>
         $$
     where the coefficients U(d), T(d), and V(d) are mu-bit binary approximations to the true values. The preparation involves classical alias sampling.
     '''
@@ -193,23 +197,23 @@
         Args:
             T_array: The (XZX + YZY) operator coefficients, equivalent to tilde(T)**2 in the reference. Formatted such that the ith coefficient, Ti = T(i), is given by T_array[i] = ((1-sign(Ti))/2,abs(Ti)).
             U_array: The (Z) operator coefficients, equivalent to tilde(U)**2 in the reference. Formatted the same as T_array.
             V_array: The (ZZ) operator coefficients, equivalent to tilde(V)**2 in the reference. Formatted the same as T_array.
             M_vals: Number of grid points (spin orbitals) along each spatial dimension.
             approx_error: The desired accuracy to represent each coefficient
                 (which sets mu size and keep/alt integers).
-                See `cirq_ft.linalg.lcu_util.preprocess_lcu_coefficients_for_reversible_sampling`
+                See `qualtran.linalg.lcu_util.preprocess_lcu_coefficients_for_reversible_sampling`
                 for more information.
         """
 
         # NOTE: the order of T, V, and U is important since T -> 00, V -> 01, U -> 10 in terms of the UV registers
         coefficients = [coeff[1] for coeff in T_array + V_array + U_array]
         theta = np.array([coeff[0] for coeff in T_array + V_array + U_array]) # entries should be 0 or 1
 
-        alt, keep, mu = linalg.preprocess_lcu_coefficients_for_reversible_sampling(
+        alt, keep, mu = preprocess_lcu_coefficients_for_reversible_sampling(
             lcu_coefficients=coefficients, epsilon=approx_error
         )
         theta_alt = np.array([theta[i] for i in alt])
 
         logM_vals = np.ceil(np.log2(M_vals)).astype('int_')
         D = len(M_vals)
 
@@ -235,40 +239,39 @@
 
     @cached_property
     def selection_bitsize(self) -> int:
         # factor of 2 comes from U and V bits
         return int(sum(self.logM_vals) + 2)
 
     @cached_property
-    def junk_registers(self) -> Tuple[infra.Register]:
+    def junk_registers(self) -> Tuple[_infra.registers.Register]:
         # These (except for theta) make up the temp register. They are not perfectly uncomputed due to entanglement with the selection register and so must be retained and passed to the next instance of Subprepare/prepare.
-        # TODO: should theta be seperated out? Doesn't contribute to selection iteration so not a selection register but is used by select oracle.
-        return ( infra.Signature.build(
+        return ( _infra.registers.Signature.build(
             sigma_mu=self.mu,
             alt=self.alternates_bitsize,
             keep=self.keep_bitsize,
             theta=1,
             theta_alt=1,
             less_than_equal=1,
         ) )
 
     @cached_property
-    def selection_registers(self) -> Tuple[infra.SelectionRegister]:
-        U_reg = infra.SelectionRegister(name="U",bitsize=1)
-        V_reg = infra.SelectionRegister(name="V",bitsize=1)
-        d_reg = infra.SelectionRegister(name="d",bitsize=int(sum(self.logM_vals)))
+    def selection_registers(self) -> Tuple[_infra.registers.SelectionRegister]:
+        U_reg = _infra.registers.SelectionRegister(name="U",bitsize=1)
+        V_reg = _infra.registers.SelectionRegister(name="V",bitsize=1)
+        d_reg = _infra.registers.SelectionRegister(name="d",bitsize=int(sum(self.logM_vals)))
         return (
             U_reg,
             V_reg,
             d_reg,
         )
 
     @cached_property
-    def signature(self) -> infra.Signature:
-        return infra.Signature([*self.selection_registers, *self.junk_registers])
+    def signature(self) -> _infra.registers.Signature:
+        return _infra.registers.Signature([*self.selection_registers, *self.junk_registers])
 
 
     def __repr__(self) -> str:
         M_repr = cirq._compat.proper_repr(self.M_vals)
         logM_repr = cirq._compat.proper_repr(self.logM_vals)
         alt_repr = cirq._compat.proper_repr(self.alt)
         keep_repr = cirq._compat.proper_repr(self.keep)
@@ -283,15 +286,15 @@
             f'{keep_repr}, '
             f'{theta_repr}, '
             f'{theta_alt_repr}, '
             f'{self.mu})'
         )
 
     def _value_equality_values_(self):
-        # NOTE: needed to make cirq_ft.t_complexity() work. Returns values used to determine when two objects are equal. See https://github.com/quantumlib/Cirq/blob/v1.2.0/cirq-core/cirq/value/value_equality_attr.py#L26 for more info
+        # NOTE: needed to make qualtran.t_complexity() work. Returns values used to determine when two objects are equal. See https://github.com/quantumlib/Cirq/blob/v1.2.0/cirq-core/cirq/value/value_equality_attr.py#L26 for more info
         return (
             tuple(self.M_vals),
             tuple(self.logM_vals),
             self.D,
             tuple(self.alt),
             tuple(self.keep),
             tuple(self.theta),
@@ -312,44 +315,44 @@
         i=0
         d_regs = []
         for logM in self.logM_vals:
             d_regs.append(d[i:i+logM])
             i += logM
 
         # prepare a uniform superposition on the UV bits to produce |00>_UV -> (|00>_UV + |01>_UV + |10>_UV)/sqrt(3)
-        yield cirq_ft.PrepareUniformSuperposition(3).on_registers(target=list(quregs['U'])+list(quregs['V']),controls=[])
+        yield qt.bloqs.prepare_uniform_superposition.PrepareUniformSuperposition(3).on_registers(target=list(quregs['U'])+list(quregs['V']),controls=[])
         # prepare a uniform superposition over M for each dimension on the d register
         for di, d_reg in enumerate(d_regs):
-            yield cirq_ft.PrepareUniformSuperposition(self.M_vals[di]).on(*d_reg)
+            yield qt.bloqs.prepare_uniform_superposition.PrepareUniformSuperposition(self.M_vals[di]).on(*d_reg)
         # prepare uniform superposition on sigma_mu register for comparing to keep during alias sampling procedure
         yield cirq.H.on_each(*sigma_mu)
         # use QROM to iterate over combined UV-d registers to load theta, alt and keep data
-        qrom_gate = cirq_ft.QROM(
+        qrom_gate = qt.bloqs.qrom.QROM(
             [self.alt, self.keep, self.theta, self.theta_alt],
             (self.selection_bitsize,),
             (self.alternates_bitsize, self.keep_bitsize, 1, 1),
         )
-        yield qrom_gate.on_registers(selection=list(quregs['U'])+list(quregs['V'])+list(quregs['d']), target0=alt, target1=keep, target2=theta, target3=theta_alt)
+        yield qrom_gate.on_registers(selection=list(quregs['U'])+list(quregs['V'])+list(quregs['d']), target0_=alt, target1_=keep, target2_=theta, target3_=theta_alt)
         # flip less_than_equal bit when keep is less than sigma_mu
-        yield cirq_ft.LessThanEqualGate(self.mu, self.mu).on(
+        yield qt.bloqs.arithmetic.comparison.LessThanEqual(self.mu, self.mu).on(
             *keep, *sigma_mu, *less_than_equal
         )
         # swap alt data controlled on less_than_equal_bit
-        yield cirq_ft.MultiTargetCSwap.make_on(
-            control=less_than_equal, target_x=theta_alt, target_y=theta
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(
+            ctrl=less_than_equal, x=theta_alt, y=theta
         )
         ## the zero indexed alt bit corresponds to U
-        yield cirq_ft.MultiTargetCSwap.make_on(
-            control=less_than_equal, target_x=[alt[0]], target_y=U
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(
+            ctrl=less_than_equal, x=[alt[0]], y=U
         )
         ## the one indexed alt bit corresponds to V
-        yield cirq_ft.MultiTargetCSwap.make_on(
-            control=less_than_equal, target_x=[alt[1]], target_y=V
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(
+            ctrl=less_than_equal, x=[alt[1]], y=V
         )
         ## the remaining alt bits correspond to d
-        yield cirq_ft.MultiTargetCSwap.make_on(
-            control=less_than_equal, target_x=alt[2:], target_y=d
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(
+            ctrl=less_than_equal, x=alt[2:], y=d
         )
         # undo the less than comparison so the less_than_equal_bit returns to |0>
-        yield cirq_ft.LessThanEqualGate(self.mu, self.mu).on(
+        yield qt.bloqs.arithmetic.comparison.LessThanEqual(self.mu, self.mu).on(
             *keep, *sigma_mu, *less_than_equal
         )
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/prepare_oracle_pauli_lcu.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/prepare_oracle_pauli_lcu.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/reflect.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/reflect.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/selectV.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/selectV.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/selectVutils.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/selectVutils.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/select_LinearT.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/select_LinearT.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
-import cirq_ft
+import qualtran as qt
 import cirq
 import numpy as np
-from cirq_ft import infra
-from cirq._compat import cached_property
+from qualtran import _infra
+from qualtran._infra.gate_with_registers import total_bits
+from functools import cached_property
 from typing import List, Tuple, Sequence, Optional
 from numpy.typing import NDArray
 
-class FermionicSelect_LinearT(infra.GateWithRegisters):
+class FermionicSelect_LinearT(_infra.gate_with_registers.GateWithRegisters):
 
     '''
     Implements circuit from Fig . 14 of https://arxiv.org/pdf/1805.03662.pdf using cirq_ft gates. Performs the operation
 
     SELECT|theta,U,V,p,alpha,q,beta>|Psi> = (-1)^theta|theta,U,V,p,alpha,q,beta> \times 
                                                 Z_{p,alpha}|Psi>                  U ∧ ¬V ∧ ((p,alpha)=(q,beta))
                                                 Z_{p,alpha}Z_{q,beta}|Psi>       ¬U ∧ V ∧ ((p,alpha)!=(q,beta))
@@ -48,36 +49,36 @@
 
         self.__N = 2*int(np.prod(M_vals)) # total number of spin orbitals. Factor of 2 for up and down spin
         self.__Np_bits = int(sum(np.ceil(np.log2(M_vals)))) # number of bits needed to represent all p values
 
         super(FermionicSelect_LinearT, self)
 
     @cached_property
-    def control_registers(self) -> Tuple[infra.Register]:
-        registers = () if self.__control_val is None else (infra.Register('control', 1),)
+    def control_registers(self) -> Tuple[_infra.registers.Register]:
+        registers = () if self.__control_val is None else (_infra.registers.Register('control', 1),)
         return registers
 
     @cached_property
-    def selection_registers(self) -> Tuple[infra.SelectionRegister]:
-        p_reg = infra.SelectionRegister(name='p',bitsize=self.__Np_bits,iteration_length=int(self.__N/2))
-        q_reg = infra.SelectionRegister(name='q',bitsize=self.__Np_bits,iteration_length=int(self.__N/2))
-        theta_reg = cirq_ft.SelectionRegister(name="theta",bitsize=1)
-        U_reg = cirq_ft.SelectionRegister(name="U",bitsize=1)
-        V_reg = cirq_ft.SelectionRegister(name="V",bitsize=1)
-        a_reg = cirq_ft.SelectionRegister(name="a",bitsize=1)
-        b_reg = cirq_ft.SelectionRegister(name="b",bitsize=1)
+    def selection_registers(self) -> Tuple[_infra.registers.SelectionRegister]:
+        p_reg = _infra.registers.SelectionRegister(name='p',bitsize=self.__Np_bits,iteration_length=int(self.__N/2))
+        q_reg = _infra.registers.SelectionRegister(name='q',bitsize=self.__Np_bits,iteration_length=int(self.__N/2))
+        theta_reg = _infra.registers.SelectionRegister(name="theta",bitsize=1)
+        U_reg = _infra.registers.SelectionRegister(name="U",bitsize=1)
+        V_reg = _infra.registers.SelectionRegister(name="V",bitsize=1)
+        a_reg = _infra.registers.SelectionRegister(name="a",bitsize=1)
+        b_reg = _infra.registers.SelectionRegister(name="b",bitsize=1)
         return (theta_reg,U_reg,V_reg,p_reg,a_reg,q_reg,b_reg)
 
     @cached_property
-    def target_registers(self) -> Tuple[infra.Register]:
-        return (infra.Register('target', self.__N), )
+    def target_registers(self) -> Tuple[_infra.registers.Register]:
+        return (_infra.registers.Register('target', self.__N), )
 
     @cached_property
-    def signature(self) -> infra.Signature:
-        return infra.Signature(
+    def signature(self) -> _infra.registers.Signature:
+        return _infra.registers.Signature(
             [*self.control_registers, *self.selection_registers, *self.target_registers]
         )
 
     def decompose_from_registers(
         self,
         *,
         context: cirq.DecompositionContext,
@@ -86,53 +87,53 @@
         theta = quregs['theta']
         p, q = quregs['p'], quregs['q']
         U, V, a, b = quregs['U'], quregs['V'], quregs['a'], quregs['b']
         control, target = quregs.get('control', ()), quregs['target']
 
         qIterationLength = self.signature.get_left('q').iteration_length
 
-        yield cirq_ft.SelectedMajoranaFermionGate(
+        yield qt.bloqs.selected_majorana_fermion.SelectedMajoranaFermion(
             selection_regs=(
                     self.signature.get_left('a'),
                     self.signature.get_left('p'),
             ),
             control_regs=self.control_registers,
             target_gate=cirq.Y, 
         ).on_registers(control=control, p=p, a=a,target=target)
 
-        yield cirq_ft.MultiTargetCSwap.make_on(control=V, target_x=p, target_y=q)
-        yield cirq_ft.MultiTargetCSwap.make_on(control=V, target_x=a, target_y=b)
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(ctrl=V, x=p, y=q)
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(ctrl=V, x=a, y=b)
 
         q_selection_regs = (
                     self.signature.get_left('b'),
                     self.signature.get_left('q'),
             )
-        yield cirq_ft.SelectedMajoranaFermionGate(
+        yield qt.bloqs.selected_majorana_fermion.SelectedMajoranaFermion(
             selection_regs=q_selection_regs,
             control_regs=self.control_registers, 
             target_gate=cirq.X
         ).on_registers(control=control, q=q, b=b, target=target)
 
-        yield cirq_ft.MultiTargetCSwap.make_on(control=V, target_x=a, target_y=b)
-        yield cirq_ft.MultiTargetCSwap.make_on(control=V, target_x=p, target_y=q)
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(ctrl=V, x=a, y=b)
+        yield qt.bloqs.basic_gates.swap.CSwap.make_on(ctrl=V, x=p, y=q)
 
         yield cirq.S(*control) if control else cirq.global_phase_operation(1j)  # Fix errant i from XY=iZ (for U/V terms, combined with Zs below to fix -1), or fix -i from ZY = -iX or XZ = -iY (for T terms)
         yield cirq.Z(*theta).controlled_by(*control)  # Take care of overall sign from coefficient
         yield cirq.Z(*U).controlled_by(*control)  # Fix errant -1 from multiple pauli applications
         yield cirq.Z(*V).controlled_by(*control)  # Fix errant -1 from multiple pauli applications
         
         target_qubits_for_apply_to_lth_gate = [
             target[np.ravel_multi_index((b, q), (2, qIterationLength))]
             for q in range(qIterationLength)
             for b  in range(2)
         ]
 
-        yield cirq_ft.ApplyGateToLthQubit(
+        yield qt.bloqs.apply_gate_to_lth_target.ApplyGateToLthQubit(
             selection_regs=q_selection_regs,
             nth_gate=lambda *_: cirq.Z,
-            control_regs=infra.Register('control', 1 + infra.total_bits(self.control_registers)),
+            control_regs=_infra.registers.Register('control', 1 + total_bits(self.control_registers)),
         ).on_registers(
             q=q, b=b, control=[*V, *control], target=target_qubits_for_apply_to_lth_gate
         )
 
     def __repr__(self) -> str:
         return f'pyLIQTR.FermionicSelect_LinearT({self.__M_vals}, {self.__control_val})'
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/select_oracle_pauli_lcu.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/select_oracle_pauli_lcu.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/select_prepare_pauli.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/select_prepare_pauli.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,64 +14,64 @@
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
 
-import   cirq_ft   as       cirq_ft
+import   qualtran   as       qt
 #from    pyLIQTR.circuits.operators.prepare     import   Prepare
 from     pyLIQTR.utils.resource_analysis         import   legacy_resource_profile
 
 
 
 from    pyLIQTR.circuits.operators.prepare_oracle_pauli_lcu     import  QSP_Prepare  as   Prepare
   
 
 
 
-class prepare_pauli_lcu(cirq_ft.GateWithRegisters):
+class prepare_pauli_lcu(qt._infra.gate_with_registers.GateWithRegisters):
 
 
     def __init__(self, selection_bitsize=3, alphas=None):
 
         self._selection_bitsize      =   selection_bitsize
         self._alphas                 =   alphas
 
         self._Prepare                =   Prepare
 
     @property
     def signature(self):
-        sig  = cirq_ft.Signature.build(selection=self._selection_bitsize)
+        sig  = qt._infra.registers.Signature.build(selection=self._selection_bitsize)
         return(sig)
 
 
     @property
     def _prepare_cost(self):
         """
         quregs = cirq_ft.infra.get_named_qubits(self.signature)
         selection_qb   =  list(quregs['selection'])
         return( legacy_resource_profile(self._prepare_gate.on(*selection_qb)) )
         """
         #Note the analytical expression from https://arxiv.org/pdf/1905.10724.pdf A.3.2 seemed to be 
         #off by a factor of 1/2
         d=self._selection_bitsize
-        return cirq_ft.infra.TComplexity(t=0,\
+        return qt.cirq_interop.t_complexity_protocol.TComplexity(t=0,\
                                          clifford=2**(d-1),\
                                             rotations=2**(d))
 
 
     @property
     def _prepare_gate(self):
-        quregs = cirq_ft.infra.get_named_qubits(self.signature)
+        quregs = qt._infra.gate_with_registers.get_named_qubits(self.signature)
         return (self._Prepare(qubit_reg = list(quregs['selection']), alphas=self._alphas))
     
 
                 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
         prepare_cost  =  self._prepare_cost
         return (prepare_cost)
 
 
 
     def decompose_from_registers(self, context, **quregs):
         yield self._prepare_gate.on(*quregs['selection'])
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/test_hamiltonian_encodings.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_hamiltonian_encodings.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/test_multiCZ.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_multiCZ.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/test_reflect.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_reflect.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/operators/tests/test_selectV.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/operators/tests/test_selectV.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import sys
 from io import StringIO
 
 from pyLIQTR.utils.Hamiltonian import Hamiltonian
 from pyLIQTR.circuits.operators.selectV import ChildsSelectV,QROMSelectV
 from pyLIQTR.utils.printing import _build_qasm_qubit_map
 
-from pyLIQTR.utils.qsp_helpers import circuit_decompose_once, print_to_openqasm
+from pyLIQTR.utils.qsp_helpers import circuit_decompose_once
 
 class TestSelectV:
     @pytest.fixture(scope="class")
     def getHamiltonianAndQubits(self):
         terms = [("XXXX",1),("YYYY",1),("ZZZZ",1),
                  ("XIIY",-1),("IXYI",-2),("IZIZ",-3)]
         ham = Hamiltonian(terms)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/pyLCircuit.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/pyLCircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 import math
 from enum import Enum
 
 from pyLIQTR.circuits.pyLOperator import pyLOperator
 from pyLIQTR.utils.circuit_decomposition import decompose_op
 from pyLIQTR.gate_decomp.cirq_transforms import clifford_plus_t_direct_transform
 from pyLIQTR.gate_decomp.rotation_gates import decomp_mixin, T_COUNT_CONST, T_COUNT_SLOPE, T_COUNT_STD_DEV
-from pyLIQTR.utils.printing import to_openqasm
+from pyLIQTR.utils.printing import openqasm
 
-from cirq_ft import infra, algos, t_complexity
-
-from src.pyLIQTR.utils.printing import openqasm
+from qualtran import _infra, bloqs
+import qualtran.cirq_interop.testing as qt_test
+import qualtran.cirq_interop.t_complexity_protocol as t_complexity
 
 # class syntax
 class RESOURCE_ANALYSIS_MODE(Enum):
     Exact = 0
 RESOURCE_ANALYSIS_MODE = Enum('ResourceAnalysisMode', ['Exact'])
 
 # functional syntax
@@ -255,23 +255,23 @@
     
     def resourceAnalyze(self,rotation_gate_precision=1e-8,circuit_precision=None,mode=RESOURCE_ANALYSIS_MODE.Exact,decompose_rotations=True):
         # NOTE: Currently only estimates resources from rotation gates based on precision, ie does not generate explicit circuits and count
         self.clear_resources()
         for x in self.all_operations():
             if self._is_pyLOperator(x):
                 self._do_resource_analysis(x,mode)
-            elif isinstance(x._gate, infra.GateWithRegisters):
+            elif isinstance(x._gate, _infra.gate_with_registers.GateWithRegisters):
                 # Handle Complex (cirq-ft) Gate/Qubits operations
                 # Hold off on calling the cirq.decompose and simply run the cirq_ft.t_complexity
                 # then populate self.resources intelligently from that result
                 # tmp = cirq.Circuit(x)
                 # tmp = tmp._decompose_(self=tmp)
                 gate_dict = {"PRECLIFFT_{}".format(str(x.gate)):1}
 
-                t = t_complexity(x)
+                t = t_complexity.t_complexity(x)
 
                 # estimate gate counts based on number of rotations, but only if we don't want rotations
                 if decompose_rotations:
                     if circuit_precision is not None:
                         Ts_from_rotations = get_T_counts_from_rotations(t.rotations,circuit_precision=circuit_precision)
                     else:
                         Ts_from_rotations = get_T_counts_from_rotations(t.rotations,gate_precision=rotation_gate_precision)
@@ -284,15 +284,15 @@
 
 
                 self.resources = gate_dict
             elif isinstance(x._gate, cirq.QuantumFourierTransformGate):
                 # Need to add some specific logic for this as currently cirq doesn't have a way to calculate the resources of it's own QFT
                 gate_dict = {"PRECLIFFT_{}".format(str(x.gate)):1}
 
-                t = t_complexity(x)
+                t = t_complexity.t_complexity(x)
 
                 # estimate gate counts based on number of rotations, but only if we don't want rotations
                 if decompose_rotations:
                     if circuit_precision is not None:
                         Ts_from_rotations = get_T_counts_from_rotations(t.rotations,circuit_precision=circuit_precision)
                     else:
                         Ts_from_rotations = get_T_counts_from_rotations(t.rotations,gate_precision=rotation_gate_precision)
@@ -331,16 +331,15 @@
                     else:
                         gate_dict[gateStr] += 1
                 self.resources = gate_dict
 
         return self.resources
 
     def to_openqasm(self,use_rotation_decomp_gates=False):
-        # yield from to_openqasm(self,use_rotation_decomp_gates=use_rotation_decomp_gates)
-        yield from openqasm(self, rotation_allowed=use_rotation_decomp_gates)
+        yield from to_openqasm(self,use_rotation_decomp_gates=use_rotation_decomp_gates)
 
 
 def get_T_counts_from_rotations(num_rotation_gates,gate_precision=1e-8,circuit_precision=None):
     
     if circuit_precision is not None:
         precision = (circuit_precision / num_rotation_gates)
     else:
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/pyLOperator.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/pyLOperator.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/qsp.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/qsp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/tests/test_pyLCircuit.py` & `pyliqtr-1.2.0/src/pyLIQTR/circuits/tests/test_pyLOperator.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,57 +17,24 @@
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
 import pytest
 import numpy as np
 import cirq
 
-"""
-Some testing ideas to implement:
-create valid circuit [should pass]
-attempt to create valid circuit [should fail]
-add valid gate to circuit [pass/fail]
-add invalid (not sure what this would be just yet) gate to circuit [fail]
-add multiple gates to circuit [pass]
-add large number of gates to circuit [pass]
-can be printed [small/large]
-valid circuit can be decomposed into gate(s) [pass]
-empty circuit can be decomposed into gate(s) [fail?]
-"""
-from pyLIQTR.circuits.pyLCircuit import pyLCircuit as circuit
+from pyLIQTR.circuits.pyLOperator import pyLOperator as po
 
 
-class TestPylCircuit:
+class TestPyLOperator:
     @pytest.fixture(scope="class")
     def single_gate(self):
         qubits = cirq.LineQubit.range(1)
         single_gate = cirq.X.on(qubits[0])
 
         yield single_gate
         del single_gate
 
-    @pytest.fixture(scope="class")
-    def ten_gates(self):
-        qubits = cirq.LineQubit.range(10)
-        ten_gates = cirq.X.on(qubits)
-
-        yield ten_gates
-        del ten_gates
-
-    @pytest.fixture(scope="class")
-    def hundred_gates(self):
-        qubits = cirq.LineQubit.range(100)
-        hundred_gates = cirq.X.on(qubits)
-
-        yield hundred_gates
-        del hundred_gates
-
-    @pytest.fixture(scope="class")
-    def thousand_gates(self):
-        qubits = cirq.LineQubit.range(1000)
-        thousand_gates = cirq.X.on(qubits)
-
-        yield thousand_gates
-        del thousand_gates
-
-    def test_pylcircuit_init(self):
-        print("")
+    def test_base_class_pyloperator_creation(self, single_gate):
+        """This test will simply try and create a single gate operator without using the child class that instantiates the abstract methods"""
+        with pytest.raises(TypeError):
+            # should raise the following error [TypeError: Can't instantiate abstract class pyLOperator with abstract methods _num_qubits_, _qid_shape_, get_resouces, num_qubits]
+            plo = po(single_gate)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/circuits/tests/test_pyLOperator.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/conversions.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,28 +13,25 @@
 
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
-import pytest
-import numpy as np
-import cirq
-
-from pyLIQTR.circuits.pyLOperator import pyLOperator as po
-
-
-class TestPyLOperator:
-    @pytest.fixture(scope="class")
-    def single_gate(self):
-        qubits = cirq.LineQubit.range(1)
-        single_gate = cirq.X.on(qubits[0])
-
-        yield single_gate
-        del single_gate
-
-    def test_base_class_pyloperator_creation(self, single_gate):
-        """This test will simply try and create a single gate operator without using the child class that instantiates the abstract methods"""
-        with pytest.raises(TypeError):
-            # should raise the following error [TypeError: Can't instantiate abstract class pyLOperator with abstract methods _num_qubits_, _qid_shape_, get_resouces, num_qubits]
-            plo = po(single_gate)
+################################################################################
+###                                                                          ###
+###    CONVERSIONS   -    Conversion between QSP phase angle conventions.    ###
+###                                                                          ###
+################################################################################
+
+
+import  numpy   as   np
+
+
+def phases_Wx_to_R(phis):
+    N = len(phis)
+    ph = np.zeros(N)
+    ph[0] = phis[0] + np.pi/4
+    for n in range(1,N-1):
+        ph[n] = phis[n] + np.pi/2
+    ph[-1] = phis[-1] + np.pi/4
+    return(ph)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/atomic_lattice.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/atomic_lattice.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/cell_complex.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/cell_complex.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/geometry.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/geometry.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/lattice.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/lattice.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/lattice_definitions.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/lattice_definitions.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/burgers_nonlinear.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/burgers_nonlinear.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/linearization_tools.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/linearization_tools.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/multilinear_algebra.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/multilinear_algebra.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/linearization_tools/vlasov_spectral.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/linearization_tools/vlasov_spectral.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/multilinear_algebra.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/multilinear_algebra.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/operator_complex.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/operator_complex.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/operator_lattice.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/operator_lattice.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/operator_sims.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/operator_sims.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/operator_strings.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/operator_strings.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/operators.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/operators.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/physical_data.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/physical_data.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/simqsp.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/simqsp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/tensor_methods.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/tensor_methods.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/time_dynamics.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/time_dynamics.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/clam/utilities.py` & `pyliqtr-1.2.0/src/pyLIQTR/clam/utilities.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/cirq_transforms.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/cirq_transforms.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/clifford_gates.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/clifford_gates.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/ellipse.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/ellipse.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/exact_decomp.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/exact_decomp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/gate_approximation.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/gate_approximation.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/grid_operator.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/grid_operator.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/matrices.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/matrices.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/point_enumeration.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/point_enumeration.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/rings.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/rings.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/rotation_gates.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/rotation_gates.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/solve_diophantine.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/solve_diophantine.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/benchmarks.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/conftest.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_cirq_transformers.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_cirq_transformers.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_exact_decomp.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_exact_decomp.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_matrices.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_matrices.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_point_enumeration.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_point_enumeration.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/gate_decomp/tests/test_solve_diophantine.py` & `pyliqtr-1.2.0/src/pyLIQTR/gate_decomp/tests/test_solve_diophantine.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/pest_interface/pest_python.py` & `pyliqtr-1.2.0/src/pyLIQTR/pest_interface/pest_python.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/angler.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/angler.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/fourier_response/fourier_response.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/fourier_response/fourier_response.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/named_factors.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/named_factors.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/ChebyshevPoly.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/ChebyshevPoly.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/angler_optimization.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/angler_optimization.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/expander.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/expander.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/optimization/fitter.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/optimization/fitter.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/phase_factors.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/phase_factors.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/phase_factors/simulation.py` & `pyliqtr-1.2.0/src/pyLIQTR/phase_factors/simulation.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/qubitization/phase_estimation.py` & `pyliqtr-1.2.0/src/pyLIQTR/qubitization/phase_estimation.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
 
 import numpy    as  np
 import cirq     as  cirq
-import cirq_ft  as  cirq_ft
-import cirq_ft.infra.testing as cirq_test
+import qualtran as  qt
+import qualtran.cirq_interop.testing as qt_test
 
 
 from pyLIQTR.qubitization.qubitized_gates   import   QubitizedReflection, QubitizedRotation, QubitizedWalkOperator
 
 
 from pyLIQTR.BlockEncodings.BlockEncoding   import   BlockEncoding
 from pyLIQTR.BlockEncodings.getEncoding     import   getEncoding
@@ -33,15 +33,15 @@
 
 
 
 
 
 
 
-class QubitizedPhaseEstimation(cirq_ft.GateWithRegisters):
+class QubitizedPhaseEstimation(qt._infra.gate_with_registers.GateWithRegisters):
     
 
     ##
     ## Check circuit conventions to see if we can reuse the
     ## phase qubit for reflections between iterations or if 
     ## we need independent values.
     ##
@@ -54,22 +54,22 @@
 
             self._block_encoding          =  block_encoding(instance)
             self._block_encoding_ctl      =  block_encoding(instance,control_val=1)
 
         else:
 
             self._block_encoding          =  block_encoding
-            self._block_encoding_ctl      =  getEncoding( self._block_encoding.PI,
-                                                          self._block_encoding._encoding_type, 
+            self._block_encoding_ctl      =  getEncoding( instance=self._block_encoding.PI,
+                                                          encoding=self._block_encoding._encoding_type, 
                                                           control_val=1 )
 
         alpha = self._block_encoding.alpha
 
         if (eps is not None):
-            self._prec  =  int(np.ceil( np.log( (np.sqrt(2.0)*np.pi*alpha) / (2*eps) ) ))         
+            self._prec  =  int(np.ceil( np.log2( (np.sqrt(2.0)*np.pi*alpha) / (2*eps) ) ))         
         else:
             self._prec  =  prec
 
         self._multi_pauli_gate        =  cirq.Z
         self._multi_control_value     =  multi_control_val
 
 
@@ -94,41 +94,46 @@
     @property
     def target_registers(self):
         return(self._block_encoding.target_registers)
 
 
     @property
     def junk_registers(self):
-        return(self._block_encoding.junk_registers)
+        other_regs = [*self.selection_registers,*self.control_registers,*self.target_registers]
+        junk_regs = ()
+        for reg in [*self._block_encoding.signature]:
+            if reg not in other_regs:
+                junk_regs += (reg,)
+        return(junk_regs)
 
 
     @property
     def all_qubits(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.all_qubits)
     
     @property
     def circuit(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.circuit)   
 
 
 
     @property
     def signature(self):
 
         registers = []
 
-        r_prec = cirq_ft.Register('prec',  self._prec  )
+        r_prec = qt._infra.registers.Register('prec',  self._prec + 1 )
         registers.append(r_prec)
 
         # r_phase = cirq_ft.Register('phase', self._prec-1  )
         # registers.append(r_phase)
 
-        sig    =  cirq_ft.Signature( [ *registers,  
+        sig    =  qt._infra.registers.Signature( [ *registers,  
                                        *self.selection_registers, 
                                        *self.target_registers, 
                                        *self.junk_registers] )    
 
         return sig
     
 
@@ -140,66 +145,68 @@
 
         # for reg in self.selection_registers:
         #     selection_qubits += quregs[ reg.name ].tolist()
 
         # kw_blockregs = { 'selection'  :  selection_qubits,
         #                  'target'     :  quregs['target'] }
 
-        kw_blockregs = { 'target'     :  quregs['target'] } 
+        kw_blockregs = {} 
+        
+        for reg in self.target_registers:
+            kw_blockregs[reg.name] = quregs[ reg.name ]
 
         for reg in self.selection_registers:
             selection_qubits += quregs[ reg.name ].tolist()
             kw_blockregs[reg.name] = quregs[ reg.name ]
 
         for reg in self.junk_registers:
             kw_blockregs[reg.name] = quregs[ reg.name ]
 
         qbs_prec   =  quregs['prec']
  #       qbs_phase  =  quregs['phase']
 
         qm = context.qubit_manager
-        reg_phase = qm.qalloc(self._prec-1)
+        reg_phase = qm.qalloc(self._prec)  
 
         yield QubitizedWalkOperator(self._block_encoding_ctl,control_val=1).\
                     on_registers(**kw_blockregs,control=qbs_prec[0])
                                                                                  
-        for n in range(1,self._prec):
+        for n in range(1,self._prec+1):
 
             # prec_idx = self._prec-n-1
 
             yield QubitizedReflection( len(selection_qubits),
                                        control_val=0,
                                        multi_control_val=self._multi_control_value).\
-                                       on_registers(controls=selection_qubits,target=qbs_prec[n])    
-
+                                       on_registers(controls=selection_qubits,target=qbs_prec[n])  
+            
             for _ in range(0,int(2**(n - 1)) ):
                 yield QubitizedWalkOperator(self._block_encoding_ctl,control_val=1).\
                         on_registers(**kw_blockregs,control=reg_phase[n-1])
-#                        on_registers(**kw_blockregs,control=qbs_phase[n-1])
                 
             yield QubitizedReflection( len(selection_qubits),
                                        control_val=0,
                                        multi_control_val=self._multi_control_value).\
                                        on_registers(controls=selection_qubits,target=qbs_prec[n])    
 
 
 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
 
-        walk_cost        =  cirq_ft.t_complexity( QubitizedWalkOperator( self._block_encoding ))
-        walk_cost_total  =  cirq_ft.infra.TComplexity()
+        walk_cost        =  qt.cirq_interop.t_complexity_protocol.t_complexity( QubitizedWalkOperator( self._block_encoding ))
+        walk_cost_total  =  qt.cirq_interop.t_complexity_protocol.TComplexity()
 
-        for n in range(1,self._prec):
+        for n in range(1,self._prec+1):
             walk_cost_total  +=  walk_cost*int(2**(n - 1))
 
         walk_cost_total  +=  walk_cost
 
-        reflection_cost   =  cirq_ft.t_complexity( QubitizedReflection( self._n_selection,control_val=0 ))
+        reflection_cost   =  qt.cirq_interop.t_complexity_protocol.t_complexity( QubitizedReflection( self._n_selection,control_val=0 ))
 
-        return ( walk_cost_total + 2*(self._prec-1)*reflection_cost)
+        return ( walk_cost_total + 2*(self._prec)*reflection_cost)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/qubitization/qsvt.py` & `pyliqtr-1.2.0/src/pyLIQTR/qubitization/qsvt.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 ###                                                                          ###
 ###           QSVT  -  Circuits and methods for QSP, QET, and QSVT           ###
 ###                                                                          ###
 ################################################################################
 from typing import Any, DefaultDict, Iterable, Optional, Tuple, TypeVar, Union
 import  numpy                  as  np
 import  cirq                   as  cirq
-import  cirq_ft                as  cirq_ft
-import  cirq_ft.infra.testing  as  cirq_test
+import  qualtran               as  qt
+import  qualtran.cirq_interop.testing  as  qt_test
 from cirq import QasmArgs
 
 from  pyLIQTR.phase_factors.phase_factors   import  PhaseFactors
 from  pyLIQTR.qubitization.qubitized_gates  import  QubitizedReflection, QubitizedRotation
 ###
 ### Need to add phase regsiter attribute (like .selection_registers)
 ###
 
 TDefault = TypeVar('TDefault')
 RaiseTypeErrorIfNotProvided: Any = ([],)
 
 
 
-class QSVT_abstract(cirq_ft.GateWithRegisters):
+class QSVT_abstract(qt._infra.gate_with_registers.GateWithRegisters):
     def __init__( self, 
                   block_encoding, 
                   phis, 
                 #   instance=None, 
                   phase_convention='R',
                 #   control_val=None,
                   multi_control_val=1,
@@ -90,20 +90,20 @@
         num = 0
         for reg in registers:
             num += reg.bitsize
         return (num)      
     
     @property
     def all_qubits(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.all_qubits)
 
     @property
     def circuit(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.circuit)  
     
     @property
     def selection_registers(self):
         return(self._block_encoding.selection_registers)
 
     @property
@@ -116,31 +116,31 @@
 
     @property
     def junk_registers(self):
         return(self._block_encoding.junk_registers)
 
     @property
     def phase_registers(self):
-        return( [cirq_ft.Register('phase',1)] )
+        return( [qt._infra.registers.Register('phase',1)] )
 
     # @property
     # def phase_registers(self):
     #     return(self.junk_registers)
 
     @property
     def signature(self):
 
     #    phase_reg =  (cirq_ft.Register('phase',1),)
 
         if self._controlled:
-            ctl_reg =  (cirq_ft.Register('control',1),)
+            ctl_reg =  (qt._infra.registers.Register('control',1),)
         else:
             ctl_reg = ()
 
-        return cirq_ft.Signature( [ *ctl_reg, *self.selection_registers, 
+        return qt._infra.registers.Signature( [ *ctl_reg, *self.selection_registers, 
               *self.target_registers, *self.junk_registers, *self.phase_registers] )
     
 #            [ *phase_reg, *ctl_reg, *self.selection_registers, 
 #              *self.target_registers, *self.junk_registers, *self.phase_registers] )
 
     def _circuit_diagram_info_(self, args: cirq.CircuitDiagramInfoArgs) -> cirq.CircuitDiagramInfo:
             
@@ -243,59 +243,71 @@
         yield QubitizedRotation( n_rotation_controls,rads=self._phis[-1], **kw_rotation_args).\
                                     on_registers(**kw_rotation_regs) 
         yield cirq.H.on(reg_phase[0])
 
         
 
 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
 
         n_reflect_controls  =  0
 
         for reg in self.selection_registers:
             n_reflect_controls += reg.bitsize
 
         for reg in self.junk_registers:
             n_reflect_controls += reg.bitsize
 
 
-        encoding_cost   =  cirq_ft.t_complexity(self._block_encoding)
-        rotation_cost   =  cirq_ft.t_complexity( QubitizedRotation( n_reflect_controls, control_val=self._control_val ))
-        clifford_cost   =  cirq_ft.infra.TComplexity(clifford=(2 + 2*(self._n_phis-1)))
+        encoding_cost   =  qt.cirq_interop.t_complexity_protocol.t_complexity(self._block_encoding)
+        rotation_cost   =  qt.cirq_interop.t_complexity_protocol.t_complexity( QubitizedRotation( n_reflect_controls, control_val=self._control_val ))
+        clifford_cost   =  qt.cirq_interop.t_complexity_protocol.TComplexity(clifford=(2 + 2*(self._n_phis-1)))
 
         return ( rotation_cost*(self._n_phis) + encoding_cost*(self._n_phis-1) + clifford_cost)
 
     #def _qasm_(self, args: 'cirq.QasmArgs') -> str:
     def _qasm_(
         self,
         *,
         args: Optional[QasmArgs] = None,
         qubits: Optional[Iterable['cirq.Qid']] = None,
         default: DefaultDict = RaiseTypeErrorIfNotProvided,
     ) -> Union[str, TDefault]:
-
         # args.validate_version('2.0')
-        # allQ = [*self.__phs_q, *self.__anc_q, *self.__ctl_q, *self.__tgt_q]
-        # allQStr = ",".join([args.format(str(x)) for x in allQ])
-        # return "{}({})\n".format(self.__strName,allQStr)
+        # # build up all the qubits, minus the ancilla ones for now
+        # allQ = [
+        #     *self.selection_registers,
+        #     *self.control_registers,
+        #     *self.target_registers,
+        #     *self.phase_registers
+        #     ]
+
+        # ops = self.decompose_from_registers(allQ)
+        # return QasmOutput(
+        #     operations=self._block_encoding,
+        #     qubits=allQ,
+        #     # header=None,
+        #     # precision=10,
+        #     # version='2.0',
+        # )
         raise NotImplementedError
 
 
 
 
 
 
 
 
 
 
 
 
 
-class QSVT_real_polynomial_sum(cirq_ft.GateWithRegisters):
+class QSVT_real_polynomial_sum(qt._infra.gate_with_registers.GateWithRegisters):
     
     def __init__( self, 
                   block_encoding, 
                   phis, 
                   instance=None, 
                   ctl_s_gate=False, 
                   ctl_z_gate=False, 
@@ -348,21 +360,21 @@
                                                      control_val=self._control_val_1  )
 
         super().__init__(**kwargs)
 
 
     @property
     def all_qubits(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.all_qubits)
 
 
     @property
     def circuit(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.circuit)  
 
 
     @property
     def n_phis(self):
         return( (len(self._phis_0),len(self._phis_1)) )
 
@@ -391,22 +403,22 @@
     def phase_registers(self):
         return(self.qsvt_gate_0.phase)
 
 
     @property
     def signature(self):
 
-        phase_reg =  (cirq_ft.Register('phase',1),)
+        phase_reg =  (qt._infra.registers.Register('phase',1),)
 
         if self._controlled:
-            ctl_reg =  (cirq_ft.Register('control',1),)
+            ctl_reg =  (qt._infra.registers.Register('control',1),)
         else:
             ctl_reg = ()
 
-        return cirq_ft.Signature(
+        return qt._infra.registers.Signature(
             [ *phase_reg, *self.control_registers,
               *self.target_registers,  *self.selection_registers, 
               *self.junk_registers] )
 
 
     def decompose_from_registers(self, context, **quregs):
 
@@ -438,24 +450,24 @@
 
         yield self.qsvt_gate_0.on_registers(**kw_qsvt_regs)  
         
         if self._ctl_h_gate:
             yield cirq.H.on(quregs['control'][0])
         
 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
 
         n_reflect_controls  =  0
 
-        encoding_cost_0   =  cirq_ft.t_complexity(self.qsvt_gate_0)
-        encoding_cost_1   =  cirq_ft.t_complexity(self.qsvt_gate_1)
+        encoding_cost_0   =  qt.cirq_interop.t_complexity_protocol.t_complexity(self.qsvt_gate_0)
+        encoding_cost_1   =  qt.cirq_interop.t_complexity_protocol.t_complexity(self.qsvt_gate_1)
 
         cliff  =  2*self._ctl_h_gate + self._ctl_s_gate + self._ctl_z_gate
 
-        clifford_cost   =  cirq_ft.infra.TComplexity(clifford=cliff)
+        clifford_cost   =  qt.cirq_interop.t_complexity_protocol.TComplexity(clifford=cliff)
 
         return ( encoding_cost_0 + encoding_cost_1 + clifford_cost)
 
 
 
 
 
@@ -549,29 +561,29 @@
         
 
         yield encoding_plus_rotation(self._phis[-2],kw_block_regs)
         yield cirq.Rx(rads=self._phis[-1]).on(reg_phase[0])
 
 
 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
 
         n_reflect_controls  =  0
 
         for reg in self.selection_registers:
             n_reflect_controls += reg.bitsize
 
         for reg in self.junk_registers:
             n_reflect_controls += reg.bitsize
 
 
 
-        encoding_cost   =  cirq_ft.t_complexity(self._block_encoding)
-        rotation_cost   =  cirq_ft.t_complexity( QubitizedRotation( n_reflect_controls))
-        clifford_cost   =  cirq_ft.infra.TComplexity(clifford=(2 + 2*(self._n_phis-1)))
+        encoding_cost   =  qt.cirq_interop.t_complexity_protocol.t_complexity(self._block_encoding)
+        rotation_cost   =  qt.cirq_interop.t_complexity_protocol.t_complexity( QubitizedRotation( n_reflect_controls))
+        clifford_cost   =  qt.cirq_interop.t_complexity_protocol.TComplexity(clifford=(2 + 2*(self._n_phis-1)))
 
         return ( rotation_cost*(self._n_phis) + encoding_cost*(self._n_phis-1) + clifford_cost)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/qubitization/qsvt_dynamics.py` & `pyliqtr-1.2.0/src/pyLIQTR/qubitization/qsvt_dynamics.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 def qsvt_dynamics( encoding,
                    instance=None,
                    times=[],
                    eps=1e-3,
                    sequence="qsvt",
                    phase_algorithm="optimization",
                    phase_sets=None,
+                   time_rescale=True,
                    **kwargs ):
 
     is_array           =  True
     is_array_instance  =  False
 
     if (isinstance(times,float) or isinstance(times,int)):
         is_array  =  False
@@ -103,21 +104,29 @@
 
 
     if (isinstance(instance,list) or isinstance(instance,tuple)):
         is_array_instance  =  True
         times = np.array(times)
 
     if instance is not None:
-        alpha = instance.alpha
+        alpha = encoding(instance).alpha        
     else:
         alpha = encoding.alpha
 
+
+
+
     if (phase_sets is None):
 
-        phase_sets  =  simulation_phases( times*alpha,
+        if time_rescale:
+            time_set = times*alpha
+        else:
+            time_set = times
+
+        phase_sets  =  simulation_phases( time_set,
                                           sequence=sequence,
                                           phase_algorithm=phase_algorithm,
                                           eps=eps ) 
     else:
 
         if (isinstance(phase_sets[0],PhaseFactors)):
             is_array  =  False
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/qubitization/qubitized_gates.py` & `pyliqtr-1.2.0/src/pyLIQTR/qubitization/qubitized_gates.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,49 +23,49 @@
 ###          QUBITIZED_GATES  -  Qubitized quantum circuit components        ###
 ###                                                                          ###
 ################################################################################
 
 
 import  numpy                  as  np
 import  cirq                   as  cirq 
-import  cirq_ft                as  cirq_ft
-import  cirq_ft.infra.testing  as  cirq_test
+import  qualtran               as  qt
+import  qualtran.cirq_interop.testing  as  qt_test
 
 
 
 
 
 
-class QubitizedReflection(cirq_ft.GateWithRegisters):
+class QubitizedReflection(qt._infra.gate_with_registers.GateWithRegisters):
 
     def __init__(self,n_controls,target_gate=cirq.Z,multi_control_val=1,control_val=1):
 
         self._n_controls         =  n_controls
         self._target_gate        =  target_gate
         self._multi_control_val  =  multi_control_val
         self._control_val        =  control_val
 
         return
 
 
     @property
     def all_qubits(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.all_qubits)
 
 
     @property
     def circuit(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.circuit)   
 
 
     @property
     def signature(self):
-        return cirq_ft.Signature.build( controls=self._n_controls,
+        return qt._infra.registers.Signature.build( controls=self._n_controls,
                                         target=1 )
     
 
 
     def decompose_from_registers(self, context, **quregs):
 
         controls  =  quregs['controls']
@@ -75,35 +75,35 @@
             for qb in controls:
                 yield cirq.X.on(qb) 
 
         if not self._control_val:
             yield cirq.X.on(target[0])
 
 
-        yield cirq_ft.algos.MultiControlPauli( [1] * len(controls), 
+        yield qt.bloqs.multi_control_multi_target_pauli.MultiControlPauli( [1] * len(controls), 
                                                target_gate=self._target_gate).\
                                                 on_registers(controls=controls, target=target)
         
         if not self._control_val:
             yield cirq.X.on(target[0])
             
         if not self._multi_control_val:
             for qb in controls:
                 yield cirq.X.on(qb) 
 
 
 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
-        multi_cost =  cirq_ft.t_complexity( cirq_ft.algos.MultiControlPauli([0] * self._n_controls, 
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
+        multi_cost =  qt.cirq_interop.t_complexity_protocol.t_complexity( qt.bloqs.multi_control_multi_target_pauli.MultiControlPauli([0] * self._n_controls, 
                                             target_gate=self._target_gate))
     
         if (not self._control_val):
-            clifford_cost = cirq_ft.infra.TComplexity(clifford=self._n_controls)
+            clifford_cost = qt.cirq_interop.t_complexity_protocol.TComplexity(clifford=self._n_controls)
         else:
-            clifford_cost = cirq_ft.infra.TComplexity()
+            clifford_cost = qt.cirq_interop.t_complexity_protocol.TComplexity()
         
         return (multi_cost + 2*clifford_cost)
 
 
 
     def _circuit_diagram_info_(self, args: cirq.CircuitDiagramInfoArgs) -> cirq.CircuitDiagramInfo:
             
@@ -123,15 +123,15 @@
 
 
 
 
 
 
 
-class QubitizedRotation(cirq_ft.GateWithRegisters):
+class QubitizedRotation(qt._infra.gate_with_registers.GateWithRegisters):
     
 
     def __init__(self, n_controls, 
                        rads=np.pi/2,
                        multi_target_gate=cirq.X,
                        rotation_gate=cirq.Rz,
                        multi_control_val=1,
@@ -157,32 +157,32 @@
             self._controlled = True
 
         return
 
 
     @property
     def all_qubits(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.all_qubits)
 
 
     @property
     def circuit(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.circuit)  
 
 
     @property
     def signature(self):
 
         if self._controlled:
-            return cirq_ft.Signature.build( control=self._n_controls,
+            return qt._infra.registers.Signature.build( control=self._n_controls,
                                             target=1, rotation_control=1 )
         else:
-            return cirq_ft.Signature.build( control=self._n_controls,
+            return qt._infra.registers.Signature.build( control=self._n_controls,
                                             target=1 )
     
 
 
     def decompose_from_registers(self, context, **quregs):
 
         controls  =  quregs['control']
@@ -229,27 +229,27 @@
                             
         if (not self._multi_control_val):
             for control in controls:
                 yield cirq.X(control)
                 
                 
                 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
 
-        multi_cost =  cirq_ft.t_complexity( QubitizedReflection(self._n_controls) )
-        rotation_cost = cirq_ft.infra.TComplexity(rotations=1)
+        multi_cost =  qt.cirq_interop.t_complexity_protocol.t_complexity( QubitizedReflection(self._n_controls) )
+        rotation_cost = qt.cirq_interop.t_complexity_protocol.TComplexity(rotations=1)
 
         ##
         ##  Fix this to properly handle controlled rotation
         ##
 
         if (not self._multi_control_val):
-            clifford_cost = cirq_ft.infra.TComplexity(clifford=self._n_controls)
+            clifford_cost = qt.cirq_interop.t_complexity_protocol.TComplexity(clifford=self._n_controls)
         else:
-            clifford_cost = cirq_ft.infra.TComplexity()
+            clifford_cost = qt.cirq_interop.t_complexity_protocol.TComplexity()
         
         return (2*multi_cost + rotation_cost + 2*clifford_cost)
     
 
 
     def _circuit_diagram_info_(self, args: cirq.CircuitDiagramInfoArgs) -> cirq.CircuitDiagramInfo:
 
@@ -275,15 +275,15 @@
 
 
 
 
 
 
 
-class QubitizedWalkOperator(cirq_ft.GateWithRegisters):
+class QubitizedWalkOperator(qt._infra.gate_with_registers.GateWithRegisters):
     
     def __init__( self, block_encoding, multi_control_val=1, control_val=1, instance=None  ):
 
         self._control_val             =  control_val
         self._multi_control_val       =  multi_control_val
 
         # self._block_encoding          =  block_encoding
@@ -313,21 +313,21 @@
             self._n_junk += reg.bitsize
 
         return
 
 
     @property
     def all_qubits(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.all_qubits)
 
 
     @property
     def circuit(self):
-        helper = cirq_test.GateHelper(self)
+        helper = qt_test.GateHelper(self)
         return(helper.circuit)  
     
 
     @property
     def selection_registers(self):
         return(self._block_encoding.selection_registers)
 
@@ -340,35 +340,43 @@
     @property
     def target_registers(self):
         return(self._block_encoding.target_registers)
 
 
     @property
     def junk_registers(self):
-        return(self._block_encoding.junk_registers)
+        other_regs = [*self.selection_registers,*self.control_registers,*self.target_registers]
+        junk_regs = ()
+        for reg in [*self._block_encoding.signature]:
+            if reg not in other_regs:
+                junk_regs += (reg,)
+        return(junk_regs)
 
 
     @property
     def signature(self):
 
         if not self._controlled_encoding:
-            ctl_reg =  (cirq_ft.Register('control',1),)
+            ctl_reg =  (qt._infra.registers.Register('control',1),)
         else:
             ctl_reg = self.control_registers
 
-        return cirq_ft.Signature(
+        return qt._infra.registers.Signature(
             [ *ctl_reg, *self.selection_registers, 
               *self.target_registers, *self.junk_registers] )
 
 
     def decompose_from_registers(self, context, **quregs):
 
         selection_qubits = []
 
-        kw_blockregs = { 'target'     :  quregs['target'] } 
+        kw_blockregs = {} 
+
+        for reg in self.target_registers:
+            kw_blockregs[reg.name] = quregs[ reg.name ]
 
         for reg in self.selection_registers:
             selection_qubits += quregs[ reg.name ].tolist()
             kw_blockregs[reg.name] = quregs[ reg.name ]
 
         for reg in self.junk_registers:
             kw_blockregs[reg.name] = quregs[ reg.name ]
@@ -391,18 +399,18 @@
         wire_symbols  = ['@' if self._control_val else '@(0)'] 
         wire_symbols += ['W'] * (self._n_selection + self._n_targets + self._n_junk)
 
         return cirq.CircuitDiagramInfo(wire_symbols=wire_symbols)
 
 
 
-    def _t_complexity_(self) -> cirq_ft.infra.TComplexity:
+    def _t_complexity_(self) -> qt.cirq_interop.t_complexity_protocol.TComplexity:
 
-        encoding_cost  =  cirq_ft.t_complexity(self._block_encoding)
-        reflect_cost   =  cirq_ft.t_complexity( QubitizedReflection( self._n_selection ))
+        encoding_cost  =  qt.cirq_interop.t_complexity_protocol.t_complexity(self._block_encoding)
+        reflect_cost   =  qt.cirq_interop.t_complexity_protocol.t_complexity( QubitizedReflection( self._n_selection ))
         
         return (reflect_cost + encoding_cost)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/tests/test_cirq_ft_resource_analyze_multiple_gates.py` & `pyliqtr-1.2.0/src/pyLIQTR/tests/test_qualtran_resource_analyze_multiple_gates.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,19 +39,20 @@
 """
 
 import numpy as np
 from typing import *
 
 import cirq
 
-import cirq_ft
-from cirq_ft import t_complexity, infra, GenericSelect
-from cirq_ft.algos.hubbard_model import *
-from cirq_ft.algos.multi_control_multi_target_pauli import MultiTargetCNOT, MultiControlPauli
-from cirq_ft.algos.qubitization_walk_operator_test import get_walk_operator_for_1d_Ising_model
+import qualtran as qt
+from qualtran import _infra
+import qualtran.bloqs.hubbard_model as qt_hm
+from qualtran.bloqs.select_pauli_lcu import SelectPauliLCU
+from qualtran.bloqs.multi_control_multi_target_pauli import MultiTargetCNOT, MultiControlPauli
+from qualtran.bloqs.qubitization_walk_operator_test import get_walk_operator_for_1d_Ising_model
 import pytest
 
 from pyLIQTR.circuits.pyLCircuit import pyLCircuit as pylc
 
 def _z_to_odd(n: int):
     if n % 2 == 1:
         return cirq.Z
@@ -91,80 +92,80 @@
     """
     def test_cirqft_generic_select(self):
         target_bitsize = 4
         us = ['XIXI', 'YIYI', 'ZZZZ', 'ZXYZ']
         us = [cirq.DensePauliString(u) for u in us]
         selection_bitsize = int(np.ceil(np.log2(len(us))))
 
-        gate = GenericSelect(selection_bitsize, target_bitsize, select_unitaries=us)
-        cft_op = gate.on_registers(**infra.get_named_qubits(gate.signature))
-        cft = t_complexity(cft_op)
+        gate = SelectPauliLCU(selection_bitsize, target_bitsize, select_unitaries=us)
+        cft_op = gate.on_registers(**qt._infra.gate_with_registers.get_named_qubits(gate.signature))
+        cft = qt.cirq_interop.t_complexity_protocol.t_complexity(cft_op)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
 
         assert pylcra['CliffT']['T'] == cft.t
         assert pylcra['CliffT']['Rotations'] == cft.rotations
         assert pylcra['CliffT']['Clifford'] == cft.clifford
 
     def test_cirqft_apply_gate_to_lth_qubit(self):
-        apply_z_to_odd = cirq_ft.ApplyGateToLthQubit(
-            cirq_ft.SelectionRegister('selection', 3, 4),
+        apply_z_to_odd = qt.bloqs.apply_gate_to_lth_target.ApplyGateToLthQubit(
+            _infra.registers.SelectionRegister('selection', 3, 4),
             nth_gate=_z_to_odd,
             # control_regs=cirq_ft.Signature.build(control=2),
         )
-        cft_op = apply_z_to_odd.on_registers(**infra.get_named_qubits(apply_z_to_odd.signature))
-        cft = t_complexity(cft_op)
+        cft_op = apply_z_to_odd.on_registers(**_infra.gate_with_registers.get_named_qubits(apply_z_to_odd.signature))
+        cft = qt.cirq_interop.t_complexity_protocol.t_complexity(cft_op)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
 
         assert pylcra['CliffT']['T'] == cft.t
         assert pylcra['CliffT']['Rotations'] == cft.rotations
         assert pylcra['CliffT']['Clifford'] == cft.clifford
 
     def test_cirqft_hubbard(self):
         x_dim, y_dim, t = 2, 2, 5
         mu = 4 * t
-        gate = PrepareHubbard(x_dim=x_dim, y_dim=x_dim, t=t, mu=mu)
-        cft_op = gate.on_registers(**infra.get_named_qubits(gate.signature))
-        cft = t_complexity(cft_op)
+        gate = qt_hm.PrepareHubbard(x_dim=x_dim, y_dim=x_dim, t=t, mu=mu)
+        cft_op = gate.on_registers(**_infra.gate_with_registers.get_named_qubits(gate.signature))
+        cft = qt.cirq_interop.t_complexity_protocol.t_complexity(cft_op)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
 
         assert pylcra['CliffT']['T'] == cft.t
         assert pylcra['CliffT']['Rotations'] == cft.rotations
         assert pylcra['CliffT']['Clifford'] == cft.clifford
 
     def test_cirqft_multi_target_cnot(self):
-        gate = MultiTargetCNOT(num_targets=2) 
-        cft_op = gate.on_registers(**infra.get_named_qubits(gate.signature))
-        cft = t_complexity(cft_op)
+        gate = MultiTargetCNOT(bitsize=2) 
+        cft_op = gate.on_registers(**_infra.gate_with_registers.get_named_qubits(gate.signature))
+        cft = qt.cirq_interop.t_complexity_protocol.t_complexity(cft_op)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
 
         assert pylcra['CliffT']['T'] == cft.t
         assert pylcra['CliffT']['Rotations'] == cft.rotations
         assert pylcra['CliffT']['Clifford'] == cft.clifford
 
     def test_cirqft_multicontrol_pauli(self):
         cvs = (0, 1)
         gate = MultiControlPauli(cvs=cvs, target_gate=cirq.Z) 
-        cft_op = gate.on_registers(**infra.get_named_qubits(gate.signature))
-        cft = t_complexity(cft_op)
+        cft_op = gate.on_registers(**_infra.gate_with_registers.get_named_qubits(gate.signature))
+        cft = qt.cirq_interop.t_complexity_protocol.t_complexity(cft_op)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
 
         assert pylcra['CliffT']['T'] == cft.t
@@ -173,32 +174,32 @@
 
     def test_cirqft_walk_operator(self):
         num_sites: int = 200
         eps: float = 1e-5
         m_bits: int = 14
 
         walk = get_walk_operator_for_1d_Ising_model(num_sites, eps)
-        cft_op = walk.on_registers(**infra.get_named_qubits(walk.signature))
-        cft = t_complexity(cft_op)
+        cft_op = walk.on_registers(**_infra.gate_with_registers.get_named_qubits(walk.signature))
+        cft = qt.cirq_interop.t_complexity_protocol.t_complexity(cft_op)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
 
         assert pylcra['CliffT']['T'] == cft.t
         assert pylcra['CliffT']['Rotations'] == cft.rotations
         assert pylcra['CliffT']['Clifford'] == cft.clifford
 
     def test_cirqft_prepare_uniform_superposition(self):
         # For now I'll tie the number if T-Basis states to 10 to test this
         # there is no particular reason for using 10 just to keep the number of iterations low enough to not impact performance.
-        gate = cirq_ft.PrepareUniformSuperposition(n=10, cv=(1,))
-        cft_op = gate.on_registers(**infra.get_named_qubits(gate.signature))
-        cft = cirq_ft.t_complexity(gate)
+        gate = qt.bloqs.prepare_uniform_superposition.PrepareUniformSuperposition(n=10, cvs=(1,))
+        cft_op = gate.on_registers(**_infra.gate_with_registers.get_named_qubits(gate.signature))
+        cft = qt.cirq_interop.t_complexity_protocol.t_complexity(gate)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
 
         assert pylcra['CliffT']['T'] == cft.t
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/tests/test_cirq_ft_resource_analyze_single_gate.py` & `pyliqtr-1.2.0/src/pyLIQTR/tests/test_qualtran_resource_analyze_single_gate.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,18 @@
 """
 
 import numpy as np
 from typing import *
 
 import cirq
 
-from cirq_ft import And, t_complexity, infra
-from cirq_ft.algos.hubbard_model import *
+from qualtran import _infra
+from qualtran.bloqs.and_bloq import And
+from qualtran.cirq_interop.t_complexity_protocol import t_complexity
+from qualtran.bloqs.hubbard_model import *
 
 from pyLIQTR.circuits.pyLCircuit import pyLCircuit as pylc
 
 def _z_to_odd(n: int):
     if n % 2 == 1:
         return cirq.Z
     return cirq.I
@@ -82,30 +84,30 @@
     WARNING: we set the decompose_rotations=False flag in pyLCircuit.resourceAnalyze() so that we can keep the comparison 
     with the cirq-ft resource analysis compatible. If we let it default to True then pyLIQTR will convert the rotation gates into
     Clifford+T's and cause all of the counts to be drastically different.
     """
     def test_cirqft_and(self):
         """This tests the cirq-ft And gate and compares our resource analysis against that."""
         gate = And() 
-        cft_op = gate.on_registers(**infra.get_named_qubits(gate.signature))
+        cft_op = gate.on_registers(**_infra.gate_with_registers.get_named_qubits(gate.signature))
         cft = t_complexity(cft_op)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
 
         assert pylcra['CliffT']['T'] == cft.t
         assert pylcra['CliffT']['Rotations'] == cft.rotations
         assert pylcra['CliffT']['Clifford'] == cft.clifford
 
     def test_cirqft_adjoint_and(self):
         """This tests our ability to analyze the resources of cirq-ft's Adjoint And gate."""
         gate = And() ** -1
-        cft_op = gate.on_registers(**infra.get_named_qubits(gate.signature))
+        cft_op = gate.on_registers(**_infra.gate_with_registers.get_named_qubits(gate.signature))
         cft = t_complexity(cft_op)
 
         cirq.decompose_once(cft_op)
 
         pylc_and = pylc([cft_op])
         pylcra = pylc_and.resourceAnalyze(decompose_rotations=False)
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/Hamiltonian.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/Hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/circuit_decomposition.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/circuit_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/get_hdf5.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/get_hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,23 @@
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
 import pandas as pd
 import numpy as np
 import math
 from openfermion.chem import MolecularData
-from openfermionpyscf import run_pyscf
+
+from pyLIQTR.utils.utils import isWindows
+if not isWindows():
+    from openfermionpyscf import run_pyscf
 from openfermion import jordan_wigner
 import cirq
 
-def get_hdf5(target_mol_no):
-    chem_data = pd.read_csv("chemistry_instances.csv")
+def get_hdf5(target_mol_no,filename='chemistry_instances.csv'):
+    chem_data = pd.read_csv(filename)
     mol_name = chem_data['molecule']
     mol_basis = chem_data['basis']
     mol_geom = chem_data['geometry']
     mol_mult = chem_data['multiplicity']
     mol_charge = chem_data['charge']
     
     target_mol_name = mol_name[target_mol_no]
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/pauli_string_manip.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/pauli_string_manip.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/plot_helpers.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/resource_analysis.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/resource_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
 import random
 import numpy    as  np
 import cirq     as  cirq
-import cirq_ft  as  cirq_ft
+import qualtran as  qt
 from typing import Dict, Any
 
 
 from   pyLIQTR.utils.circuit_decomposition import decompose_once, circuit_decompose_multi
 from   pyLIQTR.gate_decomp.cirq_transforms import clifford_plus_t_direct_transform
 from pyLIQTR.gate_decomp.rotation_gates import T_COUNT_CONST, T_COUNT_SLOPE, T_COUNT_STD_DEV
 
@@ -38,15 +38,15 @@
     circuit_precision -- If not None, the approximation error for each rotation gate will be bounded by `circuit_precision` divided by the number of rotation gates in `circuit_element`
     profile -- set to True to include rotation gates as a separate count rather than estimating their Clifford+T counts
     """
     try:
         resource_dict = {'LogicalQubits':cirq.num_qubits(circuit_element)}
     except:
         resource_dict={}
-    t_cliff_rot_resources = cirq_ft.t_complexity(circuit_element)
+    t_cliff_rot_resources = qt.cirq_interop.t_complexity_protocol.t_complexity(circuit_element)
 
     resource_dict["T"] = t_cliff_rot_resources.t 
     resource_dict["Clifford"] = t_cliff_rot_resources.clifford
 
 
     ## if profile is specified only take cirq_ft counting, otherwise
     ## do full Clifford+T estimation.
@@ -147,15 +147,15 @@
 
 def t_complexity_from_circuit(circ):
 
     n_t = count_t_gates(circ)
 
     n_clifford,n_rotation,n_other = count_clifford_and_rotations(circ)
 
-    t_complexity = cirq_ft.infra.TComplexity(t=n_t,clifford=n_clifford,rotations=n_rotation)
+    t_complexity = qt.cirq_interop.t_complexity_protocol.TComplexity(t=n_t,clifford=n_clifford,rotations=n_rotation)
 
     return(t_complexity)
 
 
 def legacy_resource_profile(gate):
     
     circ = cirq.Circuit()
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/tests/test_resoure_analyze.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/tests/test_resoure_analyze.py`

 * *Files identical despite different names*

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/tests/test_utils.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
+import platform
 import cirq
 import pkg_resources
 import pytest
 from openfermion.circuits import trotterize_exp_qubop_to_qasm
 from openfermion import jordan_wigner
 from openfermion.chem import MolecularData
 from cirq.contrib import qasm_import
@@ -29,16 +30,16 @@
 #qsp
 # import pyLIQTR.QSP.gen_qsp                 as qspFuncs
 # import pyLIQTR.QSP.QSP                     as pQSP
 # import pyLIQTR.sim_methods.quantum_ops  as vs        
 from pyLIQTR.utils.Hamiltonian             import Hamiltonian as pyH
 from pyLIQTR.utils.qsp_helpers             import circuit_decompose_once
 #utils
-from pyLIQTR.utils.utils import open_fermion_to_qasm
-from pyLIQTR.utils.printing import to_openqasm
+from pyLIQTR.utils.utils import isWindows, open_fermion_to_qasm
+from pyLIQTR.utils.printing import openqasm
 from pyLIQTR.gate_decomp.cirq_transforms import clifford_plus_t_direct_transform
 
 
 TEST_QASM_FILE = pkg_resources.resource_filename(
     "pyLIQTR", r"utils/tests/test_data/test_qasm_file.qasm"
 )
 TEST_QASM_NO_ROTATIONS_FILE = pkg_resources.resource_filename(
@@ -145,15 +146,15 @@
             fp.write(jw_ham_trotterized_circuit)
             fp.close()
 
     # Set the range to the number of iterations you'd like to run, this is good for testing the seed generator of vlasov
     @pytest.mark.skip
     @pytest.mark.parametrize('execution_number', range(10))
     def test_to_openqasm(self, vlasov_n8_qsp, execution_number):
-        circuit_output = "".join([line for line in to_openqasm(circuit_in=vlasov_n8_qsp)])
+        circuit_output = "".join([line for line in openqasm(circuit_in=vlasov_n8_qsp)])
         assert(circuit_output is not "")
         #first 1000 chars
         test_output = circuit_output[0:1000]
         # Something appears to have changed in the seed generator in this version of cirq-ft which caused the vlasov to be different
         # so I've commented out the old one and am using the new.
         # true_output = '// Generated from Cirq, Openfermion, and MIT LL\n\nOPENQASM 2.0;\ninclude "qelib1.inc";\n\n// Qubits: [q(0), q(1), q(2), q(3), q(4), q(5), q(6), q(7), ctl_q9, ctl_q10, ctl_q11, ctl_q12, phs_q8, z_anc_q13, z_anc_q14, z_anc_q15, z_anc_q16]\nqreg q[17];\n\nreset q[8];\nreset q[9];\nreset q[10];\nreset q[11];\nreset q[12];\nreset q[13];\nreset q[14];\nreset q[15];\nreset q[16];\nsdg q[0];\nsdg q[1];\nsdg q[2];\nsdg q[3];\nsdg q[4];\nsdg q[5];\nsdg q[6];\nsdg q[7];\nx q[8];\nx q[9];\nx q[10];\nx q[11];\nh q[12];\nreset q[13];\nreset q[14];\nreset q[15];\nreset q[16];\nz q[12];\nsdg q[8];\nh q[13];\nh q[14];\nh q[15];\nh q[16];\nh q[12];\nh q[8];\nz q[12];\nsdg q[8];\nt q[12];\nh q[8];\nh q[12];\ns q[8];\nt q[12];\nt q[8];\nh q[12];\nt q[8];\nh q[12];\nh q[8];\nt q[12];\nt q[8];\nh q[12];\nh q[8];\nt q[12];\ns q[8];\nh q[12];\nt q[8];\nt q[12];\nh q[8];\nh q[12];\nt q[8];\nt q[12];\nh q[8];\nh q[12];\ns q[8];\ns q[12];\nt q[8];\nt q[12];\nh q[8];\nh q[12];\nt q[8];\ns q[12];\nh q[8];\nt q[12];\nt q[8];\nh q[12];\nh q[8];\nt q[12];\nt q[8];\nh q[12];\nh q[8];\ns q[12];\ns q[8\n'
         true_output = '// Generated from Cirq, Openfermion, and MIT LL\n\nOPENQASM 2.0;\ninclude "qelib1.inc";\n\n// Qubits: [q(0), q(1), q(2), q(3), q(4), q(5), q(6), q(7), ctl_q9, ctl_q10, ctl_q11, ctl_q12, phs_q8, z_anc_q13, z_anc_q14, z_anc_q15, z_anc_q16]\nqreg q[17];\n\nreset q[8];\nreset q[9];\nreset q[10];\nreset q[11];\nreset q[12];\nreset q[13];\nreset q[14];\nreset q[15];\nreset q[16];\nsdg q[0];\nsdg q[1];\nsdg q[2];\nsdg q[3];\nsdg q[4];\nsdg q[5];\nsdg q[6];\nsdg q[7];\nx q[8];\nx q[9];\nx q[10];\nx q[11];\nh q[12];\nreset q[13];\nreset q[14];\nreset q[15];\nreset q[16];\nz q[12];\nsdg q[8];\nh q[13];\nh q[14];\nh q[15];\nh q[16];\nh q[12];\nh q[8];\nz q[12];\nsdg q[8];\nt q[12];\nh q[8];\nh q[12];\ns q[8];\nt q[12];\nt q[8];\nh q[12];\nh q[8];\ns q[12];\ns q[8];\nt q[12];\nt q[8];\nh q[12];\nh q[8];\nt q[12];\ns q[8];\nh q[12];\nt q[8];\nt q[12];\nh q[8];\nh q[12];\ns q[8];\nt q[12];\nt q[8];\nh q[12];\nh q[8];\nt q[12];\ns q[8];\nh q[12];\nt q[8];\ns q[12];\nh q[8];\nt q[12];\ns q[8];\nh q[12];\nt q[8];\nt q[12];\nh q[8];\nh q[12];\ns q[8];\ns q[12];\nt q[8];\nt q[12];\nh q[8];'
@@ -182,8 +183,24 @@
         molecule.load()
 
         mol_ham = molecule.get_molecular_hamiltonian()
         jw_ham = jordan_wigner(mol_ham)
         invalid_trotterized_hamiltonian = trotterize_exp_qubop_to_qasm(
             jw_ham * 2, evolution_time=1, trotter_number=1, trotter_order=1
         )
-        assert invalid_trotterized_hamiltonian is None
+        assert invalid_trotterized_hamiltonian is None
+
+    @pytest.mark.skipif(platform.system() != 'Windows', reason = "cannot run this test on Mac or Linux")
+    def test_is_windows_on_windows(self):
+        assert isWindows() == True
+
+    @pytest.mark.skipif(platform.system() == 'Windows', reason = "cannot run this test on Windows")
+    def test_is_windows_on_mac_or_linux(self):
+        assert isWindows() == False
+    
+    @pytest.mark.skipif(platform.system() != 'Mac', reason = "cannot run this test on anything other than Mac")
+    def test_is_mac(self):
+        assert isMac() == True
+
+    @pytest.mark.skipif(platform.system() != 'Linux', reason = "cannot run this test on anything other than Linux")
+    def test_is_mac(self):
+        assert isLinux() == True
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR/utils/utils.py` & `pyliqtr-1.2.0/src/pyLIQTR/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part
 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government
 rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed
 above. Use of this work other than as specifically authorized by the U.S. Government
 may violate any copyrights that exist in this work.
 """
+import platform
 import numpy       as np
 from typing import List, Tuple
 from cirq   import LineQubit
 import cirq
 #from pyLIQTR.
 from pyLIQTR.circuits.pyLCircuit import get_T_counts_from_rotations
 
@@ -162,8 +163,35 @@
     if tuple_in[1] == 'ctl':
         return ctl_q[tuple_in[0]]
     elif tuple_in[1] == 'tgt':
         return tgt_q[tuple_in[0]]
     elif tuple_in[1] == 'anc':
         return anc_q[tuple_in[0]]
     else:
-        raise RuntimeError('Function getQubitFromMap malfunctioning...')
+        raise RuntimeError('Function getQubitFromMap malfunctioning...')
+    
+def isWindows() -> bool:
+    """will determine if the OS we are running on is Windows or not.
+    
+    Return:
+        True if OS is Windows
+        False otherwise
+    """
+    return platform.system() == 'Windows'
+
+def isMac() -> bool:
+    """will determine if the OS we are running on is Mac or not.
+    
+    Return:
+        True if OS is Mac
+        False otherwise
+    """
+    return platform.platform().startswith('mac')
+
+def isLinux() -> bool:
+    """will determine if the OS we are running on is Linux or not.
+    
+    Return:
+        True if OS is Linux
+        False otherwise
+    """
+    return platform.system() == 'Linux'
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR.egg-info/PKG-INFO` & `pyliqtr-1.2.0/src/pyLIQTR.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pyLIQTR
-Version: 1.0.1
+Version: 1.2.0
 Summary: A python package for generating quantum circuits using quantum algorithms.
 Author: Kevin Obenland, Justin Elenewski, Arthur Kurlej,  Joe Belarge, John Blue, and Robert Rood
 Author-email: Kevin.Obenland@ll.mit.edu
 License: BDS-2
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: cirq-core==1.3.0.dev20231102230836
-Requires-Dist: cirq-ft==1.3.0.dev20231102230836
-Requires-Dist: cirq-google==1.3.0.dev20231102230836
+Requires-Dist: cirq-core==1.3.0.dev20231018023458
+Requires-Dist: qualtran==0.2.0
+Requires-Dist: ipykernel
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: scipy
+Requires-Dist: scipy<1.13.0
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: openfermion
 Requires-Dist: portalocker
 Requires-Dist: ply
 Requires-Dist: gmpy2
 Requires-Dist: networkx
+Requires-Dist: juliacall
+Requires-Dist: juliapkg
 Provides-Extra: dev
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: jupyterlab; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
@@ -35,121 +37,142 @@
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: pypandoc; extra == "dev"
 Requires-Dist: recommonmark; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 
 # pyLIQTR
-_Kevin Obenland, Justin Elenewski, Kaitlyn Morrell, Rylee Neumann, Arthur Kurlej, Robert Rood, John Blue, Joe Belarge & Parker Kuklinski_
+
+_Kevin Obenland, Justin Elenewski, Kaitlyn Morrell, Rylee Stuart Neumann, Arthur Kurlej, Robert Rood, John Blue, Joe Belarge, Benjamin Rempfer & Parker Kuklinski_
 
 ---
+
 ## Description
-`pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms and generating Clifford+T resource estimates. 
 
-This package is built extensively atop `cirq` & the recent release of `cirq-ft`. 
+`pyLIQTR` (<em>LI</em>ncoln Laboratory <em>Q</em>uantum algorithm <em>T</em>est and <em>R</em>esearch), is a python library for building quantum circuits derived from quantum algorithms and generating Clifford+T resource estimates.
+
+This package is built extensively atop `cirq` & the recent release of `qualtran`.
 
 pyLIQTR is primarily structured as:
+
 - pyLIQTR.ProblemInstances
-    - A set of code that provides an easy interface (through `pyLIQTR.ProblemInstances.getInstance`) to generate Hamiltonians that capture various physical models of interest.
+  - A set of code that provides an easy interface (through `pyLIQTR.ProblemInstances.getInstance`) to generate Hamiltonians that capture various physical models of interest.
 - pyLIQTR.BlockEncodings
-    - A set of codes that provides an easy interface (through `pyLIQTR.BlockEncodings.getEncoding`) to generate BlockEncodings that encode the action of a ProblemInstance through various different encodings.
+  - A set of codes that provides an easy interface (through `pyLIQTR.BlockEncodings.getEncoding`) to generate BlockEncodings that encode the action of a ProblemInstance through various different encodings.
 - pyLIQTR.clam
-    - A set of code that provides various classical utilities supporting:
-        - Integration of classical ODE’s (following application problems)
-        - Conversion of spin / fermionic Hamiltonians to classical numerics
-        - Simulation of quantum dynamics
-        - Quadratic / Integrable Hamiltonians (fast; polynomial scaling)
-        - General Hamiltonians (exponentially scaling)
-        - Source / Notebooks: This is scattered diffusely throughout the examples (Vlasov, Nonequilibrium, Heisenberg / Hubbard).
+  - A set of code that provides various classical utilities supporting:
+    - Integration of classical ODE’s (following application problems)
+    - Conversion of spin / fermionic Hamiltonians to classical numerics
+    - Simulation of quantum dynamics
+    - Quadratic / Integrable Hamiltonians (fast; polynomial scaling)
+    - General Hamiltonians (exponentially scaling)
+    - Source / Notebooks: This is scattered diffusely throughout the examples (Vlasov, Nonequilibrium, Heisenberg / Hubbard).
 - pyLIQTR.qubitization
-    - A set of code that provides ways of building QSP/QSVT circuits in the context of the pyLIQTR package.
+  - A set of code that provides ways of building QSP/QSVT circuits in the context of the pyLIQTR package.
 - pyLIQTR.phase_factors
-    - A set of code that calculates the angles required for a given QSP/QSVT sequence
+  - A set of code that calculates the angles required for a given QSP/QSVT sequence
 - pyLIQTR.circuits
-    - A set of pyLIQTR cirq circuits/gates used in our implementation of block encodings and algorithms.
+  - A set of pyLIQTR cirq circuits/gates used in our implementation of block encodings and algorithms.
 - pyLIQTR.gate_decomp
-    - A set of code that performs gate synthesis (converting rotations to Clifford+T gates) for a specified precision.
+  - A set of code that performs gate synthesis (converting rotations to Clifford+T gates) for a specified precision.
 - pyLIQTR.pest_interface
-    - A pythonic interface to the PEST Julia package.
+  - A pythonic interface to the PEST Julia package.
 - pyLIQTR.utils
-    - A set of various utility functions. 
-    - `pyLIQTR.utils.resource_analysis.estimate_resources` (adds robust estimation in addition to `cirq_ft.t_complexity`) can be used to determine the Clifford+T cost of any circuit generated with pyLIQTR
-    - `pyLIQTR.utils.circuit_decomposition.circuit_decompose_multi` (adds robust decomposition in addition to `cirq`'s decomposition functions) can be used to decompose circuits to 1+2QB gates
+  - A set of various utility functions.
+  - `pyLIQTR.utils.resource_analysis.estimate_resources` (adds robust estimation in addition to `qualtran.t_complexity`) can be used to determine the Clifford+T cost of any circuit generated with pyLIQTR
+  - `pyLIQTR.utils.circuit_decomposition.circuit_decompose_multi` (adds robust decomposition in addition to `cirq`'s decomposition functions) can be used to decompose circuits to 1+2QB gates
 
 In addition, a seperate Julia package for generating electronic structure hamiltonians (root/PEST) is included with pyLIQTR.
 
 pyLIQTR is a work-in-progress, as time goes on, we hope to provide better and more extensive documentation and examples in addition to new features. Please reach out to us if anything is unclear, so we can prioritize the documentation of the aspects that are most frequently used or most unclear.
 
 ---
+
 ## Features
-The features of this package are described in detail in [FEATURES.md](FEATURES.md). This includes not only descriptions, but also source files and example notebooks.
+
+The features of this package are described in detail in [FEATURES.md](Features.md). This includes not only descriptions, but also source files and example notebooks.
 
 ---
 
 ## Installation and Environment Setup
-It is recommended that conda be used to manage the environment. A setup.py file is included to facilitate this.
+
+- You can install the latest public tagged release from [PYPI](https://pypi.org/project/pyLIQTR/) using pip:
+
+        pip install pyLIQTR
+
+- You can install the latest state of the main branch:
+
+        pip install git+https://github.com/isi-usc-edu/pyLIQTR.git
+
+If you are going to be activelty developing the pyLIQTR source code, it is recommended that conda be used to manage the environment. A setup.py file is included to facilitate this.
 Change directory to the location of setup.py, then perform the following commands.
 
 - Create and activate the environment:
 
         on Windows use:
         conda create -n <Environment Name> "python>=3.8,<=3.11.5"
         on Mac use:
         conda create -n <Environment Name> python'>=3.8,<=3.11.5'
 
         conda activate <Environment Name>
-        
+
 - Install the package
 
         pip install .
 
-- Or, as a developer (for all platforms and shells):
+- If you are working as a developer (for all platforms and shells):
 
+        on Windows use:
+        pip install -e .[dev]
+        on Mac use:
         pip install -e ."[dev]"
-        
+
+<a id="optional-installs"></a>
 ### Optional Installs
-- Install MPSolve polynomial solver, which is used in the angle generation algorithm. Instructions for installation can be found here: https://numpi.dm.unipi.it/software/mpsolve
+
+- Install openfermionpyscf, which is used for the DoubleFactorized block encoding.
+    pip install openfermionpyscf
 - If not installed, then scipy will be used to calculate valid angles. Angle generation using scipy will generally take longer than angle generation using mpsolve.
 Effort is underway to deprecate the existing angle generation in favor of a more portable and efficient method.
-- Install openfermion & pyscf. 
-    - Openfermion is used for the implementation of Suzuki-Trotter and as the input to our implementation of GSE. This is required to use the GSE implementation.
-    - pyscf is used in conjunction with openfermion in order to generate new problem instances as input into our GSE implementation.
+- Install pyscf.
+  - pyscf is used in conjunction with openfermion in order to generate new problem instances as input into our GSE and Double Factorization implementation.
+    pip install pyscf
 
 ---
 
 ## Overview of Examples Included as Jupyter Notebooks
 
 Notebooks showcasing features are organized as follows in the /Examples directory.
+
 - Algorithm_and_Infrastructure
-    - A set of notebooks that go over the ProblemInstance and BlockEncoding infrastructure, in addition to a QSVT/QSP overview. Note that these are still being drafted.
+  - A set of notebooks that go over the ProblemInstance and BlockEncoding infrastructure, in addition to a QSVT/QSP overview. Note that these are still being drafted.
 - AngleGeneration
-    - Contains three notebooks describing the reworked angle generation features
+  - Contains three notebooks describing the reworked angle generation features
 - ApplicationInstances
-    - Contains four directories showing different types of physical models and how one may use the pyLIQTR package to generate circuits and provide resource estimates.
+  - Contains four directories showing different types of physical models and how one may use the pyLIQTR package to generate circuits and provide resource estimates.
 - PEST
-    - An introduction to the generating electronic structure hamiltonians using the PEST package.
+  - An introduction to the generating electronic structure hamiltonians using the PEST package.
+
 ---
 
 ## Citation
-To be populated once code is posted. Cannot create DOI on zenodo without link to repo.
 
-Should generally also include citations of cirq.
+Please use this DOI number reference, published on [Zenodo](https://zenodo.org), when citing the software:
+
+![DOI](image.png)
 
 ---
 
 ## Disclaimer
 
 DISTRIBUTION STATEMENT A. Approved for public release: distribution unlimited.
 
 © 2023 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
-    
+
     Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014)
     SPDX-License-Identifier: BSD-2-Clause
-    
+
 This material is based upon work supported by the Under Secretary of Defense for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Under Secretary of Defense for Research and Engineering.
 
 A portion of this research was sponsored by the United States Air Force Research Laboratory and the United States Air Force Artificial Intelligence Accelerator and was accomplished under Cooperative Agreement Number FA8750-19-2-1000. The views and conclusions contained in this document are those of the authors and should not be interpreted as representing the official policies, either expressed or implied, of the United States Air Force or the U.S. Government. The U.S. Government is authorized to reproduce and distribute reprints for Government purposes notwithstanding any copyright notation herein.
 
 The software/firmware is provided to you on an As-Is basis
-
-
-
```

### Comparing `pyLIQTR-1.0.1/src/pyLIQTR.egg-info/SOURCES.txt` & `pyliqtr-1.2.0/src/pyLIQTR.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -8,55 +8,88 @@
 src/pyLIQTR/_version.py
 src/pyLIQTR.egg-info/PKG-INFO
 src/pyLIQTR.egg-info/SOURCES.txt
 src/pyLIQTR.egg-info/dependency_links.txt
 src/pyLIQTR.egg-info/requires.txt
 src/pyLIQTR.egg-info/top_level.txt
 src/pyLIQTR/BlockEncodings/BlockEncoding.py
+src/pyLIQTR/BlockEncodings/CarlemanLinearization.py
+src/pyLIQTR/BlockEncodings/DoubleFactorized.py
 src/pyLIQTR/BlockEncodings/LinearT.py
 src/pyLIQTR/BlockEncodings/PauliStringLCU.py
 src/pyLIQTR/BlockEncodings/__init__.py
 src/pyLIQTR/BlockEncodings/fermi_hubbard_square_encoding.py
 src/pyLIQTR/BlockEncodings/getEncoding.py
 src/pyLIQTR/PhaseEstimation/__init__.py
 src/pyLIQTR/PhaseEstimation/pe.py
 src/pyLIQTR/PhaseEstimation/pe_gates.py
 src/pyLIQTR/PhaseEstimation/pe_sim.py
 src/pyLIQTR/PhaseEstimation/tests/__init__.py
 src/pyLIQTR/ProblemInstances/ChemicalHamiltonian.py
 src/pyLIQTR/ProblemInstances/ElectronicStructure.py
 src/pyLIQTR/ProblemInstances/LatticeInstance.py
 src/pyLIQTR/ProblemInstances/MatrixInstance.py
+src/pyLIQTR/ProblemInstances/NonlinearODE.py
 src/pyLIQTR/ProblemInstances/ProblemInstance.py
 src/pyLIQTR/ProblemInstances/__init__.py
 src/pyLIQTR/ProblemInstances/fermionic_models.py
 src/pyLIQTR/ProblemInstances/getInstance.py
 src/pyLIQTR/ProblemInstances/spin_models.py
 src/pyLIQTR/circuits/__init__.py
 src/pyLIQTR/circuits/pyLCircuit.py
 src/pyLIQTR/circuits/pyLOperator.py
 src/pyLIQTR/circuits/qsp.py
 src/pyLIQTR/circuits/operators/AddMod.py
+src/pyLIQTR/circuits/operators/BinaryToUnary.py
+src/pyLIQTR/circuits/operators/BitwiseZRotation.py
+src/pyLIQTR/circuits/operators/ControlledUniformSuperposition.py
+src/pyLIQTR/circuits/operators/DF_InnerPrepare.py
+src/pyLIQTR/circuits/operators/DF_OuterPrepare.py
+src/pyLIQTR/circuits/operators/DF_RotationsBlock.py
+src/pyLIQTR/circuits/operators/ExampleFMatrices.py
+src/pyLIQTR/circuits/operators/FixupTableQROM.py
+src/pyLIQTR/circuits/operators/FlaggedPrepareUniformSuperposition.py
+src/pyLIQTR/circuits/operators/PhaseGradientRotation.py
+src/pyLIQTR/circuits/operators/ProductPauliExponentials.py
+src/pyLIQTR/circuits/operators/QROMwithMeasurementUncompute.py
+src/pyLIQTR/circuits/operators/RotationsQROM.py
 src/pyLIQTR/circuits/operators/__init__.py
+src/pyLIQTR/circuits/operators/cascading_translation.py
+src/pyLIQTR/circuits/operators/cyclic_shift.py
+src/pyLIQTR/circuits/operators/diagonal_bitstring.py
 src/pyLIQTR/circuits/operators/hamiltonian_encodings.py
 src/pyLIQTR/circuits/operators/multiCZ.py
 src/pyLIQTR/circuits/operators/prepare.py
 src/pyLIQTR/circuits/operators/prepare_LinearT.py
 src/pyLIQTR/circuits/operators/prepare_oracle_pauli_lcu.py
 src/pyLIQTR/circuits/operators/reflect.py
 src/pyLIQTR/circuits/operators/selectV.py
 src/pyLIQTR/circuits/operators/selectVutils.py
 src/pyLIQTR/circuits/operators/select_LinearT.py
 src/pyLIQTR/circuits/operators/select_oracle_pauli_lcu.py
 src/pyLIQTR/circuits/operators/select_prepare_pauli.py
+src/pyLIQTR/circuits/operators/swap_network.py
+src/pyLIQTR/circuits/operators/translation.py
 src/pyLIQTR/circuits/operators/tests/__init__.py
+src/pyLIQTR/circuits/operators/tests/test_BinaryToUnary.py
+src/pyLIQTR/circuits/operators/tests/test_DataAndKeyCondition.py
+src/pyLIQTR/circuits/operators/tests/test_PhaseGradientRotation.py
+src/pyLIQTR/circuits/operators/tests/test_ProductPauliExponentials.py
+src/pyLIQTR/circuits/operators/tests/test_QROMwithMeasurementUncompute.py
+src/pyLIQTR/circuits/operators/tests/test_RotationsQROM.py
+src/pyLIQTR/circuits/operators/tests/test_cyclic_shift.py
+src/pyLIQTR/circuits/operators/tests/test_diagonal_bitstring.py
 src/pyLIQTR/circuits/operators/tests/test_hamiltonian_encodings.py
 src/pyLIQTR/circuits/operators/tests/test_multiCZ.py
+src/pyLIQTR/circuits/operators/tests/test_prepare.py
+src/pyLIQTR/circuits/operators/tests/test_qtAdd.py
 src/pyLIQTR/circuits/operators/tests/test_reflect.py
 src/pyLIQTR/circuits/operators/tests/test_selectV.py
+src/pyLIQTR/circuits/operators/tests/test_translation.py
+src/pyLIQTR/circuits/operators/tests/utils.py
 src/pyLIQTR/circuits/tests/__init__.py
 src/pyLIQTR/circuits/tests/test_pyLCircuit.py
 src/pyLIQTR/circuits/tests/test_pyLOperator.py
 src/pyLIQTR/clam/__init__.py
 src/pyLIQTR/clam/_version.py
 src/pyLIQTR/clam/atomic_lattice.py
 src/pyLIQTR/clam/cell_complex.py
@@ -117,20 +150,22 @@
 src/pyLIQTR/phase_factors/optimization/fitter.py
 src/pyLIQTR/qubitization/__init__.py
 src/pyLIQTR/qubitization/phase_estimation.py
 src/pyLIQTR/qubitization/qsvt.py
 src/pyLIQTR/qubitization/qsvt_dynamics.py
 src/pyLIQTR/qubitization/qubitized_gates.py
 src/pyLIQTR/tests/__init__.py
-src/pyLIQTR/tests/test_cirq_ft_resource_analyze_multiple_gates.py
-src/pyLIQTR/tests/test_cirq_ft_resource_analyze_single_gate.py
+src/pyLIQTR/tests/test_qualtran_resource_analyze_multiple_gates.py
+src/pyLIQTR/tests/test_qualtran_resource_analyze_single_gate.py
 src/pyLIQTR/utils/Hamiltonian.py
 src/pyLIQTR/utils/__init__.py
 src/pyLIQTR/utils/circuit_decomposition.py
+src/pyLIQTR/utils/df_utils.py
 src/pyLIQTR/utils/get_hdf5.py
+src/pyLIQTR/utils/global_ancilla_manager.py
 src/pyLIQTR/utils/pauli_string_manip.py
 src/pyLIQTR/utils/plot_helpers.py
 src/pyLIQTR/utils/printing.py
 src/pyLIQTR/utils/qsp_helpers.py
 src/pyLIQTR/utils/resource_analysis.py
 src/pyLIQTR/utils/utils.py
 src/pyLIQTR/utils/tests/__init__.py
```

