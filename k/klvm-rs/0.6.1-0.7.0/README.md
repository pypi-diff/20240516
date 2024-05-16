# Comparing `tmp/klvm_rs-0.6.1.tar.gz` & `tmp/klvm_rs-0.7.0.tar.gz`

## Comparing `klvm_rs-0.6.1.tar` & `klvm_rs-0.7.0.tar`

### file list

```diff
@@ -1,845 +1,894 @@
--rw-r--r--   0      501       20      224 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.cargo/config.toml
--rw-r--r--   0      501       20      290 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.github/workflows/audit-check.yaml.bak
--rw-r--r--   0      501       20     1692 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.github/workflows/benchmark.yml
--rw-r--r--   0      501       20     2379 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.github/workflows/build-arm64-wheels.yml
--rw-r--r--   0      501       20      924 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.github/workflows/build-crate.yml
--rw-r--r--   0      501       20     3777 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.github/workflows/build-m1-wheel.yml.bak
--rw-r--r--   0      501       20     1056 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.github/workflows/build-npm.yml
--rw-r--r--   0      501       20     9334 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.github/workflows/build-test.yml
--rw-r--r--   0      501       20      885 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.github/workflows/dependency-review.yml.bak
--rw-r--r--   0      501       20       14 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/.gitignore
--rw-r--r--   0      501       20    11347 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/LICENSE
--rw-r--r--   0      501       20      912 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/README.md
--rw-r--r--   0      501       20      619 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/RELEASE.md
--rw-r--r--   0      501       20     2219 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/activate
--rw-r--r--   0      501       20   138437 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benches/block_af9c3d98.bin
--rw-r--r--   0      501       20     2986 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benches/deserialize.rs
--rw-r--r--   0      501       20     9215 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benches/run-program.rs
--rw-r--r--   0      501       20  1560006 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/block-2000.hex
--rw-r--r--   0      501       20     1771 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/compressed-2000.envhex
--rw-r--r--   0      501       20   596274 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/compressed-2000.hex
--rw-r--r--   0      501       20      426 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/concat.hex
--rw-r--r--   0      501       20      509 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/concat.klvm
--rw-r--r--   0      501       20      198 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/count-even.hex
--rw-r--r--   0      501       20      320 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/count-even.klvm
--rw-r--r--   0      501       20      198 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/factorial.hex
--rw-r--r--   0      501       20      247 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/factorial.klvm
--rw-r--r--   0      501       20       22 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/hash-string.hex
--rw-r--r--   0      501       20       51 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/hash-string.klvm
--rw-r--r--   0      501       20      210 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/hash-tree.hex
--rw-r--r--   0      501       20      246 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/hash-tree.klvm
--rw-r--r--   0      501       20      714 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/large-block.hex
--rw-r--r--   0      501       20      401 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/large-block.klvm
--rw-r--r--   0      501       20      178 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_add.hex
--rw-r--r--   0      501       20      193 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_add.klvm
--rw-r--r--   0      501       20      166 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_ior.hex
--rw-r--r--   0      501       20      183 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_ior.klvm
--rw-r--r--   0      501       20      188 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_not.hex
--rw-r--r--   0      501       20      224 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_not.klvm
--rw-r--r--   0      501       20      178 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_sub.hex
--rw-r--r--   0      501       20      193 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_sub.klvm
--rw-r--r--   0      501       20      182 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_xor.hex
--rw-r--r--   0      501       20      207 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/loop_xor.klvm
--rw-r--r--   0      501       20     1364 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/matrix-multiply.hex
--rw-r--r--   0      501       20     1793 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/matrix-multiply.klvm
--rw-r--r--   0      501       20      218 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/point-pow.hex
--rw-r--r--   0      501       20      288 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/point-pow.klvm
--rw-r--r--   0      501       20      226 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/pubkey-tree.hex
--rw-r--r--   0      501       20      318 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/pubkey-tree.klvm
--rw-r--r--   0      501       20      228 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/shift-left.hex
--rw-r--r--   0      501       20      292 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/shift-left.klvm
--rw-r--r--   0      501       20      318 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/substr-tree.hex
--rw-r--r--   0      501       20      488 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/substr-tree.klvm
--rw-r--r--   0      501       20      254 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/substr.hex
--rw-r--r--   0      501       20      390 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/substr.klvm
--rw-r--r--   0      501       20      210 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/sum-tree.hex
--rw-r--r--   0      501       20      237 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmark/sum-tree.klvm
--rw-r--r--   0      501       20     3976 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/benchmarks.txt
--rw-r--r--   0      501       20     2273 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/docs/new-operator-checklist.md
--rw-r--r--   0      501       20    62286 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-bls-ops.txt
--rw-r--r--   0      501       20     1286 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-bls-zk.txt
--rw-r--r--   0      501       20    31892 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-blspy-g1.txt
--rw-r--r--   0      501       20    60143 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-blspy-g2.txt
--rw-r--r--   0      501       20    52970 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-blspy-hash.txt
--rw-r--r--   0      501       20    43673 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-blspy-pairing.txt
--rw-r--r--   0      501       20    23174 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-blspy-verify.txt
--rw-r--r--   0      501       20     3762 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-core-ops.txt
--rw-r--r--   0      501       20    19990 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-modpow.txt
--rw-r--r--   0      501       20    69027 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-more-ops.txt
--rw-r--r--   0      501       20     7730 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-secp-verify.txt
--rw-r--r--   0      501       20    11662 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-secp256k1.txt
--rw-r--r--   0      501       20    11662 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-secp256r1.txt
--rw-r--r--   0      501       20    66095 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/op-tests/test-sha256.txt
--rw-r--r--   0      501       20    55362 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/allocator.rs
--rw-r--r--   0      501       20    11218 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/bls_ops.rs
--rw-r--r--   0      501       20     6952 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/chik_dialect.rs
--rw-r--r--   0      501       20     2879 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/core_ops.rs
--rw-r--r--   0      501       20      288 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/cost.rs
--rw-r--r--   0      501       20      598 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/dialect.rs
--rw-r--r--   0      501       20      164 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/err_utils.rs
--rw-r--r--   0      501       20     3265 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/f_table.rs
--rw-r--r--   0      501       20      845 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/lib.rs
--rw-r--r--   0      501       20    35984 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/more_ops.rs
--rw-r--r--   0      501       20    10410 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/number.rs
--rw-r--r--   0      501       20    18938 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/op_utils.rs
--rw-r--r--   0      501       20      608 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/reduction.rs
--rw-r--r--   0      501       20    48277 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/run_program.rs
--rw-r--r--   0      501       20     1927 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/runtime_dialect.rs
--rw-r--r--   0      501       20     2825 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/secp_ops.rs
--rw-r--r--   0      501       20      383 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/bytes32.rs
--rw-r--r--   0      501       20     1342 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/de.rs
--rw-r--r--   0      501       20     6680 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/de_br.rs
--rw-r--r--   0      501       20    10932 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/de_tree.rs
--rw-r--r--   0      501       20      221 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/errors.rs
--rw-r--r--   0      501       20      538 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/mod.rs
--rw-r--r--   0      501       20     8745 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/object_cache.rs
--rw-r--r--   0      501       20     7154 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/parse_atom.rs
--rw-r--r--   0      501       20    14027 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/read_cache_lookup.rs
--rw-r--r--   0      501       20     3073 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/ser.rs
--rw-r--r--   0      501       20     2817 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/ser_br.rs
--rw-r--r--   0      501       20     2414 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/test.rs
--rw-r--r--   0      501       20    23381 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/tools.rs
--rw-r--r--   0      501       20      596 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/utils.rs
--rw-r--r--   0      501       20     6233 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/serde/write_atom.rs
--rw-r--r--   0      501       20     1341 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/sha2.rs
--rw-r--r--   0      501       20    17040 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/test_ops.rs
--rw-r--r--   0      501       20     3721 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/tests.rs
--rw-r--r--   0      501       20     8722 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/src/traverse_path.rs
--rwxr-xr-x   0      501       20     8807 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/generate-programs.py
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-add.envhex
--rw-r--r--   0      501       20    40242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-add.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-all.envhex
--rw-r--r--   0      501       20  1200242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-all.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-and.envhex
--rw-r--r--   0      501       20    40242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-and.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-any.envhex
--rw-r--r--   0      501       20  1200242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-any.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-cat.envhex
--rw-r--r--   0      501       20    40242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-cat.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-mul.envhex
--rw-r--r--   0      501       20    40242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-mul.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-or.envhex
--rw-r--r--   0      501       20    40242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-or.hex
--rw-r--r--   0      501       20        7 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-point_add.envhex
--rw-r--r--   0      501       20    48191 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-point_add.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-sha.envhex
--rw-r--r--   0      501       20    40242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-sha.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-sub.envhex
--rw-r--r--   0      501       20    40242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-sub.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-1.envhex
--rw-r--r--   0      501       20    20252 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-1.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-2.envhex
--rw-r--r--   0      501       20    12248 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-2.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-3.envhex
--rw-r--r--   0      501       20    12248 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-3.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-4.envhex
--rw-r--r--   0      501       20    12248 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-4.hex
--rw-r--r--   0      501       20       13 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-5.envhex
--rw-r--r--   0      501       20      383 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-5.hex
--rw-r--r--   0      501       20       15 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-6.envhex
--rw-r--r--   0      501       20      381 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-6.hex
--rw-r--r--   0      501       20       15 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-7.envhex
--rw-r--r--   0      501       20      381 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-7.hex
--rw-r--r--   0      501       20       15 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-8.envhex
--rw-r--r--   0      501       20      381 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-8.hex
--rw-r--r--   0      501       20       15 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-9.envhex
--rw-r--r--   0      501       20      381 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-unknown-9.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-xor.envhex
--rw-r--r--   0      501       20    40242 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/args-xor.hex
--rw-r--r--   0      501       20       13 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-add.envhex
--rw-r--r--   0      501       20      261 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-add.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-ash.envhex
--rw-r--r--   0      501       20      369 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-ash.hex
--rw-r--r--   0      501       20        7 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-cat.envhex
--rw-r--r--   0      501       20      223 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-cat.hex
--rw-r--r--   0      501       20       15 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-cons.envhex
--rw-r--r--   0      501       20      211 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-cons.hex
--rw-r--r--   0      501       20       13 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-div.envhex
--rw-r--r--   0      501       20      363 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-div.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-lsh.envhex
--rw-r--r--   0      501       20      369 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-lsh.hex
--rw-r--r--   0      501       20        7 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-mul.envhex
--rw-r--r--   0      501       20      257 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-mul.hex
--rw-r--r--   0      501       20       15 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-not.envhex
--rw-r--r--   0      501       20      355 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-not.hex
--rw-r--r--   0      501       20       11 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-pubkey.envhex
--rw-r--r--   0      501       20      355 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-pubkey.hex
--rw-r--r--   0      501       20       13 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-sub.envhex
--rw-r--r--   0      501       20      261 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/recursive-sub.hex
--rw-r--r--   0      501       20       15 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/softfork-1.envhex
--rw-r--r--   0      501       20      229 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/softfork-1.hex
--rw-r--r--   0      501       20       15 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/softfork-2.envhex
--rw-r--r--   0      501       20      221 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/programs/softfork-2.hex
--rwxr-xr-x   0      501       20     4581 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/run-programs.py
--rwxr-xr-x   0      501       20     1574 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/tests/run.py
--rw-r--r--   0      501       20     2219 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/bin/activate
--rw-r--r--   0      501       20     1271 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/bin/activate.csh
--rw-r--r--   0      501       20     2423 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/bin/activate.fish
--rwxr-xr-x   0      501       20      264 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/bin/easy_install
--rwxr-xr-x   0      501       20      264 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/bin/easy_install-3.7
--rwxr-xr-x   0      501       20      255 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/bin/pip
--rwxr-xr-x   0      501       20      255 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/bin/pip3
--rwxr-xr-x   0      501       20      255 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/bin/pip3.7
--rwxr-xr-x   0      501       20    49640 2024-04-06 23:31:12.000000 klvm_rs-0.6.1/venv/bin/python
--rwxr-xr-x   0      501       20    49640 2024-04-06 23:31:12.000000 klvm_rs-0.6.1/venv/bin/python3
--rw-r--r--   0      501       20      126 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/easy_install.py
--rw-r--r--   0      501       20      357 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/__init__.py
--rw-r--r--   0      501       20     1198 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/__main__.py
--rw-r--r--   0      501       20     1444 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/__pip-runner__.py
--rw-r--r--   0      501       20      573 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/__init__.py
--rw-r--r--   0      501       20    10243 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/build_env.py
--rw-r--r--   0      501       20    10734 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cache.py
--rw-r--r--   0      501       20      132 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0      501       20     6676 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0      501       20     7842 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0      501       20    29497 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0      501       20      774 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0      501       20     2472 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0      501       20     4338 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0      501       20    10817 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0      501       20     1968 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0      501       20    18172 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0      501       20     5118 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0      501       20      116 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0      501       20     3882 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0      501       20     7582 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0      501       20     1685 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0      501       20     4129 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0      501       20     9815 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0      501       20     6591 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0      501       20     5289 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0      501       20     2951 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0      501       20     1703 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0      501       20     1132 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0      501       20     4793 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0      501       20     3188 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0      501       20    32389 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0      501       20    12343 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0      501       20     5697 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0      501       20     6419 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0      501       20     3886 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0      501       20     7396 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0      501       20    13529 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/configuration.py
--rw-r--r--   0      501       20      858 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0      501       20     1221 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0      501       20      729 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0      501       20     6494 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0      501       20     1164 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0      501       20    24244 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0      501       20       30 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0      501       20    16504 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0      501       20    37873 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0      501       20     6557 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0      501       20    15365 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0      501       20     6100 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0      501       20     7680 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0      501       20     2556 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0      501       20      340 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/main.py
--rw-r--r--   0      501       20     4280 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0      501       20     2595 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0      501       20    25277 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0      501       20      107 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0      501       20     1882 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0      501       20     8181 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0      501       20     7457 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0      501       20     9773 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0      501       20       63 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0      501       20      990 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0      501       20     6626 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0      501       20     2520 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0      501       20     1030 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/index.py
--rw-r--r--   0      501       20     2617 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0      501       20    18602 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/link.py
--rw-r--r--   0      501       20      738 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0      501       20     4644 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0      501       20     1907 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0      501       20     3858 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0      501       20     3600 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0      501       20       50 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0      501       20    16507 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0      501       20     2145 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0      501       20     6096 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/download.py
--rw-r--r--   0      501       20     7638 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0      501       20    18443 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/session.py
--rw-r--r--   0      501       20     4073 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0      501       20     1791 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0      501       20     4133 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0      501       20     1422 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0      501       20     1474 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0      501       20     2198 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0      501       20     1075 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0      501       20     1417 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0      501       20     3064 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0      501       20     5122 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0      501       20     9784 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0      501       20       51 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0      501       20     1354 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0      501       20     4105 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0      501       20    27407 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0      501       20    25091 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0      501       20     6987 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0      501       20     2807 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0      501       20    16611 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0      501       20    17646 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0      501       20    35763 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0      501       20     2858 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0      501       20    24045 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0      501       20      583 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0      501       20    24129 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0      501       20     5220 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0      501       20    18963 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0      501       20    27878 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0      501       20     5705 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0      501       20     9914 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0      501       20     2526 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0      501       20     5455 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0      501       20    11533 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0      501       20     8167 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0      501       20     1015 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0      501       20     1665 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0      501       20     1884 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0      501       20     5377 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0      501       20      242 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0      501       20     5764 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0      501       20     3206 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0      501       20     1115 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0      501       20     2118 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0      501       20     1169 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0      501       20     3064 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0      501       20     5122 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0      501       20      716 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0      501       20     3110 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0      501       20     4831 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0      501       20      795 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0      501       20    11632 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0      501       20    22253 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0      501       20     1193 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0      501       20     2108 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0      501       20     5662 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0      501       20     9200 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0      501       20     7702 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0      501       20     8821 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0      501       20     1759 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0      501       20     3456 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0      501       20     4549 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0      501       20      596 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0      501       20     3519 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0      501       20    18116 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0      501       20     5238 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0      501       20    11729 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0      501       20    22811 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0      501       20    13079 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0      501       20     4966 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0      501       20      465 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0      501       20     1379 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0      501       20     5033 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0      501       20     1535 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0      501       20      242 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0      501       20     5271 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0      501       20     1033 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0      501       20      778 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0      501       20    16416 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0      501       20     3946 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0      501       20     4154 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0      501       20     7105 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0      501       20      774 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0      501       20       94 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0      501       20      255 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0      501       20   275233 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0      501       20     4279 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0      501       20     4797 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0      501       20    31274 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0      501       20     1763 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0      501       20    10032 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0      501       20     3915 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0      501       20     5420 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0      501       20     3242 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0      501       20     3732 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0      501       20      542 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0      501       20     1860 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0      501       20     1683 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0      501       20     4006 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0      501       20    12176 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0      501       20     3934 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0      501       20    13566 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0      501       20     1753 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0      501       20    36913 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0      501       20     1753 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0      501       20    20735 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0      501       20     1759 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0      501       20    14537 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0      501       20    25796 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0      501       20    42498 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0      501       20     1752 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0      501       20    27055 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0      501       20   104562 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0      501       20    98484 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0      501       20    98196 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0      501       20   101363 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0      501       20   128035 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0      501       20   102774 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0      501       20    95372 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0      501       20     5380 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0      501       20     6077 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0      501       20     3715 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0      501       20     2131 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0      501       20    30391 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0      501       20    13560 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0      501       20      402 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0      501       20     6400 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0      501       20     4137 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0      501       20     4007 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0      501       20    14848 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0      501       20     8505 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0      501       20     2812 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0      501       20      244 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0      501       20      266 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0      501       20     2522 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0      501       20    11128 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0      501       20     3325 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0      501       20       75 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0      501       20     2839 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0      501       20    10678 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0      501       20     6741 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0      501       20     1866 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0      501       20     1079 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0      501       20     3709 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0      501       20     6181 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0      501       20     7134 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0      501       20      581 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0      501       20    41259 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0      501       20    51697 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0      501       20    20834 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0      501       20    51991 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0      501       20    14811 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0      501       20     5058 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0      501       20    39801 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0      501       20    10820 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0      501       20    18102 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0      501       20    97792 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0      501       20   182784 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0      501       20   108032 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0      501       20    66262 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0      501       20    23513 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0      501       20    91648 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0      501       20   168448 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0      501       20   101888 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0      501       20    43898 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0      501       20      981 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0      501       20       64 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0      501       20    49330 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0      501       20      849 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0      501       20     3374 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0      501       20      321 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0      501       20    12950 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0      501       20    44375 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0      501       20     1881 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0      501       20       21 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0      501       20   206539 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0      501       20     1132 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0      501       20     1081 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0      501       20     6080 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0      501       20    34557 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0      501       20      661 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0      501       20      497 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0      501       20    11488 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0      501       20     4378 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0      501       20     1431 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0      501       20     8487 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0      501       20     4676 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0      501       20    30110 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0      501       20    15699 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0      501       20     4200 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0      501       20    14665 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0      501       20   108287 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0      501       20      562 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0      501       20    12936 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0      501       20     1176 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0      501       20     4068 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0      501       20     4910 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0      501       20     2655 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0      501       20     6911 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0      501       20      160 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0      501       20     6596 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0      501       20     2999 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0      501       20      353 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0      501       20    23685 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0      501       20     1697 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0      501       20     1938 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0      501       20    40386 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0      501       20     2917 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0      501       20     4810 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0      501       20     4104 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0      501       20     3314 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0      501       20     5086 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0      501       20    35441 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0      501       20    21938 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0      501       20     5871 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0      501       20    19351 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0      501       20     5073 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0      501       20     2212 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0      501       20     5014 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0      501       20     7335 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0      501       20     4674 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0      501       20    11753 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0      501       20    32005 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0      501       20    11174 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0      501       20    70232 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0      501       20    53376 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0      501       20      986 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0      501       20     2591 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0      501       20     3072 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0      501       20     3092 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0      501       20     4630 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0      501       20     6257 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0      501       20     3419 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0      501       20     6184 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0      501       20    63187 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0      501       20     9110 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0      501       20     9171 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0      501       20     6426 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0      501       20    12936 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0      501       20   213344 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0      501       20    23685 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0      501       20     9023 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0      501       20    39129 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0      501       20    25341 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0      501       20    13402 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0      501       20    10787 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0      501       20     6805 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0      501       20      491 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0      501       20      138 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0      501       20    11920 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0      501       20      546 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0      501       20    10927 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0      501       20     5178 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0      501       20      435 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0      501       20     1397 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0      501       20    21443 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0      501       20     6377 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0      501       20    10187 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0      501       20      575 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0      501       20     1286 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0      501       20    18560 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0      501       20     3823 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0      501       20     3879 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0      501       20      733 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0      501       20    35288 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0      501       20      695 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0      501       20    30180 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0      501       20     4235 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0      501       20     2912 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0      501       20    33240 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0      501       20      537 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0      501       20      156 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0      501       20     5872 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0      501       20     1583 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0      501       20    17592 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0      501       20     4794 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0      501       20     6090 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0      501       20     8478 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0      501       20    10096 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0      501       20   140235 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0      501       20     1064 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0      501       20     2114 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0      501       20      265 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0      501       20     9695 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0      501       20     3225 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0      501       20     1236 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0      501       20     1643 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0      501       20     7063 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0      501       20      423 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0      501       20     5472 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0      501       20    19919 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0      501       20      351 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0      501       20      417 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0      501       20    22820 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0      501       20     1926 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0      501       20     2783 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0      501       20     1840 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0      501       20      890 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0      501       20    10368 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0      501       20     6819 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0      501       20     3264 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0      501       20     9842 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0      501       20     4503 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0      501       20    18015 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0      501       20     1054 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0      501       20     7131 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0      501       20    97992 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0      501       20     1288 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0      501       20     5497 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0      501       20     6630 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0      501       20     7954 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0      501       20      972 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0      501       20     2501 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0      501       20      642 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0      501       20     1616 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0      501       20     2508 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0      501       20     9585 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0      501       20     5053 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0      501       20     3252 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0      501       20    14007 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0      501       20    14172 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0      501       20     3667 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0      501       20    11903 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0      501       20     8198 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0      501       20     5305 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0      501       20     4970 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0      501       20      828 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0      501       20     3396 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0      501       20    10574 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0      501       20    37414 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0      501       20    59836 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0      501       20     8165 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0      501       20    11303 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0      501       20     1391 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0      501       20      166 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0      501       20     4436 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0      501       20     4773 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0      501       20     2843 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0      501       20     1591 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0      501       20    24224 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0      501       20     4374 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0      501       20     4425 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0      501       20    26332 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0      501       20     1258 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0      501       20    34995 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0      501       20    39684 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0      501       20     3370 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0      501       20    45686 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0      501       20     3627 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0      501       20      102 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0      501       20    26070 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0      501       20     9169 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0      501       20    34549 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/six.py
--rw-r--r--   0      501       20    18364 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0      501       20     3314 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0      501       20     1944 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0      501       20     1496 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0      501       20     1376 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0      501       20     1908 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0      501       20     1383 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0      501       20     7550 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0      501       20     2790 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0      501       20     2145 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0      501       20     8011 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0      501       20      396 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0      501       20    22633 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0      501       20     2943 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0      501       20      254 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0      501       20    80114 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0      501       20     3333 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0      501       20    10811 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0      501       20       64 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0      501       20    20070 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0      501       20    39095 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0      501       20      957 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0      501       20    17632 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0      501       20    13922 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0      501       20    11036 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0      501       20     4528 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0      501       20    17081 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0      501       20    34448 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0      501       20     7097 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0      501       20     8217 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0      501       20     8579 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0      501       20     2440 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0      501       20     1417 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0      501       20    34665 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0      501       20    19786 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0      501       20     5985 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0      501       20    30641 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0      501       20     1155 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0      501       20     4901 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0      501       20     1605 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0      501       20      498 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0      501       20     3997 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0      501       20     3510 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0      501       20    22003 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0      501       20    17177 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0      501       20     5758 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0      501       20     6895 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0      501       20    10003 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0      501       20    14298 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0      501       20     5403 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0      501       20      476 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0      501       20    10579 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0      501       20     8979 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0      501       20     1305 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0      501       20     6563 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0      501       20     4307 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0      501       20      286 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/py.typed
--rw-r--r--   0      501       20        4 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/INSTALLER
--rw-r--r--   0      501       20     1093 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/LICENSE.txt
--rw-r--r--   0      501       20     4072 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/METADATA
--rw-r--r--   0      501       20    76671 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/RECORD
--rw-r--r--   0      501       20        0 2024-04-11 05:24:36.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/REQUESTED
--rw-r--r--   0      501       20       92 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/WHEEL
--rw-r--r--   0      501       20      124 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/entry_points.txt
--rw-r--r--   0      501       20        4 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/top_level.txt
--rw-r--r--   0      501       20   108570 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/__init__.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0      501       20    24701 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0      501       20      720 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0      501       20      513 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0      501       20      860 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rw-r--r--   0      501       20     1416 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0      501       20     8248 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0      501       20     4355 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0      501       20    28025 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0      501       20      421 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0      501       20    11556 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0      501       20   232055 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/pyparsing.py
--rw-r--r--   0      501       20    30098 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/six.py
--rw-r--r--   0      501       20     2101 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0      501       20      396 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/py2_warn.py
--rw-r--r--   0      501       20      558 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/py31compat.py
--rw-r--r--   0      501       20     7341 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/__init__.py
--rw-r--r--   0      501       20      218 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0      501       20     2388 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_imp.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0      501       20    15130 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0      501       20      744 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0      501       20      562 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0      501       20      865 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/_compat.py
--rw-r--r--   0      501       20     1416 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0      501       20     8268 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0      501       20     4742 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0      501       20    27778 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0      501       20    12933 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0      501       20     1520 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0      501       20    11978 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0      501       20   232055 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/pyparsing.py
--rw-r--r--   0      501       20    30098 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/six.py
--rw-r--r--   0      501       20     6626 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/archive_util.py
--rw-r--r--   0      501       20     9960 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/build_meta.py
--rw-r--r--   0      501       20    65536 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/cli-32.exe
--rw-r--r--   0      501       20    74752 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/cli-64.exe
--rw-r--r--   0      501       20    65536 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/cli.exe
--rw-r--r--   0      501       20      568 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/__init__.py
--rw-r--r--   0      501       20     2426 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/alias.py
--rw-r--r--   0      501       20    18406 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0      501       20     1508 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0      501       20      922 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/bdist_wininst.py
--rw-r--r--   0      501       20     4415 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0      501       20    13048 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0      501       20     9737 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/build_py.py
--rw-r--r--   0      501       20     8188 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/develop.py
--rw-r--r--   0      501       20      960 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0      501       20    87657 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0      501       20    25548 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0      501       20     4705 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/install.py
--rw-r--r--   0      501       20     2203 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0      501       20     3875 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0      501       20     2519 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0      501       20      628 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0      501       20     4994 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0      501       20      468 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/register.py
--rw-r--r--   0      501       20     2164 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/rotate.py
--rw-r--r--   0      501       20      658 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0      501       20     8092 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/sdist.py
--rw-r--r--   0      501       20     5085 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/setopt.py
--rw-r--r--   0      501       20     9623 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/test.py
--rw-r--r--   0      501       20      462 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/upload.py
--rw-r--r--   0      501       20     7314 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0      501       20    21757 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/config.py
--rw-r--r--   0      501       20      949 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/dep_util.py
--rw-r--r--   0      501       20     5517 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/depends.py
--rw-r--r--   0      501       20    39211 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/dist.py
--rw-r--r--   0      501       20      524 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/errors.py
--rw-r--r--   0      501       20     1729 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/extension.py
--rw-r--r--   0      501       20     2128 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0      501       20     5084 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/glob.py
--rw-r--r--   0      501       20    65536 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/gui-32.exe
--rw-r--r--   0      501       20    75264 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/gui-64.exe
--rw-r--r--   0      501       20    65536 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/gui.exe
--rw-r--r--   0      501       20     5336 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/installer.py
--rw-r--r--   0      501       20      787 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/launch.py
--rw-r--r--   0      501       20     2384 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/lib2to3_ex.py
--rw-r--r--   0      501       20     5264 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/monkey.py
--rw-r--r--   0      501       20    50989 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/msvc.py
--rw-r--r--   0      501       20     3223 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/namespaces.py
--rw-r--r--   0      501       20    40737 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/package_index.py
--rw-r--r--   0      501       20     1504 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/py27compat.py
--rw-r--r--   0      501       20      838 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/py31compat.py
--rw-r--r--   0      501       20     1330 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/py33compat.py
--rw-r--r--   0      501       20      245 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/py34compat.py
--rw-r--r--   0      501       20    14284 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/sandbox.py
--rw-r--r--   0      501       20      218 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0      501       20      138 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/script.tmpl
--rw-r--r--   0      501       20     2346 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/site-patch.py
--rw-r--r--   0      501       20     8543 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/ssl_support.py
--rw-r--r--   0      501       20      996 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0      501       20      144 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/version.py
--rw-r--r--   0      501       20     8371 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/wheel.py
--rw-r--r--   0      501       20      714 2024-04-11 05:24:34.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/windows_support.py
--rw-r--r--   0      501       20        4 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/INSTALLER
--rw-r--r--   0      501       20     1078 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/LICENSE
--rw-r--r--   0      501       20     4806 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/METADATA
--rw-r--r--   0      501       20    14645 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/RECORD
--rw-r--r--   0      501       20        0 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/REQUESTED
--rw-r--r--   0      501       20       92 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/WHEEL
--rw-r--r--   0      501       20      239 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/dependency_links.txt
--rw-r--r--   0      501       20     3143 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/entry_points.txt
--rw-r--r--   0      501       20       38 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/top_level.txt
--rw-r--r--   0      501       20        1 2024-04-11 05:24:35.000000 klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/zip-safe
--rw-r--r--   0      501       20      113 2024-04-11 05:24:33.000000 klvm_rs-0.6.1/venv/pyvenv.cfg
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 klvm_rs-0.6.1/wheel/Cargo.toml
--rw-r--r--   0      501       20      606 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/README.md
--rw-r--r--   0      501       20      100 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/__init__.py
--rw-r--r--   0      501       20      873 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/at.py
--rw-r--r--   0      501       20     5444 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/casts.py
--rw-r--r--   0      501       20      941 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/chik_dialect.py
--rw-r--r--   0      501       20     5402 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/curry_and_treehash.py
--rw-r--r--   0      501       20     3732 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/de.py
--rw-r--r--   0      501       20      133 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/eval_error.py
--rw-r--r--   0      501       20      609 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/klvm_rs.pyi
--rw-r--r--   0      501       20      695 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/klvm_storage.py
--rw-r--r--   0      501       20     4903 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/klvm_tree.py
--rw-r--r--   0      501       20    10761 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/program.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/py.typed
--rw-r--r--   0      501       20     1164 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/replace.py
--rw-r--r--   0      501       20     5038 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/ser.py
--rw-r--r--   0      501       20     3559 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/klvm_rs/tree_hash.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/tests/__init__.py
--rw-r--r--   0      501       20     6721 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/tests/test_apis.py
--rw-r--r--   0      501       20     1530 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/tests/test_curry_and_treehash.py
--rw-r--r--   0      501       20    16181 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/tests/test_program.py
--rw-r--r--   0      501       20     5046 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/python/tests/test_serialize.py
--rw-r--r--   0      501       20      828 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/src/adapt_response.rs
--rw-r--r--   0      501       20     2652 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/src/api.rs
--rw-r--r--   0      501       20     1388 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/src/lazy_node.rs
--rw-r--r--   0      501       20       52 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/wheel/src/lib.rs
--rw-r--r--   0      501       20    48403 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/Cargo.lock
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 klvm_rs-0.6.1/Cargo.toml
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 klvm_rs-0.6.1/pyproject.toml
--rw-r--r--   0      501       20      609 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/klvm_rs.pyi
--rw-r--r--   0      501       20     4903 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/klvm_tree.py
--rw-r--r--   0      501       20     5038 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/ser.py
--rw-r--r--   0      501       20      695 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/klvm_storage.py
--rw-r--r--   0      501       20      941 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/chik_dialect.py
--rw-r--r--   0      501       20     5444 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/casts.py
--rw-r--r--   0      501       20     3559 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/tree_hash.py
--rw-r--r--   0      501       20      100 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/__init__.py
--rw-r--r--   0      501       20      133 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/eval_error.py
--rw-r--r--   0      501       20      873 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/at.py
--rw-r--r--   0      501       20    10761 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/program.py
--rw-r--r--   0      501       20        0 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/py.typed
--rw-r--r--   0      501       20     5402 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/curry_and_treehash.py
--rw-r--r--   0      501       20     3732 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/de.py
--rw-r--r--   0      501       20     1164 2024-04-11 05:24:12.000000 klvm_rs-0.6.1/python/klvm_rs/replace.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 klvm_rs-0.6.1/PKG-INFO
+-rw-r--r--   0      501       20      224 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.cargo/config.toml
+-rw-r--r--   0      501       20      290 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.github/workflows/audit-check.yaml.bak
+-rw-r--r--   0      501       20     1692 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.github/workflows/benchmark.yml
+-rw-r--r--   0      501       20     2316 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.github/workflows/build-arm64-wheels.yml
+-rw-r--r--   0      501       20      924 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.github/workflows/build-crate.yml
+-rw-r--r--   0      501       20     3777 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.github/workflows/build-m1-wheel.yml.bak
+-rw-r--r--   0      501       20     1056 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.github/workflows/build-npm.yml
+-rw-r--r--   0      501       20     9327 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.github/workflows/build-test.yml
+-rw-r--r--   0      501       20      885 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.github/workflows/dependency-review.yml.bak
+-rw-r--r--   0      501       20       14 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/.gitignore
+-rw-r--r--   0      501       20    11347 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/LICENSE
+-rw-r--r--   0      501       20      912 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/README.md
+-rw-r--r--   0      501       20      619 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/RELEASE.md
+-rw-r--r--   0      501       20     2198 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/activate
+-rw-r--r--   0      501       20   138437 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benches/block_af9c3d98.bin
+-rw-r--r--   0      501       20     2986 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benches/deserialize.rs
+-rw-r--r--   0      501       20     9215 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benches/run-program.rs
+-rw-r--r--   0      501       20  1560006 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/block-2000.hex
+-rw-r--r--   0      501       20     1771 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/compressed-2000.envhex
+-rw-r--r--   0      501       20   596274 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/compressed-2000.hex
+-rw-r--r--   0      501       20      426 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/concat.hex
+-rw-r--r--   0      501       20      509 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/concat.klvm
+-rw-r--r--   0      501       20      198 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/count-even.hex
+-rw-r--r--   0      501       20      320 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/count-even.klvm
+-rw-r--r--   0      501       20      198 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/factorial.hex
+-rw-r--r--   0      501       20      247 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/factorial.klvm
+-rw-r--r--   0      501       20       22 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/hash-string.hex
+-rw-r--r--   0      501       20       51 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/hash-string.klvm
+-rw-r--r--   0      501       20      210 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/hash-tree.hex
+-rw-r--r--   0      501       20      246 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/hash-tree.klvm
+-rw-r--r--   0      501       20      714 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/large-block.hex
+-rw-r--r--   0      501       20      401 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/large-block.klvm
+-rw-r--r--   0      501       20      178 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_add.hex
+-rw-r--r--   0      501       20      193 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_add.klvm
+-rw-r--r--   0      501       20      166 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_ior.hex
+-rw-r--r--   0      501       20      183 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_ior.klvm
+-rw-r--r--   0      501       20      188 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_not.hex
+-rw-r--r--   0      501       20      224 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_not.klvm
+-rw-r--r--   0      501       20      178 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_sub.hex
+-rw-r--r--   0      501       20      193 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_sub.klvm
+-rw-r--r--   0      501       20      182 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_xor.hex
+-rw-r--r--   0      501       20      207 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/loop_xor.klvm
+-rw-r--r--   0      501       20     1364 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/matrix-multiply.hex
+-rw-r--r--   0      501       20     1793 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/matrix-multiply.klvm
+-rw-r--r--   0      501       20      218 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/point-pow.hex
+-rw-r--r--   0      501       20      288 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/point-pow.klvm
+-rw-r--r--   0      501       20      226 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/pubkey-tree.hex
+-rw-r--r--   0      501       20      318 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/pubkey-tree.klvm
+-rw-r--r--   0      501       20      228 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/shift-left.hex
+-rw-r--r--   0      501       20      292 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/shift-left.klvm
+-rw-r--r--   0      501       20      318 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/substr-tree.hex
+-rw-r--r--   0      501       20      488 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/substr-tree.klvm
+-rw-r--r--   0      501       20      254 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/substr.hex
+-rw-r--r--   0      501       20      390 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/substr.klvm
+-rw-r--r--   0      501       20      210 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/sum-tree.hex
+-rw-r--r--   0      501       20      237 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmark/sum-tree.klvm
+-rw-r--r--   0      501       20     3976 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/benchmarks.txt
+-rw-r--r--   0      501       20     2273 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/docs/new-operator-checklist.md
+-rw-r--r--   0      501       20    62286 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-bls-ops.txt
+-rw-r--r--   0      501       20     1286 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-bls-zk.txt
+-rw-r--r--   0      501       20    31892 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-blspy-g1.txt
+-rw-r--r--   0      501       20    60143 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-blspy-g2.txt
+-rw-r--r--   0      501       20    52970 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-blspy-hash.txt
+-rw-r--r--   0      501       20    43673 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-blspy-pairing.txt
+-rw-r--r--   0      501       20    23174 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-blspy-verify.txt
+-rw-r--r--   0      501       20     3762 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-core-ops.txt
+-rw-r--r--   0      501       20    19990 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-modpow.txt
+-rw-r--r--   0      501       20    69027 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-more-ops.txt
+-rw-r--r--   0      501       20     7730 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-secp-verify.txt
+-rw-r--r--   0      501       20    11662 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-secp256k1.txt
+-rw-r--r--   0      501       20    11662 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-secp256r1.txt
+-rw-r--r--   0      501       20    66095 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/op-tests/test-sha256.txt
+-rw-r--r--   0      501       20    55363 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/allocator.rs
+-rw-r--r--   0      501       20    11218 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/bls_ops.rs
+-rw-r--r--   0      501       20     6953 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/chik_dialect.rs
+-rw-r--r--   0      501       20     2879 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/core_ops.rs
+-rw-r--r--   0      501       20      288 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/cost.rs
+-rw-r--r--   0      501       20      598 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/dialect.rs
+-rw-r--r--   0      501       20      164 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/err_utils.rs
+-rw-r--r--   0      501       20     3265 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/f_table.rs
+-rw-r--r--   0      501       20      845 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/lib.rs
+-rw-r--r--   0      501       20    35984 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/more_ops.rs
+-rw-r--r--   0      501       20    10410 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/number.rs
+-rw-r--r--   0      501       20    18938 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/op_utils.rs
+-rw-r--r--   0      501       20      608 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/reduction.rs
+-rw-r--r--   0      501       20    48314 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/run_program.rs
+-rw-r--r--   0      501       20     1927 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/runtime_dialect.rs
+-rw-r--r--   0      501       20     2825 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/secp_ops.rs
+-rw-r--r--   0      501       20      383 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/bytes32.rs
+-rw-r--r--   0      501       20     1342 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/de.rs
+-rw-r--r--   0      501       20     6680 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/de_br.rs
+-rw-r--r--   0      501       20    10932 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/de_tree.rs
+-rw-r--r--   0      501       20      221 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/errors.rs
+-rw-r--r--   0      501       20      593 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/mod.rs
+-rw-r--r--   0      501       20     8745 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/object_cache.rs
+-rw-r--r--   0      501       20     7154 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/parse_atom.rs
+-rw-r--r--   0      501       20    14029 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/read_cache_lookup.rs
+-rw-r--r--   0      501       20     3073 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/ser.rs
+-rw-r--r--   0      501       20     3862 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/ser_br.rs
+-rw-r--r--   0      501       20     2414 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/test.rs
+-rw-r--r--   0      501       20    23382 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/tools.rs
+-rw-r--r--   0      501       20      596 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/utils.rs
+-rw-r--r--   0      501       20     6233 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/serde/write_atom.rs
+-rw-r--r--   0      501       20     1341 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/sha2.rs
+-rw-r--r--   0      501       20    17128 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/test_ops.rs
+-rw-r--r--   0      501       20     3721 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/tests.rs
+-rw-r--r--   0      501       20     8722 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/src/traverse_path.rs
+-rwxr-xr-x   0      501       20     8807 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/generate-programs.py
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-add.envhex
+-rw-r--r--   0      501       20    40242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-add.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-all.envhex
+-rw-r--r--   0      501       20  1200242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-all.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-and.envhex
+-rw-r--r--   0      501       20    40242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-and.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-any.envhex
+-rw-r--r--   0      501       20  1200242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-any.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-cat.envhex
+-rw-r--r--   0      501       20    40242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-cat.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-mul.envhex
+-rw-r--r--   0      501       20    40242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-mul.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-or.envhex
+-rw-r--r--   0      501       20    40242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-or.hex
+-rw-r--r--   0      501       20        7 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-point_add.envhex
+-rw-r--r--   0      501       20    48191 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-point_add.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-sha.envhex
+-rw-r--r--   0      501       20    40242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-sha.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-sub.envhex
+-rw-r--r--   0      501       20    40242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-sub.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-1.envhex
+-rw-r--r--   0      501       20    20252 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-1.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-2.envhex
+-rw-r--r--   0      501       20    12248 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-2.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-3.envhex
+-rw-r--r--   0      501       20    12248 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-3.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-4.envhex
+-rw-r--r--   0      501       20    12248 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-4.hex
+-rw-r--r--   0      501       20       13 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-5.envhex
+-rw-r--r--   0      501       20      383 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-5.hex
+-rw-r--r--   0      501       20       15 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-6.envhex
+-rw-r--r--   0      501       20      381 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-6.hex
+-rw-r--r--   0      501       20       15 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-7.envhex
+-rw-r--r--   0      501       20      381 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-7.hex
+-rw-r--r--   0      501       20       15 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-8.envhex
+-rw-r--r--   0      501       20      381 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-8.hex
+-rw-r--r--   0      501       20       15 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-9.envhex
+-rw-r--r--   0      501       20      381 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-unknown-9.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-xor.envhex
+-rw-r--r--   0      501       20    40242 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/args-xor.hex
+-rw-r--r--   0      501       20       13 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-add.envhex
+-rw-r--r--   0      501       20      261 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-add.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-ash.envhex
+-rw-r--r--   0      501       20      369 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-ash.hex
+-rw-r--r--   0      501       20        7 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-cat.envhex
+-rw-r--r--   0      501       20      223 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-cat.hex
+-rw-r--r--   0      501       20       15 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-cons.envhex
+-rw-r--r--   0      501       20      211 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-cons.hex
+-rw-r--r--   0      501       20       13 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-div.envhex
+-rw-r--r--   0      501       20      363 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-div.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-lsh.envhex
+-rw-r--r--   0      501       20      369 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-lsh.hex
+-rw-r--r--   0      501       20        7 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-mul.envhex
+-rw-r--r--   0      501       20      257 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-mul.hex
+-rw-r--r--   0      501       20       15 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-not.envhex
+-rw-r--r--   0      501       20      355 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-not.hex
+-rw-r--r--   0      501       20       11 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-pubkey.envhex
+-rw-r--r--   0      501       20      355 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-pubkey.hex
+-rw-r--r--   0      501       20       13 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-sub.envhex
+-rw-r--r--   0      501       20      261 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/recursive-sub.hex
+-rw-r--r--   0      501       20       15 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/softfork-1.envhex
+-rw-r--r--   0      501       20      229 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/softfork-1.hex
+-rw-r--r--   0      501       20       15 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/softfork-2.envhex
+-rw-r--r--   0      501       20      221 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/programs/softfork-2.hex
+-rwxr-xr-x   0      501       20     4581 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/run-programs.py
+-rwxr-xr-x   0      501       20     1574 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/tests/run.py
+-rw-r--r--   0      501       20     8834 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/bin/Activate.ps1
+-rw-r--r--   0      501       20     2198 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/bin/activate
+-rw-r--r--   0      501       20     1250 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/bin/activate.csh
+-rw-r--r--   0      501       20     2402 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/bin/activate.fish
+-rwxr-xr-x   0      501       20      255 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/bin/pip
+-rwxr-xr-x   0      501       20      255 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/bin/pip3
+-rwxr-xr-x   0      501       20      255 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/bin/pip3.8
+-rwxr-xr-x   0      501       20    33816 2024-05-16 01:24:30.000000 klvm_rs-0.7.0/venv/bin/python
+-rwxr-xr-x   0      501       20    33816 2024-05-16 01:24:30.000000 klvm_rs-0.7.0/venv/bin/python3
+-rw-r--r--   0      501       20     3686 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0      501       20       44 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/_distutils_hack/override.py
+-rw-r--r--   0      501       20      152 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/distutils-precedence.pth
+-rw-r--r--   0      501       20      357 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/__init__.py
+-rw-r--r--   0      501       20     1198 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/__main__.py
+-rw-r--r--   0      501       20     1444 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0      501       20      573 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0      501       20    10243 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0      501       20    10734 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cache.py
+-rw-r--r--   0      501       20      132 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0      501       20     6676 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0      501       20     7842 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0      501       20    29497 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0      501       20      774 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0      501       20     2472 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0      501       20     4338 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0      501       20    10817 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0      501       20     1968 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0      501       20    18172 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0      501       20     5118 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0      501       20      116 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0      501       20     3882 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0      501       20     7582 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0      501       20     1685 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0      501       20     4129 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0      501       20     9815 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0      501       20     6591 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0      501       20     5289 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0      501       20     2951 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0      501       20     1703 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0      501       20     1132 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0      501       20     4793 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0      501       20     3188 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0      501       20    32389 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0      501       20    12343 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0      501       20     5697 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0      501       20     6419 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0      501       20     3886 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0      501       20     7396 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0      501       20    13529 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0      501       20      858 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0      501       20     1221 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0      501       20      729 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0      501       20     6494 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0      501       20     1164 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0      501       20    24244 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0      501       20       30 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0      501       20    16504 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0      501       20    37873 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0      501       20     6557 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0      501       20    15365 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0      501       20     6100 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0      501       20     7680 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0      501       20     2556 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0      501       20      340 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/main.py
+-rw-r--r--   0      501       20     4280 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0      501       20     2595 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0      501       20    25277 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0      501       20      107 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0      501       20     1882 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0      501       20     8181 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0      501       20     7457 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0      501       20     9773 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0      501       20       63 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0      501       20      990 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0      501       20     6626 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0      501       20     2520 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0      501       20     1030 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0      501       20     2617 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0      501       20    18602 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0      501       20      738 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0      501       20     4644 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0      501       20     1907 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0      501       20     3858 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0      501       20     3600 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0      501       20       50 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0      501       20    16507 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0      501       20     2145 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0      501       20     6096 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0      501       20     7638 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0      501       20    18443 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0      501       20     4073 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0      501       20     1791 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0      501       20     4133 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0      501       20     1422 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0      501       20     1474 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0      501       20     2198 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0      501       20     1075 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0      501       20     1417 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0      501       20     3064 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0      501       20     5122 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0      501       20     9784 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0      501       20       51 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0      501       20     1354 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0      501       20     4105 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0      501       20    27407 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0      501       20    25091 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0      501       20     6987 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0      501       20     2807 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0      501       20    16611 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0      501       20    17646 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0      501       20    35763 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0      501       20     2858 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0      501       20    24045 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0      501       20      583 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0      501       20    24129 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0      501       20     5220 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0      501       20    18963 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0      501       20    27878 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0      501       20     5705 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0      501       20     9914 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0      501       20     2526 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0      501       20     5455 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0      501       20    11533 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0      501       20     8167 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0      501       20     1015 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0      501       20     1665 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0      501       20     1884 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0      501       20     5377 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0      501       20      242 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0      501       20     5764 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0      501       20     3206 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0      501       20     1115 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0      501       20     2118 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0      501       20     1169 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0      501       20     3064 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0      501       20     5122 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0      501       20      716 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0      501       20     3110 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0      501       20     4831 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0      501       20      795 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0      501       20    11632 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0      501       20    22253 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0      501       20     1193 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0      501       20     2108 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0      501       20     5662 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0      501       20     9200 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0      501       20     7702 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0      501       20     8821 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0      501       20     1759 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0      501       20     3456 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0      501       20     4549 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0      501       20      596 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0      501       20     3519 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0      501       20    18116 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0      501       20     5238 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0      501       20    11729 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0      501       20    22811 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0      501       20    13079 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0      501       20     4966 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0      501       20      465 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0      501       20     1379 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0      501       20     5033 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0      501       20     1535 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0      501       20      242 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0      501       20     5271 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0      501       20     1033 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0      501       20      778 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0      501       20    16416 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0      501       20     3946 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0      501       20     4154 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0      501       20     7105 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0      501       20      774 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0      501       20       94 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0      501       20      255 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0      501       20   275233 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0      501       20     4279 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0      501       20     4797 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0      501       20    31274 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0      501       20     1763 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0      501       20    10032 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0      501       20     3915 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0      501       20     5420 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0      501       20     3242 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0      501       20     3732 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0      501       20      542 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0      501       20     1860 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0      501       20     1683 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0      501       20     4006 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0      501       20    12176 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0      501       20     3934 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0      501       20    13566 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0      501       20     1753 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0      501       20    36913 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0      501       20     1753 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0      501       20    20735 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0      501       20     1759 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0      501       20    14537 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0      501       20    25796 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0      501       20    42498 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0      501       20     1752 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0      501       20    27055 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0      501       20   104562 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0      501       20    98484 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0      501       20    98196 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0      501       20   101363 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0      501       20   128035 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0      501       20   102774 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0      501       20    95372 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0      501       20     5380 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0      501       20     6077 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0      501       20     3715 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0      501       20     2131 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0      501       20    30391 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0      501       20    13560 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0      501       20      402 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0      501       20     6400 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0      501       20     4137 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0      501       20     4007 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0      501       20    14848 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0      501       20     8505 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0      501       20     2812 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0      501       20      244 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0      501       20      266 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0      501       20     2522 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0      501       20    11128 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0      501       20     3325 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0      501       20       75 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0      501       20     2839 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0      501       20    10678 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0      501       20     6741 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0      501       20     1866 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0      501       20     1079 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0      501       20     3709 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0      501       20     6181 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0      501       20     7134 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0      501       20      581 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0      501       20    41259 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0      501       20    51697 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0      501       20    20834 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0      501       20    51991 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0      501       20    14811 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0      501       20     5058 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0      501       20    39801 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0      501       20    10820 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0      501       20    18102 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0      501       20    97792 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0      501       20   182784 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0      501       20   108032 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0      501       20    66262 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0      501       20    23513 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0      501       20    91648 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0      501       20   168448 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0      501       20   101888 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0      501       20    43898 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0      501       20      981 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0      501       20       64 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0      501       20    49330 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0      501       20      849 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0      501       20     3374 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0      501       20      321 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0      501       20    12950 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0      501       20    44375 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0      501       20     1881 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0      501       20       21 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0      501       20   206539 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0      501       20     1132 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0      501       20     1081 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0      501       20     6080 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0      501       20    34557 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0      501       20      661 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0      501       20      497 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0      501       20    11488 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0      501       20     4378 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0      501       20     1431 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0      501       20     8487 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0      501       20     4676 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0      501       20    30110 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0      501       20    15699 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0      501       20     4200 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0      501       20    14665 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0      501       20   108287 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0      501       20      562 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0      501       20    12936 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0      501       20     1176 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0      501       20     4068 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0      501       20     4910 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0      501       20     2655 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0      501       20     6911 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0      501       20      160 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0      501       20     6596 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0      501       20     2999 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0      501       20      353 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0      501       20    23685 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0      501       20     1697 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0      501       20     1938 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0      501       20    40386 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0      501       20     2917 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0      501       20     4810 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0      501       20     4104 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0      501       20     3314 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0      501       20     5086 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0      501       20    35441 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0      501       20    21938 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0      501       20     5871 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0      501       20    19351 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0      501       20     5073 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0      501       20     2212 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0      501       20     5014 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0      501       20     7335 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0      501       20     4674 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0      501       20    11753 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0      501       20    32005 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0      501       20    11174 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0      501       20    70232 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0      501       20    53376 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0      501       20      986 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0      501       20     2591 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0      501       20     3072 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0      501       20     3092 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0      501       20     4630 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0      501       20     6257 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0      501       20     3419 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0      501       20     6184 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0      501       20    63187 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0      501       20     9110 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0      501       20     9171 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0      501       20     6426 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0      501       20    12936 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0      501       20   213344 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0      501       20    23685 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0      501       20     9023 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0      501       20    39129 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0      501       20    25341 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0      501       20    13402 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0      501       20    10787 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0      501       20     6805 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0      501       20      491 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0      501       20      138 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0      501       20    11920 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0      501       20      546 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0      501       20    10927 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0      501       20     5178 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0      501       20      435 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0      501       20     1397 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0      501       20    21443 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0      501       20     6377 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0      501       20    10187 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0      501       20      575 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0      501       20     1286 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0      501       20    18560 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0      501       20     3823 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0      501       20     3879 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0      501       20      733 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0      501       20    35288 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0      501       20      695 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0      501       20    30180 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0      501       20     4235 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0      501       20     2912 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0      501       20    33240 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0      501       20      537 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0      501       20      156 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0      501       20     5872 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0      501       20     1583 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0      501       20    17592 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0      501       20     4794 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0      501       20     6090 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0      501       20     8478 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0      501       20    10096 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0      501       20   140235 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0      501       20     1064 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0      501       20     2114 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0      501       20      265 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0      501       20     9695 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0      501       20     3225 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0      501       20     1236 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0      501       20     1643 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0      501       20     7063 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0      501       20      423 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0      501       20     5472 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0      501       20    19919 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0      501       20      351 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0      501       20      417 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0      501       20    22820 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0      501       20     1926 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0      501       20     2783 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0      501       20     1840 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0      501       20      890 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0      501       20    10368 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0      501       20     6819 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0      501       20     3264 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0      501       20     9842 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0      501       20     4503 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0      501       20    18015 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0      501       20     1054 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0      501       20     7131 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0      501       20    97992 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0      501       20     1288 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0      501       20     5497 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0      501       20     6630 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0      501       20     7954 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0      501       20      972 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0      501       20     2501 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0      501       20      642 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0      501       20     1616 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0      501       20     2508 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0      501       20     9585 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0      501       20     5053 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0      501       20     3252 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0      501       20    14007 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0      501       20    14172 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0      501       20     3667 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0      501       20    11903 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0      501       20     8198 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0      501       20     5305 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0      501       20     4970 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0      501       20      828 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0      501       20     3396 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0      501       20    10574 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0      501       20    37414 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0      501       20    59836 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0      501       20     8165 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0      501       20    11303 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0      501       20     1391 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0      501       20      166 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0      501       20     4436 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0      501       20     4773 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0      501       20     2843 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0      501       20     1591 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0      501       20    24224 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0      501       20     4374 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0      501       20     4425 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0      501       20    26332 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0      501       20     1258 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0      501       20    34995 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0      501       20    39684 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0      501       20     3370 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0      501       20    45686 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0      501       20     3627 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0      501       20      102 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0      501       20    26070 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0      501       20     9169 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0      501       20    34549 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/six.py
+-rw-r--r--   0      501       20    18364 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0      501       20     3314 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0      501       20     1944 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0      501       20     1496 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0      501       20     1376 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0      501       20     1908 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0      501       20     1383 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0      501       20     7550 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0      501       20     2790 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0      501       20     2145 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0      501       20     8011 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0      501       20      396 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0      501       20    22633 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0      501       20     2943 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0      501       20      254 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0      501       20    80114 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0      501       20     3333 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0      501       20    10811 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0      501       20       64 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0      501       20    20070 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0      501       20    39095 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0      501       20      957 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0      501       20    17632 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0      501       20    13922 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0      501       20    11036 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0      501       20     4528 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0      501       20    17081 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0      501       20    34448 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0      501       20     7097 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0      501       20     8217 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0      501       20     8579 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0      501       20     2440 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0      501       20     1417 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0      501       20    34665 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0      501       20    19786 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0      501       20     5985 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0      501       20    30641 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0      501       20     1155 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0      501       20     4901 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0      501       20     1605 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0      501       20      498 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0      501       20     3997 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0      501       20     3510 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0      501       20    22003 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0      501       20    17177 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0      501       20     5758 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0      501       20     6895 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0      501       20    10003 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0      501       20    14298 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0      501       20     5403 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0      501       20      476 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0      501       20    10579 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0      501       20     8979 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0      501       20     1305 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0      501       20     6563 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0      501       20     4307 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0      501       20      286 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/py.typed
+-rw-r--r--   0      501       20        4 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/INSTALLER
+-rw-r--r--   0      501       20     1093 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/LICENSE.txt
+-rw-r--r--   0      501       20     4072 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/METADATA
+-rw-r--r--   0      501       20    76671 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/RECORD
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/REQUESTED
+-rw-r--r--   0      501       20       92 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/WHEEL
+-rw-r--r--   0      501       20      124 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/entry_points.txt
+-rw-r--r--   0      501       20        4 2024-05-16 01:24:56.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/top_level.txt
+-rw-r--r--   0      501       20   108202 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0      501       20    24701 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0      501       20      736 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0      501       20      562 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0      501       20     1128 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rw-r--r--   0      501       20     2022 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0      501       20     1812 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_typing.py
+-rw-r--r--   0      501       20     9518 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0      501       20     4929 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0      501       20    31944 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0      501       20    24067 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0      501       20     1811 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0      501       20    15470 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0      501       20   232055 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py
+-rw-r--r--   0      501       20     2362 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0      501       20      104 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+-rw-r--r--   0      501       20     7681 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/__init__.py
+-rw-r--r--   0      501       20      218 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0      501       20      250 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0      501       20    20813 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0      501       20     8572 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0      501       20    14894 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0      501       20    47437 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0      501       20    18079 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0      501       20      799 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0      501       20     5562 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0      501       20     4913 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0      501       20    35579 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-r--r--   0      501       20    21537 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0      501       20    16030 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-r--r--   0      501       20     5767 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0      501       20     8022 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0      501       20    31685 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0      501       20    17190 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0      501       20     6232 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0      501       20     5637 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0      501       20     2776 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0      501       20    13117 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0      501       20    27482 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0      501       20     2822 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0      501       20     2603 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0      501       20     1298 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0      501       20     8397 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0      501       20     2017 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0      501       20      671 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0      501       20    11712 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0      501       20    19005 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0      501       20     7597 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0      501       20     4827 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0      501       20     8876 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0      501       20    16380 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0      501       20      139 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0      501       20     3491 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0      501       20     7778 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0      501       20    50421 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0      501       20     3577 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0      501       20    10515 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0      501       20    17784 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0      501       20     8148 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0      501       20    12832 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0      501       20     1969 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0      501       20    30453 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0      501       20    23540 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0      501       20      455 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/py35compat.py
+-rw-r--r--   0      501       20      212 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0      501       20     4408 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0      501       20    21349 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0      501       20    12483 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0      501       20    14696 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0      501       20    20985 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0      501       20    12514 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0      501       20     5133 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0      501       20     2388 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_imp.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0      501       20    15130 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0      501       20      736 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0      501       20      562 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0      501       20     1128 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py
+-rw-r--r--   0      501       20     2022 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0      501       20     1812 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_typing.py
+-rw-r--r--   0      501       20     9509 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0      501       20     4917 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0      501       20    31944 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0      501       20    24067 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0      501       20     1811 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0      501       20    15470 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0      501       20   232055 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py
+-rw-r--r--   0      501       20     7077 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/archive_util.py
+-rw-r--r--   0      501       20    10280 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/build_meta.py
+-rw-r--r--   0      501       20    65536 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0      501       20    74752 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0      501       20    65536 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/cli.exe
+-rw-r--r--   0      501       20      551 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0      501       20     2381 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/alias.py
+-rw-r--r--   0      501       20    16604 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0      501       20      900 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0      501       20     4415 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0      501       20    13027 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0      501       20     9473 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0      501       20     8045 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/develop.py
+-rw-r--r--   0      501       20      960 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0      501       20    85308 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0      501       20    25079 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0      501       20     4705 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/install.py
+-rw-r--r--   0      501       20     2203 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0      501       20     3875 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0      501       20     2593 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0      501       20      628 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0      501       20     4946 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0      501       20      468 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/register.py
+-rw-r--r--   0      501       20     2128 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0      501       20      658 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0      501       20     7818 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0      501       20     5051 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0      501       20     9469 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/test.py
+-rw-r--r--   0      501       20      462 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/upload.py
+-rw-r--r--   0      501       20     7218 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0      501       20    22020 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/config.py
+-rw-r--r--   0      501       20      949 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/dep_util.py
+-rw-r--r--   0      501       20     5474 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/depends.py
+-rw-r--r--   0      501       20    40150 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/dist.py
+-rw-r--r--   0      501       20      524 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/errors.py
+-rw-r--r--   0      501       20     1684 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/extension.py
+-rw-r--r--   0      501       20     2389 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0      501       20     4873 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/glob.py
+-rw-r--r--   0      501       20    65536 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0      501       20    75264 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0      501       20    65536 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/gui.exe
+-rw-r--r--   0      501       20     3567 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/installer.py
+-rw-r--r--   0      501       20      812 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/launch.py
+-rw-r--r--   0      501       20     2335 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py
+-rw-r--r--   0      501       20     5217 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/monkey.py
+-rw-r--r--   0      501       20    51126 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/msvc.py
+-rw-r--r--   0      501       20     3093 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/namespaces.py
+-rw-r--r--   0      501       20    40718 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/package_index.py
+-rw-r--r--   0      501       20      245 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/py34compat.py
+-rw-r--r--   0      501       20    14151 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/sandbox.py
+-rw-r--r--   0      501       20      218 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0      501       20      138 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/script.tmpl
+-rw-r--r--   0      501       20     8565 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/ssl_support.py
+-rw-r--r--   0      501       20      941 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0      501       20      144 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/version.py
+-rw-r--r--   0      501       20     8288 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/wheel.py
+-rw-r--r--   0      501       20      714 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/windows_support.py
+-rw-r--r--   0      501       20        4 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/INSTALLER
+-rw-r--r--   0      501       20     1050 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/LICENSE
+-rw-r--r--   0      501       20     4759 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/METADATA
+-rw-r--r--   0      501       20    22796 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/RECORD
+-rw-r--r--   0      501       20        0 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/REQUESTED
+-rw-r--r--   0      501       20       92 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/WHEEL
+-rw-r--r--   0      501       20      239 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/dependency_links.txt
+-rw-r--r--   0      501       20     2869 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/entry_points.txt
+-rw-r--r--   0      501       20       41 2024-05-16 01:24:55.000000 klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/top_level.txt
+-rw-r--r--   0      501       20      102 2024-05-16 01:24:54.000000 klvm_rs-0.7.0/venv/pyvenv.cfg
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 klvm_rs-0.7.0/wheel/Cargo.toml
+-rw-r--r--   0      501       20      606 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/README.md
+-rw-r--r--   0      501       20      100 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/__init__.py
+-rw-r--r--   0      501       20      873 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/at.py
+-rw-r--r--   0      501       20     5444 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/casts.py
+-rw-r--r--   0      501       20      941 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/chik_dialect.py
+-rw-r--r--   0      501       20     5402 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/curry_and_treehash.py
+-rw-r--r--   0      501       20     3732 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/de.py
+-rw-r--r--   0      501       20      133 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/eval_error.py
+-rw-r--r--   0      501       20      609 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/klvm_rs.pyi
+-rw-r--r--   0      501       20      695 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/klvm_storage.py
+-rw-r--r--   0      501       20     4903 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/klvm_tree.py
+-rw-r--r--   0      501       20    10761 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/program.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/py.typed
+-rw-r--r--   0      501       20     1164 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/replace.py
+-rw-r--r--   0      501       20     5038 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/ser.py
+-rw-r--r--   0      501       20     3559 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/klvm_rs/tree_hash.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/tests/__init__.py
+-rw-r--r--   0      501       20     6721 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/tests/test_apis.py
+-rw-r--r--   0      501       20     1530 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/tests/test_curry_and_treehash.py
+-rw-r--r--   0      501       20    16181 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/tests/test_program.py
+-rw-r--r--   0      501       20     5046 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/python/tests/test_serialize.py
+-rw-r--r--   0      501       20      828 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/src/adapt_response.rs
+-rw-r--r--   0      501       20     2652 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/src/api.rs
+-rw-r--r--   0      501       20     1388 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/src/lazy_node.rs
+-rw-r--r--   0      501       20       52 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/wheel/src/lib.rs
+-rw-r--r--   0      501       20    48403 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/Cargo.lock
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 klvm_rs-0.7.0/Cargo.toml
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 klvm_rs-0.7.0/pyproject.toml
+-rw-r--r--   0      501       20      609 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/klvm_rs.pyi
+-rw-r--r--   0      501       20     4903 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/klvm_tree.py
+-rw-r--r--   0      501       20     5038 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/ser.py
+-rw-r--r--   0      501       20      695 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/klvm_storage.py
+-rw-r--r--   0      501       20      941 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/chik_dialect.py
+-rw-r--r--   0      501       20     5444 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/casts.py
+-rw-r--r--   0      501       20     3559 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/tree_hash.py
+-rw-r--r--   0      501       20      100 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/__init__.py
+-rw-r--r--   0      501       20      133 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/eval_error.py
+-rw-r--r--   0      501       20      873 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/at.py
+-rw-r--r--   0      501       20    10761 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/program.py
+-rw-r--r--   0      501       20        0 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/py.typed
+-rw-r--r--   0      501       20     5402 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/curry_and_treehash.py
+-rw-r--r--   0      501       20     3732 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/de.py
+-rw-r--r--   0      501       20     1164 2024-05-16 01:23:27.000000 klvm_rs-0.7.0/python/klvm_rs/replace.py
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 klvm_rs-0.7.0/PKG-INFO
```

### Comparing `klvm_rs-0.6.1/.github/workflows/benchmark.yml` & `klvm_rs-0.7.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/.github/workflows/build-arm64-wheels.yml` & `klvm_rs-0.7.0/.github/workflows/build-arm64-wheels.yml`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             yum -y install openssl-devel && \
             source $HOME/.cargo/env && \
             rustup target add aarch64-unknown-linux-musl && \
             rm -rf venv && \
             export PATH=/opt/python/cp310-cp310/bin/:$PATH && \
             export PATH=/opt/python/cp39-cp39/bin/:$PATH && \
             export PATH=/opt/python/cp38-cp38/bin/:$PATH && \
-            export PATH=/opt/python/cp37-cp37m/bin/:$PATH && \
             /opt/python/cp38-cp38/bin/python -m venv venv && \
             if [ ! -f "activate" ]; then ln -s venv/bin/activate; fi && \
             . ./activate && \
             pip install maturin && \
             CC=gcc maturin build -m wheel/Cargo.toml --release --strip --manylinux 2014 --features=openssl \
           '
```

### Comparing `klvm_rs-0.6.1/.github/workflows/build-crate.yml` & `klvm_rs-0.7.0/.github/workflows/build-crate.yml`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/.github/workflows/build-m1-wheel.yml.bak` & `klvm_rs-0.7.0/.github/workflows/build-m1-wheel.yml.bak`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/.github/workflows/build-npm.yml` & `klvm_rs-0.7.0/.github/workflows/build-npm.yml`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/.github/workflows/build-test.yml` & `klvm_rs-0.7.0/.github/workflows/build-test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   build_wheels:
     name: Wheel on ${{ matrix.os }} py-${{ matrix.python }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest, windows-latest]
-        python: [3.7]
+        python: [3.8]
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - uses: chik-network/actions/setup-python@main
@@ -67,15 +67,15 @@
             sh rustup-init.sh -y && \
             yum -y --disablerepo=epel install openssl-devel && \
             source $HOME/.cargo/env && \
             rustup target add x86_64-unknown-linux-musl && \
             PY_VERSION=${{ matrix.python }}
             PY_VERSION=${PY_VERSION/.} && \
             echo "Python version with dot removed is $PY_VERSION" && \
-            if [ "$PY_VERSION" = "37" ]; \
+            if [ "$PY_VERSION" = "38" ]; \
             then export SCND_VERSION="${PY_VERSION}m"; \
             else export SCND_VERSION="$PY_VERSION"; fi && \
             echo "Exporting path /opt/python/cp$PY_VERSION-cp$SCND_VERSION/bin" && \
             export PATH=/opt/python/cp$PY_VERSION-cp$SCND_VERSION/bin/:$PATH && \
             /opt/python/cp38-cp38/bin/python -m venv /venv && \
             . /venv/bin/activate && \
             pip install --upgrade pip && \
@@ -110,15 +110,15 @@
         echo ${WHEEL_PATH}
         pip install ${WHEEL_PATH}
 
     - name: Install other wheels
       run: |
         . ./activate
         python -m pip install pytest
-        python -m pip install blspy==2.0.2
+        python -m pip install blspy
 
     - name: Run tests from wheel
       run: |
         . ./activate
         cd wheel/python
         pytest --import-mode append tests
         # we use `append` because otherwise the `klvm_rs` source is added
@@ -180,15 +180,15 @@
   fuzz_targets:
     name: Run fuzz targets
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest]
-        python: [3.7]
+        python: [3.8]
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 1
       - name: Install rust
         uses: dtolnay/rust-toolchain@master
         with:
@@ -215,15 +215,15 @@
   unit_tests:
     name: Unit tests
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest, windows-latest]
-        python: [3.7]
+        python: [3.8]
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 1
       - name: Install rust
         uses: dtolnay/rust-toolchain@stable
         with:
```

### Comparing `klvm_rs-0.6.1/.github/workflows/dependency-review.yml.bak` & `klvm_rs-0.7.0/.github/workflows/dependency-review.yml.bak`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/LICENSE` & `klvm_rs-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/README.md` & `klvm_rs-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/RELEASE.md` & `klvm_rs-0.7.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/activate` & `klvm_rs-0.7.0/activate`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 if [ -z "${VIRTUAL_ENV_DISABLE_PROMPT:-}" ] ; then
     _OLD_VIRTUAL_PS1="${PS1:-}"
     if [ "x(venv) " != x ] ; then
 	PS1="(venv) ${PS1:-}"
     else
     if [ "`basename \"$VIRTUAL_ENV\"`" = "__" ] ; then
         # special case for Aspen magic directories
-        # see http://www.zetadev.com/software/aspen/
+        # see https://aspen.io/
         PS1="[`basename \`dirname \"$VIRTUAL_ENV\"\``] $PS1"
     else
         PS1="(`basename \"$VIRTUAL_ENV\"`)$PS1"
     fi
     fi
     export PS1
 fi
```

### Comparing `klvm_rs-0.6.1/benches/block_af9c3d98.bin` & `klvm_rs-0.7.0/benches/block_af9c3d98.bin`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benches/deserialize.rs` & `klvm_rs-0.7.0/benches/deserialize.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benches/run-program.rs` & `klvm_rs-0.7.0/benches/run-program.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benchmark/block-2000.hex` & `klvm_rs-0.7.0/benchmark/block-2000.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benchmark/compressed-2000.envhex` & `klvm_rs-0.7.0/benchmark/compressed-2000.envhex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benchmark/compressed-2000.hex` & `klvm_rs-0.7.0/benchmark/compressed-2000.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benchmark/large-block.hex` & `klvm_rs-0.7.0/benchmark/large-block.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benchmark/matrix-multiply.hex` & `klvm_rs-0.7.0/benchmark/matrix-multiply.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benchmark/matrix-multiply.klvm` & `klvm_rs-0.7.0/benchmark/matrix-multiply.klvm`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/benchmarks.txt` & `klvm_rs-0.7.0/benchmarks.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/docs/new-operator-checklist.md` & `klvm_rs-0.7.0/docs/new-operator-checklist.md`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-bls-ops.txt` & `klvm_rs-0.7.0/op-tests/test-bls-ops.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-bls-zk.txt` & `klvm_rs-0.7.0/op-tests/test-bls-zk.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-blspy-g1.txt` & `klvm_rs-0.7.0/op-tests/test-blspy-g1.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-blspy-g2.txt` & `klvm_rs-0.7.0/op-tests/test-blspy-g2.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-blspy-hash.txt` & `klvm_rs-0.7.0/op-tests/test-blspy-hash.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-blspy-pairing.txt` & `klvm_rs-0.7.0/op-tests/test-blspy-pairing.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-blspy-verify.txt` & `klvm_rs-0.7.0/op-tests/test-blspy-verify.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-core-ops.txt` & `klvm_rs-0.7.0/op-tests/test-core-ops.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-modpow.txt` & `klvm_rs-0.7.0/op-tests/test-modpow.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-more-ops.txt` & `klvm_rs-0.7.0/op-tests/test-more-ops.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-secp-verify.txt` & `klvm_rs-0.7.0/op-tests/test-secp-verify.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-secp256k1.txt` & `klvm_rs-0.7.0/op-tests/test-secp256k1.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-secp256r1.txt` & `klvm_rs-0.7.0/op-tests/test-secp256r1.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/op-tests/test-sha256.txt` & `klvm_rs-0.7.0/op-tests/test-sha256.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/allocator.rs` & `klvm_rs-0.7.0/src/allocator.rs`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
             small_atoms: self.small_atoms,
         }
     }
 
     pub fn restore_checkpoint(&mut self, cp: &Checkpoint) {
         // if any of these asserts fire, it means we're trying to restore to
         // a state that has already been "long-jumped" passed (via another
-        // restore to an earler state). You can only restore backwards in time,
+        // restore to an earlier state). You can only restore backwards in time,
         // not forwards.
         assert!(self.u8_vec.len() >= cp.u8s);
         assert!(self.pair_vec.len() >= cp.pairs);
         assert!(self.atom_vec.len() >= cp.atoms);
         self.u8_vec.truncate(cp.u8s);
         self.pair_vec.truncate(cp.pairs);
         self.atom_vec.truncate(cp.atoms);
```

### Comparing `klvm_rs-0.6.1/src/bls_ops.rs` & `klvm_rs-0.7.0/src/bls_ops.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/chik_dialect.rs` & `klvm_rs-0.7.0/src/chik_dialect.rs`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         o: NodePtr,
         argument_list: NodePtr,
         max_cost: Cost,
         extension: OperatorSet,
     ) -> Response {
         let op_len = allocator.atom_len(o);
         if op_len == 4 {
-            // these are unkown operators with assigned cost
+            // these are unknown operators with assigned cost
             // the formula is:
             // +---+---+---+------------+
             // | multiplier|XX | XXXXXX |
             // +---+---+---+---+--------+
             //  ^           ^    ^
             //  |           |    + 6 bits ignored when computing cost
             // cost         |
```

### Comparing `klvm_rs-0.6.1/src/core_ops.rs` & `klvm_rs-0.7.0/src/core_ops.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/dialect.rs` & `klvm_rs-0.7.0/src/dialect.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/f_table.rs` & `klvm_rs-0.7.0/src/f_table.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/lib.rs` & `klvm_rs-0.7.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/more_ops.rs` & `klvm_rs-0.7.0/src/more_ops.rs`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 // increased from 419535 to better model Raspberry PI
 const PUBKEY_BASE_COST: Cost = 1325730;
 // increased from 12 to closer model Raspberry PI
 const PUBKEY_COST_PER_BYTE: Cost = 38;
 
 // the new coinid operator
-// we subtract 153 cost as a discount, to incentivice using this operator rather
+// we subtract 153 cost as a discount, to incentivize using this operator rather
 // than "naked" sha256
 const COINID_COST: Cost =
     SHA256_BASE_COST + SHA256_COST_PER_ARG * 3 + SHA256_COST_PER_BYTE * (32 + 32 + 8) - 153;
 
 const MODPOW_BASE_COST: Cost = 17000;
 const MODPOW_COST_PER_BYTE_BASE_VALUE: Cost = 38;
 // the cost for exponent and modular scale by the square of the size of the
```

### Comparing `klvm_rs-0.6.1/src/number.rs` & `klvm_rs-0.7.0/src/number.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/op_utils.rs` & `klvm_rs-0.7.0/src/op_utils.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/reduction.rs` & `klvm_rs-0.7.0/src/reduction.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/run_program.rs` & `klvm_rs-0.7.0/src/run_program.rs`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 const STACK_SIZE_LIMIT: usize = 20000000;
 
 #[cfg(feature = "pre-eval")]
 pub type PreEval =
     Box<dyn Fn(&mut Allocator, NodePtr, NodePtr) -> Result<Option<Box<PostEval>>, EvalErr>>;
 
 #[cfg(feature = "pre-eval")]
-pub type PostEval = dyn Fn(Option<NodePtr>);
+pub type PostEval = dyn Fn(&mut Allocator, Option<NodePtr>);
 
 #[repr(u8)]
 enum Operation {
     Apply,
     Cons,
     ExitGuard,
     SwapEval,
@@ -491,15 +491,15 @@
                 Operation::ExitGuard => self.exit_guard(cost)?,
                 Operation::Cons => self.cons_op()?,
                 Operation::SwapEval => augment_cost_errors(self.swap_eval_op(), max_cost_ptr)?,
                 #[cfg(feature = "pre-eval")]
                 Operation::PostEval => {
                     let f = self.posteval_stack.pop().unwrap();
                     let peek: Option<NodePtr> = self.val_stack.last().copied();
-                    f(peek);
+                    f(&mut self.allocator, peek);
                     0
                 }
             };
         }
         Ok(Reduction(cost, self.pop()?))
     }
 }
```

### Comparing `klvm_rs-0.6.1/src/runtime_dialect.rs` & `klvm_rs-0.7.0/src/runtime_dialect.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/secp_ops.rs` & `klvm_rs-0.7.0/src/secp_ops.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/de.rs` & `klvm_rs-0.7.0/src/serde/de.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/de_br.rs` & `klvm_rs-0.7.0/src/serde/de_br.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/de_tree.rs` & `klvm_rs-0.7.0/src/serde/de_tree.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/object_cache.rs` & `klvm_rs-0.7.0/src/serde/object_cache.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/parse_atom.rs` & `klvm_rs-0.7.0/src/serde/parse_atom.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/read_cache_lookup.rs` & `klvm_rs-0.7.0/src/serde/read_cache_lookup.rs`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 break;
             }
             partial_paths = new_partial_paths;
         }
         possible_responses
     }
 
-    /// If multiple paths exist, the lexigraphically smallest one will be returned.
+    /// If multiple paths exist, the lexicographically smallest one will be returned.
     pub fn find_path(&self, id: &Bytes32, serialized_length: u64) -> Option<Vec<u8>> {
         let mut paths = self.find_paths(id, serialized_length);
         if !paths.is_empty() {
             paths.sort();
             paths.truncate(1);
             paths.pop()
         } else {
```

### Comparing `klvm_rs-0.6.1/src/serde/ser.rs` & `klvm_rs-0.7.0/src/serde/ser.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/ser_br.rs` & `klvm_rs-0.7.0/src/serde/ser_br.rs`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use std::io;
 use std::io::Cursor;
 
 use super::object_cache::{serialized_length, treehash, ObjectCache};
 use super::read_cache_lookup::ReadCacheLookup;
 use super::write_atom::write_atom;
 use crate::allocator::{Allocator, NodePtr, SExp};
+use crate::serde::ser::LimitedWriter;
 
 const BACK_REFERENCE: u8 = 0xfe;
 const CONS_BOX_MARKER: u8 = 0xff;
 
 #[derive(PartialEq, Eq)]
 enum ReadOp {
     Parse,
@@ -73,14 +74,52 @@
             read_op_stack.pop();
             read_cache_lookup.pop2_and_cons();
         }
     }
     Ok(())
 }
 
+pub fn node_to_bytes_backrefs_limit(
+    a: &Allocator,
+    node: NodePtr,
+    limit: usize,
+) -> io::Result<Vec<u8>> {
+    let buffer = Cursor::new(Vec::new());
+    let mut writer = LimitedWriter::new(buffer, limit);
+    node_to_stream_backrefs(a, node, &mut writer)?;
+    let vec = writer.into_inner().into_inner();
+    Ok(vec)
+}
+
 pub fn node_to_bytes_backrefs(a: &Allocator, node: NodePtr) -> io::Result<Vec<u8>> {
     let mut buffer = Cursor::new(Vec::new());
-
     node_to_stream_backrefs(a, node, &mut buffer)?;
     let vec = buffer.into_inner();
     Ok(vec)
 }
+
+#[test]
+fn test_serialize_limit() {
+    let mut a = Allocator::new();
+
+    let leaf = a.new_atom(&[1, 2, 3, 4, 5]).unwrap();
+    let l1 = a.new_pair(leaf, leaf).unwrap();
+    let l2 = a.new_pair(l1, l1).unwrap();
+    let l3 = a.new_pair(l2, l2).unwrap();
+
+    let expected = &[255, 255, 255, 133, 1, 2, 3, 4, 5, 254, 2, 254, 2, 254, 2];
+
+    {
+        assert_eq!(node_to_bytes_backrefs(&a, l3).unwrap(), expected);
+    }
+
+    {
+        assert_eq!(node_to_bytes_backrefs_limit(&a, l3, 15).unwrap(), expected);
+    }
+
+    {
+        assert_eq!(
+            node_to_bytes_backrefs_limit(&a, l3, 14).unwrap_err().kind(),
+            io::ErrorKind::OutOfMemory
+        );
+    }
+}
```

### Comparing `klvm_rs-0.6.1/src/serde/test.rs` & `klvm_rs-0.7.0/src/serde/test.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/tools.rs` & `klvm_rs-0.7.0/src/serde/tools.rs`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     let mut f = Cursor::new(b);
     let mut ops_counter = 1;
     let mut b = [0; 1];
     while ops_counter > 0 {
         ops_counter -= 1;
         f.read_exact(&mut b)?;
         if b[0] == CONS_BOX_MARKER {
-            // we expect to parse two more items from the strem
+            // we expect to parse two more items from the stream
             // the left and right sub tree
             ops_counter += 2;
         } else if b[0] == BACK_REFERENCE {
             // This is a back-ref. We don't actually need to resolve it, just
             // parse the path and move on
             let mut first_byte = [0; 1];
             f.read_exact(&mut first_byte)?;
```

### Comparing `klvm_rs-0.6.1/src/serde/utils.rs` & `klvm_rs-0.7.0/src/serde/utils.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/serde/write_atom.rs` & `klvm_rs-0.7.0/src/serde/write_atom.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/sha2.rs` & `klvm_rs-0.7.0/src/sha2.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/test_ops.rs` & `klvm_rs-0.7.0/src/test_ops.rs`

 * *Files 1% similar despite different names*

```diff
@@ -409,15 +409,15 @@
     let tracking = Rc::new(RefCell::new(HashMap::new()));
     let pre_eval_tracking = tracking.clone();
     let pre_eval_f: Box<
         dyn Fn(
             &mut Allocator,
             NodePtr,
             NodePtr,
-        ) -> Result<Option<Box<(dyn Fn(Option<NodePtr>))>>, EvalErr>,
+        ) -> Result<Option<Box<(dyn Fn(&mut Allocator, Option<NodePtr>))>>, EvalErr>,
     > = Box::new(move |_allocator, prog, args| {
         let tracking_key = pre_eval_tracking.borrow().len();
         // Ensure lifetime of mutable borrow is contained.
         // It must end before the lifetime of the following closure.
         {
             let mut tracking_mutable = pre_eval_tracking.borrow_mut();
             tracking_mutable.insert(
@@ -426,25 +426,26 @@
                     prog,
                     args,
                     outcome: None,
                 },
             );
         }
         let post_eval_tracking = pre_eval_tracking.clone();
-        let post_eval_f: Box<dyn Fn(Option<NodePtr>)> = Box::new(move |outcome| {
-            let mut tracking_mutable = post_eval_tracking.borrow_mut();
-            tracking_mutable.insert(
-                tracking_key,
-                EvalFTracker {
-                    prog,
-                    args,
-                    outcome,
-                },
-            );
-        });
+        let post_eval_f: Box<dyn Fn(&mut Allocator, Option<NodePtr>)> =
+            Box::new(move |_a, outcome| {
+                let mut tracking_mutable = post_eval_tracking.borrow_mut();
+                tracking_mutable.insert(
+                    tracking_key,
+                    EvalFTracker {
+                        prog,
+                        args,
+                        outcome,
+                    },
+                );
+            });
         Ok(Some(post_eval_f))
     });
 
     let result = run_program_with_pre_eval(
         &mut allocator,
         &ChikDialect::new(NO_UNKNOWN_OPS),
         program,
```

### Comparing `klvm_rs-0.6.1/src/tests.rs` & `klvm_rs-0.7.0/src/tests.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/src/traverse_path.rs` & `klvm_rs-0.7.0/src/traverse_path.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/generate-programs.py` & `klvm_rs-0.7.0/tests/generate-programs.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-add.hex` & `klvm_rs-0.7.0/tests/programs/args-add.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-all.hex` & `klvm_rs-0.7.0/tests/programs/args-all.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-and.hex` & `klvm_rs-0.7.0/tests/programs/args-and.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-any.hex` & `klvm_rs-0.7.0/tests/programs/args-any.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-cat.hex` & `klvm_rs-0.7.0/tests/programs/args-cat.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-mul.hex` & `klvm_rs-0.7.0/tests/programs/args-mul.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-or.hex` & `klvm_rs-0.7.0/tests/programs/args-or.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-point_add.hex` & `klvm_rs-0.7.0/tests/programs/args-point_add.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-sha.hex` & `klvm_rs-0.7.0/tests/programs/args-sha.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-sub.hex` & `klvm_rs-0.7.0/tests/programs/args-sub.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-unknown-1.hex` & `klvm_rs-0.7.0/tests/programs/args-unknown-1.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-unknown-2.hex` & `klvm_rs-0.7.0/tests/programs/args-unknown-2.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-unknown-3.hex` & `klvm_rs-0.7.0/tests/programs/args-unknown-3.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-unknown-4.hex` & `klvm_rs-0.7.0/tests/programs/args-unknown-4.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/programs/args-xor.hex` & `klvm_rs-0.7.0/tests/programs/args-xor.hex`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/run-programs.py` & `klvm_rs-0.7.0/tests/run-programs.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/tests/run.py` & `klvm_rs-0.7.0/tests/run.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/bin/activate` & `klvm_rs-0.7.0/venv/bin/activate`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 if [ -z "${VIRTUAL_ENV_DISABLE_PROMPT:-}" ] ; then
     _OLD_VIRTUAL_PS1="${PS1:-}"
     if [ "x(venv) " != x ] ; then
 	PS1="(venv) ${PS1:-}"
     else
     if [ "`basename \"$VIRTUAL_ENV\"`" = "__" ] ; then
         # special case for Aspen magic directories
-        # see http://www.zetadev.com/software/aspen/
+        # see https://aspen.io/
         PS1="[`basename \`dirname \"$VIRTUAL_ENV\"\``] $PS1"
     else
         PS1="(`basename \"$VIRTUAL_ENV\"`)$PS1"
     fi
     fi
     export PS1
 fi
```

### Comparing `klvm_rs-0.6.1/venv/bin/activate.csh` & `klvm_rs-0.7.0/venv/bin/activate.csh`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 if (! "$?VIRTUAL_ENV_DISABLE_PROMPT") then
     if ("venv" != "") then
         set env_name = "venv"
     else
         if (`basename "VIRTUAL_ENV"` == "__") then
             # special case for Aspen magic directories
-            # see http://www.zetadev.com/software/aspen/
+            # see https://aspen.io/
             set env_name = `basename \`dirname "$VIRTUAL_ENV"\``
         else
             set env_name = `basename "$VIRTUAL_ENV"`
         endif
     endif
     set prompt = "[$env_name] $prompt"
     unset env_name
```

### Comparing `klvm_rs-0.6.1/venv/bin/activate.fish` & `klvm_rs-0.7.0/venv/bin/activate.fish`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         if test -n "(venv) "
             printf "%s%s" "(venv) " (set_color normal)
         else
             # ...Otherwise, prepend env
             set -l _checkbase (basename "$VIRTUAL_ENV")
             if test $_checkbase = "__"
                 # special case for Aspen magic directories
-                # see http://www.zetadev.com/software/aspen/
+                # see https://aspen.io/
                 printf "%s[%s]%s " (set_color -b blue white) (basename (dirname "$VIRTUAL_ENV")) (set_color normal)
             else
                 printf "%s(%s)%s" (set_color -b blue white) (basename "$VIRTUAL_ENV") (set_color normal)
             end
         end
 
         # Restore the return status of the previous command.
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/__main__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/__pip-runner__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/build_env.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cache.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/autocompletion.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/base_command.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/cmdoptions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/command_context.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/main.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/main_parser.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/parser.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/progress_bars.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/req_command.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/cli/spinners.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/cache.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/check.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/completion.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/configuration.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/debug.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/download.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/freeze.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/hash.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/help.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/index.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/inspect.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/install.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/list.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/search.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/show.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/uninstall.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/commands/wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/configuration.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/base.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/installed.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/sdist.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/distributions/wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/exceptions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/index/collector.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/index/package_finder.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/index/sources.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/locations/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/locations/_distutils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/locations/_sysconfig.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/locations/base.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/_json.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/base.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_dists.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/importlib/_envs.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/metadata/pkg_resources.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/candidate.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/direct_url.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/format_control.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/index.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/installation_report.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/link.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/scheme.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/search_scope.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/selection_prefs.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/target_python.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/models/wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/auth.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/cache.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/download.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/lazy_wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/session.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/utils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/network/xmlrpc.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/build_tracker.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/metadata.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_editable.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_editable.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/check.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/freeze.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/install/editable_legacy.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/install/legacy.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/install/wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/operations/prepare.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/pyproject.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/constructors.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/req_file.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/req_install.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/req_set.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/req/req_uninstall.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/base.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/legacy/resolver.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/base.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/self_outdated_check.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/_log.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/appdirs.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/compatibility_tags.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/deprecation.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/direct_url_helpers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/distutils_args.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/egg_link.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/encoding.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/entrypoints.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/filesystem.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/filetypes.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/glibc.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/hashes.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/inject_securetransport.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/logging.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/misc.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/models.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/packaging.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/setuptools_build.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/subprocess.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/temp_dir.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/unpacking.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/urls.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/virtualenv.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/utils/wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/bazaar.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/git.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/mercurial.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/subversion.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/vcs/versioncontrol.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_internal/wheel_builder.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/adapter.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/cache.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/controller.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/serialize.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/certifi/cacert.pem` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/certifi/core.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/big5freq.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/big5prober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/chardistribution.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/charsetprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/cp949prober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/enums.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/escprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/escsm.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/eucjpprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/euckrfreq.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/euckrprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/euctwfreq.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/euctwprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312freq.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/gb2312prober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/hebrewprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/jisfreq.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/johabfreq.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/johabprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/jpcntx.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langthaimodel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/latin1prober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/macromanprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/mbcssm.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/metadata/languages.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/sjisprober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/universaldetector.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/utf1632prober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/chardet/utf8prober.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/ansi.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/ansitowin32.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/initialise.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/utils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/win32.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/colorama/winterm.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/database.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/index.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/locators.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/manifest.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/markers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/metadata.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/resources.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/scripts.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/t32.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/t64-arm.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/t64.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/util.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/version.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/w32.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/w64-arm.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/w64.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distlib/wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distro/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/distro/distro.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/codec.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/core.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/idnadata.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/intranges.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/idna/uts46data.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/msgpack/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/msgpack/exceptions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/msgpack/ext.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/msgpack/fallback.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/__about__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/_manylinux.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/_musllinux.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/_structures.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/markers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/requirements.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/specifiers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/tags.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/utils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/packaging/version.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pkg_resources/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/__main__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/android.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/api.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/macos.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/unix.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/platformdirs/windows.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/cmdline.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/console.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/filter.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/filters/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatter.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/groff.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/html.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/img.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/irc.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/latex.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/other.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/svg.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/lexer.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/lexers/python.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/modeline.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/plugin.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/regexopt.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/scanner.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/sphinxext.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/style.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/styles/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/token.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/unistring.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pygments/util.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/actions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/common.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/core.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/exceptions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/helpers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/results.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/testing.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/unicode.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyparsing/util.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/_internal_utils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/adapters.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/api.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/auth.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/certs.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/cookies.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/exceptions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/help.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/hooks.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/models.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/packages.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/sessions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/status_codes.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/structures.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/requests/utils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/providers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/reporters.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/resolvers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/resolvelib/structs.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/__main__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_cell_widths.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_codes.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_emoji_replace.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_export_format.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_inspect.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_log_render.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_loop.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_null_file.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_palettes.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_ratio.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_spinners.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_win32_console.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_windows.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_windows_renderer.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/_wrap.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/abc.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/align.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/ansi.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/bar.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/box.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/cells.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/color.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/color_triplet.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/columns.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/console.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/constrain.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/containers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/control.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/default_styles.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/diagnose.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/emoji.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/errors.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/file_proxy.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/filesize.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/highlighter.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/json.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/jupyter.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/layout.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/live.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/live_render.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/logging.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/markup.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/measure.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/padding.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/pager.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/palette.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/panel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/pretty.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/progress.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/progress_bar.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/prompt.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/protocol.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/repr.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/rule.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/scope.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/screen.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/segment.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/spinner.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/status.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/style.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/styled.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/syntax.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/table.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/terminal_theme.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/text.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/theme.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/traceback.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/rich/tree.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/six.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/_asyncio.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/_utils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/after.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/before.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/before_sleep.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/nap.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/retry.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/stop.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tenacity/wait.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tomli/_parser.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/tomli/_re.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/typing_extensions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/_collections.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/connection.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/connectionpool.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/exceptions.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/fields.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/filepost.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/packages/six.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/poolmanager.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/request.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/response.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/connection.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/proxy.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/request.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/response.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/retry.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/timeout.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/url.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/urllib3/util/wait.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/labels.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/mklabels.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/tests.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/LICENSE.txt` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/METADATA` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pip-23.0.1.dist-info/RECORD` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pip-23.0.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 ../../../bin/pip,sha256=E68zi1dbZTse4fKXbO_iDcyHIZ9KjuRoDB8Wa-Tv98w,255
 ../../../bin/pip3,sha256=E68zi1dbZTse4fKXbO_iDcyHIZ9KjuRoDB8Wa-Tv98w,255
-../../../bin/pip3.7,sha256=E68zi1dbZTse4fKXbO_iDcyHIZ9KjuRoDB8Wa-Tv98w,255
+../../../bin/pip3.8,sha256=E68zi1dbZTse4fKXbO_iDcyHIZ9KjuRoDB8Wa-Tv98w,255
 pip-23.0.1.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
 pip-23.0.1.dist-info/LICENSE.txt,sha256=Y0MApmnUmurmWxLGxIySTFGkzfPR_whtw0VtyLyqIQQ,1093
 pip-23.0.1.dist-info/METADATA,sha256=POh89utz-H1e0K-xDY9CL9gs-x0MjH-AWxbhJG3aaVE,4072
 pip-23.0.1.dist-info/RECORD,,
 pip-23.0.1.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pip-23.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
 pip-23.0.1.dist-info/entry_points.txt,sha256=w694mjHYSfmSoUVVSaHoQ9UkOBBdtKKIJbyDRLdKju8,124
 pip-23.0.1.dist-info/top_level.txt,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
 pip/__init__.py,sha256=5yroedzc2dKKbcynDrHX8vBoLxqU27KmFvvHmdqQN9w,357
 pip/__main__.py,sha256=mXwWDftNLMKfwVqKFWGE_uuBZvGSIiUELhLkeysIuZc,1198
 pip/__pip-runner__.py,sha256=EnrfKmKMzWAdqg_JicLCOP9Y95Ux7zHh4ObvqLtQcjo,1444
-pip/__pycache__/__init__.cpython-37.pyc,,
-pip/__pycache__/__main__.cpython-37.pyc,,
-pip/__pycache__/__pip-runner__.cpython-37.pyc,,
+pip/__pycache__/__init__.cpython-38.pyc,,
+pip/__pycache__/__main__.cpython-38.pyc,,
+pip/__pycache__/__pip-runner__.cpython-38.pyc,,
 pip/_internal/__init__.py,sha256=nnFCuxrPMgALrIDxSoy-H6Zj4W4UY60D-uL1aJyq0pc,573
-pip/_internal/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/__pycache__/build_env.cpython-37.pyc,,
-pip/_internal/__pycache__/cache.cpython-37.pyc,,
-pip/_internal/__pycache__/configuration.cpython-37.pyc,,
-pip/_internal/__pycache__/exceptions.cpython-37.pyc,,
-pip/_internal/__pycache__/main.cpython-37.pyc,,
-pip/_internal/__pycache__/pyproject.cpython-37.pyc,,
-pip/_internal/__pycache__/self_outdated_check.cpython-37.pyc,,
-pip/_internal/__pycache__/wheel_builder.cpython-37.pyc,,
+pip/_internal/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/__pycache__/build_env.cpython-38.pyc,,
+pip/_internal/__pycache__/cache.cpython-38.pyc,,
+pip/_internal/__pycache__/configuration.cpython-38.pyc,,
+pip/_internal/__pycache__/exceptions.cpython-38.pyc,,
+pip/_internal/__pycache__/main.cpython-38.pyc,,
+pip/_internal/__pycache__/pyproject.cpython-38.pyc,,
+pip/_internal/__pycache__/self_outdated_check.cpython-38.pyc,,
+pip/_internal/__pycache__/wheel_builder.cpython-38.pyc,,
 pip/_internal/build_env.py,sha256=1ESpqw0iupS_K7phZK5zshVE5Czy9BtGLFU4W6Enva8,10243
 pip/_internal/cache.py,sha256=C3n78VnBga9rjPXZqht_4A4d-T25poC7K0qBM7FHDhU,10734
 pip/_internal/cli/__init__.py,sha256=FkHBgpxxb-_gd6r1FjnNhfMOzAUYyXoXKJ6abijfcFU,132
-pip/_internal/cli/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/autocompletion.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/base_command.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/cmdoptions.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/command_context.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/main.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/main_parser.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/parser.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/progress_bars.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/req_command.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/spinners.cpython-37.pyc,,
-pip/_internal/cli/__pycache__/status_codes.cpython-37.pyc,,
+pip/_internal/cli/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/autocompletion.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/base_command.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/cmdoptions.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/command_context.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/main.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/main_parser.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/parser.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/progress_bars.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/req_command.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/spinners.cpython-38.pyc,,
+pip/_internal/cli/__pycache__/status_codes.cpython-38.pyc,,
 pip/_internal/cli/autocompletion.py,sha256=wY2JPZY2Eji1vhR7bVo-yCBPJ9LCy6P80iOAhZD1Vi8,6676
 pip/_internal/cli/base_command.py,sha256=t1D5x40Hfn9HnPnMt-iSxvqL14nht2olBCacW74pc-k,7842
 pip/_internal/cli/cmdoptions.py,sha256=0OHXkgnppCtC4QyF28ZL8FBosVUXG5pWj2uzO1CgWhM,29497
 pip/_internal/cli/command_context.py,sha256=RHgIPwtObh5KhMrd3YZTkl8zbVG-6Okml7YbFX4Ehg0,774
 pip/_internal/cli/main.py,sha256=ioJ8IVlb2K1qLOxR-tXkee9lURhYV89CDM71MKag7YY,2472
 pip/_internal/cli/main_parser.py,sha256=laDpsuBDl6kyfywp9eMMA9s84jfH2TJJn-vmL0GG90w,4338
 pip/_internal/cli/parser.py,sha256=tWP-K1uSxnJyXu3WE0kkH3niAYRBeuUaxeydhzOdhL4,10817
 pip/_internal/cli/progress_bars.py,sha256=So4mPoSjXkXiSHiTzzquH3VVyVD_njXlHJSExYPXAow,1968
 pip/_internal/cli/req_command.py,sha256=ypTutLv4j_efxC2f6C6aCQufxre-zaJdi5m_tWlLeBk,18172
 pip/_internal/cli/spinners.py,sha256=hIJ83GerdFgFCdobIA23Jggetegl_uC4Sp586nzFbPE,5118
 pip/_internal/cli/status_codes.py,sha256=sEFHUaUJbqv8iArL3HAtcztWZmGOFX01hTesSytDEh0,116
 pip/_internal/commands/__init__.py,sha256=5oRO9O3dM2vGuh0bFw4HOVletryrz5HHMmmPWwJrH9U,3882
-pip/_internal/commands/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/cache.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/check.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/completion.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/configuration.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/debug.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/download.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/freeze.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/hash.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/help.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/index.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/inspect.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/install.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/list.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/search.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/show.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/uninstall.cpython-37.pyc,,
-pip/_internal/commands/__pycache__/wheel.cpython-37.pyc,,
+pip/_internal/commands/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/cache.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/check.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/completion.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/configuration.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/debug.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/download.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/freeze.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/hash.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/help.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/index.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/inspect.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/install.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/list.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/search.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/show.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/uninstall.cpython-38.pyc,,
+pip/_internal/commands/__pycache__/wheel.cpython-38.pyc,,
 pip/_internal/commands/cache.py,sha256=muaT0mbL-ZUpn6AaushVAipzTiMwE4nV2BLbJBwt_KQ,7582
 pip/_internal/commands/check.py,sha256=0gjXR7j36xJT5cs2heYU_dfOfpnFfzX8OoPNNoKhqdM,1685
 pip/_internal/commands/completion.py,sha256=H0TJvGrdsoleuIyQKzJbicLFppYx2OZA0BLNpQDeFjI,4129
 pip/_internal/commands/configuration.py,sha256=NB5uf8HIX8-li95YLoZO09nALIWlLCHDF5aifSKcBn8,9815
 pip/_internal/commands/debug.py,sha256=AesEID-4gPFDWTwPiPaGZuD4twdT-imaGuMR5ZfSn8s,6591
 pip/_internal/commands/download.py,sha256=LwKEyYMG2L67nQRyGo8hQdNEeMU2bmGWqJfcB8JDXas,5289
 pip/_internal/commands/freeze.py,sha256=gCjoD6foBZPBAAYx5t8zZLkJhsF_ZRtnb3dPuD7beO8,2951
@@ -85,198 +85,198 @@
 pip/_internal/commands/list.py,sha256=Fk1TSxB33NlRS4qlLQ0xwnytnF9-zkQJbKQYv2xc4Q4,12343
 pip/_internal/commands/search.py,sha256=sbBZiARRc050QquOKcCvOr2K3XLsoYebLKZGRi__iUI,5697
 pip/_internal/commands/show.py,sha256=t5jia4zcYJRJZy4U_Von7zMl03hJmmcofj6oDNTnj7Y,6419
 pip/_internal/commands/uninstall.py,sha256=OIqO9tqadY8kM4HwhFf1Q62fUIp7v8KDrTRo8yWMz7Y,3886
 pip/_internal/commands/wheel.py,sha256=mbFJd4dmUfrVFJkQbK8n2zHyRcD3AI91f7EUo9l3KYg,7396
 pip/_internal/configuration.py,sha256=uBKTus43pDIO6IzT2mLWQeROmHhtnoabhniKNjPYvD0,13529
 pip/_internal/distributions/__init__.py,sha256=Hq6kt6gXBgjNit5hTTWLAzeCNOKoB-N0pGYSqehrli8,858
-pip/_internal/distributions/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/distributions/__pycache__/base.cpython-37.pyc,,
-pip/_internal/distributions/__pycache__/installed.cpython-37.pyc,,
-pip/_internal/distributions/__pycache__/sdist.cpython-37.pyc,,
-pip/_internal/distributions/__pycache__/wheel.cpython-37.pyc,,
+pip/_internal/distributions/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/distributions/__pycache__/base.cpython-38.pyc,,
+pip/_internal/distributions/__pycache__/installed.cpython-38.pyc,,
+pip/_internal/distributions/__pycache__/sdist.cpython-38.pyc,,
+pip/_internal/distributions/__pycache__/wheel.cpython-38.pyc,,
 pip/_internal/distributions/base.py,sha256=jrF1Vi7eGyqFqMHrieh1PIOrGU7KeCxhYPZnbvtmvGY,1221
 pip/_internal/distributions/installed.py,sha256=NI2OgsgH9iBq9l5vB-56vOg5YsybOy-AU4VE5CSCO2I,729
 pip/_internal/distributions/sdist.py,sha256=SQBdkatXSigKGG_SaD0U0p1Jwdfrg26UCNcHgkXZfdA,6494
 pip/_internal/distributions/wheel.py,sha256=m-J4XO-gvFerlYsFzzSXYDvrx8tLZlJFTCgDxctn8ig,1164
 pip/_internal/exceptions.py,sha256=cU4dz7x-1uFGrf2A1_Np9tKcy599bRJKRJkikgARxW4,24244
 pip/_internal/index/__init__.py,sha256=vpt-JeTZefh8a-FC22ZeBSXFVbuBcXSGiILhQZJaNpQ,30
-pip/_internal/index/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/index/__pycache__/collector.cpython-37.pyc,,
-pip/_internal/index/__pycache__/package_finder.cpython-37.pyc,,
-pip/_internal/index/__pycache__/sources.cpython-37.pyc,,
+pip/_internal/index/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/index/__pycache__/collector.cpython-38.pyc,,
+pip/_internal/index/__pycache__/package_finder.cpython-38.pyc,,
+pip/_internal/index/__pycache__/sources.cpython-38.pyc,,
 pip/_internal/index/collector.py,sha256=3OmYZ3tCoRPGOrELSgQWG-03M-bQHa2-VCA3R_nJAaU,16504
 pip/_internal/index/package_finder.py,sha256=rrUw4vj7QE_eMt022jw--wQiKznMaUgVBkJ1UCrVUxo,37873
 pip/_internal/index/sources.py,sha256=SVyPitv08-Qalh2_Bk5diAJ9GAA_d-a93koouQodAG0,6557
 pip/_internal/locations/__init__.py,sha256=Dh8LJWG8LRlDK4JIj9sfRF96TREzE--N_AIlx7Tqoe4,15365
-pip/_internal/locations/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/locations/__pycache__/_distutils.cpython-37.pyc,,
-pip/_internal/locations/__pycache__/_sysconfig.cpython-37.pyc,,
-pip/_internal/locations/__pycache__/base.cpython-37.pyc,,
+pip/_internal/locations/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/locations/__pycache__/_distutils.cpython-38.pyc,,
+pip/_internal/locations/__pycache__/_sysconfig.cpython-38.pyc,,
+pip/_internal/locations/__pycache__/base.cpython-38.pyc,,
 pip/_internal/locations/_distutils.py,sha256=cmi6h63xYNXhQe7KEWEMaANjHFy5yQOPt_1_RCWyXMY,6100
 pip/_internal/locations/_sysconfig.py,sha256=jyNVtUfMIf0mtyY-Xp1m9yQ8iwECozSVVFmjkN9a2yw,7680
 pip/_internal/locations/base.py,sha256=RQiPi1d4FVM2Bxk04dQhXZ2PqkeljEL2fZZ9SYqIQ78,2556
 pip/_internal/main.py,sha256=r-UnUe8HLo5XFJz8inTcOOTiu_sxNhgHb6VwlGUllOI,340
 pip/_internal/metadata/__init__.py,sha256=84j1dPJaIoz5Q2ZTPi0uB1iaDAHiUNfKtYSGQCfFKpo,4280
-pip/_internal/metadata/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/metadata/__pycache__/_json.cpython-37.pyc,,
-pip/_internal/metadata/__pycache__/base.cpython-37.pyc,,
-pip/_internal/metadata/__pycache__/pkg_resources.cpython-37.pyc,,
+pip/_internal/metadata/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/metadata/__pycache__/_json.cpython-38.pyc,,
+pip/_internal/metadata/__pycache__/base.cpython-38.pyc,,
+pip/_internal/metadata/__pycache__/pkg_resources.cpython-38.pyc,,
 pip/_internal/metadata/_json.py,sha256=BTkWfFDrWFwuSodImjtbAh8wCL3isecbnjTb5E6UUDI,2595
 pip/_internal/metadata/base.py,sha256=vIwIo1BtoqegehWMAXhNrpLGYBq245rcaCNkBMPnTU8,25277
 pip/_internal/metadata/importlib/__init__.py,sha256=9ZVO8BoE7NEZPmoHp5Ap_NJo0HgNIezXXg-TFTtt3Z4,107
-pip/_internal/metadata/importlib/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/metadata/importlib/__pycache__/_compat.cpython-37.pyc,,
-pip/_internal/metadata/importlib/__pycache__/_dists.cpython-37.pyc,,
-pip/_internal/metadata/importlib/__pycache__/_envs.cpython-37.pyc,,
+pip/_internal/metadata/importlib/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/metadata/importlib/__pycache__/_compat.cpython-38.pyc,,
+pip/_internal/metadata/importlib/__pycache__/_dists.cpython-38.pyc,,
+pip/_internal/metadata/importlib/__pycache__/_envs.cpython-38.pyc,,
 pip/_internal/metadata/importlib/_compat.py,sha256=GAe_prIfCE4iUylrnr_2dJRlkkBVRUbOidEoID7LPoE,1882
 pip/_internal/metadata/importlib/_dists.py,sha256=BUV8y6D0PePZrEN3vfJL-m1FDqZ6YPRgAiBeBinHhNg,8181
 pip/_internal/metadata/importlib/_envs.py,sha256=7BxanCh3T7arusys__O2ZHJdnmDhQXFmfU7x1-jB5xI,7457
 pip/_internal/metadata/pkg_resources.py,sha256=WjwiNdRsvxqxL4MA5Tb5a_q3Q3sUhdpbZF8wGLtPMI0,9773
 pip/_internal/models/__init__.py,sha256=3DHUd_qxpPozfzouoqa9g9ts1Czr5qaHfFxbnxriepM,63
-pip/_internal/models/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/models/__pycache__/candidate.cpython-37.pyc,,
-pip/_internal/models/__pycache__/direct_url.cpython-37.pyc,,
-pip/_internal/models/__pycache__/format_control.cpython-37.pyc,,
-pip/_internal/models/__pycache__/index.cpython-37.pyc,,
-pip/_internal/models/__pycache__/installation_report.cpython-37.pyc,,
-pip/_internal/models/__pycache__/link.cpython-37.pyc,,
-pip/_internal/models/__pycache__/scheme.cpython-37.pyc,,
-pip/_internal/models/__pycache__/search_scope.cpython-37.pyc,,
-pip/_internal/models/__pycache__/selection_prefs.cpython-37.pyc,,
-pip/_internal/models/__pycache__/target_python.cpython-37.pyc,,
-pip/_internal/models/__pycache__/wheel.cpython-37.pyc,,
+pip/_internal/models/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/models/__pycache__/candidate.cpython-38.pyc,,
+pip/_internal/models/__pycache__/direct_url.cpython-38.pyc,,
+pip/_internal/models/__pycache__/format_control.cpython-38.pyc,,
+pip/_internal/models/__pycache__/index.cpython-38.pyc,,
+pip/_internal/models/__pycache__/installation_report.cpython-38.pyc,,
+pip/_internal/models/__pycache__/link.cpython-38.pyc,,
+pip/_internal/models/__pycache__/scheme.cpython-38.pyc,,
+pip/_internal/models/__pycache__/search_scope.cpython-38.pyc,,
+pip/_internal/models/__pycache__/selection_prefs.cpython-38.pyc,,
+pip/_internal/models/__pycache__/target_python.cpython-38.pyc,,
+pip/_internal/models/__pycache__/wheel.cpython-38.pyc,,
 pip/_internal/models/candidate.py,sha256=6pcABsaR7CfIHlbJbr2_kMkVJFL_yrYjTx6SVWUnCPQ,990
 pip/_internal/models/direct_url.py,sha256=f3WiKUwWPdBkT1xm7DlolS32ZAMYh3jbkkVH-BUON5A,6626
 pip/_internal/models/format_control.py,sha256=DJpMYjxeYKKQdwNcML2_F0vtAh-qnKTYe-CpTxQe-4g,2520
 pip/_internal/models/index.py,sha256=tYnL8oxGi4aSNWur0mG8DAP7rC6yuha_MwJO8xw0crI,1030
 pip/_internal/models/installation_report.py,sha256=Hymmzv9-e3WhtewYm2NIOeMyAB6lXp736mpYqb9scZ0,2617
 pip/_internal/models/link.py,sha256=nfybVSpXgVHeU0MkC8hMkN2IgMup8Pdaudg74_sQEC8,18602
 pip/_internal/models/scheme.py,sha256=3EFQp_ICu_shH1-TBqhl0QAusKCPDFOlgHFeN4XowWs,738
 pip/_internal/models/search_scope.py,sha256=iGPQQ6a4Lau8oGQ_FWj8aRLik8A21o03SMO5KnSt-Cg,4644
 pip/_internal/models/selection_prefs.py,sha256=KZdi66gsR-_RUXUr9uejssk3rmTHrQVJWeNA2sV-VSY,1907
 pip/_internal/models/target_python.py,sha256=qKpZox7J8NAaPmDs5C_aniwfPDxzvpkrCKqfwndG87k,3858
 pip/_internal/models/wheel.py,sha256=YqazoIZyma_Q1ejFa1C7NHKQRRWlvWkdK96VRKmDBeI,3600
 pip/_internal/network/__init__.py,sha256=jf6Tt5nV_7zkARBrKojIXItgejvoegVJVKUbhAa5Ioc,50
-pip/_internal/network/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/network/__pycache__/auth.cpython-37.pyc,,
-pip/_internal/network/__pycache__/cache.cpython-37.pyc,,
-pip/_internal/network/__pycache__/download.cpython-37.pyc,,
-pip/_internal/network/__pycache__/lazy_wheel.cpython-37.pyc,,
-pip/_internal/network/__pycache__/session.cpython-37.pyc,,
-pip/_internal/network/__pycache__/utils.cpython-37.pyc,,
-pip/_internal/network/__pycache__/xmlrpc.cpython-37.pyc,,
+pip/_internal/network/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/network/__pycache__/auth.cpython-38.pyc,,
+pip/_internal/network/__pycache__/cache.cpython-38.pyc,,
+pip/_internal/network/__pycache__/download.cpython-38.pyc,,
+pip/_internal/network/__pycache__/lazy_wheel.cpython-38.pyc,,
+pip/_internal/network/__pycache__/session.cpython-38.pyc,,
+pip/_internal/network/__pycache__/utils.cpython-38.pyc,,
+pip/_internal/network/__pycache__/xmlrpc.cpython-38.pyc,,
 pip/_internal/network/auth.py,sha256=MQVP0k4hUXk8ReYEfsGQ5t7_TS7cNHQuaHJuBlJLHxU,16507
 pip/_internal/network/cache.py,sha256=hgXftU-eau4MWxHSLquTMzepYq5BPC2zhCkhN3glBy8,2145
 pip/_internal/network/download.py,sha256=HvDDq9bVqaN3jcS3DyVJHP7uTqFzbShdkf7NFSoHfkw,6096
 pip/_internal/network/lazy_wheel.py,sha256=PbPyuleNhtEq6b2S7rufoGXZWMD15FAGL4XeiAQ8FxA,7638
 pip/_internal/network/session.py,sha256=BpDOJ7_Xw5VkgPYWsePzcaqOfcyRZcB2AW7W0HGBST0,18443
 pip/_internal/network/utils.py,sha256=6A5SrUJEEUHxbGtbscwU2NpCyz-3ztiDlGWHpRRhsJ8,4073
 pip/_internal/network/xmlrpc.py,sha256=AzQgG4GgS152_cqmGr_Oz2MIXsCal-xfsis7fA7nmU0,1791
 pip/_internal/operations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_internal/operations/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/operations/__pycache__/check.cpython-37.pyc,,
-pip/_internal/operations/__pycache__/freeze.cpython-37.pyc,,
-pip/_internal/operations/__pycache__/prepare.cpython-37.pyc,,
+pip/_internal/operations/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/operations/__pycache__/check.cpython-38.pyc,,
+pip/_internal/operations/__pycache__/freeze.cpython-38.pyc,,
+pip/_internal/operations/__pycache__/prepare.cpython-38.pyc,,
 pip/_internal/operations/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_internal/operations/build/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/operations/build/__pycache__/build_tracker.cpython-37.pyc,,
-pip/_internal/operations/build/__pycache__/metadata.cpython-37.pyc,,
-pip/_internal/operations/build/__pycache__/metadata_editable.cpython-37.pyc,,
-pip/_internal/operations/build/__pycache__/metadata_legacy.cpython-37.pyc,,
-pip/_internal/operations/build/__pycache__/wheel.cpython-37.pyc,,
-pip/_internal/operations/build/__pycache__/wheel_editable.cpython-37.pyc,,
-pip/_internal/operations/build/__pycache__/wheel_legacy.cpython-37.pyc,,
+pip/_internal/operations/build/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/operations/build/__pycache__/build_tracker.cpython-38.pyc,,
+pip/_internal/operations/build/__pycache__/metadata.cpython-38.pyc,,
+pip/_internal/operations/build/__pycache__/metadata_editable.cpython-38.pyc,,
+pip/_internal/operations/build/__pycache__/metadata_legacy.cpython-38.pyc,,
+pip/_internal/operations/build/__pycache__/wheel.cpython-38.pyc,,
+pip/_internal/operations/build/__pycache__/wheel_editable.cpython-38.pyc,,
+pip/_internal/operations/build/__pycache__/wheel_legacy.cpython-38.pyc,,
 pip/_internal/operations/build/build_tracker.py,sha256=vf81EwomN3xe9G8qRJED0VGqNikmRQRQoobNsxi5Xrs,4133
 pip/_internal/operations/build/metadata.py,sha256=9S0CUD8U3QqZeXp-Zyt8HxwU90lE4QrnYDgrqZDzBnc,1422
 pip/_internal/operations/build/metadata_editable.py,sha256=VLL7LvntKE8qxdhUdEJhcotFzUsOSI8NNS043xULKew,1474
 pip/_internal/operations/build/metadata_legacy.py,sha256=o-eU21As175hDC7dluM1fJJ_FqokTIShyWpjKaIpHZw,2198
 pip/_internal/operations/build/wheel.py,sha256=sT12FBLAxDC6wyrDorh8kvcZ1jG5qInCRWzzP-UkJiQ,1075
 pip/_internal/operations/build/wheel_editable.py,sha256=yOtoH6zpAkoKYEUtr8FhzrYnkNHQaQBjWQ2HYae1MQg,1417
 pip/_internal/operations/build/wheel_legacy.py,sha256=C9j6rukgQI1n_JeQLoZGuDdfUwzCXShyIdPTp6edbMQ,3064
 pip/_internal/operations/check.py,sha256=WsN7z0_QSgJjw0JsWWcqOHj4wWTaFv0J7mxgUByDCOg,5122
 pip/_internal/operations/freeze.py,sha256=mwTZ2uML8aQgo3k8MR79a7SZmmmvdAJqdyaknKbavmg,9784
 pip/_internal/operations/install/__init__.py,sha256=mX7hyD2GNBO2mFGokDQ30r_GXv7Y_PLdtxcUv144e-s,51
-pip/_internal/operations/install/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/operations/install/__pycache__/editable_legacy.cpython-37.pyc,,
-pip/_internal/operations/install/__pycache__/legacy.cpython-37.pyc,,
-pip/_internal/operations/install/__pycache__/wheel.cpython-37.pyc,,
+pip/_internal/operations/install/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/operations/install/__pycache__/editable_legacy.cpython-38.pyc,,
+pip/_internal/operations/install/__pycache__/legacy.cpython-38.pyc,,
+pip/_internal/operations/install/__pycache__/wheel.cpython-38.pyc,,
 pip/_internal/operations/install/editable_legacy.py,sha256=ee4kfJHNuzTdKItbfAsNOSEwq_vD7DRPGkBdK48yBhU,1354
 pip/_internal/operations/install/legacy.py,sha256=cHdcHebyzf8w7OaOLwcsTNSMSSV8WBoAPFLay_9CjE8,4105
 pip/_internal/operations/install/wheel.py,sha256=CxzEg2wTPX4SxNTPIx0ozTqF1X7LhpCyP3iM2FjcKUE,27407
 pip/_internal/operations/prepare.py,sha256=BeYXrLFpRoV5XBnRXQHxRA2plyC36kK9Pms5D9wjCo4,25091
 pip/_internal/pyproject.py,sha256=QqSZR5AGwtf3HTa8NdbDq2yj9T2r9S2h9gnU4aX2Kvg,6987
 pip/_internal/req/__init__.py,sha256=rUQ9d_Sh3E5kNYqX9pkN0D06YL-LrtcbJQ-LiIonq08,2807
-pip/_internal/req/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/req/__pycache__/constructors.cpython-37.pyc,,
-pip/_internal/req/__pycache__/req_file.cpython-37.pyc,,
-pip/_internal/req/__pycache__/req_install.cpython-37.pyc,,
-pip/_internal/req/__pycache__/req_set.cpython-37.pyc,,
-pip/_internal/req/__pycache__/req_uninstall.cpython-37.pyc,,
+pip/_internal/req/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/req/__pycache__/constructors.cpython-38.pyc,,
+pip/_internal/req/__pycache__/req_file.cpython-38.pyc,,
+pip/_internal/req/__pycache__/req_install.cpython-38.pyc,,
+pip/_internal/req/__pycache__/req_set.cpython-38.pyc,,
+pip/_internal/req/__pycache__/req_uninstall.cpython-38.pyc,,
 pip/_internal/req/constructors.py,sha256=ypjtq1mOQ3d2mFkFPMf_6Mr8SLKeHQk3tUKHA1ddG0U,16611
 pip/_internal/req/req_file.py,sha256=N6lPO3c0to_G73YyGAnk7VUYmed5jV4Qxgmt1xtlXVg,17646
 pip/_internal/req/req_install.py,sha256=X4WNQlTtvkeATwWdSiJcNLihwbYI_EnGDgE99p-Aa00,35763
 pip/_internal/req/req_set.py,sha256=j3esG0s6SzoVReX9rWn4rpYNtyET_fwxbwJPRimvRxo,2858
 pip/_internal/req/req_uninstall.py,sha256=ZFQfgSNz6H1BMsgl87nQNr2iaQCcbFcmXpW8rKVQcic,24045
 pip/_internal/resolution/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_internal/resolution/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/resolution/__pycache__/base.cpython-37.pyc,,
+pip/_internal/resolution/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/resolution/__pycache__/base.cpython-38.pyc,,
 pip/_internal/resolution/base.py,sha256=qlmh325SBVfvG6Me9gc5Nsh5sdwHBwzHBq6aEXtKsLA,583
 pip/_internal/resolution/legacy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_internal/resolution/legacy/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/resolution/legacy/__pycache__/resolver.cpython-37.pyc,,
+pip/_internal/resolution/legacy/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/resolution/legacy/__pycache__/resolver.cpython-38.pyc,,
 pip/_internal/resolution/legacy/resolver.py,sha256=9em8D5TcSsEN4xZM1WreaRShOnyM4LlvhMSHpUPsocE,24129
 pip/_internal/resolution/resolvelib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_internal/resolution/resolvelib/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__/base.cpython-37.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__/candidates.cpython-37.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__/factory.cpython-37.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__/found_candidates.cpython-37.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__/provider.cpython-37.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__/reporter.cpython-37.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__/requirements.cpython-37.pyc,,
-pip/_internal/resolution/resolvelib/__pycache__/resolver.cpython-37.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/base.cpython-38.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/candidates.cpython-38.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/factory.cpython-38.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/found_candidates.cpython-38.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/provider.cpython-38.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/reporter.cpython-38.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/requirements.cpython-38.pyc,,
+pip/_internal/resolution/resolvelib/__pycache__/resolver.cpython-38.pyc,,
 pip/_internal/resolution/resolvelib/base.py,sha256=u1O4fkvCO4mhmu5i32xrDv9AX5NgUci_eYVyBDQhTIM,5220
 pip/_internal/resolution/resolvelib/candidates.py,sha256=6kQZeMzwibnL4lO6bW0hUQQjNEvXfADdFphRRkRvOtc,18963
 pip/_internal/resolution/resolvelib/factory.py,sha256=OnjkLIgyk5Tol7uOOqapA1D4qiRHWmPU18DF1yN5N8o,27878
 pip/_internal/resolution/resolvelib/found_candidates.py,sha256=hvL3Hoa9VaYo-qEOZkBi2Iqw251UDxPz-uMHVaWmLpE,5705
 pip/_internal/resolution/resolvelib/provider.py,sha256=Vd4jW_NnyifB-HMkPYtZIO70M3_RM0MbL5YV6XyBM-w,9914
 pip/_internal/resolution/resolvelib/reporter.py,sha256=3ZVVYrs5PqvLFJkGLcuXoMK5mTInFzl31xjUpDBpZZk,2526
 pip/_internal/resolution/resolvelib/requirements.py,sha256=B1ndvKPSuyyyTEXt9sKhbwminViSWnBrJa7qO2ln4Z0,5455
 pip/_internal/resolution/resolvelib/resolver.py,sha256=nYZ9bTFXj5c1ILKnkSgU7tUCTYyo5V5J-J0sKoA7Wzg,11533
 pip/_internal/self_outdated_check.py,sha256=pnqBuKKZQ8OxKP0MaUUiDHl3AtyoMJHHG4rMQ7YcYXY,8167
 pip/_internal/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_internal/utils/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/_log.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/appdirs.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/compat.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/compatibility_tags.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/datetime.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/deprecation.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/direct_url_helpers.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/distutils_args.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/egg_link.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/encoding.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/entrypoints.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/filesystem.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/filetypes.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/glibc.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/hashes.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/inject_securetransport.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/logging.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/misc.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/models.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/packaging.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/setuptools_build.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/subprocess.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/temp_dir.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/unpacking.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/urls.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/virtualenv.cpython-37.pyc,,
-pip/_internal/utils/__pycache__/wheel.cpython-37.pyc,,
+pip/_internal/utils/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/_log.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/appdirs.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/compat.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/compatibility_tags.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/datetime.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/deprecation.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/direct_url_helpers.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/distutils_args.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/egg_link.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/encoding.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/entrypoints.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/filesystem.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/filetypes.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/glibc.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/hashes.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/inject_securetransport.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/logging.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/misc.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/models.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/packaging.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/setuptools_build.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/subprocess.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/temp_dir.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/unpacking.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/urls.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/virtualenv.cpython-38.pyc,,
+pip/_internal/utils/__pycache__/wheel.cpython-38.pyc,,
 pip/_internal/utils/_log.py,sha256=-jHLOE_THaZz5BFcCnoSL9EYAtJ0nXem49s9of4jvKw,1015
 pip/_internal/utils/appdirs.py,sha256=swgcTKOm3daLeXTW6v5BUS2Ti2RvEnGRQYH_yDXklAo,1665
 pip/_internal/utils/compat.py,sha256=ACyBfLgj3_XG-iA5omEDrXqDM0cQKzi8h8HRBInzG6Q,1884
 pip/_internal/utils/compatibility_tags.py,sha256=ydin8QG8BHqYRsPY4OL6cmb44CbqXl1T0xxS97VhHkk,5377
 pip/_internal/utils/datetime.py,sha256=m21Y3wAtQc-ji6Veb6k_M5g6A0ZyFI4egchTdnwh-pQ,242
 pip/_internal/utils/deprecation.py,sha256=OLc7GzDwPob9y8jscDYCKUNBV-9CWwqFplBOJPLOpBM,5764
 pip/_internal/utils/direct_url_helpers.py,sha256=6F1tc2rcKaCZmgfVwsE6ObIe_Pux23mUVYA-2D9wCFc,3206
@@ -297,116 +297,116 @@
 pip/_internal/utils/subprocess.py,sha256=0EMhgfPGFk8FZn6Qq7Hp9PN6YHuQNWiVby4DXcTCON4,9200
 pip/_internal/utils/temp_dir.py,sha256=aCX489gRa4Nu0dMKRFyGhV6maJr60uEynu5uCbKR4Qg,7702
 pip/_internal/utils/unpacking.py,sha256=SBb2iV1crb89MDRTEKY86R4A_UOWApTQn9VQVcMDOlE,8821
 pip/_internal/utils/urls.py,sha256=AhaesUGl-9it6uvG6fsFPOr9ynFpGaTMk4t5XTX7Z_Q,1759
 pip/_internal/utils/virtualenv.py,sha256=S6f7csYorRpiD6cvn3jISZYc3I8PJC43H5iMFpRAEDU,3456
 pip/_internal/utils/wheel.py,sha256=lXOgZyTlOm5HmK8tw5iw0A3_5A6wRzsXHOaQkIvvloU,4549
 pip/_internal/vcs/__init__.py,sha256=UAqvzpbi0VbZo3Ub6skEeZAw-ooIZR-zX_WpCbxyCoU,596
-pip/_internal/vcs/__pycache__/__init__.cpython-37.pyc,,
-pip/_internal/vcs/__pycache__/bazaar.cpython-37.pyc,,
-pip/_internal/vcs/__pycache__/git.cpython-37.pyc,,
-pip/_internal/vcs/__pycache__/mercurial.cpython-37.pyc,,
-pip/_internal/vcs/__pycache__/subversion.cpython-37.pyc,,
-pip/_internal/vcs/__pycache__/versioncontrol.cpython-37.pyc,,
+pip/_internal/vcs/__pycache__/__init__.cpython-38.pyc,,
+pip/_internal/vcs/__pycache__/bazaar.cpython-38.pyc,,
+pip/_internal/vcs/__pycache__/git.cpython-38.pyc,,
+pip/_internal/vcs/__pycache__/mercurial.cpython-38.pyc,,
+pip/_internal/vcs/__pycache__/subversion.cpython-38.pyc,,
+pip/_internal/vcs/__pycache__/versioncontrol.cpython-38.pyc,,
 pip/_internal/vcs/bazaar.py,sha256=j0oin0fpGRHcCFCxEcpPCQoFEvA-DMLULKdGP8Nv76o,3519
 pip/_internal/vcs/git.py,sha256=mjhwudCx9WlLNkxZ6_kOKmueF0rLoU2i1xeASKF6yiQ,18116
 pip/_internal/vcs/mercurial.py,sha256=Bzbd518Jsx-EJI0IhIobiQqiRsUv5TWYnrmRIFWE0Gw,5238
 pip/_internal/vcs/subversion.py,sha256=vhZs8L-TNggXqM1bbhl-FpbxE3TrIB6Tgnx8fh3S2HE,11729
 pip/_internal/vcs/versioncontrol.py,sha256=KUOc-hN51em9jrqxKwUR3JnkgSE-xSOqMiiJcSaL6B8,22811
 pip/_internal/wheel_builder.py,sha256=8cObBCu4mIsMJqZM7xXI9DO3vldiAnRNa1Gt6izPPTs,13079
 pip/_vendor/__init__.py,sha256=fNxOSVD0auElsD8fN9tuq5psfgMQ-RFBtD4X5gjlRkg,4966
-pip/_vendor/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/__pycache__/six.cpython-37.pyc,,
-pip/_vendor/__pycache__/typing_extensions.cpython-37.pyc,,
+pip/_vendor/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/__pycache__/six.cpython-38.pyc,,
+pip/_vendor/__pycache__/typing_extensions.cpython-38.pyc,,
 pip/_vendor/cachecontrol/__init__.py,sha256=hrxlv3q7upsfyMw8k3gQ9vagBax1pYHSGGqYlZ0Zk0M,465
-pip/_vendor/cachecontrol/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/_cmd.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/adapter.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/cache.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/compat.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/controller.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/filewrapper.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/heuristics.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/serialize.cpython-37.pyc,,
-pip/_vendor/cachecontrol/__pycache__/wrapper.cpython-37.pyc,,
+pip/_vendor/cachecontrol/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/_cmd.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/adapter.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/cache.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/compat.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/controller.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/filewrapper.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/heuristics.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/serialize.cpython-38.pyc,,
+pip/_vendor/cachecontrol/__pycache__/wrapper.cpython-38.pyc,,
 pip/_vendor/cachecontrol/_cmd.py,sha256=lxUXqfNTVx84zf6tcWbkLZHA6WVBRtJRpfeA9ZqhaAY,1379
 pip/_vendor/cachecontrol/adapter.py,sha256=ew9OYEQHEOjvGl06ZsuX8W3DAvHWsQKHwWAxISyGug8,5033
 pip/_vendor/cachecontrol/cache.py,sha256=Tty45fOjH40fColTGkqKQvQQmbYsMpk-nCyfLcv2vG4,1535
 pip/_vendor/cachecontrol/caches/__init__.py,sha256=h-1cUmOz6mhLsjTjOrJ8iPejpGdLCyG4lzTftfGZvLg,242
-pip/_vendor/cachecontrol/caches/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/cachecontrol/caches/__pycache__/file_cache.cpython-37.pyc,,
-pip/_vendor/cachecontrol/caches/__pycache__/redis_cache.cpython-37.pyc,,
+pip/_vendor/cachecontrol/caches/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/cachecontrol/caches/__pycache__/file_cache.cpython-38.pyc,,
+pip/_vendor/cachecontrol/caches/__pycache__/redis_cache.cpython-38.pyc,,
 pip/_vendor/cachecontrol/caches/file_cache.py,sha256=GpexcE29LoY4MaZwPUTcUBZaDdcsjqyLxZFznk8Hbr4,5271
 pip/_vendor/cachecontrol/caches/redis_cache.py,sha256=mp-QWonP40I3xJGK3XVO-Gs9a3UjzlqqEmp9iLJH9F4,1033
 pip/_vendor/cachecontrol/compat.py,sha256=LNx7vqBndYdHU8YuJt53ab_8rzMGTXVrvMb7CZJkxG0,778
 pip/_vendor/cachecontrol/controller.py,sha256=bAYrt7x_VH4toNpI066LQxbHpYGpY1MxxmZAhspplvw,16416
 pip/_vendor/cachecontrol/filewrapper.py,sha256=X4BAQOO26GNOR7nH_fhTzAfeuct2rBQcx_15MyFBpcs,3946
 pip/_vendor/cachecontrol/heuristics.py,sha256=8kAyuZLSCyEIgQr6vbUwfhpqg9ows4mM0IV6DWazevI,4154
 pip/_vendor/cachecontrol/serialize.py,sha256=_U1NU_C-SDgFzkbAxAsPDgMTHeTWZZaHCQnZN_jh0U8,7105
 pip/_vendor/cachecontrol/wrapper.py,sha256=X3-KMZ20Ho3VtqyVaXclpeQpFzokR5NE8tZSfvKVaB8,774
 pip/_vendor/certifi/__init__.py,sha256=bK_nm9bLJzNvWZc2oZdiTwg2KWD4HSPBWGaM0zUDvMw,94
 pip/_vendor/certifi/__main__.py,sha256=1k3Cr95vCxxGRGDljrW3wMdpZdL3Nhf0u1n-k2qdsCY,255
-pip/_vendor/certifi/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/certifi/__pycache__/__main__.cpython-37.pyc,,
-pip/_vendor/certifi/__pycache__/core.cpython-37.pyc,,
+pip/_vendor/certifi/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/certifi/__pycache__/__main__.cpython-38.pyc,,
+pip/_vendor/certifi/__pycache__/core.cpython-38.pyc,,
 pip/_vendor/certifi/cacert.pem,sha256=LBHDzgj_xA05AxnHK8ENT5COnGNElNZe0svFUHMf1SQ,275233
 pip/_vendor/certifi/core.py,sha256=ZwiOsv-sD_ouU1ft8wy_xZ3LQ7UbcVzyqj2XNyrsZis,4279
 pip/_vendor/chardet/__init__.py,sha256=57R-HSxj0PWmILMN0GFmUNqEMfrEVSamXyjD-W6_fbs,4797
-pip/_vendor/chardet/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/big5freq.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/big5prober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/chardistribution.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/charsetgroupprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/charsetprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/codingstatemachine.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/codingstatemachinedict.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/cp949prober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/enums.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/escprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/escsm.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/eucjpprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/euckrfreq.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/euckrprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/euctwfreq.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/euctwprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/gb2312freq.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/gb2312prober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/hebrewprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/jisfreq.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/johabfreq.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/johabprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/jpcntx.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/langbulgarianmodel.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/langgreekmodel.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/langhebrewmodel.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/langhungarianmodel.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/langrussianmodel.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/langthaimodel.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/langturkishmodel.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/latin1prober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/macromanprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/mbcharsetprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/mbcsgroupprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/mbcssm.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/resultdict.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/sbcharsetprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/sbcsgroupprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/sjisprober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/universaldetector.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/utf1632prober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/utf8prober.cpython-37.pyc,,
-pip/_vendor/chardet/__pycache__/version.cpython-37.pyc,,
+pip/_vendor/chardet/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/big5freq.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/big5prober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/chardistribution.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/charsetgroupprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/charsetprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/codingstatemachine.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/codingstatemachinedict.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/cp949prober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/enums.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/escprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/escsm.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/eucjpprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/euckrfreq.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/euckrprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/euctwfreq.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/euctwprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/gb2312freq.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/gb2312prober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/hebrewprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/jisfreq.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/johabfreq.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/johabprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/jpcntx.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/langbulgarianmodel.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/langgreekmodel.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/langhebrewmodel.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/langhungarianmodel.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/langrussianmodel.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/langthaimodel.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/langturkishmodel.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/latin1prober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/macromanprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/mbcharsetprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/mbcsgroupprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/mbcssm.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/resultdict.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/sbcharsetprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/sbcsgroupprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/sjisprober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/universaldetector.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/utf1632prober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/utf8prober.cpython-38.pyc,,
+pip/_vendor/chardet/__pycache__/version.cpython-38.pyc,,
 pip/_vendor/chardet/big5freq.py,sha256=ltcfP-3PjlNHCoo5e4a7C4z-2DhBTXRfY6jbMbB7P30,31274
 pip/_vendor/chardet/big5prober.py,sha256=lPMfwCX6v2AaPgvFh_cSWZcgLDbWiFCHLZ_p9RQ9uxE,1763
 pip/_vendor/chardet/chardistribution.py,sha256=13B8XUG4oXDuLdXvfbIWwLFeR-ZU21AqTS1zcdON8bU,10032
 pip/_vendor/chardet/charsetgroupprober.py,sha256=UKK3SaIZB2PCdKSIS0gnvMtLR9JJX62M-fZJu3OlWyg,3915
 pip/_vendor/chardet/charsetprober.py,sha256=L3t8_wIOov8em-vZWOcbkdsrwe43N6_gqNh5pH7WPd4,5420
 pip/_vendor/chardet/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_vendor/chardet/cli/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/chardet/cli/__pycache__/chardetect.cpython-37.pyc,,
+pip/_vendor/chardet/cli/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/chardet/cli/__pycache__/chardetect.cpython-38.pyc,,
 pip/_vendor/chardet/cli/chardetect.py,sha256=zibMVg5RpKb-ME9_7EYG4ZM2Sf07NHcQzZ12U-rYJho,3242
 pip/_vendor/chardet/codingstatemachine.py,sha256=K7k69sw3jY5DmTXoSJQVsUtFIQKYPQVOSJJhBuGv_yE,3732
 pip/_vendor/chardet/codingstatemachinedict.py,sha256=0GY3Hi2qIZvDrOOJ3AtqppM1RsYxr_66ER4EHjuMiMc,542
 pip/_vendor/chardet/cp949prober.py,sha256=0jKRV7fECuWI16rNnks0ZECKA1iZYCIEaP8A1ZvjUSI,1860
 pip/_vendor/chardet/enums.py,sha256=TzECiZoCKNMqgwU76cPCeKWFBqaWvAdLMev5_bCkhY8,1683
 pip/_vendor/chardet/escprober.py,sha256=Kho48X65xE0scFylIdeJjM2bcbvRvv0h0WUbMWrJD3A,4006
 pip/_vendor/chardet/escsm.py,sha256=AqyXpA2FQFD7k-buBty_7itGEYkhmVa8X09NLRul3QM,12176
@@ -431,65 +431,65 @@
 pip/_vendor/chardet/langturkishmodel.py,sha256=XY0eGdTIy4eQ9Xg1LVPZacb-UBhHBR-cq0IpPVHowKc,95372
 pip/_vendor/chardet/latin1prober.py,sha256=p15EEmFbmQUwbKLC7lOJVGHEZwcG45ubEZYTGu01J5g,5380
 pip/_vendor/chardet/macromanprober.py,sha256=9anfzmY6TBfUPDyBDOdY07kqmTHpZ1tK0jL-p1JWcOY,6077
 pip/_vendor/chardet/mbcharsetprober.py,sha256=Wr04WNI4F3X_VxEverNG-H25g7u-MDDKlNt-JGj-_uU,3715
 pip/_vendor/chardet/mbcsgroupprober.py,sha256=iRpaNBjV0DNwYPu_z6TiHgRpwYahiM7ztI_4kZ4Uz9A,2131
 pip/_vendor/chardet/mbcssm.py,sha256=hUtPvDYgWDaA2dWdgLsshbwRfm3Q5YRlRogdmeRUNQw,30391
 pip/_vendor/chardet/metadata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_vendor/chardet/metadata/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/chardet/metadata/__pycache__/languages.cpython-37.pyc,,
+pip/_vendor/chardet/metadata/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/chardet/metadata/__pycache__/languages.cpython-38.pyc,,
 pip/_vendor/chardet/metadata/languages.py,sha256=FhvBIdZFxRQ-dTwkb_0madRKgVBCaUMQz9I5xqjE5iQ,13560
 pip/_vendor/chardet/resultdict.py,sha256=ez4FRvN5KaSosJeJ2WzUyKdDdg35HDy_SSLPXKCdt5M,402
 pip/_vendor/chardet/sbcharsetprober.py,sha256=-nd3F90i7GpXLjehLVHqVBE0KlWzGvQUPETLBNn4o6U,6400
 pip/_vendor/chardet/sbcsgroupprober.py,sha256=gcgI0fOfgw_3YTClpbra_MNxwyEyJ3eUXraoLHYb59E,4137
 pip/_vendor/chardet/sjisprober.py,sha256=aqQufMzRw46ZpFlzmYaYeT2-nzmKb-hmcrApppJ862k,4007
 pip/_vendor/chardet/universaldetector.py,sha256=xYBrg4x0dd9WnT8qclfADVD9ondrUNkqPmvte1pa520,14848
 pip/_vendor/chardet/utf1632prober.py,sha256=pw1epGdMj1hDGiCu1AHqqzOEfjX8MVdiW7O1BlT8-eQ,8505
 pip/_vendor/chardet/utf8prober.py,sha256=8m08Ub5490H4jQ6LYXvFysGtgKoKsHUd2zH_i8_TnVw,2812
 pip/_vendor/chardet/version.py,sha256=lGtJcxGM44Qz4Cbk4rbbmrKxnNr1-97U25TameLehZw,244
 pip/_vendor/colorama/__init__.py,sha256=wePQA4U20tKgYARySLEC047ucNX-g8pRLpYBuiHlLb8,266
-pip/_vendor/colorama/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/colorama/__pycache__/ansi.cpython-37.pyc,,
-pip/_vendor/colorama/__pycache__/ansitowin32.cpython-37.pyc,,
-pip/_vendor/colorama/__pycache__/initialise.cpython-37.pyc,,
-pip/_vendor/colorama/__pycache__/win32.cpython-37.pyc,,
-pip/_vendor/colorama/__pycache__/winterm.cpython-37.pyc,,
+pip/_vendor/colorama/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/colorama/__pycache__/ansi.cpython-38.pyc,,
+pip/_vendor/colorama/__pycache__/ansitowin32.cpython-38.pyc,,
+pip/_vendor/colorama/__pycache__/initialise.cpython-38.pyc,,
+pip/_vendor/colorama/__pycache__/win32.cpython-38.pyc,,
+pip/_vendor/colorama/__pycache__/winterm.cpython-38.pyc,,
 pip/_vendor/colorama/ansi.py,sha256=Top4EeEuaQdBWdteKMEcGOTeKeF19Q-Wo_6_Cj5kOzQ,2522
 pip/_vendor/colorama/ansitowin32.py,sha256=vPNYa3OZbxjbuFyaVo0Tmhmy1FZ1lKMWCnT7odXpItk,11128
 pip/_vendor/colorama/initialise.py,sha256=-hIny86ClXo39ixh5iSCfUIa2f_h_bgKRDW7gqs-KLU,3325
 pip/_vendor/colorama/tests/__init__.py,sha256=MkgPAEzGQd-Rq0w0PZXSX2LadRWhUECcisJY8lSrm4Q,75
-pip/_vendor/colorama/tests/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/colorama/tests/__pycache__/ansi_test.cpython-37.pyc,,
-pip/_vendor/colorama/tests/__pycache__/ansitowin32_test.cpython-37.pyc,,
-pip/_vendor/colorama/tests/__pycache__/initialise_test.cpython-37.pyc,,
-pip/_vendor/colorama/tests/__pycache__/isatty_test.cpython-37.pyc,,
-pip/_vendor/colorama/tests/__pycache__/utils.cpython-37.pyc,,
-pip/_vendor/colorama/tests/__pycache__/winterm_test.cpython-37.pyc,,
+pip/_vendor/colorama/tests/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/colorama/tests/__pycache__/ansi_test.cpython-38.pyc,,
+pip/_vendor/colorama/tests/__pycache__/ansitowin32_test.cpython-38.pyc,,
+pip/_vendor/colorama/tests/__pycache__/initialise_test.cpython-38.pyc,,
+pip/_vendor/colorama/tests/__pycache__/isatty_test.cpython-38.pyc,,
+pip/_vendor/colorama/tests/__pycache__/utils.cpython-38.pyc,,
+pip/_vendor/colorama/tests/__pycache__/winterm_test.cpython-38.pyc,,
 pip/_vendor/colorama/tests/ansi_test.py,sha256=FeViDrUINIZcr505PAxvU4AjXz1asEiALs9GXMhwRaE,2839
 pip/_vendor/colorama/tests/ansitowin32_test.py,sha256=RN7AIhMJ5EqDsYaCjVo-o4u8JzDD4ukJbmevWKS70rY,10678
 pip/_vendor/colorama/tests/initialise_test.py,sha256=BbPy-XfyHwJ6zKozuQOvNvQZzsx9vdb_0bYXn7hsBTc,6741
 pip/_vendor/colorama/tests/isatty_test.py,sha256=Pg26LRpv0yQDB5Ac-sxgVXG7hsA1NYvapFgApZfYzZg,1866
 pip/_vendor/colorama/tests/utils.py,sha256=1IIRylG39z5-dzq09R_ngufxyPZxgldNbrxKxUGwGKE,1079
 pip/_vendor/colorama/tests/winterm_test.py,sha256=qoWFPEjym5gm2RuMwpf3pOis3a5r_PJZFCzK254JL8A,3709
 pip/_vendor/colorama/win32.py,sha256=YQOKwMTwtGBbsY4dL5HYTvwTeP9wIQra5MvPNddpxZs,6181
 pip/_vendor/colorama/winterm.py,sha256=XCQFDHjPi6AHYNdZwy0tA02H-Jh48Jp-HvCjeLeLp3U,7134
 pip/_vendor/distlib/__init__.py,sha256=acgfseOC55dNrVAzaBKpUiH3Z6V7Q1CaxsiQ3K7pC-E,581
-pip/_vendor/distlib/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/compat.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/database.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/index.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/locators.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/manifest.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/markers.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/metadata.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/resources.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/scripts.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/util.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/version.cpython-37.pyc,,
-pip/_vendor/distlib/__pycache__/wheel.cpython-37.pyc,,
+pip/_vendor/distlib/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/compat.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/database.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/index.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/locators.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/manifest.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/markers.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/metadata.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/resources.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/scripts.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/util.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/version.cpython-38.pyc,,
+pip/_vendor/distlib/__pycache__/wheel.cpython-38.pyc,,
 pip/_vendor/distlib/compat.py,sha256=tfoMrj6tujk7G4UC2owL6ArgDuCKabgBxuJRGZSmpko,41259
 pip/_vendor/distlib/database.py,sha256=o_mw0fAr93NDAHHHfqG54Y1Hi9Rkfrp2BX15XWZYK50,51697
 pip/_vendor/distlib/index.py,sha256=HFiDG7LMoaBs829WuotrfIwcErOOExUOR_AeBtw_TCU,20834
 pip/_vendor/distlib/locators.py,sha256=wNzG-zERzS_XGls-nBPVVyLRHa2skUlkn0-5n0trMWA,51991
 pip/_vendor/distlib/manifest.py,sha256=nQEhYmgoreaBZzyFzwYsXxJARu3fo4EkunU163U16iE,14811
 pip/_vendor/distlib/markers.py,sha256=TpHHHLgkzyT7YHbwj-2i6weRaq-Ivy2-MUnrDkjau-U,5058
 pip/_vendor/distlib/metadata.py,sha256=g_DIiu8nBXRzA-mWPRpatHGbmFZqaFoss7z9TG7QSUU,39801
@@ -502,123 +502,123 @@
 pip/_vendor/distlib/version.py,sha256=WG__LyAa2GwmA6qSoEJtvJE8REA1LZpbSizy8WvhJLk,23513
 pip/_vendor/distlib/w32.exe,sha256=R4csx3-OGM9kL4aPIzQKRo5TfmRSHZo6QWyLhDhNBks,91648
 pip/_vendor/distlib/w64-arm.exe,sha256=xdyYhKj0WDcVUOCb05blQYvzdYIKMbmJn2SZvzkcey4,168448
 pip/_vendor/distlib/w64.exe,sha256=ejGf-rojoBfXseGLpya6bFTFPWRG21X5KvU8J5iU-K0,101888
 pip/_vendor/distlib/wheel.py,sha256=Rgqs658VsJ3R2845qwnZD8XQryV2CzWw2mghwLvxxsI,43898
 pip/_vendor/distro/__init__.py,sha256=2fHjF-SfgPvjyNZ1iHh_wjqWdR_Yo5ODHwZC0jLBPhc,981
 pip/_vendor/distro/__main__.py,sha256=bu9d3TifoKciZFcqRBuygV3GSuThnVD_m2IK4cz96Vs,64
-pip/_vendor/distro/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/distro/__pycache__/__main__.cpython-37.pyc,,
-pip/_vendor/distro/__pycache__/distro.cpython-37.pyc,,
+pip/_vendor/distro/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/distro/__pycache__/__main__.cpython-38.pyc,,
+pip/_vendor/distro/__pycache__/distro.cpython-38.pyc,,
 pip/_vendor/distro/distro.py,sha256=UZO1LjIhtFCMdlbiz39gj3raV-Amf3SBwzGzfApiMHw,49330
 pip/_vendor/idna/__init__.py,sha256=KJQN1eQBr8iIK5SKrJ47lXvxG0BJ7Lm38W4zT0v_8lk,849
-pip/_vendor/idna/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/idna/__pycache__/codec.cpython-37.pyc,,
-pip/_vendor/idna/__pycache__/compat.cpython-37.pyc,,
-pip/_vendor/idna/__pycache__/core.cpython-37.pyc,,
-pip/_vendor/idna/__pycache__/idnadata.cpython-37.pyc,,
-pip/_vendor/idna/__pycache__/intranges.cpython-37.pyc,,
-pip/_vendor/idna/__pycache__/package_data.cpython-37.pyc,,
-pip/_vendor/idna/__pycache__/uts46data.cpython-37.pyc,,
+pip/_vendor/idna/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/idna/__pycache__/codec.cpython-38.pyc,,
+pip/_vendor/idna/__pycache__/compat.cpython-38.pyc,,
+pip/_vendor/idna/__pycache__/core.cpython-38.pyc,,
+pip/_vendor/idna/__pycache__/idnadata.cpython-38.pyc,,
+pip/_vendor/idna/__pycache__/intranges.cpython-38.pyc,,
+pip/_vendor/idna/__pycache__/package_data.cpython-38.pyc,,
+pip/_vendor/idna/__pycache__/uts46data.cpython-38.pyc,,
 pip/_vendor/idna/codec.py,sha256=6ly5odKfqrytKT9_7UrlGklHnf1DSK2r9C6cSM4sa28,3374
 pip/_vendor/idna/compat.py,sha256=0_sOEUMT4CVw9doD3vyRhX80X19PwqFoUBs7gWsFME4,321
 pip/_vendor/idna/core.py,sha256=1JxchwKzkxBSn7R_oCE12oBu3eVux0VzdxolmIad24M,12950
 pip/_vendor/idna/idnadata.py,sha256=xUjqKqiJV8Ho_XzBpAtv5JFoVPSupK-SUXvtjygUHqw,44375
 pip/_vendor/idna/intranges.py,sha256=YBr4fRYuWH7kTKS2tXlFjM24ZF1Pdvcir-aywniInqg,1881
 pip/_vendor/idna/package_data.py,sha256=C_jHJzmX8PI4xq0jpzmcTMxpb5lDsq4o5VyxQzlVrZE,21
 pip/_vendor/idna/uts46data.py,sha256=zvjZU24s58_uAS850Mcd0NnD0X7_gCMAMjzWNIeUJdc,206539
 pip/_vendor/msgpack/__init__.py,sha256=NryGaKLDk_Egd58ZxXpnuI7OWO27AXz7S6CBFRM3sAY,1132
-pip/_vendor/msgpack/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/msgpack/__pycache__/exceptions.cpython-37.pyc,,
-pip/_vendor/msgpack/__pycache__/ext.cpython-37.pyc,,
-pip/_vendor/msgpack/__pycache__/fallback.cpython-37.pyc,,
+pip/_vendor/msgpack/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/msgpack/__pycache__/exceptions.cpython-38.pyc,,
+pip/_vendor/msgpack/__pycache__/ext.cpython-38.pyc,,
+pip/_vendor/msgpack/__pycache__/fallback.cpython-38.pyc,,
 pip/_vendor/msgpack/exceptions.py,sha256=dCTWei8dpkrMsQDcjQk74ATl9HsIBH0ybt8zOPNqMYc,1081
 pip/_vendor/msgpack/ext.py,sha256=TuldJPkYu8Wo_Xh0tFGL2l06-gY88NSR8tOje9fo2Wg,6080
 pip/_vendor/msgpack/fallback.py,sha256=OORDn86-fHBPlu-rPlMdM10KzkH6S_Rx9CHN1b7o4cg,34557
 pip/_vendor/packaging/__about__.py,sha256=ugASIO2w1oUyH8_COqQ2X_s0rDhjbhQC3yJocD03h2c,661
 pip/_vendor/packaging/__init__.py,sha256=b9Kk5MF7KxhhLgcDmiUWukN-LatWFxPdNug0joPhHSk,497
-pip/_vendor/packaging/__pycache__/__about__.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/_manylinux.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/_musllinux.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/_structures.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/markers.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/requirements.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/specifiers.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/tags.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/utils.cpython-37.pyc,,
-pip/_vendor/packaging/__pycache__/version.cpython-37.pyc,,
+pip/_vendor/packaging/__pycache__/__about__.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/_manylinux.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/_musllinux.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/_structures.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/markers.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/requirements.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/specifiers.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/tags.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/utils.cpython-38.pyc,,
+pip/_vendor/packaging/__pycache__/version.cpython-38.pyc,,
 pip/_vendor/packaging/_manylinux.py,sha256=XcbiXB-qcjv3bcohp6N98TMpOP4_j3m-iOA8ptK2GWY,11488
 pip/_vendor/packaging/_musllinux.py,sha256=_KGgY_qc7vhMGpoqss25n2hiLCNKRtvz9mCrS7gkqyc,4378
 pip/_vendor/packaging/_structures.py,sha256=q3eVNmbWJGG_S0Dit_S3Ao8qQqz_5PYTXFAKBZe5yr4,1431
 pip/_vendor/packaging/markers.py,sha256=AJBOcY8Oq0kYc570KuuPTkvuqjAlhufaE2c9sCUbm64,8487
 pip/_vendor/packaging/requirements.py,sha256=NtDlPBtojpn1IUC85iMjPNsUmufjpSlwnNA-Xb4m5NA,4676
 pip/_vendor/packaging/specifiers.py,sha256=LRQ0kFsHrl5qfcFNEEJrIFYsnIHQUJXY9fIsakTrrqE,30110
 pip/_vendor/packaging/tags.py,sha256=lmsnGNiJ8C4D_Pf9PbM0qgbZvD9kmB9lpZBQUZa3R_Y,15699
 pip/_vendor/packaging/utils.py,sha256=dJjeat3BS-TYn1RrUFVwufUMasbtzLfYRoy_HXENeFQ,4200
 pip/_vendor/packaging/version.py,sha256=_fLRNrFrxYcHVfyo8vk9j8s6JM8N_xsSxVFr6RJyco8,14665
 pip/_vendor/pkg_resources/__init__.py,sha256=NnpQ3g6BCHzpMgOR_OLBmYtniY4oOzdKpwqghfq_6ug,108287
-pip/_vendor/pkg_resources/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/pkg_resources/__pycache__/py31compat.cpython-37.pyc,,
+pip/_vendor/pkg_resources/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/pkg_resources/__pycache__/py31compat.cpython-38.pyc,,
 pip/_vendor/pkg_resources/py31compat.py,sha256=CRk8fkiPRDLsbi5pZcKsHI__Pbmh_94L8mr9Qy9Ab2U,562
 pip/_vendor/platformdirs/__init__.py,sha256=9iY4Z8iJDZB0djln6zHHwrPVWpB54TCygcnh--MujU0,12936
 pip/_vendor/platformdirs/__main__.py,sha256=ZmsnTxEOxtTvwa-Y_Vfab_JN3X4XCVeN8X0yyy9-qnc,1176
-pip/_vendor/platformdirs/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/platformdirs/__pycache__/__main__.cpython-37.pyc,,
-pip/_vendor/platformdirs/__pycache__/android.cpython-37.pyc,,
-pip/_vendor/platformdirs/__pycache__/api.cpython-37.pyc,,
-pip/_vendor/platformdirs/__pycache__/macos.cpython-37.pyc,,
-pip/_vendor/platformdirs/__pycache__/unix.cpython-37.pyc,,
-pip/_vendor/platformdirs/__pycache__/version.cpython-37.pyc,,
-pip/_vendor/platformdirs/__pycache__/windows.cpython-37.pyc,,
+pip/_vendor/platformdirs/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/platformdirs/__pycache__/__main__.cpython-38.pyc,,
+pip/_vendor/platformdirs/__pycache__/android.cpython-38.pyc,,
+pip/_vendor/platformdirs/__pycache__/api.cpython-38.pyc,,
+pip/_vendor/platformdirs/__pycache__/macos.cpython-38.pyc,,
+pip/_vendor/platformdirs/__pycache__/unix.cpython-38.pyc,,
+pip/_vendor/platformdirs/__pycache__/version.cpython-38.pyc,,
+pip/_vendor/platformdirs/__pycache__/windows.cpython-38.pyc,,
 pip/_vendor/platformdirs/android.py,sha256=GKizhyS7ESRiU67u8UnBJLm46goau9937EchXWbPBlk,4068
 pip/_vendor/platformdirs/api.py,sha256=MXKHXOL3eh_-trSok-JUTjAR_zjmmKF3rjREVABjP8s,4910
 pip/_vendor/platformdirs/macos.py,sha256=-3UXQewbT0yMhMdkzRXfXGAntmLIH7Qt4a9Hlf8I5_Y,2655
 pip/_vendor/platformdirs/unix.py,sha256=P-WQjSSieE38DXjMDa1t4XHnKJQ5idEaKT0PyXwm8KQ,6911
 pip/_vendor/platformdirs/version.py,sha256=qaN-fw_htIgKUVXoAuAEVgKxQu3tZ9qE2eiKkWIS7LA,160
 pip/_vendor/platformdirs/windows.py,sha256=LOrXLgI0CjQldDo2zhOZYGYZ6g4e_cJOCB_pF9aMRWQ,6596
 pip/_vendor/pygments/__init__.py,sha256=5oLcMLXD0cTG8YcHBPITtK1fS0JBASILEvEnWkTezgE,2999
 pip/_vendor/pygments/__main__.py,sha256=p0_rz3JZmNZMNZBOqDojaEx1cr9wmA9FQZX_TYl74lQ,353
-pip/_vendor/pygments/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/__main__.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/cmdline.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/console.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/filter.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/formatter.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/lexer.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/modeline.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/plugin.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/regexopt.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/scanner.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/sphinxext.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/style.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/token.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/unistring.cpython-37.pyc,,
-pip/_vendor/pygments/__pycache__/util.cpython-37.pyc,,
+pip/_vendor/pygments/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/__main__.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/cmdline.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/console.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/filter.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/formatter.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/lexer.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/modeline.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/plugin.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/regexopt.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/scanner.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/sphinxext.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/style.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/token.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/unistring.cpython-38.pyc,,
+pip/_vendor/pygments/__pycache__/util.cpython-38.pyc,,
 pip/_vendor/pygments/cmdline.py,sha256=rc0fah4eknRqFgn1wKNEwkq0yWnSqYOGaA4PaIeOxVY,23685
 pip/_vendor/pygments/console.py,sha256=hQfqCFuOlGk7DW2lPQYepsw-wkOH1iNt9ylNA1eRymM,1697
 pip/_vendor/pygments/filter.py,sha256=NglMmMPTRRv-zuRSE_QbWid7JXd2J4AvwjCW2yWALXU,1938
 pip/_vendor/pygments/filters/__init__.py,sha256=b5YuXB9rampSy2-cMtKxGQoMDfrG4_DcvVwZrzTlB6w,40386
-pip/_vendor/pygments/filters/__pycache__/__init__.cpython-37.pyc,,
+pip/_vendor/pygments/filters/__pycache__/__init__.cpython-38.pyc,,
 pip/_vendor/pygments/formatter.py,sha256=6-TS2Y8pUMeWIUolWwr1O8ruC-U6HydWDwOdbAiJgJQ,2917
 pip/_vendor/pygments/formatters/__init__.py,sha256=YTqGeHS17fNXCLMZpf7oCxBCKLB9YLsZ8IAsjGhawyg,4810
-pip/_vendor/pygments/formatters/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/_mapping.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/bbcode.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/groff.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/html.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/img.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/irc.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/latex.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/other.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/pangomarkup.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/rtf.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/svg.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/terminal.cpython-37.pyc,,
-pip/_vendor/pygments/formatters/__pycache__/terminal256.cpython-37.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/_mapping.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/bbcode.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/groff.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/html.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/img.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/irc.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/latex.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/other.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/pangomarkup.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/rtf.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/svg.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/terminal.cpython-38.pyc,,
+pip/_vendor/pygments/formatters/__pycache__/terminal256.cpython-38.pyc,,
 pip/_vendor/pygments/formatters/_mapping.py,sha256=fCZgvsM6UEuZUG7J6lr47eVss5owKd_JyaNbDfxeqmQ,4104
 pip/_vendor/pygments/formatters/bbcode.py,sha256=JrL4ITjN-KzPcuQpPMBf1pm33eW2sDUNr8WzSoAJsJA,3314
 pip/_vendor/pygments/formatters/groff.py,sha256=xrOFoLbafSA9uHsSLRogy79_Zc4GWJ8tMK2hCdTJRsw,5086
 pip/_vendor/pygments/formatters/html.py,sha256=QNt9prPgxmbKx2M-nfDwoR1bIg06-sNouQuWnE434Wc,35441
 pip/_vendor/pygments/formatters/img.py,sha256=h75Y7IRZLZxDEIwyoOsdRLTwm7kLVPbODKkgEiJ0iKI,21938
 pip/_vendor/pygments/formatters/irc.py,sha256=iwk5tDJOxbCV64SCmOFyvk__x6RD60ay0nUn7ko9n7U,5871
 pip/_vendor/pygments/formatters/latex.py,sha256=thPbytJCIs2AUXsO3NZwqKtXJ-upOlcXP4CXsx94G4w,19351
@@ -626,81 +626,81 @@
 pip/_vendor/pygments/formatters/pangomarkup.py,sha256=ZZzMsKJKXrsDniFeMTkIpe7aQ4VZYRHu0idWmSiUJ2U,2212
 pip/_vendor/pygments/formatters/rtf.py,sha256=abrKlWjipBkQvhIICxtjYTUNv6WME0iJJObFvqVuudE,5014
 pip/_vendor/pygments/formatters/svg.py,sha256=6MM9YyO8NhU42RTQfTWBiagWMnsf9iG5gwhqSriHORE,7335
 pip/_vendor/pygments/formatters/terminal.py,sha256=NpEGvwkC6LgMLQTjVzGrJXji3XcET1sb5JCunSCzoRo,4674
 pip/_vendor/pygments/formatters/terminal256.py,sha256=4v4OVizvsxtwWBpIy_Po30zeOzE5oJg_mOc1-rCjMDk,11753
 pip/_vendor/pygments/lexer.py,sha256=ZPB_TGn_qzrXodRFwEdPzzJk6LZBo9BlfSy3lacc6zg,32005
 pip/_vendor/pygments/lexers/__init__.py,sha256=8d80-XfL5UKDCC1wRD1a_ZBZDkZ2HOe7Zul8SsnNYFE,11174
-pip/_vendor/pygments/lexers/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/pygments/lexers/__pycache__/_mapping.cpython-37.pyc,,
-pip/_vendor/pygments/lexers/__pycache__/python.cpython-37.pyc,,
+pip/_vendor/pygments/lexers/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/pygments/lexers/__pycache__/_mapping.cpython-38.pyc,,
+pip/_vendor/pygments/lexers/__pycache__/python.cpython-38.pyc,,
 pip/_vendor/pygments/lexers/_mapping.py,sha256=zEiCV5FPiBioMJQJjw9kk7IJ5Y9GwknS4VJPYlcNchs,70232
 pip/_vendor/pygments/lexers/python.py,sha256=gZROs9iNSOA18YyVghP1cUCD0OwYZ04a6PCwgSOCeSA,53376
 pip/_vendor/pygments/modeline.py,sha256=gIbMSYrjSWPk0oATz7W9vMBYkUyTK2OcdVyKjioDRvA,986
 pip/_vendor/pygments/plugin.py,sha256=5rPxEoB_89qQMpOs0nI4KyLOzAHNlbQiwEMOKxqNmv8,2591
 pip/_vendor/pygments/regexopt.py,sha256=c6xcXGpGgvCET_3VWawJJqAnOp0QttFpQEdOPNY2Py0,3072
 pip/_vendor/pygments/scanner.py,sha256=F2T2G6cpkj-yZtzGQr-sOBw5w5-96UrJWveZN6va2aM,3092
 pip/_vendor/pygments/sphinxext.py,sha256=F8L0211sPnXaiWutN0lkSUajWBwlgDMIEFFAbMWOvZY,4630
 pip/_vendor/pygments/style.py,sha256=RRnussX1YiK9Z7HipIvKorImxu3-HnkdpPCO4u925T0,6257
 pip/_vendor/pygments/styles/__init__.py,sha256=iZDZ7PBKb55SpGlE1--cx9cbmWx5lVTH4bXO87t2Vok,3419
-pip/_vendor/pygments/styles/__pycache__/__init__.cpython-37.pyc,,
+pip/_vendor/pygments/styles/__pycache__/__init__.cpython-38.pyc,,
 pip/_vendor/pygments/token.py,sha256=vA2yNHGJBHfq4jNQSah7C9DmIOp34MmYHPA8P-cYAHI,6184
 pip/_vendor/pygments/unistring.py,sha256=gP3gK-6C4oAFjjo9HvoahsqzuV4Qz0jl0E0OxfDerHI,63187
 pip/_vendor/pygments/util.py,sha256=KgwpWWC3By5AiNwxGTI7oI9aXupH2TyZWukafBJe0Mg,9110
 pip/_vendor/pyparsing/__init__.py,sha256=ZPdI7pPo4IYXcABw-51AcqOzsxVvDtqnQbyn_qYWZvo,9171
-pip/_vendor/pyparsing/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/actions.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/common.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/core.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/exceptions.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/helpers.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/results.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/testing.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/unicode.cpython-37.pyc,,
-pip/_vendor/pyparsing/__pycache__/util.cpython-37.pyc,,
+pip/_vendor/pyparsing/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/actions.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/common.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/core.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/exceptions.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/helpers.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/results.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/testing.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/unicode.cpython-38.pyc,,
+pip/_vendor/pyparsing/__pycache__/util.cpython-38.pyc,,
 pip/_vendor/pyparsing/actions.py,sha256=wU9i32e0y1ymxKE3OUwSHO-SFIrt1h_wv6Ws0GQjpNU,6426
 pip/_vendor/pyparsing/common.py,sha256=lFL97ooIeR75CmW5hjURZqwDCTgruqltcTCZ-ulLO2Q,12936
 pip/_vendor/pyparsing/core.py,sha256=AzTm1KFT1FIhiw2zvXZJmrpQoAwB0wOmeDCiR6SYytw,213344
 pip/_vendor/pyparsing/diagram/__init__.py,sha256=KW0PV_TvWKnL7jysz0pQbZ24nzWWu2ZfNaeyUIIywIg,23685
-pip/_vendor/pyparsing/diagram/__pycache__/__init__.cpython-37.pyc,,
+pip/_vendor/pyparsing/diagram/__pycache__/__init__.cpython-38.pyc,,
 pip/_vendor/pyparsing/exceptions.py,sha256=3LbSafD32NYb1Tzt85GHNkhEAU1eZkTtNSk24cPMemo,9023
 pip/_vendor/pyparsing/helpers.py,sha256=QpUOjW0-psvueMwWb9bQpU2noqKCv98_wnw1VSzSdVo,39129
 pip/_vendor/pyparsing/results.py,sha256=HgNvWVXBdQP-Q6PtJfoCEeOJk2nwEvG-2KVKC5sGA30,25341
 pip/_vendor/pyparsing/testing.py,sha256=7tu4Abp4uSeJV0N_yEPRmmNUhpd18ZQP3CrX41DM814,13402
 pip/_vendor/pyparsing/unicode.py,sha256=fwuhMj30SQ165Cv7HJpu-rSxGbRm93kN9L4Ei7VGc1Y,10787
 pip/_vendor/pyparsing/util.py,sha256=kq772O5YSeXOSdP-M31EWpbH_ayj7BMHImBYo9xPD5M,6805
 pip/_vendor/pyproject_hooks/__init__.py,sha256=kCehmy0UaBa9oVMD7ZIZrnswfnP3LXZ5lvnNJAL5JBM,491
-pip/_vendor/pyproject_hooks/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/pyproject_hooks/__pycache__/_compat.cpython-37.pyc,,
-pip/_vendor/pyproject_hooks/__pycache__/_impl.cpython-37.pyc,,
+pip/_vendor/pyproject_hooks/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/pyproject_hooks/__pycache__/_compat.cpython-38.pyc,,
+pip/_vendor/pyproject_hooks/__pycache__/_impl.cpython-38.pyc,,
 pip/_vendor/pyproject_hooks/_compat.py,sha256=by6evrYnqkisiM-MQcvOKs5bgDMzlOSgZqRHNqf04zE,138
 pip/_vendor/pyproject_hooks/_impl.py,sha256=61GJxzQip0IInhuO69ZI5GbNQ82XEDUB_1Gg5_KtUoc,11920
 pip/_vendor/pyproject_hooks/_in_process/__init__.py,sha256=9gQATptbFkelkIy0OfWFEACzqxXJMQDWCH9rBOAZVwQ,546
-pip/_vendor/pyproject_hooks/_in_process/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/pyproject_hooks/_in_process/__pycache__/_in_process.cpython-37.pyc,,
+pip/_vendor/pyproject_hooks/_in_process/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/pyproject_hooks/_in_process/__pycache__/_in_process.cpython-38.pyc,,
 pip/_vendor/pyproject_hooks/_in_process/_in_process.py,sha256=m2b34c917IW5o-Q_6TYIHlsK9lSUlNiyrITTUH_zwew,10927
 pip/_vendor/requests/__init__.py,sha256=64HgJ8cke-XyNrj1ErwNq0F9SqyAThUTh5lV6m7-YkI,5178
-pip/_vendor/requests/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/__version__.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/_internal_utils.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/adapters.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/api.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/auth.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/certs.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/compat.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/cookies.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/exceptions.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/help.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/hooks.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/models.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/packages.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/sessions.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/status_codes.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/structures.cpython-37.pyc,,
-pip/_vendor/requests/__pycache__/utils.cpython-37.pyc,,
+pip/_vendor/requests/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/__version__.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/_internal_utils.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/adapters.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/api.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/auth.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/certs.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/compat.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/cookies.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/exceptions.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/help.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/hooks.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/models.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/packages.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/sessions.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/status_codes.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/structures.cpython-38.pyc,,
+pip/_vendor/requests/__pycache__/utils.cpython-38.pyc,,
 pip/_vendor/requests/__version__.py,sha256=h48zn-oFukaXrYHocdadp_hIszWyd_PGrS8Eiii6aoc,435
 pip/_vendor/requests/_internal_utils.py,sha256=aSPlF4uDhtfKxEayZJJ7KkAxtormeTfpwKSBSwtmAUw,1397
 pip/_vendor/requests/adapters.py,sha256=GFEz5koZaMZD86v0SHXKVB5SE9MgslEjkCQzldkNwVM,21443
 pip/_vendor/requests/api.py,sha256=dyvkDd5itC9z2g0wHl_YfD1yf6YwpGWLO7__8e21nks,6377
 pip/_vendor/requests/auth.py,sha256=h-HLlVx9j8rKV5hfSAycP2ApOSglTz77R0tz7qCbbEE,10187
 pip/_vendor/requests/certs.py,sha256=PVPooB0jP5hkZEULSCwC074532UFbR2Ptgu0I5zwmCs,575
 pip/_vendor/requests/compat.py,sha256=IhK9quyX0RRuWTNcg6d2JGSAOUbM6mym2p_2XjLTwf4,1286
@@ -711,105 +711,105 @@
 pip/_vendor/requests/models.py,sha256=dDZ-iThotky-Noq9yy97cUEJhr3wnY6mv-xR_ePg_lk,35288
 pip/_vendor/requests/packages.py,sha256=njJmVifY4aSctuW3PP5EFRCxjEwMRDO6J_feG2dKWsI,695
 pip/_vendor/requests/sessions.py,sha256=KUqJcRRLovNefUs7ScOXSUVCcfSayTFWtbiJ7gOSlTI,30180
 pip/_vendor/requests/status_codes.py,sha256=FvHmT5uH-_uimtRz5hH9VCbt7VV-Nei2J9upbej6j8g,4235
 pip/_vendor/requests/structures.py,sha256=-IbmhVz06S-5aPSZuUthZ6-6D9XOjRuTXHOabY041XM,2912
 pip/_vendor/requests/utils.py,sha256=0gzSOcx9Ya4liAbHnHuwt4jM78lzCZZoDFgkmsInNUg,33240
 pip/_vendor/resolvelib/__init__.py,sha256=UL-B2BDI0_TRIqkfGwLHKLxY-LjBlomz7941wDqzB1I,537
-pip/_vendor/resolvelib/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/resolvelib/__pycache__/providers.cpython-37.pyc,,
-pip/_vendor/resolvelib/__pycache__/reporters.cpython-37.pyc,,
-pip/_vendor/resolvelib/__pycache__/resolvers.cpython-37.pyc,,
-pip/_vendor/resolvelib/__pycache__/structs.cpython-37.pyc,,
+pip/_vendor/resolvelib/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/resolvelib/__pycache__/providers.cpython-38.pyc,,
+pip/_vendor/resolvelib/__pycache__/reporters.cpython-38.pyc,,
+pip/_vendor/resolvelib/__pycache__/resolvers.cpython-38.pyc,,
+pip/_vendor/resolvelib/__pycache__/structs.cpython-38.pyc,,
 pip/_vendor/resolvelib/compat/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_vendor/resolvelib/compat/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/resolvelib/compat/__pycache__/collections_abc.cpython-37.pyc,,
+pip/_vendor/resolvelib/compat/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/resolvelib/compat/__pycache__/collections_abc.cpython-38.pyc,,
 pip/_vendor/resolvelib/compat/collections_abc.py,sha256=uy8xUZ-NDEw916tugUXm8HgwCGiMO0f-RcdnpkfXfOs,156
 pip/_vendor/resolvelib/providers.py,sha256=roVmFBItQJ0TkhNua65h8LdNny7rmeqVEXZu90QiP4o,5872
 pip/_vendor/resolvelib/reporters.py,sha256=fW91NKf-lK8XN7i6Yd_rczL5QeOT3sc6AKhpaTEnP3E,1583
 pip/_vendor/resolvelib/resolvers.py,sha256=2wYzVGBGerbmcIpH8cFmgSKgLSETz8jmwBMGjCBMHG4,17592
 pip/_vendor/resolvelib/structs.py,sha256=IVIYof6sA_N4ZEiE1C1UhzTX495brCNnyCdgq6CYq28,4794
 pip/_vendor/rich/__init__.py,sha256=dRxjIL-SbFVY0q3IjSMrfgBTHrm1LZDgLOygVBwiYZc,6090
 pip/_vendor/rich/__main__.py,sha256=TT8sb9PTnsnKhhrGuHkLN0jdN0dtKhtPkEr9CidDbPM,8478
-pip/_vendor/rich/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/__main__.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_cell_widths.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_emoji_codes.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_emoji_replace.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_export_format.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_extension.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_inspect.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_log_render.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_loop.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_null_file.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_palettes.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_pick.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_ratio.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_spinners.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_stack.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_timer.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_win32_console.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_windows.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_windows_renderer.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/_wrap.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/abc.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/align.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/ansi.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/bar.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/box.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/cells.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/color.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/color_triplet.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/columns.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/console.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/constrain.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/containers.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/control.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/default_styles.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/diagnose.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/emoji.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/errors.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/file_proxy.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/filesize.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/highlighter.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/json.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/jupyter.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/layout.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/live.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/live_render.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/logging.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/markup.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/measure.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/padding.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/pager.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/palette.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/panel.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/pretty.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/progress.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/progress_bar.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/prompt.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/protocol.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/region.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/repr.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/rule.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/scope.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/screen.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/segment.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/spinner.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/status.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/style.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/styled.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/syntax.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/table.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/terminal_theme.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/text.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/theme.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/themes.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/traceback.cpython-37.pyc,,
-pip/_vendor/rich/__pycache__/tree.cpython-37.pyc,,
+pip/_vendor/rich/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/__main__.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_cell_widths.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_emoji_codes.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_emoji_replace.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_export_format.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_extension.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_inspect.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_log_render.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_loop.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_null_file.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_palettes.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_pick.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_ratio.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_spinners.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_stack.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_timer.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_win32_console.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_windows.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_windows_renderer.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/_wrap.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/abc.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/align.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/ansi.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/bar.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/box.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/cells.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/color.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/color_triplet.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/columns.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/console.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/constrain.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/containers.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/control.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/default_styles.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/diagnose.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/emoji.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/errors.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/file_proxy.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/filesize.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/highlighter.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/json.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/jupyter.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/layout.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/live.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/live_render.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/logging.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/markup.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/measure.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/padding.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/pager.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/palette.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/panel.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/pretty.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/progress.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/progress_bar.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/prompt.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/protocol.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/region.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/repr.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/rule.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/scope.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/screen.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/segment.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/spinner.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/status.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/style.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/styled.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/syntax.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/table.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/terminal_theme.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/text.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/theme.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/themes.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/traceback.cpython-38.pyc,,
+pip/_vendor/rich/__pycache__/tree.cpython-38.pyc,,
 pip/_vendor/rich/_cell_widths.py,sha256=2n4EiJi3X9sqIq0O16kUZ_zy6UYMd3xFfChlKfnW1Hc,10096
 pip/_vendor/rich/_emoji_codes.py,sha256=hu1VL9nbVdppJrVoijVshRlcRRe_v3dju3Mmd2sKZdY,140235
 pip/_vendor/rich/_emoji_replace.py,sha256=n-kcetsEUx2ZUmhQrfeMNc-teeGhpuSQ5F8VPBsyvDo,1064
 pip/_vendor/rich/_export_format.py,sha256=nHArqOljIlYn6NruhWsAsh-fHo7oJC3y9BDJyAa-QYQ,2114
 pip/_vendor/rich/_extension.py,sha256=Xt47QacCKwYruzjDi-gOBq724JReDj9Cm9xUi5fr-34,265
 pip/_vendor/rich/_inspect.py,sha256=oZJGw31e64dwXSCmrDnvZbwVb1ZKhWfU8wI3VWohjJk,9695
 pip/_vendor/rich/_log_render.py,sha256=1ByI0PA1ZpxZY3CGJOK54hjlq4X-Bz_boIjIqCd8Kns,3225
@@ -878,125 +878,125 @@
 pip/_vendor/rich/text.py,sha256=andXaxWW_wBveMiZZpd5viQwucWo7SPopcM3ZCQeO0c,45686
 pip/_vendor/rich/theme.py,sha256=GKNtQhDBZKAzDaY0vQVQQFzbc0uWfFe6CJXA-syT7zQ,3627
 pip/_vendor/rich/themes.py,sha256=0xgTLozfabebYtcJtDdC5QkX5IVUEaviqDUJJh4YVFk,102
 pip/_vendor/rich/traceback.py,sha256=6LkGguCEAxKv8v8xmKfMeYPPJ1UXUEHDv4726To6FiQ,26070
 pip/_vendor/rich/tree.py,sha256=BMbUYNjS9uodNPfvtY_odmU09GA5QzcMbQ5cJZhllQI,9169
 pip/_vendor/six.py,sha256=TOOfQi7nFGfMrIvtdr6wX4wyHH8M7aknmuLfo2cBBrM,34549
 pip/_vendor/tenacity/__init__.py,sha256=rjcWJVq5PcNJNC42rt-TAGGskM-RUEkZbDKu1ra7IPo,18364
-pip/_vendor/tenacity/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/_asyncio.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/_utils.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/after.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/before.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/before_sleep.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/nap.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/retry.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/stop.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/tornadoweb.cpython-37.pyc,,
-pip/_vendor/tenacity/__pycache__/wait.cpython-37.pyc,,
+pip/_vendor/tenacity/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/_asyncio.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/_utils.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/after.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/before.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/before_sleep.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/nap.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/retry.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/stop.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/tornadoweb.cpython-38.pyc,,
+pip/_vendor/tenacity/__pycache__/wait.cpython-38.pyc,,
 pip/_vendor/tenacity/_asyncio.py,sha256=HEb0BVJEeBJE9P-m9XBxh1KcaF96BwoeqkJCL5sbVcQ,3314
 pip/_vendor/tenacity/_utils.py,sha256=-y68scDcyoqvTJuJJ0GTfjdSCljEYlbCYvgk7nM4NdM,1944
 pip/_vendor/tenacity/after.py,sha256=dlmyxxFy2uqpLXDr838DiEd7jgv2AGthsWHGYcGYsaI,1496
 pip/_vendor/tenacity/before.py,sha256=7XtvRmO0dRWUp8SVn24OvIiGFj8-4OP5muQRUiWgLh0,1376
 pip/_vendor/tenacity/before_sleep.py,sha256=ThyDvqKU5yle_IvYQz_b6Tp6UjUS0PhVp6zgqYl9U6Y,1908
 pip/_vendor/tenacity/nap.py,sha256=fRWvnz1aIzbIq9Ap3gAkAZgDH6oo5zxMrU6ZOVByq0I,1383
 pip/_vendor/tenacity/retry.py,sha256=Cy504Ss3UrRV7lnYgvymF66WD1wJ2dbM869kDcjuDes,7550
 pip/_vendor/tenacity/stop.py,sha256=sKHmHaoSaW6sKu3dTxUVKr1-stVkY7lw4Y9yjZU30zQ,2790
 pip/_vendor/tenacity/tornadoweb.py,sha256=E8lWO2nwe6dJgoB-N2HhQprYLDLB_UdSgFnv-EN6wKE,2145
 pip/_vendor/tenacity/wait.py,sha256=tdLTESRm5E237VHG0SxCDXRa0DHKPKVq285kslHVURc,8011
 pip/_vendor/tomli/__init__.py,sha256=JhUwV66DB1g4Hvt1UQCVMdfCu-IgAV8FXmvDU9onxd4,396
-pip/_vendor/tomli/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/tomli/__pycache__/_parser.cpython-37.pyc,,
-pip/_vendor/tomli/__pycache__/_re.cpython-37.pyc,,
-pip/_vendor/tomli/__pycache__/_types.cpython-37.pyc,,
+pip/_vendor/tomli/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/tomli/__pycache__/_parser.cpython-38.pyc,,
+pip/_vendor/tomli/__pycache__/_re.cpython-38.pyc,,
+pip/_vendor/tomli/__pycache__/_types.cpython-38.pyc,,
 pip/_vendor/tomli/_parser.py,sha256=g9-ENaALS-B8dokYpCuzUFalWlog7T-SIYMjLZSWrtM,22633
 pip/_vendor/tomli/_re.py,sha256=dbjg5ChZT23Ka9z9DHOXfdtSpPwUfdgMXnj8NOoly-w,2943
 pip/_vendor/tomli/_types.py,sha256=-GTG2VUqkpxwMqzmVO4F7ybKddIbAnuAHXfmWQcTi3Q,254
 pip/_vendor/typing_extensions.py,sha256=VKZ_nHsuzDbKOVUY2CTdavwBgfZ2EXRyluZHRzUYAbg,80114
 pip/_vendor/urllib3/__init__.py,sha256=iXLcYiJySn0GNbWOOZDDApgBL1JgP44EZ8i1760S8Mc,3333
-pip/_vendor/urllib3/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/_collections.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/_version.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/connection.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/connectionpool.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/exceptions.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/fields.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/filepost.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/poolmanager.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/request.cpython-37.pyc,,
-pip/_vendor/urllib3/__pycache__/response.cpython-37.pyc,,
+pip/_vendor/urllib3/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/_collections.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/_version.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/connection.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/connectionpool.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/exceptions.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/fields.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/filepost.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/poolmanager.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/request.cpython-38.pyc,,
+pip/_vendor/urllib3/__pycache__/response.cpython-38.pyc,,
 pip/_vendor/urllib3/_collections.py,sha256=Rp1mVyBgc_UlAcp6M3at1skJBXR5J43NawRTvW2g_XY,10811
 pip/_vendor/urllib3/_version.py,sha256=JWE--BUVy7--9FsXILONIpQ43irftKGjT9j2H_fdF2M,64
 pip/_vendor/urllib3/connection.py,sha256=8976wL6sGeVMW0JnXvx5mD00yXu87uQjxtB9_VL8dx8,20070
 pip/_vendor/urllib3/connectionpool.py,sha256=vS4UaHLoR9_5aGLXSQ776y_jTxgqqjx0YsjkYksWGOo,39095
 pip/_vendor/urllib3/contrib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_vendor/urllib3/contrib/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/urllib3/contrib/__pycache__/_appengine_environ.cpython-37.pyc,,
-pip/_vendor/urllib3/contrib/__pycache__/appengine.cpython-37.pyc,,
-pip/_vendor/urllib3/contrib/__pycache__/ntlmpool.cpython-37.pyc,,
-pip/_vendor/urllib3/contrib/__pycache__/pyopenssl.cpython-37.pyc,,
-pip/_vendor/urllib3/contrib/__pycache__/securetransport.cpython-37.pyc,,
-pip/_vendor/urllib3/contrib/__pycache__/socks.cpython-37.pyc,,
+pip/_vendor/urllib3/contrib/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/urllib3/contrib/__pycache__/_appengine_environ.cpython-38.pyc,,
+pip/_vendor/urllib3/contrib/__pycache__/appengine.cpython-38.pyc,,
+pip/_vendor/urllib3/contrib/__pycache__/ntlmpool.cpython-38.pyc,,
+pip/_vendor/urllib3/contrib/__pycache__/pyopenssl.cpython-38.pyc,,
+pip/_vendor/urllib3/contrib/__pycache__/securetransport.cpython-38.pyc,,
+pip/_vendor/urllib3/contrib/__pycache__/socks.cpython-38.pyc,,
 pip/_vendor/urllib3/contrib/_appengine_environ.py,sha256=bDbyOEhW2CKLJcQqAKAyrEHN-aklsyHFKq6vF8ZFsmk,957
 pip/_vendor/urllib3/contrib/_securetransport/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_vendor/urllib3/contrib/_securetransport/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/urllib3/contrib/_securetransport/__pycache__/bindings.cpython-37.pyc,,
-pip/_vendor/urllib3/contrib/_securetransport/__pycache__/low_level.cpython-37.pyc,,
+pip/_vendor/urllib3/contrib/_securetransport/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/urllib3/contrib/_securetransport/__pycache__/bindings.cpython-38.pyc,,
+pip/_vendor/urllib3/contrib/_securetransport/__pycache__/low_level.cpython-38.pyc,,
 pip/_vendor/urllib3/contrib/_securetransport/bindings.py,sha256=4Xk64qIkPBt09A5q-RIFUuDhNc9mXilVapm7WnYnzRw,17632
 pip/_vendor/urllib3/contrib/_securetransport/low_level.py,sha256=B2JBB2_NRP02xK6DCa1Pa9IuxrPwxzDzZbixQkb7U9M,13922
 pip/_vendor/urllib3/contrib/appengine.py,sha256=VR68eAVE137lxTgjBDwCna5UiBZTOKa01Aj_-5BaCz4,11036
 pip/_vendor/urllib3/contrib/ntlmpool.py,sha256=NlfkW7WMdW8ziqudopjHoW299og1BTWi0IeIibquFwk,4528
 pip/_vendor/urllib3/contrib/pyopenssl.py,sha256=hDJh4MhyY_p-oKlFcYcQaVQRDv6GMmBGuW9yjxyeejM,17081
 pip/_vendor/urllib3/contrib/securetransport.py,sha256=yhZdmVjY6PI6EeFbp7qYOp6-vp1Rkv2NMuOGaEj7pmc,34448
 pip/_vendor/urllib3/contrib/socks.py,sha256=aRi9eWXo9ZEb95XUxef4Z21CFlnnjbEiAo9HOseoMt4,7097
 pip/_vendor/urllib3/exceptions.py,sha256=0Mnno3KHTNfXRfY7638NufOPkUb6mXOm-Lqj-4x2w8A,8217
 pip/_vendor/urllib3/fields.py,sha256=kvLDCg_JmH1lLjUUEY_FLS8UhY7hBvDPuVETbY8mdrM,8579
 pip/_vendor/urllib3/filepost.py,sha256=5b_qqgRHVlL7uLtdAYBzBh-GHmU5AfJVt_2N0XS3PeY,2440
 pip/_vendor/urllib3/packages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_vendor/urllib3/packages/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/urllib3/packages/__pycache__/six.cpython-37.pyc,,
+pip/_vendor/urllib3/packages/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/urllib3/packages/__pycache__/six.cpython-38.pyc,,
 pip/_vendor/urllib3/packages/backports/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pip/_vendor/urllib3/packages/backports/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/urllib3/packages/backports/__pycache__/makefile.cpython-37.pyc,,
+pip/_vendor/urllib3/packages/backports/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/urllib3/packages/backports/__pycache__/makefile.cpython-38.pyc,,
 pip/_vendor/urllib3/packages/backports/makefile.py,sha256=nbzt3i0agPVP07jqqgjhaYjMmuAi_W5E0EywZivVO8E,1417
 pip/_vendor/urllib3/packages/six.py,sha256=b9LM0wBXv7E7SrbCjAm4wwN-hrH-iNxv18LgWNMMKPo,34665
 pip/_vendor/urllib3/poolmanager.py,sha256=0KOOJECoeLYVjUHvv-0h4Oq3FFQQ2yb-Fnjkbj8gJO0,19786
 pip/_vendor/urllib3/request.py,sha256=ZFSIqX0C6WizixecChZ3_okyu7BEv0lZu1VT0s6h4SM,5985
 pip/_vendor/urllib3/response.py,sha256=fmDJAFkG71uFTn-sVSTh2Iw0WmcXQYqkbRjihvwBjU8,30641
 pip/_vendor/urllib3/util/__init__.py,sha256=JEmSmmqqLyaw8P51gUImZh8Gwg9i1zSe-DoqAitn2nc,1155
-pip/_vendor/urllib3/util/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/connection.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/proxy.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/queue.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/request.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/response.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/retry.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/ssl_.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/ssl_match_hostname.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/ssltransport.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/timeout.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/url.cpython-37.pyc,,
-pip/_vendor/urllib3/util/__pycache__/wait.cpython-37.pyc,,
+pip/_vendor/urllib3/util/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/connection.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/proxy.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/queue.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/request.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/response.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/retry.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/ssl_.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/ssl_match_hostname.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/ssltransport.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/timeout.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/url.cpython-38.pyc,,
+pip/_vendor/urllib3/util/__pycache__/wait.cpython-38.pyc,,
 pip/_vendor/urllib3/util/connection.py,sha256=5Lx2B1PW29KxBn2T0xkN1CBgRBa3gGVJBKoQoRogEVk,4901
 pip/_vendor/urllib3/util/proxy.py,sha256=zUvPPCJrp6dOF0N4GAVbOcl6o-4uXKSrGiTkkr5vUS4,1605
 pip/_vendor/urllib3/util/queue.py,sha256=nRgX8_eX-_VkvxoX096QWoz8Ps0QHUAExILCY_7PncM,498
 pip/_vendor/urllib3/util/request.py,sha256=C0OUt2tcU6LRiQJ7YYNP9GvPrSvl7ziIBekQ-5nlBZk,3997
 pip/_vendor/urllib3/util/response.py,sha256=GJpg3Egi9qaJXRwBh5wv-MNuRWan5BIu40oReoxWP28,3510
 pip/_vendor/urllib3/util/retry.py,sha256=4laWh0HpwGijLiBmdBIYtbhYekQnNzzhx2W9uys0RHA,22003
 pip/_vendor/urllib3/util/ssl_.py,sha256=X4-AqW91aYPhPx6-xbf66yHFQKbqqfC_5Zt4WkLX1Hc,17177
 pip/_vendor/urllib3/util/ssl_match_hostname.py,sha256=Ir4cZVEjmAk8gUAIHWSi7wtOO83UCYABY2xFD1Ql_WA,5758
 pip/_vendor/urllib3/util/ssltransport.py,sha256=NA-u5rMTrDFDFC8QzRKUEKMG0561hOD4qBTr3Z4pv6E,6895
 pip/_vendor/urllib3/util/timeout.py,sha256=QSbBUNOB9yh6AnDn61SrLQ0hg5oz0I9-uXEG91AJuIg,10003
 pip/_vendor/urllib3/util/url.py,sha256=HLCLEKt8D-QMioTNbneZSzGTGyUkns4w_lSJP1UzE2E,14298
 pip/_vendor/urllib3/util/wait.py,sha256=fOX0_faozG2P7iVojQoE1mbydweNyTcm-hXEfFrTtLI,5403
 pip/_vendor/vendor.txt,sha256=3i3Zr7_kRDD9UEva0I8YOMroCZ8xuZ9OWd_Q4jmazqE,476
 pip/_vendor/webencodings/__init__.py,sha256=qOBJIuPy_4ByYH6W_bNgJF-qYQ2DoU-dKsDu5yRWCXg,10579
-pip/_vendor/webencodings/__pycache__/__init__.cpython-37.pyc,,
-pip/_vendor/webencodings/__pycache__/labels.cpython-37.pyc,,
-pip/_vendor/webencodings/__pycache__/mklabels.cpython-37.pyc,,
-pip/_vendor/webencodings/__pycache__/tests.cpython-37.pyc,,
-pip/_vendor/webencodings/__pycache__/x_user_defined.cpython-37.pyc,,
+pip/_vendor/webencodings/__pycache__/__init__.cpython-38.pyc,,
+pip/_vendor/webencodings/__pycache__/labels.cpython-38.pyc,,
+pip/_vendor/webencodings/__pycache__/mklabels.cpython-38.pyc,,
+pip/_vendor/webencodings/__pycache__/tests.cpython-38.pyc,,
+pip/_vendor/webencodings/__pycache__/x_user_defined.cpython-38.pyc,,
 pip/_vendor/webencodings/labels.py,sha256=4AO_KxTddqGtrL9ns7kAPjb0CcN6xsCIxbK37HY9r3E,8979
 pip/_vendor/webencodings/mklabels.py,sha256=GYIeywnpaLnP0GSic8LFWgd0UVvO_l1Nc6YoF-87R_4,1305
 pip/_vendor/webencodings/tests.py,sha256=OtGLyjhNY1fvkW1GvLJ_FV9ZoqC9Anyjr7q3kxTbzNs,6563
 pip/_vendor/webencodings/x_user_defined.py,sha256=yOqWSdmpytGfUgh_Z6JYgDNhoc-BAHyyeeT15Fr42tM,4307
 pip/py.typed,sha256=EBVvvPRTn_eIpz5e5QztSCdrMX7Qwd7VP93RSoIlZ2I,286
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 """
 Package resource API
 --------------------
 
 A resource is a logical file contained within a package, or a logical
 subdirectory thereof.  The package resource API expects resource names
 to have their path parts separated with ``/``, *not* whatever the local
@@ -11,16 +10,14 @@
 
 The package resource API is designed to work with normal filesystem packages,
 .egg files, and unpacked .egg files.  It can also work in a limited way with
 .zip files and with custom PEP 302 loaders that support the ``get_data()``
 method.
 """
 
-from __future__ import absolute_import
-
 import sys
 import os
 import io
 import time
 import re
 import types
 import zipfile
@@ -37,30 +34,28 @@
 import errno
 import tempfile
 import textwrap
 import itertools
 import inspect
 import ntpath
 import posixpath
+import importlib
 from pkgutil import get_importer
 
 try:
     import _imp
 except ImportError:
     # Python 3.2 compatibility
     import imp as _imp
 
 try:
     FileExistsError
 except NameError:
     FileExistsError = OSError
 
-from pkg_resources.extern import six
-from pkg_resources.extern.six.moves import map, filter
-
 # capture these to bypass sandboxing
 from os import utime
 try:
     from os import mkdir, rename, unlink
     WRITE_SUPPORT = True
 except ImportError:
     # no write support, probably under GAE
@@ -72,35 +67,24 @@
 try:
     import importlib.machinery as importlib_machinery
     # access attribute to force import under delayed import mechanisms.
     importlib_machinery.__name__
 except ImportError:
     importlib_machinery = None
 
-from . import py31compat
 from pkg_resources.extern import appdirs
 from pkg_resources.extern import packaging
 __import__('pkg_resources.extern.packaging.version')
 __import__('pkg_resources.extern.packaging.specifiers')
 __import__('pkg_resources.extern.packaging.requirements')
 __import__('pkg_resources.extern.packaging.markers')
-__import__('pkg_resources.py2_warn')
-
 
-__metaclass__ = type
-
-
-if (3, 0) < sys.version_info < (3, 5):
+if sys.version_info < (3, 5):
     raise RuntimeError("Python 3.5 or later is required")
 
-if six.PY2:
-    # Those builtin exceptions are only defined in Python 3
-    PermissionError = None
-    NotADirectoryError = None
-
 # declare some globals that will be defined later to
 # satisfy the linters.
 require = None
 working_set = None
 add_activation_listener = None
 resources_stream = None
 cleanup_resources = None
@@ -472,15 +456,15 @@
 
 # backward compatibility
 run_main = run_script
 
 
 def get_distribution(dist):
     """Return a current distribution object for a Requirement or string"""
-    if isinstance(dist, six.string_types):
+    if isinstance(dist, str):
         dist = Requirement.parse(dist)
     if isinstance(dist, Requirement):
         dist = get_provider(dist)
     if not isinstance(dist, Distribution):
         raise TypeError("Expected string, Requirement, or Distribution", dist)
     return dist
 
@@ -709,15 +693,16 @@
         self.by_key[dist.key] = dist
         if dist.key not in keys:
             keys.append(dist.key)
         if dist.key not in keys2:
             keys2.append(dist.key)
         self._added_new(dist)
 
-    def resolve(self, requirements, env=None, installer=None,
+    # FIXME: 'WorkingSet.resolve' is too complex (11)
+    def resolve(self, requirements, env=None, installer=None,  # noqa: C901
                 replace_conflicting=False, extras=None):
         """List all distributions needed to (recursively) meet `requirements`
 
         `requirements` must be a sequence of ``Requirement`` objects.  `env`,
         if supplied, should be an ``Environment`` instance.  If
         not supplied, it defaults to all distributions available within any
         entry or distribution in the working set.  `installer`, if supplied,
@@ -1375,15 +1360,15 @@
 
     This implementation uses the 'pyparsing' module.
     """
     try:
         marker = packaging.markers.Marker(text)
         return marker.evaluate()
     except packaging.markers.InvalidMarker as e:
-        raise SyntaxError(e)
+        raise SyntaxError(e) from e
 
 
 class NullProvider:
     """Try to implement resources and metadata for arbitrary PEP 302 loaders"""
 
     egg_name = None
     egg_info = None
@@ -1416,16 +1401,14 @@
         return self._has(path)
 
     def get_metadata(self, name):
         if not self.egg_info:
             return ""
         path = self._get_metadata_path(name)
         value = self._get(path)
-        if six.PY2:
-            return value
         try:
             return value.decode('utf-8')
         except UnicodeDecodeError as exc:
             # Include the path in the error message to simplify
             # troubleshooting, and without changing the exception type.
             exc.reason += ' in {} file at path: {}'.format(name, path)
             raise
@@ -1455,15 +1438,16 @@
                 .format(**locals()),
             )
         script_text = self.get_metadata(script).replace('\r\n', '\n')
         script_text = script_text.replace('\r', '\n')
         script_filename = self._fn(self.egg_info, script)
         namespace['__file__'] = script_filename
         if os.path.exists(script_filename):
-            source = open(script_filename).read()
+            with open(script_filename) as fid:
+                source = fid.read()
             code = compile(source, script_filename, 'exec')
             exec(code, namespace, namespace)
         else:
             from linecache import cache
             cache[script_filename] = (
                 len(script_text), 0, script_text.split('\n'), script_filename
             )
@@ -1759,15 +1743,16 @@
         size = zip_stat.file_size
         # ymdhms+wday, yday, dst
         date_time = zip_stat.date_time + (0, 0, -1)
         # 1980 offset already done
         timestamp = time.mktime(date_time)
         return timestamp, size
 
-    def _extract_resource(self, manager, zip_path):
+    # FIXME: 'ZipProvider._extract_resource' is too complex (12)
+    def _extract_resource(self, manager, zip_path):  # noqa: C901
 
         if zip_path in self._index():
             for name in self._index()[zip_path]:
                 last = self._extract_resource(
                     manager, os.path.join(zip_path, name)
                 )
             # return the extracted directory name
@@ -1907,16 +1892,15 @@
 
         with io.open(self.path, encoding='utf-8', errors="replace") as f:
             metadata = f.read()
         self._warn_on_replacement(metadata)
         return metadata
 
     def _warn_on_replacement(self, metadata):
-        # Python 2.7 compat for: replacement_char = '�'
-        replacement_char = b'\xef\xbf\xbd'.decode('utf-8')
+        replacement_char = '�'
         if replacement_char in metadata:
             tmpl = "{self.path} could not be properly decoded in UTF-8"
             msg = tmpl.format(**locals())
             warnings.warn(msg)
 
     def get_metadata_lines(self, name):
         return yield_lines(self.get_metadata(name))
@@ -1998,15 +1982,15 @@
         return
     for subitem in metadata.resource_listdir(''):
         if _is_egg_path(subitem):
             subpath = os.path.join(path_item, subitem)
             dists = find_eggs_in_zip(zipimport.zipimporter(subpath), subpath)
             for dist in dists:
                 yield dist
-        elif subitem.lower().endswith('.dist-info'):
+        elif subitem.lower().endswith(('.dist-info', '.egg-info')):
             subpath = os.path.join(path_item, subitem)
             submeta = EggMetadata(zipimport.zipimporter(subpath))
             submeta.egg_info = subpath
             yield Distribution.from_location(path_item, subitem, submeta)
 
 
 register_finder(zipimport.zipimporter, find_eggs_in_zip)
@@ -2053,15 +2037,18 @@
         yield Distribution.from_filename(
             path_item, metadata=PathMetadata(
                 path_item, os.path.join(path_item, 'EGG-INFO')
             )
         )
         return
 
-    entries = safe_listdir(path_item)
+    entries = (
+        os.path.join(path_item, child)
+        for child in safe_listdir(path_item)
+    )
 
     # for performance, before sorting by version,
     # screen entries for only those that will yield
     # distributions
     filtered = (
         entry
         for entry in entries
@@ -2103,16 +2090,14 @@
     False
 
     >>> list(NoDists()('anything'))
     []
     """
     def __bool__(self):
         return False
-    if six.PY2:
-        __nonzero__ = __bool__
 
     def __call__(self, fullpath):
         return iter(())
 
 
 def safe_listdir(path):
     """
@@ -2121,20 +2106,15 @@
     try:
         return os.listdir(path)
     except (PermissionError, NotADirectoryError):
         pass
     except OSError as e:
         # Ignore the directory if does not exist, not a directory or
         # permission denied
-        ignorable = (
-            e.errno in (errno.ENOTDIR, errno.EACCES, errno.ENOENT)
-            # Python 2 on Windows needs to be handled this way :(
-            or getattr(e, "winerror", None) == 267
-        )
-        if not ignorable:
+        if e.errno not in (errno.ENOTDIR, errno.EACCES, errno.ENOENT):
             raise
     return ()
 
 
 def distributions_from_metadata(path):
     root = os.path.dirname(path)
     if os.path.isdir(path):
@@ -2228,15 +2208,15 @@
     elif not hasattr(module, '__path__'):
         raise TypeError("Not a package:", packageName)
     handler = _find_adapter(_namespace_handlers, importer)
     subpath = handler(importer, path_item, packageName, module)
     if subpath is not None:
         path = module.__path__
         path.append(subpath)
-        loader.load_module(packageName)
+        importlib.import_module(packageName)
         _rebuild_mod_path(path, packageName, module)
     return subpath
 
 
 def _rebuild_mod_path(orig_path, package_name, module):
     """
     Rebuild module.__path__ ensuring that all entries are ordered
@@ -2284,16 +2264,16 @@
 
         if parent:
             declare_namespace(parent)
             if parent not in _namespace_packages:
                 __import__(parent)
             try:
                 path = sys.modules[parent].__path__
-            except AttributeError:
-                raise TypeError("Not a package:", parent)
+            except AttributeError as e:
+                raise TypeError("Not a package:", parent) from e
 
         # Track what packages are namespaces, so when new path items are added,
         # they can be updated
         _namespace_packages.setdefault(parent or None, []).append(packageName)
         _namespace_packages.setdefault(packageName, [])
 
         for path_item in path:
@@ -2369,38 +2349,46 @@
         return result
 
 
 def _is_egg_path(path):
     """
     Determine if given path appears to be an egg.
     """
-    return path.lower().endswith('.egg')
+    return _is_zip_egg(path) or _is_unpacked_egg(path)
+
+
+def _is_zip_egg(path):
+    return (
+        path.lower().endswith('.egg') and
+        os.path.isfile(path) and
+        zipfile.is_zipfile(path)
+    )
 
 
 def _is_unpacked_egg(path):
     """
     Determine if given path appears to be an unpacked egg.
     """
     return (
-        _is_egg_path(path) and
+        path.lower().endswith('.egg') and
         os.path.isfile(os.path.join(path, 'EGG-INFO', 'PKG-INFO'))
     )
 
 
 def _set_parent_ns(packageName):
     parts = packageName.split('.')
     name = parts.pop()
     if parts:
         parent = '.'.join(parts)
         setattr(sys.modules[parent], name, sys.modules[packageName])
 
 
 def yield_lines(strs):
     """Yield non-empty/non-comment lines of a string or sequence"""
-    if isinstance(strs, six.string_types):
+    if isinstance(strs, str):
         for s in strs.splitlines():
             s = s.strip()
             # skip blank lines/comments
             if s and not s.startswith('#'):
                 yield s
     else:
         for ss in strs:
@@ -2465,15 +2453,15 @@
         """
         Resolve the entry point from its module and attrs.
         """
         module = __import__(self.module_name, fromlist=['__name__'], level=0)
         try:
             return functools.reduce(getattr, self.attrs, module)
         except AttributeError as exc:
-            raise ImportError(str(exc))
+            raise ImportError(str(exc)) from exc
 
     def require(self, env=None, installer=None):
         if self.extras and not self.dist:
             raise UnknownExtra("Can't require() without a distribution", self)
 
         # Get the requirements for this entry point with all its extras and
         # then resolve them. We have to pass `extras` along when resolving so
@@ -2685,22 +2673,22 @@
 
         warnings.warn(tmpl.format(**vars(self)), PEP440Warning)
 
     @property
     def version(self):
         try:
             return self._version
-        except AttributeError:
+        except AttributeError as e:
             version = self._get_version()
             if version is None:
                 path = self._get_metadata_path_for_display(self.PKG_INFO)
                 msg = (
                     "Missing 'Version:' header and/or {} file at path: {}"
                 ).format(self.PKG_INFO, path)
-                raise ValueError(msg, self)
+                raise ValueError(msg, self) from e
 
             return version
 
     @property
     def _dep_map(self):
         """
         A map of extra to its list of (direct) requirements
@@ -2745,18 +2733,18 @@
         """List of Requirements needed for this distro if `extras` are used"""
         dm = self._dep_map
         deps = []
         deps.extend(dm.get(None, ()))
         for ext in extras:
             try:
                 deps.extend(dm[safe_extra(ext)])
-            except KeyError:
+            except KeyError as e:
                 raise UnknownExtra(
                     "%s has no such extra feature %r" % (self, ext)
-                )
+                ) from e
         return deps
 
     def _get_metadata_path_for_display(self, name):
         """
         Return the path to the given metadata file, if available.
         """
         try:
@@ -2830,18 +2818,14 @@
             set(super(Distribution, self).__dir__())
             | set(
                 attr for attr in self._provider.__dir__()
                 if not attr.startswith('_')
             )
         )
 
-    if not hasattr(object, '__dir__'):
-        # python 2.7 not supported
-        del __dir__
-
     @classmethod
     def from_filename(cls, filename, metadata=None, **kw):
         return cls.from_location(
             _normalize_cached(filename), os.path.basename(filename), metadata,
             **kw
         )
 
@@ -2873,15 +2857,16 @@
             return ep_map.get(group, {})
         return ep_map
 
     def get_entry_info(self, group, name):
         """Return the EntryPoint object for `group`+`name`, or ``None``"""
         return self.get_entry_map(group).get(name)
 
-    def insert_on(self, path, loc=None, replace=False):
+    # FIXME: 'Distribution.insert_on' is too complex (13)
+    def insert_on(self, path, loc=None, replace=False):  # noqa: C901
         """Ensure self.location is on path
 
         If replace=False (default):
             - If location is already in path anywhere, do nothing.
             - Else:
               - If it's an egg and its parent directory is on path,
                 insert just ahead of the parent.
@@ -3073,19 +3058,14 @@
         while sys._getframe(level).f_globals is g:
             level += 1
     except ValueError:
         pass
     warnings.warn(stacklevel=level + 1, *args, **kw)
 
 
-class RequirementParseError(ValueError):
-    def __str__(self):
-        return ' '.join(self.args)
-
-
 def parse_requirements(strs):
     """Yield ``Requirement`` objects for each specification in `strs`
 
     `strs` must be a string, or a (possibly-nested) iterable thereof.
     """
     # create a steppable iterator, so we can handle \-continuations
     lines = iter(yield_lines(strs))
@@ -3100,21 +3080,22 @@
             try:
                 line += next(lines)
             except StopIteration:
                 return
         yield Requirement(line)
 
 
+class RequirementParseError(packaging.requirements.InvalidRequirement):
+    "Compatibility wrapper for InvalidRequirement"
+
+
 class Requirement(packaging.requirements.Requirement):
     def __init__(self, requirement_string):
         """DO NOT CALL THIS UNDOCUMENTED METHOD; use Requirement.parse()!"""
-        try:
-            super(Requirement, self).__init__(requirement_string)
-        except packaging.requirements.InvalidRequirement as e:
-            raise RequirementParseError(str(e))
+        super(Requirement, self).__init__(requirement_string)
         self.unsafe_name = self.name
         project_name = safe_name(self.name)
         self.project_name, self.key = project_name, project_name.lower()
         self.specs = [
             (spec.operator, spec.version) for spec in self.specifier]
         self.extras = tuple(map(safe_extra, self.extras))
         self.hashCmp = (
@@ -3176,15 +3157,15 @@
         if t in registry:
             return registry[t]
 
 
 def ensure_directory(path):
     """Ensure that the parent directory of `path` exists"""
     dirname = os.path.dirname(path)
-    py31compat.makedirs(dirname, exist_ok=True)
+    os.makedirs(dirname, exist_ok=True)
 
 
 def _bypass_ensure_directory(path):
     """Sandbox-bypassing version of ensure_directory()"""
     if not WRITE_SUPPORT:
         raise IOError('"os.mkdir" not supported on this platform.')
     dirname, filename = split(path)
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/appdirs.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 from __future__ import absolute_import, division, print_function
 
 __all__ = [
-    "__title__", "__summary__", "__uri__", "__version__", "__author__",
-    "__email__", "__license__", "__copyright__",
+    "__title__",
+    "__summary__",
+    "__uri__",
+    "__version__",
+    "__author__",
+    "__email__",
+    "__license__",
+    "__copyright__",
 ]
 
 __title__ = "packaging"
 __summary__ = "Core utilities for Python packages"
 __uri__ = "https://github.com/pypa/packaging"
 
-__version__ = "16.8"
+__version__ = "20.4"
 
 __author__ = "Donald Stufft and individual contributors"
 __email__ = "donald@stufft.io"
 
-__license__ = "BSD or Apache License, Version 2.0"
-__copyright__ = "Copyright 2014-2016 %s" % __author__
+__license__ = "BSD-2-Clause or Apache-2.0"
+__copyright__ = "Copyright 2014-2019 %s" % __author__
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 from __future__ import absolute_import, division, print_function
 
 from .__about__ import (
-    __author__, __copyright__, __email__, __license__, __summary__, __title__,
-    __uri__, __version__
+    __author__,
+    __copyright__,
+    __email__,
+    __license__,
+    __summary__,
+    __title__,
+    __uri__,
+    __version__,
 )
 
 __all__ = [
-    "__title__", "__summary__", "__uri__", "__version__", "__author__",
-    "__email__", "__license__", "__copyright__",
+    "__title__",
+    "__summary__",
+    "__uri__",
+    "__version__",
+    "__author__",
+    "__email__",
+    "__license__",
+    "__copyright__",
 ]
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/_compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 from __future__ import absolute_import, division, print_function
 
 import sys
 
+from ._typing import TYPE_CHECKING
+
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, Dict, Tuple, Type
+
 
 PY2 = sys.version_info[0] == 2
 PY3 = sys.version_info[0] == 3
 
 # flake8: noqa
 
 if PY3:
-    string_types = str,
+    string_types = (str,)
 else:
-    string_types = basestring,
+    string_types = (basestring,)
 
 
 def with_metaclass(meta, *bases):
+    # type: (Type[Any], Tuple[Type[Any], ...]) -> Any
     """
     Create a base class with a metaclass.
     """
     # This requires a bit of explanation: the basic idea is to make a dummy
     # metaclass for one level of class instantiation that replaces itself with
     # the actual metaclass.
-    class metaclass(meta):
+    class metaclass(meta):  # type: ignore
         def __new__(cls, name, this_bases, d):
+            # type: (Type[Any], str, Tuple[Any], Dict[Any, Any]) -> Any
             return meta(name, bases, d)
-    return type.__new__(metaclass, 'temporary_class', (), {})
+
+    return type.__new__(metaclass, "temporary_class", (), {})
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/markers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,20 +9,29 @@
 import sys
 
 from pkg_resources.extern.pyparsing import ParseException, ParseResults, stringStart, stringEnd
 from pkg_resources.extern.pyparsing import ZeroOrMore, Group, Forward, QuotedString
 from pkg_resources.extern.pyparsing import Literal as L  # noqa
 
 from ._compat import string_types
+from ._typing import TYPE_CHECKING
 from .specifiers import Specifier, InvalidSpecifier
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+
+    Operator = Callable[[str, str], bool]
+
 
 __all__ = [
-    "InvalidMarker", "UndefinedComparison", "UndefinedEnvironmentName",
-    "Marker", "default_environment",
+    "InvalidMarker",
+    "UndefinedComparison",
+    "UndefinedEnvironmentName",
+    "Marker",
+    "default_environment",
 ]
 
 
 class InvalidMarker(ValueError):
     """
     An invalid marker was found, users should refer to PEP 508.
     """
@@ -38,85 +47,81 @@
     """
     A name was attempted to be used that does not exist inside of the
     environment.
     """
 
 
 class Node(object):
-
     def __init__(self, value):
+        # type: (Any) -> None
         self.value = value
 
     def __str__(self):
+        # type: () -> str
         return str(self.value)
 
     def __repr__(self):
+        # type: () -> str
         return "<{0}({1!r})>".format(self.__class__.__name__, str(self))
 
     def serialize(self):
+        # type: () -> str
         raise NotImplementedError
 
 
 class Variable(Node):
-
     def serialize(self):
+        # type: () -> str
         return str(self)
 
 
 class Value(Node):
-
     def serialize(self):
+        # type: () -> str
         return '"{0}"'.format(self)
 
 
 class Op(Node):
-
     def serialize(self):
+        # type: () -> str
         return str(self)
 
 
 VARIABLE = (
-    L("implementation_version") |
-    L("platform_python_implementation") |
-    L("implementation_name") |
-    L("python_full_version") |
-    L("platform_release") |
-    L("platform_version") |
-    L("platform_machine") |
-    L("platform_system") |
-    L("python_version") |
-    L("sys_platform") |
-    L("os_name") |
-    L("os.name") |  # PEP-345
-    L("sys.platform") |  # PEP-345
-    L("platform.version") |  # PEP-345
-    L("platform.machine") |  # PEP-345
-    L("platform.python_implementation") |  # PEP-345
-    L("python_implementation") |  # undocumented setuptools legacy
-    L("extra")
+    L("implementation_version")
+    | L("platform_python_implementation")
+    | L("implementation_name")
+    | L("python_full_version")
+    | L("platform_release")
+    | L("platform_version")
+    | L("platform_machine")
+    | L("platform_system")
+    | L("python_version")
+    | L("sys_platform")
+    | L("os_name")
+    | L("os.name")  # PEP-345
+    | L("sys.platform")  # PEP-345
+    | L("platform.version")  # PEP-345
+    | L("platform.machine")  # PEP-345
+    | L("platform.python_implementation")  # PEP-345
+    | L("python_implementation")  # undocumented setuptools legacy
+    | L("extra")  # PEP-508
 )
 ALIASES = {
-    'os.name': 'os_name',
-    'sys.platform': 'sys_platform',
-    'platform.version': 'platform_version',
-    'platform.machine': 'platform_machine',
-    'platform.python_implementation': 'platform_python_implementation',
-    'python_implementation': 'platform_python_implementation'
+    "os.name": "os_name",
+    "sys.platform": "sys_platform",
+    "platform.version": "platform_version",
+    "platform.machine": "platform_machine",
+    "platform.python_implementation": "platform_python_implementation",
+    "python_implementation": "platform_python_implementation",
 }
 VARIABLE.setParseAction(lambda s, l, t: Variable(ALIASES.get(t[0], t[0])))
 
 VERSION_CMP = (
-    L("===") |
-    L("==") |
-    L(">=") |
-    L("<=") |
-    L("!=") |
-    L("~=") |
-    L(">") |
-    L("<")
+    L("===") | L("==") | L(">=") | L("<=") | L("!=") | L("~=") | L(">") | L("<")
 )
 
 MARKER_OP = VERSION_CMP | L("not in") | L("in")
 MARKER_OP.setParseAction(lambda s, l, t: Op(t[0]))
 
 MARKER_VALUE = QuotedString("'") | QuotedString('"')
 MARKER_VALUE.setParseAction(lambda s, l, t: Value(t[0]))
@@ -135,29 +140,35 @@
 MARKER_ATOM = MARKER_ITEM | Group(LPAREN + MARKER_EXPR + RPAREN)
 MARKER_EXPR << MARKER_ATOM + ZeroOrMore(BOOLOP + MARKER_EXPR)
 
 MARKER = stringStart + MARKER_EXPR + stringEnd
 
 
 def _coerce_parse_result(results):
+    # type: (Union[ParseResults, List[Any]]) -> List[Any]
     if isinstance(results, ParseResults):
         return [_coerce_parse_result(i) for i in results]
     else:
         return results
 
 
 def _format_marker(marker, first=True):
+    # type: (Union[List[str], Tuple[Node, ...], str], Optional[bool]) -> str
+
     assert isinstance(marker, (list, tuple, string_types))
 
     # Sometimes we have a structure like [[...]] which is a single item list
     # where the single item is itself it's own list. In that case we want skip
     # the rest of this function so that we don't get extraneous () on the
     # outside.
-    if (isinstance(marker, list) and len(marker) == 1 and
-            isinstance(marker[0], (list, tuple))):
+    if (
+        isinstance(marker, list)
+        and len(marker) == 1
+        and isinstance(marker[0], (list, tuple))
+    ):
         return _format_marker(marker[0])
 
     if isinstance(marker, list):
         inner = (_format_marker(m, first=False) for m in marker)
         if first:
             return " ".join(inner)
         else:
@@ -173,50 +184,57 @@
     "not in": lambda lhs, rhs: lhs not in rhs,
     "<": operator.lt,
     "<=": operator.le,
     "==": operator.eq,
     "!=": operator.ne,
     ">=": operator.ge,
     ">": operator.gt,
-}
+}  # type: Dict[str, Operator]
 
 
 def _eval_op(lhs, op, rhs):
+    # type: (str, Op, str) -> bool
     try:
         spec = Specifier("".join([op.serialize(), rhs]))
     except InvalidSpecifier:
         pass
     else:
         return spec.contains(lhs)
 
-    oper = _operators.get(op.serialize())
+    oper = _operators.get(op.serialize())  # type: Optional[Operator]
     if oper is None:
         raise UndefinedComparison(
             "Undefined {0!r} on {1!r} and {2!r}.".format(op, lhs, rhs)
         )
 
     return oper(lhs, rhs)
 
 
-_undefined = object()
+class Undefined(object):
+    pass
+
+
+_undefined = Undefined()
 
 
 def _get_env(environment, name):
-    value = environment.get(name, _undefined)
+    # type: (Dict[str, str], str) -> str
+    value = environment.get(name, _undefined)  # type: Union[str, Undefined]
 
-    if value is _undefined:
+    if isinstance(value, Undefined):
         raise UndefinedEnvironmentName(
             "{0!r} does not exist in evaluation environment.".format(name)
         )
 
     return value
 
 
 def _evaluate_markers(markers, environment):
-    groups = [[]]
+    # type: (List[Any], Dict[str, str]) -> bool
+    groups = [[]]  # type: List[List[bool]]
 
     for marker in markers:
         assert isinstance(marker, (list, tuple, string_types))
 
         if isinstance(marker, list):
             groups[-1].append(_evaluate_markers(marker, environment))
         elif isinstance(marker, tuple):
@@ -235,61 +253,70 @@
             if marker == "or":
                 groups.append([])
 
     return any(all(item) for item in groups)
 
 
 def format_full_version(info):
-    version = '{0.major}.{0.minor}.{0.micro}'.format(info)
+    # type: (sys._version_info) -> str
+    version = "{0.major}.{0.minor}.{0.micro}".format(info)
     kind = info.releaselevel
-    if kind != 'final':
+    if kind != "final":
         version += kind[0] + str(info.serial)
     return version
 
 
 def default_environment():
-    if hasattr(sys, 'implementation'):
-        iver = format_full_version(sys.implementation.version)
-        implementation_name = sys.implementation.name
+    # type: () -> Dict[str, str]
+    if hasattr(sys, "implementation"):
+        # Ignoring the `sys.implementation` reference for type checking due to
+        # mypy not liking that the attribute doesn't exist in Python 2.7 when
+        # run with the `--py27` flag.
+        iver = format_full_version(sys.implementation.version)  # type: ignore
+        implementation_name = sys.implementation.name  # type: ignore
     else:
-        iver = '0'
-        implementation_name = ''
+        iver = "0"
+        implementation_name = ""
 
     return {
         "implementation_name": implementation_name,
         "implementation_version": iver,
         "os_name": os.name,
         "platform_machine": platform.machine(),
         "platform_release": platform.release(),
         "platform_system": platform.system(),
         "platform_version": platform.version(),
         "python_full_version": platform.python_version(),
         "platform_python_implementation": platform.python_implementation(),
-        "python_version": platform.python_version()[:3],
+        "python_version": ".".join(platform.python_version_tuple()[:2]),
         "sys_platform": sys.platform,
     }
 
 
 class Marker(object):
-
     def __init__(self, marker):
+        # type: (str) -> None
         try:
             self._markers = _coerce_parse_result(MARKER.parseString(marker))
         except ParseException as e:
             err_str = "Invalid marker: {0!r}, parse error at {1!r}".format(
-                marker, marker[e.loc:e.loc + 8])
+                marker, marker[e.loc : e.loc + 8]
+            )
             raise InvalidMarker(err_str)
 
     def __str__(self):
+        # type: () -> str
         return _format_marker(self._markers)
 
     def __repr__(self):
+        # type: () -> str
         return "<Marker({0!r})>".format(str(self))
 
     def evaluate(self, environment=None):
+        # type: (Optional[Dict[str, str]]) -> bool
         """Evaluate a marker.
 
         Return the boolean from evaluating the given marker against the
         environment. environment is an optional argument to override all or
         part of the determined environment.
 
         The environment is determined from the current Python process.
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 
 import string
 import re
 
 from pkg_resources.extern.pyparsing import stringStart, stringEnd, originalTextFor, ParseException
 from pkg_resources.extern.pyparsing import ZeroOrMore, Word, Optional, Regex, Combine
 from pkg_resources.extern.pyparsing import Literal as L  # noqa
-from pkg_resources.extern.six.moves.urllib import parse as urlparse
+from urllib import parse as urlparse
 
+from ._typing import TYPE_CHECKING
 from .markers import MARKER_EXPR, Marker
 from .specifiers import LegacySpecifier, Specifier, SpecifierSet
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import List
+
 
 class InvalidRequirement(ValueError):
     """
     An invalid requirement was found, users should refer to PEP 508.
     """
 
 
@@ -34,46 +38,49 @@
 PUNCTUATION = Word("-_.")
 IDENTIFIER_END = ALPHANUM | (ZeroOrMore(PUNCTUATION) + ALPHANUM)
 IDENTIFIER = Combine(ALPHANUM + ZeroOrMore(IDENTIFIER_END))
 
 NAME = IDENTIFIER("name")
 EXTRA = IDENTIFIER
 
-URI = Regex(r'[^ ]+')("url")
-URL = (AT + URI)
+URI = Regex(r"[^ ]+")("url")
+URL = AT + URI
 
 EXTRAS_LIST = EXTRA + ZeroOrMore(COMMA + EXTRA)
 EXTRAS = (LBRACKET + Optional(EXTRAS_LIST) + RBRACKET)("extras")
 
 VERSION_PEP440 = Regex(Specifier._regex_str, re.VERBOSE | re.IGNORECASE)
 VERSION_LEGACY = Regex(LegacySpecifier._regex_str, re.VERBOSE | re.IGNORECASE)
 
 VERSION_ONE = VERSION_PEP440 ^ VERSION_LEGACY
-VERSION_MANY = Combine(VERSION_ONE + ZeroOrMore(COMMA + VERSION_ONE),
-                       joinString=",", adjacent=False)("_raw_spec")
+VERSION_MANY = Combine(
+    VERSION_ONE + ZeroOrMore(COMMA + VERSION_ONE), joinString=",", adjacent=False
+)("_raw_spec")
 _VERSION_SPEC = Optional(((LPAREN + VERSION_MANY + RPAREN) | VERSION_MANY))
-_VERSION_SPEC.setParseAction(lambda s, l, t: t._raw_spec or '')
+_VERSION_SPEC.setParseAction(lambda s, l, t: t._raw_spec or "")
 
 VERSION_SPEC = originalTextFor(_VERSION_SPEC)("specifier")
 VERSION_SPEC.setParseAction(lambda s, l, t: t[1])
 
 MARKER_EXPR = originalTextFor(MARKER_EXPR())("marker")
 MARKER_EXPR.setParseAction(
-    lambda s, l, t: Marker(s[t._original_start:t._original_end])
+    lambda s, l, t: Marker(s[t._original_start : t._original_end])
 )
-MARKER_SEPERATOR = SEMICOLON
-MARKER = MARKER_SEPERATOR + MARKER_EXPR
+MARKER_SEPARATOR = SEMICOLON
+MARKER = MARKER_SEPARATOR + MARKER_EXPR
 
 VERSION_AND_MARKER = VERSION_SPEC + Optional(MARKER)
 URL_AND_MARKER = URL + Optional(MARKER)
 
-NAMED_REQUIREMENT = \
-    NAME + Optional(EXTRAS) + (URL_AND_MARKER | VERSION_AND_MARKER)
+NAMED_REQUIREMENT = NAME + Optional(EXTRAS) + (URL_AND_MARKER | VERSION_AND_MARKER)
 
 REQUIREMENT = stringStart + NAMED_REQUIREMENT + stringEnd
+# pkg_resources.extern.pyparsing isn't thread safe during initialization, so we do it eagerly, see
+# issue #104
+REQUIREMENT.parseString("x[]")
 
 
 class Requirement(object):
     """Parse a requirement.
 
     Parse a given requirement string into its parts, such as name, specifier,
     URL, and extras. Raises InvalidRequirement on a badly-formed requirement
@@ -82,46 +89,57 @@
 
     # TODO: Can we test whether something is contained within a requirement?
     #       If so how do we do that? Do we need to test against the _name_ of
     #       the thing as well as the version? What about the markers?
     # TODO: Can we normalize the name and extra name?
 
     def __init__(self, requirement_string):
+        # type: (str) -> None
         try:
             req = REQUIREMENT.parseString(requirement_string)
         except ParseException as e:
             raise InvalidRequirement(
-                "Invalid requirement, parse error at \"{0!r}\"".format(
-                    requirement_string[e.loc:e.loc + 8]))
+                'Parse error at "{0!r}": {1}'.format(
+                    requirement_string[e.loc : e.loc + 8], e.msg
+                )
+            )
 
         self.name = req.name
         if req.url:
             parsed_url = urlparse.urlparse(req.url)
-            if not (parsed_url.scheme and parsed_url.netloc) or (
-                    not parsed_url.scheme and not parsed_url.netloc):
-                raise InvalidRequirement("Invalid URL given")
+            if parsed_url.scheme == "file":
+                if urlparse.urlunparse(parsed_url) != req.url:
+                    raise InvalidRequirement("Invalid URL given")
+            elif not (parsed_url.scheme and parsed_url.netloc) or (
+                not parsed_url.scheme and not parsed_url.netloc
+            ):
+                raise InvalidRequirement("Invalid URL: {0}".format(req.url))
             self.url = req.url
         else:
             self.url = None
         self.extras = set(req.extras.asList() if req.extras else [])
         self.specifier = SpecifierSet(req.specifier)
         self.marker = req.marker if req.marker else None
 
     def __str__(self):
-        parts = [self.name]
+        # type: () -> str
+        parts = [self.name]  # type: List[str]
 
         if self.extras:
             parts.append("[{0}]".format(",".join(sorted(self.extras))))
 
         if self.specifier:
             parts.append(str(self.specifier))
 
         if self.url:
             parts.append("@ {0}".format(self.url))
+            if self.marker:
+                parts.append(" ")
 
         if self.marker:
             parts.append("; {0}".format(self.marker))
 
         return "".join(parts)
 
     def __repr__(self):
+        # type: () -> str
         return "<Requirement({0!r})>".format(str(self))
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,281 +5,338 @@
 
 import abc
 import functools
 import itertools
 import re
 
 from ._compat import string_types, with_metaclass
+from ._typing import TYPE_CHECKING
+from .utils import canonicalize_version
 from .version import Version, LegacyVersion, parse
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import (
+        List,
+        Dict,
+        Union,
+        Iterable,
+        Iterator,
+        Optional,
+        Callable,
+        Tuple,
+        FrozenSet,
+    )
+
+    ParsedVersion = Union[Version, LegacyVersion]
+    UnparsedVersion = Union[Version, LegacyVersion, str]
+    CallableOperator = Callable[[ParsedVersion, str], bool]
+
 
 class InvalidSpecifier(ValueError):
     """
     An invalid specifier was found, users should refer to PEP 440.
     """
 
 
-class BaseSpecifier(with_metaclass(abc.ABCMeta, object)):
-
+class BaseSpecifier(with_metaclass(abc.ABCMeta, object)):  # type: ignore
     @abc.abstractmethod
     def __str__(self):
+        # type: () -> str
         """
         Returns the str representation of this Specifier like object. This
         should be representative of the Specifier itself.
         """
 
     @abc.abstractmethod
     def __hash__(self):
+        # type: () -> int
         """
         Returns a hash value for this Specifier like object.
         """
 
     @abc.abstractmethod
     def __eq__(self, other):
+        # type: (object) -> bool
         """
         Returns a boolean representing whether or not the two Specifier like
         objects are equal.
         """
 
     @abc.abstractmethod
     def __ne__(self, other):
+        # type: (object) -> bool
         """
         Returns a boolean representing whether or not the two Specifier like
         objects are not equal.
         """
 
     @abc.abstractproperty
     def prereleases(self):
+        # type: () -> Optional[bool]
         """
         Returns whether or not pre-releases as a whole are allowed by this
         specifier.
         """
 
     @prereleases.setter
     def prereleases(self, value):
+        # type: (bool) -> None
         """
         Sets whether or not pre-releases as a whole are allowed by this
         specifier.
         """
 
     @abc.abstractmethod
     def contains(self, item, prereleases=None):
+        # type: (str, Optional[bool]) -> bool
         """
         Determines if the given item is contained within this specifier.
         """
 
     @abc.abstractmethod
     def filter(self, iterable, prereleases=None):
+        # type: (Iterable[UnparsedVersion], Optional[bool]) -> Iterable[UnparsedVersion]
         """
         Takes an iterable of items and filters them so that only items which
         are contained within this specifier are allowed in it.
         """
 
 
 class _IndividualSpecifier(BaseSpecifier):
 
-    _operators = {}
+    _operators = {}  # type: Dict[str, str]
 
     def __init__(self, spec="", prereleases=None):
+        # type: (str, Optional[bool]) -> None
         match = self._regex.search(spec)
         if not match:
             raise InvalidSpecifier("Invalid specifier: '{0}'".format(spec))
 
         self._spec = (
             match.group("operator").strip(),
             match.group("version").strip(),
-        )
+        )  # type: Tuple[str, str]
 
         # Store whether or not this Specifier should accept prereleases
         self._prereleases = prereleases
 
     def __repr__(self):
+        # type: () -> str
         pre = (
             ", prereleases={0!r}".format(self.prereleases)
             if self._prereleases is not None
             else ""
         )
 
-        return "<{0}({1!r}{2})>".format(
-            self.__class__.__name__,
-            str(self),
-            pre,
-        )
+        return "<{0}({1!r}{2})>".format(self.__class__.__name__, str(self), pre)
 
     def __str__(self):
+        # type: () -> str
         return "{0}{1}".format(*self._spec)
 
+    @property
+    def _canonical_spec(self):
+        # type: () -> Tuple[str, Union[Version, str]]
+        return self._spec[0], canonicalize_version(self._spec[1])
+
     def __hash__(self):
-        return hash(self._spec)
+        # type: () -> int
+        return hash(self._canonical_spec)
 
     def __eq__(self, other):
+        # type: (object) -> bool
         if isinstance(other, string_types):
             try:
-                other = self.__class__(other)
+                other = self.__class__(str(other))
             except InvalidSpecifier:
                 return NotImplemented
         elif not isinstance(other, self.__class__):
             return NotImplemented
 
-        return self._spec == other._spec
+        return self._canonical_spec == other._canonical_spec
 
     def __ne__(self, other):
+        # type: (object) -> bool
         if isinstance(other, string_types):
             try:
-                other = self.__class__(other)
+                other = self.__class__(str(other))
             except InvalidSpecifier:
                 return NotImplemented
         elif not isinstance(other, self.__class__):
             return NotImplemented
 
         return self._spec != other._spec
 
     def _get_operator(self, op):
-        return getattr(self, "_compare_{0}".format(self._operators[op]))
+        # type: (str) -> CallableOperator
+        operator_callable = getattr(
+            self, "_compare_{0}".format(self._operators[op])
+        )  # type: CallableOperator
+        return operator_callable
 
     def _coerce_version(self, version):
+        # type: (UnparsedVersion) -> ParsedVersion
         if not isinstance(version, (LegacyVersion, Version)):
             version = parse(version)
         return version
 
     @property
     def operator(self):
+        # type: () -> str
         return self._spec[0]
 
     @property
     def version(self):
+        # type: () -> str
         return self._spec[1]
 
     @property
     def prereleases(self):
+        # type: () -> Optional[bool]
         return self._prereleases
 
     @prereleases.setter
     def prereleases(self, value):
+        # type: (bool) -> None
         self._prereleases = value
 
     def __contains__(self, item):
+        # type: (str) -> bool
         return self.contains(item)
 
     def contains(self, item, prereleases=None):
+        # type: (UnparsedVersion, Optional[bool]) -> bool
+
         # Determine if prereleases are to be allowed or not.
         if prereleases is None:
             prereleases = self.prereleases
 
         # Normalize item to a Version or LegacyVersion, this allows us to have
         # a shortcut for ``"2.0" in Specifier(">=2")
-        item = self._coerce_version(item)
+        normalized_item = self._coerce_version(item)
 
         # Determine if we should be supporting prereleases in this specifier
         # or not, if we do not support prereleases than we can short circuit
         # logic if this version is a prereleases.
-        if item.is_prerelease and not prereleases:
+        if normalized_item.is_prerelease and not prereleases:
             return False
 
         # Actually do the comparison to determine if this item is contained
         # within this Specifier or not.
-        return self._get_operator(self.operator)(item, self.version)
+        operator_callable = self._get_operator(self.operator)  # type: CallableOperator
+        return operator_callable(normalized_item, self.version)
 
     def filter(self, iterable, prereleases=None):
+        # type: (Iterable[UnparsedVersion], Optional[bool]) -> Iterable[UnparsedVersion]
+
         yielded = False
         found_prereleases = []
 
         kw = {"prereleases": prereleases if prereleases is not None else True}
 
         # Attempt to iterate over all the values in the iterable and if any of
         # them match, yield them.
         for version in iterable:
             parsed_version = self._coerce_version(version)
 
             if self.contains(parsed_version, **kw):
                 # If our version is a prerelease, and we were not set to allow
                 # prereleases, then we'll store it for later incase nothing
                 # else matches this specifier.
-                if (parsed_version.is_prerelease and not
-                        (prereleases or self.prereleases)):
+                if parsed_version.is_prerelease and not (
+                    prereleases or self.prereleases
+                ):
                     found_prereleases.append(version)
                 # Either this is not a prerelease, or we should have been
-                # accepting prereleases from the begining.
+                # accepting prereleases from the beginning.
                 else:
                     yielded = True
                     yield version
 
         # Now that we've iterated over everything, determine if we've yielded
         # any values, and if we have not and we have any prereleases stored up
         # then we will go ahead and yield the prereleases.
         if not yielded and found_prereleases:
             for version in found_prereleases:
                 yield version
 
 
 class LegacySpecifier(_IndividualSpecifier):
 
-    _regex_str = (
-        r"""
+    _regex_str = r"""
         (?P<operator>(==|!=|<=|>=|<|>))
         \s*
         (?P<version>
             [^,;\s)]* # Since this is a "legacy" specifier, and the version
                       # string can be just about anything, we match everything
                       # except for whitespace, a semi-colon for marker support,
                       # a closing paren since versions can be enclosed in
                       # them, and a comma since it's a version separator.
         )
         """
-    )
 
-    _regex = re.compile(
-        r"^\s*" + _regex_str + r"\s*$", re.VERBOSE | re.IGNORECASE)
+    _regex = re.compile(r"^\s*" + _regex_str + r"\s*$", re.VERBOSE | re.IGNORECASE)
 
     _operators = {
         "==": "equal",
         "!=": "not_equal",
         "<=": "less_than_equal",
         ">=": "greater_than_equal",
         "<": "less_than",
         ">": "greater_than",
     }
 
     def _coerce_version(self, version):
+        # type: (Union[ParsedVersion, str]) -> LegacyVersion
         if not isinstance(version, LegacyVersion):
             version = LegacyVersion(str(version))
         return version
 
     def _compare_equal(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective == self._coerce_version(spec)
 
     def _compare_not_equal(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective != self._coerce_version(spec)
 
     def _compare_less_than_equal(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective <= self._coerce_version(spec)
 
     def _compare_greater_than_equal(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective >= self._coerce_version(spec)
 
     def _compare_less_than(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective < self._coerce_version(spec)
 
     def _compare_greater_than(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective > self._coerce_version(spec)
 
 
-def _require_version_compare(fn):
+def _require_version_compare(
+    fn  # type: (Callable[[Specifier, ParsedVersion, str], bool])
+):
+    # type: (...) -> Callable[[Specifier, ParsedVersion, str], bool]
     @functools.wraps(fn)
     def wrapped(self, prospective, spec):
+        # type: (Specifier, ParsedVersion, str) -> bool
         if not isinstance(prospective, Version):
             return False
         return fn(self, prospective, spec)
+
     return wrapped
 
 
 class Specifier(_IndividualSpecifier):
 
-    _regex_str = (
-        r"""
+    _regex_str = r"""
         (?P<operator>(~=|==|!=|<=|>=|<|>|===))
         (?P<version>
             (?:
                 # The identity operators allow for an escape hatch that will
                 # do an exact string match of the version you wish to install.
                 # This will not be parsed by PEP 440 and we cannot determine
                 # any semantic meaning from it. This operator is discouraged
@@ -363,109 +420,128 @@
                 (?:                                   # post release
                     (?:-[0-9]+)|(?:[-_\.]?(post|rev|r)[-_\.]?[0-9]*)
                 )?
                 (?:[-_\.]?dev[-_\.]?[0-9]*)?          # dev release
             )
         )
         """
-    )
 
-    _regex = re.compile(
-        r"^\s*" + _regex_str + r"\s*$", re.VERBOSE | re.IGNORECASE)
+    _regex = re.compile(r"^\s*" + _regex_str + r"\s*$", re.VERBOSE | re.IGNORECASE)
 
     _operators = {
         "~=": "compatible",
         "==": "equal",
         "!=": "not_equal",
         "<=": "less_than_equal",
         ">=": "greater_than_equal",
         "<": "less_than",
         ">": "greater_than",
         "===": "arbitrary",
     }
 
     @_require_version_compare
     def _compare_compatible(self, prospective, spec):
+        # type: (ParsedVersion, str) -> bool
+
         # Compatible releases have an equivalent combination of >= and ==. That
         # is that ~=2.2 is equivalent to >=2.2,==2.*. This allows us to
         # implement this in terms of the other specifiers instead of
         # implementing it ourselves. The only thing we need to do is construct
         # the other specifiers.
 
         # We want everything but the last item in the version, but we want to
         # ignore post and dev releases and we want to treat the pre-release as
         # it's own separate segment.
         prefix = ".".join(
             list(
                 itertools.takewhile(
-                    lambda x: (not x.startswith("post") and not
-                               x.startswith("dev")),
+                    lambda x: (not x.startswith("post") and not x.startswith("dev")),
                     _version_split(spec),
                 )
             )[:-1]
         )
 
         # Add the prefix notation to the end of our string
         prefix += ".*"
 
-        return (self._get_operator(">=")(prospective, spec) and
-                self._get_operator("==")(prospective, prefix))
+        return self._get_operator(">=")(prospective, spec) and self._get_operator("==")(
+            prospective, prefix
+        )
 
     @_require_version_compare
     def _compare_equal(self, prospective, spec):
+        # type: (ParsedVersion, str) -> bool
+
         # We need special logic to handle prefix matching
         if spec.endswith(".*"):
             # In the case of prefix matching we want to ignore local segment.
             prospective = Version(prospective.public)
             # Split the spec out by dots, and pretend that there is an implicit
             # dot in between a release segment and a pre-release segment.
-            spec = _version_split(spec[:-2])  # Remove the trailing .*
+            split_spec = _version_split(spec[:-2])  # Remove the trailing .*
 
             # Split the prospective version out by dots, and pretend that there
             # is an implicit dot in between a release segment and a pre-release
             # segment.
-            prospective = _version_split(str(prospective))
+            split_prospective = _version_split(str(prospective))
 
             # Shorten the prospective version to be the same length as the spec
             # so that we can determine if the specifier is a prefix of the
             # prospective version or not.
-            prospective = prospective[:len(spec)]
+            shortened_prospective = split_prospective[: len(split_spec)]
 
             # Pad out our two sides with zeros so that they both equal the same
             # length.
-            spec, prospective = _pad_version(spec, prospective)
+            padded_spec, padded_prospective = _pad_version(
+                split_spec, shortened_prospective
+            )
+
+            return padded_prospective == padded_spec
         else:
             # Convert our spec string into a Version
-            spec = Version(spec)
+            spec_version = Version(spec)
 
             # If the specifier does not have a local segment, then we want to
             # act as if the prospective version also does not have a local
             # segment.
-            if not spec.local:
+            if not spec_version.local:
                 prospective = Version(prospective.public)
 
-        return prospective == spec
+            return prospective == spec_version
 
     @_require_version_compare
     def _compare_not_equal(self, prospective, spec):
+        # type: (ParsedVersion, str) -> bool
         return not self._compare_equal(prospective, spec)
 
     @_require_version_compare
     def _compare_less_than_equal(self, prospective, spec):
-        return prospective <= Version(spec)
+        # type: (ParsedVersion, str) -> bool
+
+        # NB: Local version identifiers are NOT permitted in the version
+        # specifier, so local version labels can be universally removed from
+        # the prospective version.
+        return Version(prospective.public) <= Version(spec)
 
     @_require_version_compare
     def _compare_greater_than_equal(self, prospective, spec):
-        return prospective >= Version(spec)
+        # type: (ParsedVersion, str) -> bool
+
+        # NB: Local version identifiers are NOT permitted in the version
+        # specifier, so local version labels can be universally removed from
+        # the prospective version.
+        return Version(prospective.public) >= Version(spec)
 
     @_require_version_compare
-    def _compare_less_than(self, prospective, spec):
+    def _compare_less_than(self, prospective, spec_str):
+        # type: (ParsedVersion, str) -> bool
+
         # Convert our spec to a Version instance, since we'll want to work with
         # it as a version.
-        spec = Version(spec)
+        spec = Version(spec_str)
 
         # Check to see if the prospective version is less than the spec
         # version. If it's not we can short circuit and just return False now
         # instead of doing extra unneeded work.
         if not prospective < spec:
             return False
 
@@ -479,18 +555,20 @@
 
         # If we've gotten to here, it means that prospective version is both
         # less than the spec version *and* it's not a pre-release of the same
         # version in the spec.
         return True
 
     @_require_version_compare
-    def _compare_greater_than(self, prospective, spec):
+    def _compare_greater_than(self, prospective, spec_str):
+        # type: (ParsedVersion, str) -> bool
+
         # Convert our spec to a Version instance, since we'll want to work with
         # it as a version.
-        spec = Version(spec)
+        spec = Version(spec_str)
 
         # Check to see if the prospective version is greater than the spec
         # version. If it's not we can short circuit and just return False now
         # instead of doing extra unneeded work.
         if not prospective > spec:
             return False
 
@@ -499,29 +577,32 @@
         # post-release versions for the version mentioned in the specifier
         # (e.g. >3.1 should not match 3.0.post0, but should match 3.2.post0).
         if not spec.is_postrelease and prospective.is_postrelease:
             if Version(prospective.base_version) == Version(spec.base_version):
                 return False
 
         # Ensure that we do not allow a local version of the version mentioned
-        # in the specifier, which is techincally greater than, to match.
+        # in the specifier, which is technically greater than, to match.
         if prospective.local is not None:
             if Version(prospective.base_version) == Version(spec.base_version):
                 return False
 
         # If we've gotten to here, it means that prospective version is both
         # greater than the spec version *and* it's not a pre-release of the
         # same version in the spec.
         return True
 
     def _compare_arbitrary(self, prospective, spec):
+        # type: (Version, str) -> bool
         return str(prospective).lower() == str(spec).lower()
 
     @property
     def prereleases(self):
+        # type: () -> bool
+
         # If there is an explicit prereleases set for this, then we'll just
         # blindly use that.
         if self._prereleases is not None:
             return self._prereleases
 
         # Look at all of our specifiers and determine if they are inclusive
         # operators, and if they are if they are including an explicit
@@ -538,97 +619,96 @@
             if parse(version).is_prerelease:
                 return True
 
         return False
 
     @prereleases.setter
     def prereleases(self, value):
+        # type: (bool) -> None
         self._prereleases = value
 
 
 _prefix_regex = re.compile(r"^([0-9]+)((?:a|b|c|rc)[0-9]+)$")
 
 
 def _version_split(version):
-    result = []
+    # type: (str) -> List[str]
+    result = []  # type: List[str]
     for item in version.split("."):
         match = _prefix_regex.search(item)
         if match:
             result.extend(match.groups())
         else:
             result.append(item)
     return result
 
 
 def _pad_version(left, right):
+    # type: (List[str], List[str]) -> Tuple[List[str], List[str]]
     left_split, right_split = [], []
 
     # Get the release segment of our versions
     left_split.append(list(itertools.takewhile(lambda x: x.isdigit(), left)))
     right_split.append(list(itertools.takewhile(lambda x: x.isdigit(), right)))
 
     # Get the rest of our versions
-    left_split.append(left[len(left_split[0]):])
-    right_split.append(right[len(right_split[0]):])
+    left_split.append(left[len(left_split[0]) :])
+    right_split.append(right[len(right_split[0]) :])
 
     # Insert our padding
-    left_split.insert(
-        1,
-        ["0"] * max(0, len(right_split[0]) - len(left_split[0])),
-    )
-    right_split.insert(
-        1,
-        ["0"] * max(0, len(left_split[0]) - len(right_split[0])),
-    )
+    left_split.insert(1, ["0"] * max(0, len(right_split[0]) - len(left_split[0])))
+    right_split.insert(1, ["0"] * max(0, len(left_split[0]) - len(right_split[0])))
 
-    return (
-        list(itertools.chain(*left_split)),
-        list(itertools.chain(*right_split)),
-    )
+    return (list(itertools.chain(*left_split)), list(itertools.chain(*right_split)))
 
 
 class SpecifierSet(BaseSpecifier):
-
     def __init__(self, specifiers="", prereleases=None):
-        # Split on , to break each indidivual specifier into it's own item, and
+        # type: (str, Optional[bool]) -> None
+
+        # Split on , to break each individual specifier into it's own item, and
         # strip each item to remove leading/trailing whitespace.
-        specifiers = [s.strip() for s in specifiers.split(",") if s.strip()]
+        split_specifiers = [s.strip() for s in specifiers.split(",") if s.strip()]
 
         # Parsed each individual specifier, attempting first to make it a
         # Specifier and falling back to a LegacySpecifier.
         parsed = set()
-        for specifier in specifiers:
+        for specifier in split_specifiers:
             try:
                 parsed.add(Specifier(specifier))
             except InvalidSpecifier:
                 parsed.add(LegacySpecifier(specifier))
 
         # Turn our parsed specifiers into a frozen set and save them for later.
         self._specs = frozenset(parsed)
 
         # Store our prereleases value so we can use it later to determine if
         # we accept prereleases or not.
         self._prereleases = prereleases
 
     def __repr__(self):
+        # type: () -> str
         pre = (
             ", prereleases={0!r}".format(self.prereleases)
             if self._prereleases is not None
             else ""
         )
 
         return "<SpecifierSet({0!r}{1})>".format(str(self), pre)
 
     def __str__(self):
+        # type: () -> str
         return ",".join(sorted(str(s) for s in self._specs))
 
     def __hash__(self):
+        # type: () -> int
         return hash(self._specs)
 
     def __and__(self, other):
+        # type: (Union[SpecifierSet, str]) -> SpecifierSet
         if isinstance(other, string_types):
             other = SpecifierSet(other)
         elif not isinstance(other, SpecifierSet):
             return NotImplemented
 
         specifier = SpecifierSet()
         specifier._specs = frozenset(self._specs | other._specs)
@@ -644,41 +724,43 @@
                 "Cannot combine SpecifierSets with True and False prerelease "
                 "overrides."
             )
 
         return specifier
 
     def __eq__(self, other):
-        if isinstance(other, string_types):
-            other = SpecifierSet(other)
-        elif isinstance(other, _IndividualSpecifier):
+        # type: (object) -> bool
+        if isinstance(other, (string_types, _IndividualSpecifier)):
             other = SpecifierSet(str(other))
         elif not isinstance(other, SpecifierSet):
             return NotImplemented
 
         return self._specs == other._specs
 
     def __ne__(self, other):
-        if isinstance(other, string_types):
-            other = SpecifierSet(other)
-        elif isinstance(other, _IndividualSpecifier):
+        # type: (object) -> bool
+        if isinstance(other, (string_types, _IndividualSpecifier)):
             other = SpecifierSet(str(other))
         elif not isinstance(other, SpecifierSet):
             return NotImplemented
 
         return self._specs != other._specs
 
     def __len__(self):
+        # type: () -> int
         return len(self._specs)
 
     def __iter__(self):
+        # type: () -> Iterator[FrozenSet[_IndividualSpecifier]]
         return iter(self._specs)
 
     @property
     def prereleases(self):
+        # type: () -> Optional[bool]
+
         # If we have been given an explicit prerelease modifier, then we'll
         # pass that through here.
         if self._prereleases is not None:
             return self._prereleases
 
         # If we don't have any specifiers, and we don't have a forced value,
         # then we'll just return None since we don't know if this should have
@@ -688,20 +770,24 @@
 
         # Otherwise we'll see if any of the given specifiers accept
         # prereleases, if any of them do we'll return True, otherwise False.
         return any(s.prereleases for s in self._specs)
 
     @prereleases.setter
     def prereleases(self, value):
+        # type: (bool) -> None
         self._prereleases = value
 
     def __contains__(self, item):
+        # type: (Union[ParsedVersion, str]) -> bool
         return self.contains(item)
 
     def contains(self, item, prereleases=None):
+        # type: (Union[ParsedVersion, str], Optional[bool]) -> bool
+
         # Ensure that our item is a Version or LegacyVersion instance.
         if not isinstance(item, (LegacyVersion, Version)):
             item = parse(item)
 
         # Determine if we're forcing a prerelease or not, if we're not forcing
         # one for this particular filter call, then we'll use whatever the
         # SpecifierSet thinks for whether or not we should support prereleases.
@@ -717,20 +803,23 @@
         if not prereleases and item.is_prerelease:
             return False
 
         # We simply dispatch to the underlying specs here to make sure that the
         # given version is contained within all of them.
         # Note: This use of all() here means that an empty set of specifiers
         #       will always return True, this is an explicit design decision.
-        return all(
-            s.contains(item, prereleases=prereleases)
-            for s in self._specs
-        )
+        return all(s.contains(item, prereleases=prereleases) for s in self._specs)
+
+    def filter(
+        self,
+        iterable,  # type: Iterable[Union[ParsedVersion, str]]
+        prereleases=None,  # type: Optional[bool]
+    ):
+        # type: (...) -> Iterable[Union[ParsedVersion, str]]
 
-    def filter(self, iterable, prereleases=None):
         # Determine if we're forcing a prerelease or not, if we're not forcing
         # one for this particular filter call, then we'll use whatever the
         # SpecifierSet thinks for whether or not we should support prereleases.
         if prereleases is None:
             prereleases = self.prereleases
 
         # If we have any specifiers, then we want to wrap our iterable in the
@@ -740,16 +829,16 @@
             for spec in self._specs:
                 iterable = spec.filter(iterable, prereleases=bool(prereleases))
             return iterable
         # If we do not have any specifiers, then we need to have a rough filter
         # which will filter out any pre-releases, unless there are no final
         # releases, and which will filter out LegacyVersion in general.
         else:
-            filtered = []
-            found_prereleases = []
+            filtered = []  # type: List[Union[ParsedVersion, str]]
+            found_prereleases = []  # type: List[Union[ParsedVersion, str]]
 
             for item in iterable:
                 # Ensure that we some kind of Version class for this item.
                 if not isinstance(item, (LegacyVersion, Version)):
                     parsed_version = parse(item)
                 else:
                     parsed_version = item
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/packaging/version.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,54 @@
 # for complete details.
 from __future__ import absolute_import, division, print_function
 
 import collections
 import itertools
 import re
 
-from ._structures import Infinity
+from ._structures import Infinity, NegativeInfinity
+from ._typing import TYPE_CHECKING
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Callable, Iterator, List, Optional, SupportsInt, Tuple, Union
 
-__all__ = [
-    "parse", "Version", "LegacyVersion", "InvalidVersion", "VERSION_PATTERN"
-]
+    from ._structures import InfinityType, NegativeInfinityType
+
+    InfiniteTypes = Union[InfinityType, NegativeInfinityType]
+    PrePostDevType = Union[InfiniteTypes, Tuple[str, int]]
+    SubLocalType = Union[InfiniteTypes, int, str]
+    LocalType = Union[
+        NegativeInfinityType,
+        Tuple[
+            Union[
+                SubLocalType,
+                Tuple[SubLocalType, str],
+                Tuple[NegativeInfinityType, SubLocalType],
+            ],
+            ...,
+        ],
+    ]
+    CmpKey = Tuple[
+        int, Tuple[int, ...], PrePostDevType, PrePostDevType, PrePostDevType, LocalType
+    ]
+    LegacyCmpKey = Tuple[int, Tuple[str, ...]]
+    VersionComparisonMethod = Callable[
+        [Union[CmpKey, LegacyCmpKey], Union[CmpKey, LegacyCmpKey]], bool
+    ]
+
+__all__ = ["parse", "Version", "LegacyVersion", "InvalidVersion", "VERSION_PATTERN"]
 
 
 _Version = collections.namedtuple(
-    "_Version",
-    ["epoch", "release", "dev", "pre", "post", "local"],
+    "_Version", ["epoch", "release", "dev", "pre", "post", "local"]
 )
 
 
 def parse(version):
+    # type: (str) -> Union[LegacyVersion, Version]
     """
     Parse the given version string and return either a :class:`Version` object
     or a :class:`LegacyVersion` object depending on if the given version is
     a valid PEP 440 version or a legacy version.
     """
     try:
         return Version(version)
@@ -36,86 +61,135 @@
 class InvalidVersion(ValueError):
     """
     An invalid version was found, users should refer to PEP 440.
     """
 
 
 class _BaseVersion(object):
+    _key = None  # type: Union[CmpKey, LegacyCmpKey]
 
     def __hash__(self):
+        # type: () -> int
         return hash(self._key)
 
     def __lt__(self, other):
+        # type: (_BaseVersion) -> bool
         return self._compare(other, lambda s, o: s < o)
 
     def __le__(self, other):
+        # type: (_BaseVersion) -> bool
         return self._compare(other, lambda s, o: s <= o)
 
     def __eq__(self, other):
+        # type: (object) -> bool
         return self._compare(other, lambda s, o: s == o)
 
     def __ge__(self, other):
+        # type: (_BaseVersion) -> bool
         return self._compare(other, lambda s, o: s >= o)
 
     def __gt__(self, other):
+        # type: (_BaseVersion) -> bool
         return self._compare(other, lambda s, o: s > o)
 
     def __ne__(self, other):
+        # type: (object) -> bool
         return self._compare(other, lambda s, o: s != o)
 
     def _compare(self, other, method):
+        # type: (object, VersionComparisonMethod) -> Union[bool, NotImplemented]
         if not isinstance(other, _BaseVersion):
             return NotImplemented
 
         return method(self._key, other._key)
 
 
 class LegacyVersion(_BaseVersion):
-
     def __init__(self, version):
+        # type: (str) -> None
         self._version = str(version)
         self._key = _legacy_cmpkey(self._version)
 
     def __str__(self):
+        # type: () -> str
         return self._version
 
     def __repr__(self):
+        # type: () -> str
         return "<LegacyVersion({0})>".format(repr(str(self)))
 
     @property
     def public(self):
+        # type: () -> str
         return self._version
 
     @property
     def base_version(self):
+        # type: () -> str
         return self._version
 
     @property
+    def epoch(self):
+        # type: () -> int
+        return -1
+
+    @property
+    def release(self):
+        # type: () -> None
+        return None
+
+    @property
+    def pre(self):
+        # type: () -> None
+        return None
+
+    @property
+    def post(self):
+        # type: () -> None
+        return None
+
+    @property
+    def dev(self):
+        # type: () -> None
+        return None
+
+    @property
     def local(self):
+        # type: () -> None
         return None
 
     @property
     def is_prerelease(self):
+        # type: () -> bool
         return False
 
     @property
     def is_postrelease(self):
+        # type: () -> bool
         return False
 
+    @property
+    def is_devrelease(self):
+        # type: () -> bool
+        return False
 
-_legacy_version_component_re = re.compile(
-    r"(\d+ | [a-z]+ | \.| -)", re.VERBOSE,
-)
+
+_legacy_version_component_re = re.compile(r"(\d+ | [a-z]+ | \.| -)", re.VERBOSE)
 
 _legacy_version_replacement_map = {
-    "pre": "c", "preview": "c", "-": "final-", "rc": "c", "dev": "@",
+    "pre": "c",
+    "preview": "c",
+    "-": "final-",
+    "rc": "c",
+    "dev": "@",
 }
 
 
 def _parse_version_parts(s):
+    # type: (str) -> Iterator[str]
     for part in _legacy_version_component_re.split(s):
         part = _legacy_version_replacement_map.get(part, part)
 
         if not part or part == ".":
             continue
 
         if part[:1] in "0123456789":
@@ -125,38 +199,40 @@
             yield "*" + part
 
     # ensure that alpha/beta/candidate are before final
     yield "*final"
 
 
 def _legacy_cmpkey(version):
+    # type: (str) -> LegacyCmpKey
+
     # We hardcode an epoch of -1 here. A PEP 440 version can only have a epoch
     # greater than or equal to 0. This will effectively put the LegacyVersion,
     # which uses the defacto standard originally implemented by setuptools,
     # as before all PEP 440 versions.
     epoch = -1
 
     # This scheme is taken from pkg_resources.parse_version setuptools prior to
     # it's adoption of the packaging library.
-    parts = []
+    parts = []  # type: List[str]
     for part in _parse_version_parts(version.lower()):
         if part.startswith("*"):
             # remove "-" before a prerelease tag
             if part < "*final":
                 while parts and parts[-1] == "*final-":
                     parts.pop()
 
             # remove trailing zeros from each series of numeric parts
             while parts and parts[-1] == "00000000":
                 parts.pop()
 
         parts.append(part)
-    parts = tuple(parts)
 
-    return epoch, parts
+    return epoch, tuple(parts)
+
 
 # Deliberately not anchored to the start and end of the string, to make it
 # easier for 3rd party code to reuse
 VERSION_PATTERN = r"""
     v?
     (?:
         (?:(?P<epoch>[0-9]+)!)?                           # epoch
@@ -186,120 +262,171 @@
     )
     (?:\+(?P<local>[a-z0-9]+(?:[-_\.][a-z0-9]+)*))?       # local version
 """
 
 
 class Version(_BaseVersion):
 
-    _regex = re.compile(
-        r"^\s*" + VERSION_PATTERN + r"\s*$",
-        re.VERBOSE | re.IGNORECASE,
-    )
+    _regex = re.compile(r"^\s*" + VERSION_PATTERN + r"\s*$", re.VERBOSE | re.IGNORECASE)
 
     def __init__(self, version):
+        # type: (str) -> None
+
         # Validate the version and parse it into pieces
         match = self._regex.search(version)
         if not match:
             raise InvalidVersion("Invalid version: '{0}'".format(version))
 
         # Store the parsed out pieces of the version
         self._version = _Version(
             epoch=int(match.group("epoch")) if match.group("epoch") else 0,
             release=tuple(int(i) for i in match.group("release").split(".")),
-            pre=_parse_letter_version(
-                match.group("pre_l"),
-                match.group("pre_n"),
-            ),
+            pre=_parse_letter_version(match.group("pre_l"), match.group("pre_n")),
             post=_parse_letter_version(
-                match.group("post_l"),
-                match.group("post_n1") or match.group("post_n2"),
-            ),
-            dev=_parse_letter_version(
-                match.group("dev_l"),
-                match.group("dev_n"),
+                match.group("post_l"), match.group("post_n1") or match.group("post_n2")
             ),
+            dev=_parse_letter_version(match.group("dev_l"), match.group("dev_n")),
             local=_parse_local_version(match.group("local")),
         )
 
         # Generate a key which will be used for sorting
         self._key = _cmpkey(
             self._version.epoch,
             self._version.release,
             self._version.pre,
             self._version.post,
             self._version.dev,
             self._version.local,
         )
 
     def __repr__(self):
+        # type: () -> str
         return "<Version({0})>".format(repr(str(self)))
 
     def __str__(self):
+        # type: () -> str
         parts = []
 
         # Epoch
-        if self._version.epoch != 0:
-            parts.append("{0}!".format(self._version.epoch))
+        if self.epoch != 0:
+            parts.append("{0}!".format(self.epoch))
 
         # Release segment
-        parts.append(".".join(str(x) for x in self._version.release))
+        parts.append(".".join(str(x) for x in self.release))
 
         # Pre-release
-        if self._version.pre is not None:
-            parts.append("".join(str(x) for x in self._version.pre))
+        if self.pre is not None:
+            parts.append("".join(str(x) for x in self.pre))
 
         # Post-release
-        if self._version.post is not None:
-            parts.append(".post{0}".format(self._version.post[1]))
+        if self.post is not None:
+            parts.append(".post{0}".format(self.post))
 
         # Development release
-        if self._version.dev is not None:
-            parts.append(".dev{0}".format(self._version.dev[1]))
+        if self.dev is not None:
+            parts.append(".dev{0}".format(self.dev))
 
         # Local version segment
-        if self._version.local is not None:
-            parts.append(
-                "+{0}".format(".".join(str(x) for x in self._version.local))
-            )
+        if self.local is not None:
+            parts.append("+{0}".format(self.local))
 
         return "".join(parts)
 
     @property
+    def epoch(self):
+        # type: () -> int
+        _epoch = self._version.epoch  # type: int
+        return _epoch
+
+    @property
+    def release(self):
+        # type: () -> Tuple[int, ...]
+        _release = self._version.release  # type: Tuple[int, ...]
+        return _release
+
+    @property
+    def pre(self):
+        # type: () -> Optional[Tuple[str, int]]
+        _pre = self._version.pre  # type: Optional[Tuple[str, int]]
+        return _pre
+
+    @property
+    def post(self):
+        # type: () -> Optional[Tuple[str, int]]
+        return self._version.post[1] if self._version.post else None
+
+    @property
+    def dev(self):
+        # type: () -> Optional[Tuple[str, int]]
+        return self._version.dev[1] if self._version.dev else None
+
+    @property
+    def local(self):
+        # type: () -> Optional[str]
+        if self._version.local:
+            return ".".join(str(x) for x in self._version.local)
+        else:
+            return None
+
+    @property
     def public(self):
+        # type: () -> str
         return str(self).split("+", 1)[0]
 
     @property
     def base_version(self):
+        # type: () -> str
         parts = []
 
         # Epoch
-        if self._version.epoch != 0:
-            parts.append("{0}!".format(self._version.epoch))
+        if self.epoch != 0:
+            parts.append("{0}!".format(self.epoch))
 
         # Release segment
-        parts.append(".".join(str(x) for x in self._version.release))
+        parts.append(".".join(str(x) for x in self.release))
 
         return "".join(parts)
 
     @property
-    def local(self):
-        version_string = str(self)
-        if "+" in version_string:
-            return version_string.split("+", 1)[1]
-
-    @property
     def is_prerelease(self):
-        return bool(self._version.dev or self._version.pre)
+        # type: () -> bool
+        return self.dev is not None or self.pre is not None
 
     @property
     def is_postrelease(self):
-        return bool(self._version.post)
+        # type: () -> bool
+        return self.post is not None
 
+    @property
+    def is_devrelease(self):
+        # type: () -> bool
+        return self.dev is not None
+
+    @property
+    def major(self):
+        # type: () -> int
+        return self.release[0] if len(self.release) >= 1 else 0
+
+    @property
+    def minor(self):
+        # type: () -> int
+        return self.release[1] if len(self.release) >= 2 else 0
+
+    @property
+    def micro(self):
+        # type: () -> int
+        return self.release[2] if len(self.release) >= 3 else 0
+
+
+def _parse_letter_version(
+    letter,  # type: str
+    number,  # type: Union[str, bytes, SupportsInt]
+):
+    # type: (...) -> Optional[Tuple[str, int]]
 
-def _parse_letter_version(letter, number):
     if letter:
         # We consider there to be an implicit 0 in a pre-release if there is
         # not a numeral associated with it.
         if number is None:
             number = 0
 
         # We normalize any letters to their lower case form
@@ -321,73 +448,88 @@
     if not letter and number:
         # We assume if we are given a number, but we are not given a letter
         # then this is using the implicit post release syntax (e.g. 1.0-1)
         letter = "post"
 
         return letter, int(number)
 
+    return None
+
 
-_local_version_seperators = re.compile(r"[\._-]")
+_local_version_separators = re.compile(r"[\._-]")
 
 
 def _parse_local_version(local):
+    # type: (str) -> Optional[LocalType]
     """
     Takes a string like abc.1.twelve and turns it into ("abc", 1, "twelve").
     """
     if local is not None:
         return tuple(
             part.lower() if not part.isdigit() else int(part)
-            for part in _local_version_seperators.split(local)
+            for part in _local_version_separators.split(local)
         )
+    return None
 
 
-def _cmpkey(epoch, release, pre, post, dev, local):
+def _cmpkey(
+    epoch,  # type: int
+    release,  # type: Tuple[int, ...]
+    pre,  # type: Optional[Tuple[str, int]]
+    post,  # type: Optional[Tuple[str, int]]
+    dev,  # type: Optional[Tuple[str, int]]
+    local,  # type: Optional[Tuple[SubLocalType]]
+):
+    # type: (...) -> CmpKey
+
     # When we compare a release version, we want to compare it with all of the
     # trailing zeros removed. So we'll use a reverse the list, drop all the now
     # leading zeros until we come to something non zero, then take the rest
     # re-reverse it back into the correct order and make it a tuple and use
     # that for our sorting key.
-    release = tuple(
-        reversed(list(
-            itertools.dropwhile(
-                lambda x: x == 0,
-                reversed(release),
-            )
-        ))
+    _release = tuple(
+        reversed(list(itertools.dropwhile(lambda x: x == 0, reversed(release))))
     )
 
     # We need to "trick" the sorting algorithm to put 1.0.dev0 before 1.0a0.
     # We'll do this by abusing the pre segment, but we _only_ want to do this
     # if there is not a pre or a post segment. If we have one of those then
     # the normal sorting rules will handle this case correctly.
     if pre is None and post is None and dev is not None:
-        pre = -Infinity
+        _pre = NegativeInfinity  # type: PrePostDevType
     # Versions without a pre-release (except as noted above) should sort after
     # those with one.
     elif pre is None:
-        pre = Infinity
+        _pre = Infinity
+    else:
+        _pre = pre
 
     # Versions without a post segment should sort before those with one.
     if post is None:
-        post = -Infinity
+        _post = NegativeInfinity  # type: PrePostDevType
+
+    else:
+        _post = post
 
     # Versions without a development segment should sort after those with one.
     if dev is None:
-        dev = Infinity
+        _dev = Infinity  # type: PrePostDevType
+
+    else:
+        _dev = dev
 
     if local is None:
         # Versions without a local segment should sort before those with one.
-        local = -Infinity
+        _local = NegativeInfinity  # type: LocalType
     else:
         # Versions with a local segment need that segment parsed to implement
         # the sorting rules in PEP440.
         # - Alpha numeric segments sort before numeric segments
         # - Alpha numeric segments sort lexicographically
         # - Numeric segments sort numerically
         # - Shorter versions sort before longer versions when the prefixes
         #   match exactly
-        local = tuple(
-            (i, "") if isinstance(i, int) else (-Infinity, i)
-            for i in local
+        _local = tuple(
+            (i, "") if isinstance(i, int) else (NegativeInfinity, i) for i in local
         )
 
-    return epoch, release, pre, post, dev, local
+    return epoch, _release, _pre, _post, _dev, _local
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/_vendor/pyparsing.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/pkg_resources/extern/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/extern/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import importlib.util
 import sys
 
 
 class VendorImporter:
     """
     A PEP 302 meta path importer for finding optionally-vendored
     or otherwise naturally-installed packages from root_name.
@@ -16,25 +17,18 @@
     def search_path(self):
         """
         Search first the vendor package then as a natural package.
         """
         yield self.vendor_pkg + '.'
         yield ''
 
-    def find_module(self, fullname, path=None):
-        """
-        Return self when fullname starts with root_name and the
-        target module is one vendored through this importer.
-        """
+    def _module_matches_namespace(self, fullname):
+        """Figure out if the target module is vendored."""
         root, base, target = fullname.partition(self.root_name + '.')
-        if root:
-            return
-        if not any(map(target.startswith, self.vendored_names)):
-            return
-        return self
+        return not root and any(map(target.startswith, self.vendored_names))
 
     def load_module(self, fullname):
         """
         Iterate over the search path to locate and load fullname.
         """
         root, base, target = fullname.partition(self.root_name + '.')
         for prefix in self.search_path:
@@ -50,17 +44,30 @@
             raise ImportError(
                 "The '{target}' package is required; "
                 "normally this is bundled with this package so if you get "
                 "this warning, consult the packager of your "
                 "distribution.".format(**locals())
             )
 
+    def create_module(self, spec):
+        return self.load_module(spec.name)
+
+    def exec_module(self, module):
+        pass
+
+    def find_spec(self, fullname, path=None, target=None):
+        """Return a module spec for vendored names."""
+        return (
+            importlib.util.spec_from_loader(fullname, self)
+            if self._module_matches_namespace(fullname) else None
+        )
+
     def install(self):
         """
         Install this importer into sys.meta_path if not already present.
         """
         if self not in sys.meta_path:
             sys.meta_path.append(self)
 
 
-names = 'packaging', 'pyparsing', 'six', 'appdirs'
-VendorImporter(__name__, names).install()
+names = 'packaging', 'pyparsing', 'ordered_set',
+VendorImporter(__name__, names, 'setuptools._vendor').install()
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 """Extensions to the 'distutils' for large or complex distributions"""
 
-import os
+from fnmatch import fnmatchcase
 import functools
-import distutils.core
-import distutils.filelist
+import os
 import re
+
+import _distutils_hack.override  # noqa: F401
+
+import distutils.core
 from distutils.errors import DistutilsOptionError
 from distutils.util import convert_path
-from fnmatch import fnmatchcase
 
 from ._deprecation_warning import SetuptoolsDeprecationWarning
 
-from setuptools.extern.six import PY3, string_types
-from setuptools.extern.six.moves import filter, map
-
 import setuptools.version
 from setuptools.extension import Extension
 from setuptools.dist import Distribution
 from setuptools.depends import Require
 from . import monkey
 
-__metaclass__ = type
-
 
 __all__ = [
     'setup', 'Distribution', 'Command', 'Extension', 'Require',
     'SetuptoolsDeprecationWarning',
-    'find_packages'
+    'find_packages', 'find_namespace_packages',
 ]
 
-if PY3:
-    __all__.append('find_namespace_packages')
-
 __version__ = setuptools.version.__version__
 
 bootstrap_install_from = None
 
 # If we run 2to3 on .py files, should we also convert docstrings?
 # Default: yes; assume that we can detect doctests reliably
 run_2to3_on_doctests = True
@@ -116,26 +110,41 @@
 class PEP420PackageFinder(PackageFinder):
     @staticmethod
     def _looks_like_package(path):
         return True
 
 
 find_packages = PackageFinder.find
-
-if PY3:
-    find_namespace_packages = PEP420PackageFinder.find
+find_namespace_packages = PEP420PackageFinder.find
 
 
 def _install_setup_requires(attrs):
     # Note: do not use `setuptools.Distribution` directly, as
     # our PEP 517 backend patch `distutils.core.Distribution`.
-    dist = distutils.core.Distribution(dict(
-        (k, v) for k, v in attrs.items()
-        if k in ('dependency_links', 'setup_requires')
-    ))
+    class MinimalDistribution(distutils.core.Distribution):
+        """
+        A minimal version of a distribution for supporting the
+        fetch_build_eggs interface.
+        """
+        def __init__(self, attrs):
+            _incl = 'dependency_links', 'setup_requires'
+            filtered = {
+                k: attrs[k]
+                for k in set(_incl) & set(attrs)
+            }
+            distutils.core.Distribution.__init__(self, filtered)
+
+        def finalize_options(self):
+            """
+            Disable finalize_options to avoid building the working set.
+            Ref #2158.
+            """
+
+    dist = MinimalDistribution(attrs)
+
     # Honor setup.cfg's options.
     dist.parse_config_files(ignore_option_errors=True)
     if dist.setup_requires:
         dist.fetch_build_eggs(dist.setup_requires)
 
 
 def setup(**attrs):
@@ -164,33 +173,33 @@
         vars(self).update(kw)
 
     def _ensure_stringlike(self, option, what, default=None):
         val = getattr(self, option)
         if val is None:
             setattr(self, option, default)
             return default
-        elif not isinstance(val, string_types):
+        elif not isinstance(val, str):
             raise DistutilsOptionError("'%s' must be a %s (got `%s`)"
                                        % (option, what, val))
         return val
 
     def ensure_string_list(self, option):
         r"""Ensure that 'option' is a list of strings.  If 'option' is
         currently a string, we split it either on /,\s*/ or /\s+/, so
         "foo bar baz", "foo,bar,baz", and "foo,   bar baz" all become
         ["foo", "bar", "baz"].
         """
         val = getattr(self, option)
         if val is None:
             return
-        elif isinstance(val, string_types):
+        elif isinstance(val, str):
             setattr(self, option, re.split(r',\s*|\s+', val))
         else:
             if isinstance(val, list):
-                ok = all(isinstance(v, string_types) for v in val)
+                ok = all(isinstance(v, str) for v in val)
             else:
                 ok = False
             if not ok:
                 raise DistutilsOptionError(
                     "'%s' must be a list of strings (got %r)"
                     % (option, val))
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_imp.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/ordered_set.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/__about__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,14 @@
     "__copyright__",
 ]
 
 __title__ = "packaging"
 __summary__ = "Core utilities for Python packages"
 __uri__ = "https://github.com/pypa/packaging"
 
-__version__ = "19.2"
+__version__ = "20.4"
 
 __author__ = "Donald Stufft and individual contributors"
 __email__ = "donald@stufft.io"
 
-__license__ = "BSD or Apache License, Version 2.0"
+__license__ = "BSD-2-Clause or Apache-2.0"
 __copyright__ = "Copyright 2014-2019 %s" % __author__
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/_compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 from __future__ import absolute_import, division, print_function
 
 import sys
 
+from ._typing import TYPE_CHECKING
+
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, Dict, Tuple, Type
+
 
 PY2 = sys.version_info[0] == 2
 PY3 = sys.version_info[0] == 3
 
 # flake8: noqa
 
 if PY3:
     string_types = (str,)
 else:
     string_types = (basestring,)
 
 
 def with_metaclass(meta, *bases):
+    # type: (Type[Any], Tuple[Type[Any], ...]) -> Any
     """
     Create a base class with a metaclass.
     """
     # This requires a bit of explanation: the basic idea is to make a dummy
     # metaclass for one level of class instantiation that replaces itself with
     # the actual metaclass.
-    class metaclass(meta):
+    class metaclass(meta):  # type: ignore
         def __new__(cls, name, this_bases, d):
+            # type: (Type[Any], str, Tuple[Any], Dict[Any, Any]) -> Any
             return meta(name, bases, d)
 
     return type.__new__(metaclass, "temporary_class", (), {})
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/markers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,22 @@
 import sys
 
 from setuptools.extern.pyparsing import ParseException, ParseResults, stringStart, stringEnd
 from setuptools.extern.pyparsing import ZeroOrMore, Group, Forward, QuotedString
 from setuptools.extern.pyparsing import Literal as L  # noqa
 
 from ._compat import string_types
+from ._typing import TYPE_CHECKING
 from .specifiers import Specifier, InvalidSpecifier
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+
+    Operator = Callable[[str, str], bool]
+
 
 __all__ = [
     "InvalidMarker",
     "UndefinedComparison",
     "UndefinedEnvironmentName",
     "Marker",
     "default_environment",
@@ -42,38 +48,45 @@
     A name was attempted to be used that does not exist inside of the
     environment.
     """
 
 
 class Node(object):
     def __init__(self, value):
+        # type: (Any) -> None
         self.value = value
 
     def __str__(self):
+        # type: () -> str
         return str(self.value)
 
     def __repr__(self):
+        # type: () -> str
         return "<{0}({1!r})>".format(self.__class__.__name__, str(self))
 
     def serialize(self):
+        # type: () -> str
         raise NotImplementedError
 
 
 class Variable(Node):
     def serialize(self):
+        # type: () -> str
         return str(self)
 
 
 class Value(Node):
     def serialize(self):
+        # type: () -> str
         return '"{0}"'.format(self)
 
 
 class Op(Node):
     def serialize(self):
+        # type: () -> str
         return str(self)
 
 
 VARIABLE = (
     L("implementation_version")
     | L("platform_python_implementation")
     | L("implementation_name")
@@ -81,21 +94,21 @@
     | L("platform_release")
     | L("platform_version")
     | L("platform_machine")
     | L("platform_system")
     | L("python_version")
     | L("sys_platform")
     | L("os_name")
-    | L("os.name")
+    | L("os.name")  # PEP-345
     | L("sys.platform")  # PEP-345
     | L("platform.version")  # PEP-345
     | L("platform.machine")  # PEP-345
     | L("platform.python_implementation")  # PEP-345
-    | L("python_implementation")  # PEP-345
-    | L("extra")  # undocumented setuptools legacy
+    | L("python_implementation")  # undocumented setuptools legacy
+    | L("extra")  # PEP-508
 )
 ALIASES = {
     "os.name": "os_name",
     "sys.platform": "sys_platform",
     "platform.version": "platform_version",
     "platform.machine": "platform_machine",
     "platform.python_implementation": "platform_python_implementation",
@@ -127,21 +140,24 @@
 MARKER_ATOM = MARKER_ITEM | Group(LPAREN + MARKER_EXPR + RPAREN)
 MARKER_EXPR << MARKER_ATOM + ZeroOrMore(BOOLOP + MARKER_EXPR)
 
 MARKER = stringStart + MARKER_EXPR + stringEnd
 
 
 def _coerce_parse_result(results):
+    # type: (Union[ParseResults, List[Any]]) -> List[Any]
     if isinstance(results, ParseResults):
         return [_coerce_parse_result(i) for i in results]
     else:
         return results
 
 
 def _format_marker(marker, first=True):
+    # type: (Union[List[str], Tuple[Node, ...], str], Optional[bool]) -> str
+
     assert isinstance(marker, (list, tuple, string_types))
 
     # Sometimes we have a structure like [[...]] which is a single item list
     # where the single item is itself it's own list. In that case we want skip
     # the rest of this function so that we don't get extraneous () on the
     # outside.
     if (
@@ -168,50 +184,57 @@
     "not in": lambda lhs, rhs: lhs not in rhs,
     "<": operator.lt,
     "<=": operator.le,
     "==": operator.eq,
     "!=": operator.ne,
     ">=": operator.ge,
     ">": operator.gt,
-}
+}  # type: Dict[str, Operator]
 
 
 def _eval_op(lhs, op, rhs):
+    # type: (str, Op, str) -> bool
     try:
         spec = Specifier("".join([op.serialize(), rhs]))
     except InvalidSpecifier:
         pass
     else:
         return spec.contains(lhs)
 
-    oper = _operators.get(op.serialize())
+    oper = _operators.get(op.serialize())  # type: Optional[Operator]
     if oper is None:
         raise UndefinedComparison(
             "Undefined {0!r} on {1!r} and {2!r}.".format(op, lhs, rhs)
         )
 
     return oper(lhs, rhs)
 
 
-_undefined = object()
+class Undefined(object):
+    pass
+
+
+_undefined = Undefined()
 
 
 def _get_env(environment, name):
-    value = environment.get(name, _undefined)
+    # type: (Dict[str, str], str) -> str
+    value = environment.get(name, _undefined)  # type: Union[str, Undefined]
 
-    if value is _undefined:
+    if isinstance(value, Undefined):
         raise UndefinedEnvironmentName(
             "{0!r} does not exist in evaluation environment.".format(name)
         )
 
     return value
 
 
 def _evaluate_markers(markers, environment):
-    groups = [[]]
+    # type: (List[Any], Dict[str, str]) -> bool
+    groups = [[]]  # type: List[List[bool]]
 
     for marker in markers:
         assert isinstance(marker, (list, tuple, string_types))
 
         if isinstance(marker, list):
             groups[-1].append(_evaluate_markers(marker, environment))
         elif isinstance(marker, tuple):
@@ -230,25 +253,30 @@
             if marker == "or":
                 groups.append([])
 
     return any(all(item) for item in groups)
 
 
 def format_full_version(info):
+    # type: (sys._version_info) -> str
     version = "{0.major}.{0.minor}.{0.micro}".format(info)
     kind = info.releaselevel
     if kind != "final":
         version += kind[0] + str(info.serial)
     return version
 
 
 def default_environment():
+    # type: () -> Dict[str, str]
     if hasattr(sys, "implementation"):
-        iver = format_full_version(sys.implementation.version)
-        implementation_name = sys.implementation.name
+        # Ignoring the `sys.implementation` reference for type checking due to
+        # mypy not liking that the attribute doesn't exist in Python 2.7 when
+        # run with the `--py27` flag.
+        iver = format_full_version(sys.implementation.version)  # type: ignore
+        implementation_name = sys.implementation.name  # type: ignore
     else:
         iver = "0"
         implementation_name = ""
 
     return {
         "implementation_name": implementation_name,
         "implementation_version": iver,
@@ -262,29 +290,33 @@
         "python_version": ".".join(platform.python_version_tuple()[:2]),
         "sys_platform": sys.platform,
     }
 
 
 class Marker(object):
     def __init__(self, marker):
+        # type: (str) -> None
         try:
             self._markers = _coerce_parse_result(MARKER.parseString(marker))
         except ParseException as e:
             err_str = "Invalid marker: {0!r}, parse error at {1!r}".format(
                 marker, marker[e.loc : e.loc + 8]
             )
             raise InvalidMarker(err_str)
 
     def __str__(self):
+        # type: () -> str
         return _format_marker(self._markers)
 
     def __repr__(self):
+        # type: () -> str
         return "<Marker({0!r})>".format(str(self))
 
     def evaluate(self, environment=None):
+        # type: (Optional[Dict[str, str]]) -> bool
         """Evaluate a marker.
 
         Return the boolean from evaluating the given marker against the
         environment. environment is an optional argument to override all or
         part of the determined environment.
 
         The environment is determined from the current Python process.
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/requirements.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 
 import string
 import re
 
 from setuptools.extern.pyparsing import stringStart, stringEnd, originalTextFor, ParseException
 from setuptools.extern.pyparsing import ZeroOrMore, Word, Optional, Regex, Combine
 from setuptools.extern.pyparsing import Literal as L  # noqa
-from setuptools.extern.six.moves.urllib import parse as urlparse
+from urllib import parse as urlparse
 
+from ._typing import TYPE_CHECKING
 from .markers import MARKER_EXPR, Marker
 from .specifiers import LegacySpecifier, Specifier, SpecifierSet
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import List
+
 
 class InvalidRequirement(ValueError):
     """
     An invalid requirement was found, users should refer to PEP 508.
     """
 
 
@@ -85,14 +89,15 @@
 
     # TODO: Can we test whether something is contained within a requirement?
     #       If so how do we do that? Do we need to test against the _name_ of
     #       the thing as well as the version? What about the markers?
     # TODO: Can we normalize the name and extra name?
 
     def __init__(self, requirement_string):
+        # type: (str) -> None
         try:
             req = REQUIREMENT.parseString(requirement_string)
         except ParseException as e:
             raise InvalidRequirement(
                 'Parse error at "{0!r}": {1}'.format(
                     requirement_string[e.loc : e.loc + 8], e.msg
                 )
@@ -112,15 +117,16 @@
         else:
             self.url = None
         self.extras = set(req.extras.asList() if req.extras else [])
         self.specifier = SpecifierSet(req.specifier)
         self.marker = req.marker if req.marker else None
 
     def __str__(self):
-        parts = [self.name]
+        # type: () -> str
+        parts = [self.name]  # type: List[str]
 
         if self.extras:
             parts.append("[{0}]".format(",".join(sorted(self.extras))))
 
         if self.specifier:
             parts.append(str(self.specifier))
 
@@ -131,8 +137,9 @@
 
         if self.marker:
             parts.append("; {0}".format(self.marker))
 
         return "".join(parts)
 
     def __repr__(self):
+        # type: () -> str
         return "<Requirement({0!r})>".format(str(self))
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/specifiers.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,177 +5,233 @@
 
 import abc
 import functools
 import itertools
 import re
 
 from ._compat import string_types, with_metaclass
+from ._typing import TYPE_CHECKING
+from .utils import canonicalize_version
 from .version import Version, LegacyVersion, parse
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import (
+        List,
+        Dict,
+        Union,
+        Iterable,
+        Iterator,
+        Optional,
+        Callable,
+        Tuple,
+        FrozenSet,
+    )
+
+    ParsedVersion = Union[Version, LegacyVersion]
+    UnparsedVersion = Union[Version, LegacyVersion, str]
+    CallableOperator = Callable[[ParsedVersion, str], bool]
+
 
 class InvalidSpecifier(ValueError):
     """
     An invalid specifier was found, users should refer to PEP 440.
     """
 
 
-class BaseSpecifier(with_metaclass(abc.ABCMeta, object)):
+class BaseSpecifier(with_metaclass(abc.ABCMeta, object)):  # type: ignore
     @abc.abstractmethod
     def __str__(self):
+        # type: () -> str
         """
         Returns the str representation of this Specifier like object. This
         should be representative of the Specifier itself.
         """
 
     @abc.abstractmethod
     def __hash__(self):
+        # type: () -> int
         """
         Returns a hash value for this Specifier like object.
         """
 
     @abc.abstractmethod
     def __eq__(self, other):
+        # type: (object) -> bool
         """
         Returns a boolean representing whether or not the two Specifier like
         objects are equal.
         """
 
     @abc.abstractmethod
     def __ne__(self, other):
+        # type: (object) -> bool
         """
         Returns a boolean representing whether or not the two Specifier like
         objects are not equal.
         """
 
     @abc.abstractproperty
     def prereleases(self):
+        # type: () -> Optional[bool]
         """
         Returns whether or not pre-releases as a whole are allowed by this
         specifier.
         """
 
     @prereleases.setter
     def prereleases(self, value):
+        # type: (bool) -> None
         """
         Sets whether or not pre-releases as a whole are allowed by this
         specifier.
         """
 
     @abc.abstractmethod
     def contains(self, item, prereleases=None):
+        # type: (str, Optional[bool]) -> bool
         """
         Determines if the given item is contained within this specifier.
         """
 
     @abc.abstractmethod
     def filter(self, iterable, prereleases=None):
+        # type: (Iterable[UnparsedVersion], Optional[bool]) -> Iterable[UnparsedVersion]
         """
         Takes an iterable of items and filters them so that only items which
         are contained within this specifier are allowed in it.
         """
 
 
 class _IndividualSpecifier(BaseSpecifier):
 
-    _operators = {}
+    _operators = {}  # type: Dict[str, str]
 
     def __init__(self, spec="", prereleases=None):
+        # type: (str, Optional[bool]) -> None
         match = self._regex.search(spec)
         if not match:
             raise InvalidSpecifier("Invalid specifier: '{0}'".format(spec))
 
-        self._spec = (match.group("operator").strip(), match.group("version").strip())
+        self._spec = (
+            match.group("operator").strip(),
+            match.group("version").strip(),
+        )  # type: Tuple[str, str]
 
         # Store whether or not this Specifier should accept prereleases
         self._prereleases = prereleases
 
     def __repr__(self):
+        # type: () -> str
         pre = (
             ", prereleases={0!r}".format(self.prereleases)
             if self._prereleases is not None
             else ""
         )
 
         return "<{0}({1!r}{2})>".format(self.__class__.__name__, str(self), pre)
 
     def __str__(self):
+        # type: () -> str
         return "{0}{1}".format(*self._spec)
 
+    @property
+    def _canonical_spec(self):
+        # type: () -> Tuple[str, Union[Version, str]]
+        return self._spec[0], canonicalize_version(self._spec[1])
+
     def __hash__(self):
-        return hash(self._spec)
+        # type: () -> int
+        return hash(self._canonical_spec)
 
     def __eq__(self, other):
+        # type: (object) -> bool
         if isinstance(other, string_types):
             try:
-                other = self.__class__(other)
+                other = self.__class__(str(other))
             except InvalidSpecifier:
                 return NotImplemented
         elif not isinstance(other, self.__class__):
             return NotImplemented
 
-        return self._spec == other._spec
+        return self._canonical_spec == other._canonical_spec
 
     def __ne__(self, other):
+        # type: (object) -> bool
         if isinstance(other, string_types):
             try:
-                other = self.__class__(other)
+                other = self.__class__(str(other))
             except InvalidSpecifier:
                 return NotImplemented
         elif not isinstance(other, self.__class__):
             return NotImplemented
 
         return self._spec != other._spec
 
     def _get_operator(self, op):
-        return getattr(self, "_compare_{0}".format(self._operators[op]))
+        # type: (str) -> CallableOperator
+        operator_callable = getattr(
+            self, "_compare_{0}".format(self._operators[op])
+        )  # type: CallableOperator
+        return operator_callable
 
     def _coerce_version(self, version):
+        # type: (UnparsedVersion) -> ParsedVersion
         if not isinstance(version, (LegacyVersion, Version)):
             version = parse(version)
         return version
 
     @property
     def operator(self):
+        # type: () -> str
         return self._spec[0]
 
     @property
     def version(self):
+        # type: () -> str
         return self._spec[1]
 
     @property
     def prereleases(self):
+        # type: () -> Optional[bool]
         return self._prereleases
 
     @prereleases.setter
     def prereleases(self, value):
+        # type: (bool) -> None
         self._prereleases = value
 
     def __contains__(self, item):
+        # type: (str) -> bool
         return self.contains(item)
 
     def contains(self, item, prereleases=None):
+        # type: (UnparsedVersion, Optional[bool]) -> bool
+
         # Determine if prereleases are to be allowed or not.
         if prereleases is None:
             prereleases = self.prereleases
 
         # Normalize item to a Version or LegacyVersion, this allows us to have
         # a shortcut for ``"2.0" in Specifier(">=2")
-        item = self._coerce_version(item)
+        normalized_item = self._coerce_version(item)
 
         # Determine if we should be supporting prereleases in this specifier
         # or not, if we do not support prereleases than we can short circuit
         # logic if this version is a prereleases.
-        if item.is_prerelease and not prereleases:
+        if normalized_item.is_prerelease and not prereleases:
             return False
 
         # Actually do the comparison to determine if this item is contained
         # within this Specifier or not.
-        return self._get_operator(self.operator)(item, self.version)
+        operator_callable = self._get_operator(self.operator)  # type: CallableOperator
+        return operator_callable(normalized_item, self.version)
 
     def filter(self, iterable, prereleases=None):
+        # type: (Iterable[UnparsedVersion], Optional[bool]) -> Iterable[UnparsedVersion]
+
         yielded = False
         found_prereleases = []
 
         kw = {"prereleases": prereleases if prereleases is not None else True}
 
         # Attempt to iterate over all the values in the iterable and if any of
         # them match, yield them.
@@ -226,40 +282,51 @@
         "<=": "less_than_equal",
         ">=": "greater_than_equal",
         "<": "less_than",
         ">": "greater_than",
     }
 
     def _coerce_version(self, version):
+        # type: (Union[ParsedVersion, str]) -> LegacyVersion
         if not isinstance(version, LegacyVersion):
             version = LegacyVersion(str(version))
         return version
 
     def _compare_equal(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective == self._coerce_version(spec)
 
     def _compare_not_equal(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective != self._coerce_version(spec)
 
     def _compare_less_than_equal(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective <= self._coerce_version(spec)
 
     def _compare_greater_than_equal(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective >= self._coerce_version(spec)
 
     def _compare_less_than(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective < self._coerce_version(spec)
 
     def _compare_greater_than(self, prospective, spec):
+        # type: (LegacyVersion, str) -> bool
         return prospective > self._coerce_version(spec)
 
 
-def _require_version_compare(fn):
+def _require_version_compare(
+    fn  # type: (Callable[[Specifier, ParsedVersion, str], bool])
+):
+    # type: (...) -> Callable[[Specifier, ParsedVersion, str], bool]
     @functools.wraps(fn)
     def wrapped(self, prospective, spec):
+        # type: (Specifier, ParsedVersion, str) -> bool
         if not isinstance(prospective, Version):
             return False
         return fn(self, prospective, spec)
 
     return wrapped
 
 
@@ -369,14 +436,16 @@
         "<": "less_than",
         ">": "greater_than",
         "===": "arbitrary",
     }
 
     @_require_version_compare
     def _compare_compatible(self, prospective, spec):
+        # type: (ParsedVersion, str) -> bool
+
         # Compatible releases have an equivalent combination of >= and ==. That
         # is that ~=2.2 is equivalent to >=2.2,==2.*. This allows us to
         # implement this in terms of the other specifiers instead of
         # implementing it ourselves. The only thing we need to do is construct
         # the other specifiers.
 
         # We want everything but the last item in the version, but we want to
@@ -396,64 +465,83 @@
 
         return self._get_operator(">=")(prospective, spec) and self._get_operator("==")(
             prospective, prefix
         )
 
     @_require_version_compare
     def _compare_equal(self, prospective, spec):
+        # type: (ParsedVersion, str) -> bool
+
         # We need special logic to handle prefix matching
         if spec.endswith(".*"):
             # In the case of prefix matching we want to ignore local segment.
             prospective = Version(prospective.public)
             # Split the spec out by dots, and pretend that there is an implicit
             # dot in between a release segment and a pre-release segment.
-            spec = _version_split(spec[:-2])  # Remove the trailing .*
+            split_spec = _version_split(spec[:-2])  # Remove the trailing .*
 
             # Split the prospective version out by dots, and pretend that there
             # is an implicit dot in between a release segment and a pre-release
             # segment.
-            prospective = _version_split(str(prospective))
+            split_prospective = _version_split(str(prospective))
 
             # Shorten the prospective version to be the same length as the spec
             # so that we can determine if the specifier is a prefix of the
             # prospective version or not.
-            prospective = prospective[: len(spec)]
+            shortened_prospective = split_prospective[: len(split_spec)]
 
             # Pad out our two sides with zeros so that they both equal the same
             # length.
-            spec, prospective = _pad_version(spec, prospective)
+            padded_spec, padded_prospective = _pad_version(
+                split_spec, shortened_prospective
+            )
+
+            return padded_prospective == padded_spec
         else:
             # Convert our spec string into a Version
-            spec = Version(spec)
+            spec_version = Version(spec)
 
             # If the specifier does not have a local segment, then we want to
             # act as if the prospective version also does not have a local
             # segment.
-            if not spec.local:
+            if not spec_version.local:
                 prospective = Version(prospective.public)
 
-        return prospective == spec
+            return prospective == spec_version
 
     @_require_version_compare
     def _compare_not_equal(self, prospective, spec):
+        # type: (ParsedVersion, str) -> bool
         return not self._compare_equal(prospective, spec)
 
     @_require_version_compare
     def _compare_less_than_equal(self, prospective, spec):
-        return prospective <= Version(spec)
+        # type: (ParsedVersion, str) -> bool
+
+        # NB: Local version identifiers are NOT permitted in the version
+        # specifier, so local version labels can be universally removed from
+        # the prospective version.
+        return Version(prospective.public) <= Version(spec)
 
     @_require_version_compare
     def _compare_greater_than_equal(self, prospective, spec):
-        return prospective >= Version(spec)
+        # type: (ParsedVersion, str) -> bool
+
+        # NB: Local version identifiers are NOT permitted in the version
+        # specifier, so local version labels can be universally removed from
+        # the prospective version.
+        return Version(prospective.public) >= Version(spec)
 
     @_require_version_compare
-    def _compare_less_than(self, prospective, spec):
+    def _compare_less_than(self, prospective, spec_str):
+        # type: (ParsedVersion, str) -> bool
+
         # Convert our spec to a Version instance, since we'll want to work with
         # it as a version.
-        spec = Version(spec)
+        spec = Version(spec_str)
 
         # Check to see if the prospective version is less than the spec
         # version. If it's not we can short circuit and just return False now
         # instead of doing extra unneeded work.
         if not prospective < spec:
             return False
 
@@ -467,18 +555,20 @@
 
         # If we've gotten to here, it means that prospective version is both
         # less than the spec version *and* it's not a pre-release of the same
         # version in the spec.
         return True
 
     @_require_version_compare
-    def _compare_greater_than(self, prospective, spec):
+    def _compare_greater_than(self, prospective, spec_str):
+        # type: (ParsedVersion, str) -> bool
+
         # Convert our spec to a Version instance, since we'll want to work with
         # it as a version.
-        spec = Version(spec)
+        spec = Version(spec_str)
 
         # Check to see if the prospective version is greater than the spec
         # version. If it's not we can short circuit and just return False now
         # instead of doing extra unneeded work.
         if not prospective > spec:
             return False
 
@@ -498,18 +588,21 @@
 
         # If we've gotten to here, it means that prospective version is both
         # greater than the spec version *and* it's not a pre-release of the
         # same version in the spec.
         return True
 
     def _compare_arbitrary(self, prospective, spec):
+        # type: (Version, str) -> bool
         return str(prospective).lower() == str(spec).lower()
 
     @property
     def prereleases(self):
+        # type: () -> bool
+
         # If there is an explicit prereleases set for this, then we'll just
         # blindly use that.
         if self._prereleases is not None:
             return self._prereleases
 
         # Look at all of our specifiers and determine if they are inclusive
         # operators, and if they are if they are including an explicit
@@ -526,32 +619,35 @@
             if parse(version).is_prerelease:
                 return True
 
         return False
 
     @prereleases.setter
     def prereleases(self, value):
+        # type: (bool) -> None
         self._prereleases = value
 
 
 _prefix_regex = re.compile(r"^([0-9]+)((?:a|b|c|rc)[0-9]+)$")
 
 
 def _version_split(version):
-    result = []
+    # type: (str) -> List[str]
+    result = []  # type: List[str]
     for item in version.split("."):
         match = _prefix_regex.search(item)
         if match:
             result.extend(match.groups())
         else:
             result.append(item)
     return result
 
 
 def _pad_version(left, right):
+    # type: (List[str], List[str]) -> Tuple[List[str], List[str]]
     left_split, right_split = [], []
 
     # Get the release segment of our versions
     left_split.append(list(itertools.takewhile(lambda x: x.isdigit(), left)))
     right_split.append(list(itertools.takewhile(lambda x: x.isdigit(), right)))
 
     # Get the rest of our versions
@@ -563,50 +659,56 @@
     right_split.insert(1, ["0"] * max(0, len(left_split[0]) - len(right_split[0])))
 
     return (list(itertools.chain(*left_split)), list(itertools.chain(*right_split)))
 
 
 class SpecifierSet(BaseSpecifier):
     def __init__(self, specifiers="", prereleases=None):
-        # Split on , to break each indidivual specifier into it's own item, and
+        # type: (str, Optional[bool]) -> None
+
+        # Split on , to break each individual specifier into it's own item, and
         # strip each item to remove leading/trailing whitespace.
-        specifiers = [s.strip() for s in specifiers.split(",") if s.strip()]
+        split_specifiers = [s.strip() for s in specifiers.split(",") if s.strip()]
 
         # Parsed each individual specifier, attempting first to make it a
         # Specifier and falling back to a LegacySpecifier.
         parsed = set()
-        for specifier in specifiers:
+        for specifier in split_specifiers:
             try:
                 parsed.add(Specifier(specifier))
             except InvalidSpecifier:
                 parsed.add(LegacySpecifier(specifier))
 
         # Turn our parsed specifiers into a frozen set and save them for later.
         self._specs = frozenset(parsed)
 
         # Store our prereleases value so we can use it later to determine if
         # we accept prereleases or not.
         self._prereleases = prereleases
 
     def __repr__(self):
+        # type: () -> str
         pre = (
             ", prereleases={0!r}".format(self.prereleases)
             if self._prereleases is not None
             else ""
         )
 
         return "<SpecifierSet({0!r}{1})>".format(str(self), pre)
 
     def __str__(self):
+        # type: () -> str
         return ",".join(sorted(str(s) for s in self._specs))
 
     def __hash__(self):
+        # type: () -> int
         return hash(self._specs)
 
     def __and__(self, other):
+        # type: (Union[SpecifierSet, str]) -> SpecifierSet
         if isinstance(other, string_types):
             other = SpecifierSet(other)
         elif not isinstance(other, SpecifierSet):
             return NotImplemented
 
         specifier = SpecifierSet()
         specifier._specs = frozenset(self._specs | other._specs)
@@ -622,41 +724,43 @@
                 "Cannot combine SpecifierSets with True and False prerelease "
                 "overrides."
             )
 
         return specifier
 
     def __eq__(self, other):
-        if isinstance(other, string_types):
-            other = SpecifierSet(other)
-        elif isinstance(other, _IndividualSpecifier):
+        # type: (object) -> bool
+        if isinstance(other, (string_types, _IndividualSpecifier)):
             other = SpecifierSet(str(other))
         elif not isinstance(other, SpecifierSet):
             return NotImplemented
 
         return self._specs == other._specs
 
     def __ne__(self, other):
-        if isinstance(other, string_types):
-            other = SpecifierSet(other)
-        elif isinstance(other, _IndividualSpecifier):
+        # type: (object) -> bool
+        if isinstance(other, (string_types, _IndividualSpecifier)):
             other = SpecifierSet(str(other))
         elif not isinstance(other, SpecifierSet):
             return NotImplemented
 
         return self._specs != other._specs
 
     def __len__(self):
+        # type: () -> int
         return len(self._specs)
 
     def __iter__(self):
+        # type: () -> Iterator[FrozenSet[_IndividualSpecifier]]
         return iter(self._specs)
 
     @property
     def prereleases(self):
+        # type: () -> Optional[bool]
+
         # If we have been given an explicit prerelease modifier, then we'll
         # pass that through here.
         if self._prereleases is not None:
             return self._prereleases
 
         # If we don't have any specifiers, and we don't have a forced value,
         # then we'll just return None since we don't know if this should have
@@ -666,20 +770,24 @@
 
         # Otherwise we'll see if any of the given specifiers accept
         # prereleases, if any of them do we'll return True, otherwise False.
         return any(s.prereleases for s in self._specs)
 
     @prereleases.setter
     def prereleases(self, value):
+        # type: (bool) -> None
         self._prereleases = value
 
     def __contains__(self, item):
+        # type: (Union[ParsedVersion, str]) -> bool
         return self.contains(item)
 
     def contains(self, item, prereleases=None):
+        # type: (Union[ParsedVersion, str], Optional[bool]) -> bool
+
         # Ensure that our item is a Version or LegacyVersion instance.
         if not isinstance(item, (LegacyVersion, Version)):
             item = parse(item)
 
         # Determine if we're forcing a prerelease or not, if we're not forcing
         # one for this particular filter call, then we'll use whatever the
         # SpecifierSet thinks for whether or not we should support prereleases.
@@ -697,15 +805,21 @@
 
         # We simply dispatch to the underlying specs here to make sure that the
         # given version is contained within all of them.
         # Note: This use of all() here means that an empty set of specifiers
         #       will always return True, this is an explicit design decision.
         return all(s.contains(item, prereleases=prereleases) for s in self._specs)
 
-    def filter(self, iterable, prereleases=None):
+    def filter(
+        self,
+        iterable,  # type: Iterable[Union[ParsedVersion, str]]
+        prereleases=None,  # type: Optional[bool]
+    ):
+        # type: (...) -> Iterable[Union[ParsedVersion, str]]
+
         # Determine if we're forcing a prerelease or not, if we're not forcing
         # one for this particular filter call, then we'll use whatever the
         # SpecifierSet thinks for whether or not we should support prereleases.
         if prereleases is None:
             prereleases = self.prereleases
 
         # If we have any specifiers, then we want to wrap our iterable in the
@@ -715,16 +829,16 @@
             for spec in self._specs:
                 iterable = spec.filter(iterable, prereleases=bool(prereleases))
             return iterable
         # If we do not have any specifiers, then we need to have a rough filter
         # which will filter out any pre-releases, unless there are no final
         # releases, and which will filter out LegacyVersion in general.
         else:
-            filtered = []
-            found_prereleases = []
+            filtered = []  # type: List[Union[ParsedVersion, str]]
+            found_prereleases = []  # type: List[Union[ParsedVersion, str]]
 
             for item in iterable:
                 # Ensure that we some kind of Version class for this item.
                 if not isinstance(item, (LegacyVersion, Version)):
                     parsed_version = parse(item)
                 else:
                     parsed_version = item
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/utils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 from __future__ import absolute_import, division, print_function
 
 import re
 
+from ._typing import TYPE_CHECKING, cast
 from .version import InvalidVersion, Version
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import NewType, Union
+
+    NormalizedName = NewType("NormalizedName", str)
 
 _canonicalize_regex = re.compile(r"[-_.]+")
 
 
 def canonicalize_name(name):
+    # type: (str) -> NormalizedName
     # This is taken from PEP 503.
-    return _canonicalize_regex.sub("-", name).lower()
+    value = _canonicalize_regex.sub("-", name).lower()
+    return cast("NormalizedName", value)
 
 
-def canonicalize_version(version):
+def canonicalize_version(_version):
+    # type: (str) -> Union[Version, str]
     """
-    This is very similar to Version.__str__, but has one subtle differences
+    This is very similar to Version.__str__, but has one subtle difference
     with the way it handles the release segment.
     """
 
     try:
-        version = Version(version)
+        version = Version(_version)
     except InvalidVersion:
         # Legacy versions cannot be normalized
-        return version
+        return _version
 
     parts = []
 
     # Epoch
     if version.epoch != 0:
         parts.append("{0}!".format(version.epoch))
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/packaging/version.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,54 @@
 # for complete details.
 from __future__ import absolute_import, division, print_function
 
 import collections
 import itertools
 import re
 
-from ._structures import Infinity
+from ._structures import Infinity, NegativeInfinity
+from ._typing import TYPE_CHECKING
 
+if TYPE_CHECKING:  # pragma: no cover
+    from typing import Callable, Iterator, List, Optional, SupportsInt, Tuple, Union
+
+    from ._structures import InfinityType, NegativeInfinityType
+
+    InfiniteTypes = Union[InfinityType, NegativeInfinityType]
+    PrePostDevType = Union[InfiniteTypes, Tuple[str, int]]
+    SubLocalType = Union[InfiniteTypes, int, str]
+    LocalType = Union[
+        NegativeInfinityType,
+        Tuple[
+            Union[
+                SubLocalType,
+                Tuple[SubLocalType, str],
+                Tuple[NegativeInfinityType, SubLocalType],
+            ],
+            ...,
+        ],
+    ]
+    CmpKey = Tuple[
+        int, Tuple[int, ...], PrePostDevType, PrePostDevType, PrePostDevType, LocalType
+    ]
+    LegacyCmpKey = Tuple[int, Tuple[str, ...]]
+    VersionComparisonMethod = Callable[
+        [Union[CmpKey, LegacyCmpKey], Union[CmpKey, LegacyCmpKey]], bool
+    ]
 
 __all__ = ["parse", "Version", "LegacyVersion", "InvalidVersion", "VERSION_PATTERN"]
 
 
 _Version = collections.namedtuple(
     "_Version", ["epoch", "release", "dev", "pre", "post", "local"]
 )
 
 
 def parse(version):
+    # type: (str) -> Union[LegacyVersion, Version]
     """
     Parse the given version string and return either a :class:`Version` object
     or a :class:`LegacyVersion` object depending on if the given version is
     a valid PEP 440 version or a legacy version.
     """
     try:
         return Version(version)
@@ -33,95 +61,119 @@
 class InvalidVersion(ValueError):
     """
     An invalid version was found, users should refer to PEP 440.
     """
 
 
 class _BaseVersion(object):
+    _key = None  # type: Union[CmpKey, LegacyCmpKey]
+
     def __hash__(self):
+        # type: () -> int
         return hash(self._key)
 
     def __lt__(self, other):
+        # type: (_BaseVersion) -> bool
         return self._compare(other, lambda s, o: s < o)
 
     def __le__(self, other):
+        # type: (_BaseVersion) -> bool
         return self._compare(other, lambda s, o: s <= o)
 
     def __eq__(self, other):
+        # type: (object) -> bool
         return self._compare(other, lambda s, o: s == o)
 
     def __ge__(self, other):
+        # type: (_BaseVersion) -> bool
         return self._compare(other, lambda s, o: s >= o)
 
     def __gt__(self, other):
+        # type: (_BaseVersion) -> bool
         return self._compare(other, lambda s, o: s > o)
 
     def __ne__(self, other):
+        # type: (object) -> bool
         return self._compare(other, lambda s, o: s != o)
 
     def _compare(self, other, method):
+        # type: (object, VersionComparisonMethod) -> Union[bool, NotImplemented]
         if not isinstance(other, _BaseVersion):
             return NotImplemented
 
         return method(self._key, other._key)
 
 
 class LegacyVersion(_BaseVersion):
     def __init__(self, version):
+        # type: (str) -> None
         self._version = str(version)
         self._key = _legacy_cmpkey(self._version)
 
     def __str__(self):
+        # type: () -> str
         return self._version
 
     def __repr__(self):
+        # type: () -> str
         return "<LegacyVersion({0})>".format(repr(str(self)))
 
     @property
     def public(self):
+        # type: () -> str
         return self._version
 
     @property
     def base_version(self):
+        # type: () -> str
         return self._version
 
     @property
     def epoch(self):
+        # type: () -> int
         return -1
 
     @property
     def release(self):
+        # type: () -> None
         return None
 
     @property
     def pre(self):
+        # type: () -> None
         return None
 
     @property
     def post(self):
+        # type: () -> None
         return None
 
     @property
     def dev(self):
+        # type: () -> None
         return None
 
     @property
     def local(self):
+        # type: () -> None
         return None
 
     @property
     def is_prerelease(self):
+        # type: () -> bool
         return False
 
     @property
     def is_postrelease(self):
+        # type: () -> bool
         return False
 
     @property
     def is_devrelease(self):
+        # type: () -> bool
         return False
 
 
 _legacy_version_component_re = re.compile(r"(\d+ | [a-z]+ | \.| -)", re.VERBOSE)
 
 _legacy_version_replacement_map = {
     "pre": "c",
@@ -129,14 +181,15 @@
     "-": "final-",
     "rc": "c",
     "dev": "@",
 }
 
 
 def _parse_version_parts(s):
+    # type: (str) -> Iterator[str]
     for part in _legacy_version_component_re.split(s):
         part = _legacy_version_replacement_map.get(part, part)
 
         if not part or part == ".":
             continue
 
         if part[:1] in "0123456789":
@@ -146,38 +199,39 @@
             yield "*" + part
 
     # ensure that alpha/beta/candidate are before final
     yield "*final"
 
 
 def _legacy_cmpkey(version):
+    # type: (str) -> LegacyCmpKey
+
     # We hardcode an epoch of -1 here. A PEP 440 version can only have a epoch
     # greater than or equal to 0. This will effectively put the LegacyVersion,
     # which uses the defacto standard originally implemented by setuptools,
     # as before all PEP 440 versions.
     epoch = -1
 
     # This scheme is taken from pkg_resources.parse_version setuptools prior to
     # it's adoption of the packaging library.
-    parts = []
+    parts = []  # type: List[str]
     for part in _parse_version_parts(version.lower()):
         if part.startswith("*"):
             # remove "-" before a prerelease tag
             if part < "*final":
                 while parts and parts[-1] == "*final-":
                     parts.pop()
 
             # remove trailing zeros from each series of numeric parts
             while parts and parts[-1] == "00000000":
                 parts.pop()
 
         parts.append(part)
-    parts = tuple(parts)
 
-    return epoch, parts
+    return epoch, tuple(parts)
 
 
 # Deliberately not anchored to the start and end of the string, to make it
 # easier for 3rd party code to reuse
 VERSION_PATTERN = r"""
     v?
     (?:
@@ -211,14 +265,16 @@
 
 
 class Version(_BaseVersion):
 
     _regex = re.compile(r"^\s*" + VERSION_PATTERN + r"\s*$", re.VERBOSE | re.IGNORECASE)
 
     def __init__(self, version):
+        # type: (str) -> None
+
         # Validate the version and parse it into pieces
         match = self._regex.search(version)
         if not match:
             raise InvalidVersion("Invalid version: '{0}'".format(version))
 
         # Store the parsed out pieces of the version
         self._version = _Version(
@@ -239,17 +295,19 @@
             self._version.pre,
             self._version.post,
             self._version.dev,
             self._version.local,
         )
 
     def __repr__(self):
+        # type: () -> str
         return "<Version({0})>".format(repr(str(self)))
 
     def __str__(self):
+        # type: () -> str
         parts = []
 
         # Epoch
         if self.epoch != 0:
             parts.append("{0}!".format(self.epoch))
 
         # Release segment
@@ -271,70 +329,104 @@
         if self.local is not None:
             parts.append("+{0}".format(self.local))
 
         return "".join(parts)
 
     @property
     def epoch(self):
-        return self._version.epoch
+        # type: () -> int
+        _epoch = self._version.epoch  # type: int
+        return _epoch
 
     @property
     def release(self):
-        return self._version.release
+        # type: () -> Tuple[int, ...]
+        _release = self._version.release  # type: Tuple[int, ...]
+        return _release
 
     @property
     def pre(self):
-        return self._version.pre
+        # type: () -> Optional[Tuple[str, int]]
+        _pre = self._version.pre  # type: Optional[Tuple[str, int]]
+        return _pre
 
     @property
     def post(self):
+        # type: () -> Optional[Tuple[str, int]]
         return self._version.post[1] if self._version.post else None
 
     @property
     def dev(self):
+        # type: () -> Optional[Tuple[str, int]]
         return self._version.dev[1] if self._version.dev else None
 
     @property
     def local(self):
+        # type: () -> Optional[str]
         if self._version.local:
             return ".".join(str(x) for x in self._version.local)
         else:
             return None
 
     @property
     def public(self):
+        # type: () -> str
         return str(self).split("+", 1)[0]
 
     @property
     def base_version(self):
+        # type: () -> str
         parts = []
 
         # Epoch
         if self.epoch != 0:
             parts.append("{0}!".format(self.epoch))
 
         # Release segment
         parts.append(".".join(str(x) for x in self.release))
 
         return "".join(parts)
 
     @property
     def is_prerelease(self):
+        # type: () -> bool
         return self.dev is not None or self.pre is not None
 
     @property
     def is_postrelease(self):
+        # type: () -> bool
         return self.post is not None
 
     @property
     def is_devrelease(self):
+        # type: () -> bool
         return self.dev is not None
 
+    @property
+    def major(self):
+        # type: () -> int
+        return self.release[0] if len(self.release) >= 1 else 0
+
+    @property
+    def minor(self):
+        # type: () -> int
+        return self.release[1] if len(self.release) >= 2 else 0
+
+    @property
+    def micro(self):
+        # type: () -> int
+        return self.release[2] if len(self.release) >= 3 else 0
+
+
+def _parse_letter_version(
+    letter,  # type: str
+    number,  # type: Union[str, bytes, SupportsInt]
+):
+    # type: (...) -> Optional[Tuple[str, int]]
 
-def _parse_letter_version(letter, number):
     if letter:
         # We consider there to be an implicit 0 in a pre-release if there is
         # not a numeral associated with it.
         if number is None:
             number = 0
 
         # We normalize any letters to their lower case form
@@ -356,65 +448,88 @@
     if not letter and number:
         # We assume if we are given a number, but we are not given a letter
         # then this is using the implicit post release syntax (e.g. 1.0-1)
         letter = "post"
 
         return letter, int(number)
 
+    return None
+
 
 _local_version_separators = re.compile(r"[\._-]")
 
 
 def _parse_local_version(local):
+    # type: (str) -> Optional[LocalType]
     """
     Takes a string like abc.1.twelve and turns it into ("abc", 1, "twelve").
     """
     if local is not None:
         return tuple(
             part.lower() if not part.isdigit() else int(part)
             for part in _local_version_separators.split(local)
         )
+    return None
 
 
-def _cmpkey(epoch, release, pre, post, dev, local):
+def _cmpkey(
+    epoch,  # type: int
+    release,  # type: Tuple[int, ...]
+    pre,  # type: Optional[Tuple[str, int]]
+    post,  # type: Optional[Tuple[str, int]]
+    dev,  # type: Optional[Tuple[str, int]]
+    local,  # type: Optional[Tuple[SubLocalType]]
+):
+    # type: (...) -> CmpKey
+
     # When we compare a release version, we want to compare it with all of the
     # trailing zeros removed. So we'll use a reverse the list, drop all the now
     # leading zeros until we come to something non zero, then take the rest
     # re-reverse it back into the correct order and make it a tuple and use
     # that for our sorting key.
-    release = tuple(
+    _release = tuple(
         reversed(list(itertools.dropwhile(lambda x: x == 0, reversed(release))))
     )
 
     # We need to "trick" the sorting algorithm to put 1.0.dev0 before 1.0a0.
     # We'll do this by abusing the pre segment, but we _only_ want to do this
     # if there is not a pre or a post segment. If we have one of those then
     # the normal sorting rules will handle this case correctly.
     if pre is None and post is None and dev is not None:
-        pre = -Infinity
+        _pre = NegativeInfinity  # type: PrePostDevType
     # Versions without a pre-release (except as noted above) should sort after
     # those with one.
     elif pre is None:
-        pre = Infinity
+        _pre = Infinity
+    else:
+        _pre = pre
 
     # Versions without a post segment should sort before those with one.
     if post is None:
-        post = -Infinity
+        _post = NegativeInfinity  # type: PrePostDevType
+
+    else:
+        _post = post
 
     # Versions without a development segment should sort after those with one.
     if dev is None:
-        dev = Infinity
+        _dev = Infinity  # type: PrePostDevType
+
+    else:
+        _dev = dev
 
     if local is None:
         # Versions without a local segment should sort before those with one.
-        local = -Infinity
+        _local = NegativeInfinity  # type: LocalType
     else:
         # Versions with a local segment need that segment parsed to implement
         # the sorting rules in PEP440.
         # - Alpha numeric segments sort before numeric segments
         # - Alpha numeric segments sort lexicographically
         # - Numeric segments sort numerically
         # - Shorter versions sort before longer versions when the prefixes
         #   match exactly
-        local = tuple((i, "") if isinstance(i, int) else (-Infinity, i) for i in local)
+        _local = tuple(
+            (i, "") if isinstance(i, int) else (NegativeInfinity, i) for i in local
+        )
 
-    return epoch, release, pre, post, dev, local
+    return epoch, _release, _pre, _post, _dev, _local
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/_vendor/pyparsing.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/archive_util.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/archive_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,55 +121,85 @@
                 with open(target, 'wb') as f:
                     f.write(data)
             unix_attributes = info.external_attr >> 16
             if unix_attributes:
                 os.chmod(target, unix_attributes)
 
 
+def _resolve_tar_file_or_dir(tar_obj, tar_member_obj):
+    """Resolve any links and extract link targets as normal files."""
+    while tar_member_obj is not None and (
+            tar_member_obj.islnk() or tar_member_obj.issym()):
+        linkpath = tar_member_obj.linkname
+        if tar_member_obj.issym():
+            base = posixpath.dirname(tar_member_obj.name)
+            linkpath = posixpath.join(base, linkpath)
+            linkpath = posixpath.normpath(linkpath)
+        tar_member_obj = tar_obj._getmember(linkpath)
+
+    is_file_or_dir = (
+        tar_member_obj is not None and
+        (tar_member_obj.isfile() or tar_member_obj.isdir())
+    )
+    if is_file_or_dir:
+        return tar_member_obj
+
+    raise LookupError('Got unknown file type')
+
+
+def _iter_open_tar(tar_obj, extract_dir, progress_filter):
+    """Emit member-destination pairs from a tar archive."""
+    # don't do any chowning!
+    tar_obj.chown = lambda *args: None
+
+    with contextlib.closing(tar_obj):
+        for member in tar_obj:
+            name = member.name
+            # don't extract absolute paths or ones with .. in them
+            if name.startswith('/') or '..' in name.split('/'):
+                continue
+
+            prelim_dst = os.path.join(extract_dir, *name.split('/'))
+
+            try:
+                member = _resolve_tar_file_or_dir(tar_obj, member)
+            except LookupError:
+                continue
+
+            final_dst = progress_filter(name, prelim_dst)
+            if not final_dst:
+                continue
+
+            if final_dst.endswith(os.sep):
+                final_dst = final_dst[:-1]
+
+            yield member, final_dst
+
+
 def unpack_tarfile(filename, extract_dir, progress_filter=default_filter):
     """Unpack tar/tar.gz/tar.bz2 `filename` to `extract_dir`
 
     Raises ``UnrecognizedFormat`` if `filename` is not a tarfile (as determined
     by ``tarfile.open()``).  See ``unpack_archive()`` for an explanation
     of the `progress_filter` argument.
     """
     try:
         tarobj = tarfile.open(filename)
-    except tarfile.TarError:
+    except tarfile.TarError as e:
         raise UnrecognizedFormat(
             "%s is not a compressed or uncompressed tar file" % (filename,)
-        )
-    with contextlib.closing(tarobj):
-        # don't do any chowning!
-        tarobj.chown = lambda *args: None
-        for member in tarobj:
-            name = member.name
-            # don't extract absolute paths or ones with .. in them
-            if not name.startswith('/') and '..' not in name.split('/'):
-                prelim_dst = os.path.join(extract_dir, *name.split('/'))
+        ) from e
+
+    for member, final_dst in _iter_open_tar(
+            tarobj, extract_dir, progress_filter,
+    ):
+        try:
+            # XXX Ugh
+            tarobj._extract_member(member, final_dst)
+        except tarfile.ExtractError:
+            # chown/chmod/mkfifo/mknode/makedev failed
+            pass
 
-                # resolve any links and to extract the link targets as normal
-                # files
-                while member is not None and (
-                        member.islnk() or member.issym()):
-                    linkpath = member.linkname
-                    if member.issym():
-                        base = posixpath.dirname(member.name)
-                        linkpath = posixpath.join(base, linkpath)
-                        linkpath = posixpath.normpath(linkpath)
-                    member = tarobj._getmember(linkpath)
-
-                if member is not None and (member.isfile() or member.isdir()):
-                    final_dst = progress_filter(name, prelim_dst)
-                    if final_dst:
-                        if final_dst.endswith(os.sep):
-                            final_dst = final_dst[:-1]
-                        try:
-                            # XXX Ugh
-                            tarobj._extract_member(member, final_dst)
-                        except tarfile.ExtractError:
-                            # chown/chmod/mkfifo/mknode/makedev failed
-                            pass
-        return True
+    return True
 
 
 extraction_drivers = unpack_directory, unpack_zipfile, unpack_tarfile
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/build_meta.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/build_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,20 @@
 
 import io
 import os
 import sys
 import tokenize
 import shutil
 import contextlib
+import tempfile
 
 import setuptools
 import distutils
-from setuptools.py31compat import TemporaryDirectory
 
 from pkg_resources import parse_requirements
-from pkg_resources.py31compat import makedirs
 
 __all__ = ['get_requires_for_build_sdist',
            'get_requires_for_build_wheel',
            'prepare_metadata_for_build_wheel',
            'build_wheel',
            'build_sdist',
            '__legacy__',
@@ -72,38 +71,46 @@
         distutils.core.Distribution = cls
         try:
             yield
         finally:
             distutils.core.Distribution = orig
 
 
-def _to_str(s):
+@contextlib.contextmanager
+def no_install_setup_requires():
+    """Temporarily disable installing setup_requires
+
+    Under PEP 517, the backend reports build dependencies to the frontend,
+    and the frontend is responsible for ensuring they're installed.
+    So setuptools (acting as a backend) should not try to install them.
     """
-    Convert a filename to a string (on Python 2, explicitly
-    a byte string, not Unicode) as distutils checks for the
-    exact type str.
-    """
-    if sys.version_info[0] == 2 and not isinstance(s, str):
-        # Assume it's Unicode, as that's what the PEP says
-        # should be provided.
-        return s.encode(sys.getfilesystemencoding())
-    return s
+    orig = setuptools._install_setup_requires
+    setuptools._install_setup_requires = lambda attrs: None
+    try:
+        yield
+    finally:
+        setuptools._install_setup_requires = orig
 
 
 def _get_immediate_subdirectories(a_dir):
     return [name for name in os.listdir(a_dir)
             if os.path.isdir(os.path.join(a_dir, name))]
 
 
 def _file_with_extension(directory, extension):
     matching = (
         f for f in os.listdir(directory)
         if f.endswith(extension)
     )
-    file, = matching
+    try:
+        file, = matching
+    except ValueError:
+        raise ValueError(
+            'No distribution was found. Ensure that `setup.py` '
+            'is not empty and that it calls `setup()`.')
     return file
 
 
 def _open_setup_script(setup_script):
     if not os.path.exists(setup_script):
         # Supply a default setup.py
         return io.StringIO(u"from setuptools import setup; setup()")
@@ -149,17 +156,18 @@
 
     def get_requires_for_build_sdist(self, config_settings=None):
         config_settings = self._fix_config(config_settings)
         return self._get_build_requires(config_settings, requirements=[])
 
     def prepare_metadata_for_build_wheel(self, metadata_directory,
                                          config_settings=None):
-        sys.argv = sys.argv[:1] + ['dist_info', '--egg-base',
-                                   _to_str(metadata_directory)]
-        self.run_setup()
+        sys.argv = sys.argv[:1] + [
+            'dist_info', '--egg-base', metadata_directory]
+        with no_install_setup_requires():
+            self.run_setup()
 
         dist_info_directory = metadata_directory
         while True:
             dist_infos = [f for f in os.listdir(dist_info_directory)
                           if f.endswith('.dist-info')]
 
             if (
@@ -186,20 +194,21 @@
 
     def _build_with_temp_dir(self, setup_command, result_extension,
                              result_directory, config_settings):
         config_settings = self._fix_config(config_settings)
         result_directory = os.path.abspath(result_directory)
 
         # Build in a temporary directory, then copy to the target.
-        makedirs(result_directory, exist_ok=True)
-        with TemporaryDirectory(dir=result_directory) as tmp_dist_dir:
+        os.makedirs(result_directory, exist_ok=True)
+        with tempfile.TemporaryDirectory(dir=result_directory) as tmp_dist_dir:
             sys.argv = (sys.argv[:1] + setup_command +
                         ['--dist-dir', tmp_dist_dir] +
                         config_settings["--global-option"])
-            self.run_setup()
+            with no_install_setup_requires():
+                self.run_setup()
 
             result_basename = _file_with_extension(
                 tmp_dist_dir, result_extension)
             result_path = os.path.join(result_directory, result_basename)
             if os.path.exists(result_path):
                 # os.rename will fail overwriting on non-Unix.
                 os.remove(result_path)
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/cli-32.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/cli-64.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/cli.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __all__ = [
     'alias', 'bdist_egg', 'bdist_rpm', 'build_ext', 'build_py', 'develop',
     'easy_install', 'egg_info', 'install', 'install_lib', 'rotate', 'saveopts',
     'sdist', 'setopt', 'test', 'install_egg_info', 'install_scripts',
-    'bdist_wininst', 'upload_docs', 'build_clib', 'dist_info',
+    'upload_docs', 'build_clib', 'dist_info',
 ]
 
 from distutils.command.bdist import bdist
 import sys
 
 from setuptools.command import install_scripts
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/alias.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from distutils.errors import DistutilsOptionError
 
-from setuptools.extern.six.moves import map
-
 from setuptools.command.setopt import edit_config, option_base, config_file
 
 
 def shquote(arg):
     """Quote an argument for later parsing by shlex.split()"""
     for c in '"', "'", "\\", "#":
         if c in arg:
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/bdist_egg.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 """setuptools.command.bdist_egg
 
 Build .egg distributions"""
 
-from distutils.errors import DistutilsSetupError
 from distutils.dir_util import remove_tree, mkpath
 from distutils import log
 from types import CodeType
 import sys
 import os
 import re
 import textwrap
 import marshal
-import warnings
-
-from setuptools.extern import six
 
 from pkg_resources import get_build_platform, Distribution, ensure_directory
-from pkg_resources import EntryPoint
 from setuptools.extension import Library
-from setuptools import Command, SetuptoolsDeprecationWarning
+from setuptools import Command
+
+from sysconfig import get_path, get_python_version
 
-try:
-    # Python 2.7 or >=3.2
-    from sysconfig import get_path, get_python_version
-
-    def _get_purelib():
-        return get_path("purelib")
-except ImportError:
-    from distutils.sysconfig import get_python_lib, get_python_version
 
-    def _get_purelib():
-        return get_python_lib(False)
+def _get_purelib():
+    return get_path("purelib")
 
 
 def strip_module(filename):
     if '.' in filename:
         filename = os.path.splitext(filename)[0]
     if filename.endswith('module'):
         filename = filename[:-6]
@@ -51,18 +40,20 @@
         yield base, dirs, files
 
 
 def write_stub(resource, pyfile):
     _stub_template = textwrap.dedent("""
         def __bootstrap__():
             global __bootstrap__, __loader__, __file__
-            import sys, pkg_resources, imp
+            import sys, pkg_resources, importlib.util
             __file__ = pkg_resources.resource_filename(__name__, %r)
             __loader__ = None; del __bootstrap__, __loader__
-            imp.load_dynamic(__name__,__file__)
+            spec = importlib.util.spec_from_file_location(__name__,__file__)
+            mod = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(mod)
         __bootstrap__()
         """).lstrip()
     with open(pyfile, 'w') as f:
         f.write(_stub_template % resource)
 
 
 class bdist_egg(Command):
@@ -155,15 +146,15 @@
             kw.setdefault(dirname, self.bdist_dir)
         kw.setdefault('skip_build', self.skip_build)
         kw.setdefault('dry_run', self.dry_run)
         cmd = self.reinitialize_command(cmdname, **kw)
         self.run_command(cmdname)
         return cmd
 
-    def run(self):
+    def run(self):  # noqa: C901  # is too complex (14)  # FIXME
         # Generate metadata first
         self.run_command("egg_info")
         # We run install_lib before install_data, because some data hacks
         # pull their data path from the install_lib command.
         log.info("installing library code to %s", self.bdist_dir)
         instcmd = self.get_finalized_command('install')
         old_root = instcmd.root
@@ -270,57 +261,15 @@
         safe = getattr(self.distribution, 'zip_safe', None)
         if safe is not None:
             return safe
         log.warn("zip_safe flag not set; analyzing archive contents...")
         return analyze_egg(self.bdist_dir, self.stubs)
 
     def gen_header(self):
-        epm = EntryPoint.parse_map(self.distribution.entry_points or '')
-        ep = epm.get('setuptools.installation', {}).get('eggsecutable')
-        if ep is None:
-            return 'w'  # not an eggsecutable, do it the usual way.
-
-        warnings.warn(
-            "Eggsecutables are deprecated and will be removed in a future "
-            "version.",
-            SetuptoolsDeprecationWarning
-        )
-
-        if not ep.attrs or ep.extras:
-            raise DistutilsSetupError(
-                "eggsecutable entry point (%r) cannot have 'extras' "
-                "or refer to a module" % (ep,)
-            )
-
-        pyver = '{}.{}'.format(*sys.version_info)
-        pkg = ep.module_name
-        full = '.'.join(ep.attrs)
-        base = ep.attrs[0]
-        basename = os.path.basename(self.egg_output)
-
-        header = (
-            "#!/bin/sh\n"
-            'if [ `basename $0` = "%(basename)s" ]\n'
-            'then exec python%(pyver)s -c "'
-            "import sys, os; sys.path.insert(0, os.path.abspath('$0')); "
-            "from %(pkg)s import %(base)s; sys.exit(%(full)s())"
-            '" "$@"\n'
-            'else\n'
-            '  echo $0 is not the correct name for this egg file.\n'
-            '  echo Please rename it back to %(basename)s and try again.\n'
-            '  exec false\n'
-            'fi\n'
-        ) % locals()
-
-        if not self.dry_run:
-            mkpath(os.path.dirname(self.egg_output), dry_run=self.dry_run)
-            f = open(self.egg_output, 'w')
-            f.write(header)
-            f.close()
-        return 'a'
+        return 'w'
 
     def copy_metadata_to(self, target_dir):
         "Copy metadata (egg info) to the target_dir"
         # normalize the path (so that a forward-slash in egg_info will
         # match using startswith below)
         norm_egg_info = os.path.normpath(self.egg_info)
         prefix = os.path.join(norm_egg_info, '')
@@ -414,17 +363,15 @@
     """Check whether module possibly uses unsafe-for-zipfile stuff"""
 
     filename = os.path.join(base, name)
     if filename[:-1] in stubs:
         return True  # Extension module
     pkg = base[len(egg_dir) + 1:].replace(os.sep, '.')
     module = pkg + (pkg and '.' or '') + os.path.splitext(name)[0]
-    if six.PY2:
-        skip = 8  # skip magic & date
-    elif sys.version_info < (3, 7):
+    if sys.version_info < (3, 7):
         skip = 12  # skip magic & date & file size
     else:
         skip = 16  # skip magic & reserved? & date & file size
     f = open(filename, 'rb')
     f.read(skip)
     code = marshal.load(f)
     f.close()
@@ -447,15 +394,15 @@
 
 
 def iter_symbols(code):
     """Yield names and strings used by `code` and its nested code objects"""
     for name in code.co_names:
         yield name
     for const in code.co_consts:
-        if isinstance(const, six.string_types):
+        if isinstance(const, str):
             yield const
         elif isinstance(const, CodeType):
             for name in iter_symbols(const):
                 yield name
 
 
 def can_scan():
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/build_clib.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/build_ext.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/build_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 import os
 import sys
 import itertools
+from importlib.machinery import EXTENSION_SUFFIXES
 from distutils.command.build_ext import build_ext as _du_build_ext
 from distutils.file_util import copy_file
 from distutils.ccompiler import new_compiler
 from distutils.sysconfig import customize_compiler, get_config_var
 from distutils.errors import DistutilsError
 from distutils import log
 
 from setuptools.extension import Library
-from setuptools.extern import six
-
-if six.PY2:
-    import imp
-
-    EXTENSION_SUFFIXES = [
-        s for s, _, tp in imp.get_suffixes() if tp == imp.C_EXTENSION]
-else:
-    from importlib.machinery import EXTENSION_SUFFIXES
 
 try:
     # Attempt to use Cython for building extensions, if available
     from Cython.Distutils.build_ext import build_ext as _build_ext
     # Additionally, assert that the compiler module will load
     # also. Ref #1229.
     __import__('Cython.Compiler.Main')
@@ -111,19 +103,15 @@
             if ext._needs_stub:
                 self.write_stub(package_dir or os.curdir, ext, True)
 
     def get_ext_filename(self, fullname):
         filename = _build_ext.get_ext_filename(self, fullname)
         if fullname in self.ext_map:
             ext = self.ext_map[fullname]
-            use_abi3 = (
-                not six.PY2
-                and getattr(ext, 'py_limited_api')
-                and get_abi3_suffix()
-            )
+            use_abi3 = getattr(ext, 'py_limited_api') and get_abi3_suffix()
             if use_abi3:
                 so_ext = get_config_var('EXT_SUFFIX')
                 filename = filename[:-len(so_ext)]
                 filename = filename + get_abi3_suffix()
             if isinstance(ext, Library):
                 fn, ext = os.path.splitext(filename)
                 return self.shlib_compiler.library_filename(fn, libtype)
@@ -250,27 +238,31 @@
             raise DistutilsError(stub_file + " already exists! Please delete.")
         if not self.dry_run:
             f = open(stub_file, 'w')
             f.write(
                 '\n'.join([
                     "def __bootstrap__():",
                     "   global __bootstrap__, __file__, __loader__",
-                    "   import sys, os, pkg_resources, imp" + if_dl(", dl"),
+                    "   import sys, os, pkg_resources, importlib.util" +
+                    if_dl(", dl"),
                     "   __file__ = pkg_resources.resource_filename"
                     "(__name__,%r)"
                     % os.path.basename(ext._file_name),
                     "   del __bootstrap__",
                     "   if '__loader__' in globals():",
                     "       del __loader__",
                     if_dl("   old_flags = sys.getdlopenflags()"),
                     "   old_dir = os.getcwd()",
                     "   try:",
                     "     os.chdir(os.path.dirname(__file__))",
                     if_dl("     sys.setdlopenflags(dl.RTLD_NOW)"),
-                    "     imp.load_dynamic(__name__,__file__)",
+                    "     spec = importlib.util.spec_from_file_location(",
+                    "                __name__, __file__)",
+                    "     mod = importlib.util.module_from_spec(spec)",
+                    "     spec.loader.exec_module(mod)",
                     "   finally:",
                     if_dl("     sys.setdlopenflags(old_flags)"),
                     "     os.chdir(old_dir)",
                     "__bootstrap__()",
                     ""  # terminal \n
                 ])
             )
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/build_py.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/build_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 import fnmatch
 import textwrap
 import io
 import distutils.errors
 import itertools
 import stat
 
-from setuptools.extern import six
-from setuptools.extern.six.moves import map, filter, filterfalse
-
 try:
     from setuptools.lib2to3_ex import Mixin2to3
-except ImportError:
+except Exception:
 
     class Mixin2to3:
         def run_2to3(self, files, doctests=True):
             "do nothing"
 
 
 def make_writable(target):
@@ -69,17 +66,14 @@
         "lazily compute data files"
         if attr == 'data_files':
             self.data_files = self._get_data_files()
             return self.data_files
         return orig.build_py.__getattr__(self, attr)
 
     def build_module(self, module, module_file, package):
-        if six.PY2 and isinstance(package, six.string_types):
-            # avoid errors on Python 2 when unicode is passed (#190)
-            package = package.split('.')
         outfile, copied = orig.build_py.build_module(self, module, module_file,
                                                      package)
         if copied:
             self.__updated_files.append(outfile)
         return outfile, copied
 
     def _get_data_files(self):
@@ -245,15 +239,15 @@
 def _unique_everseen(iterable, key=None):
     "List unique elements, preserving order. Remember all elements ever seen."
     # unique_everseen('AAAABBBCCDAABBB') --> A B C D
     # unique_everseen('ABBCcAD', str.lower) --> A B C D
     seen = set()
     seen_add = seen.add
     if key is None:
-        for element in filterfalse(seen.__contains__, iterable):
+        for element in itertools.filterfalse(seen.__contains__, iterable):
             seen_add(element)
             yield element
     else:
         for element in iterable:
             k = key(element)
             if k not in seen:
                 seen_add(k)
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/develop.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/develop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from distutils.util import convert_path
 from distutils import log
 from distutils.errors import DistutilsError, DistutilsOptionError
 import os
 import glob
 import io
 
-from setuptools.extern import six
-
 import pkg_resources
 from setuptools.command.easy_install import easy_install
 from setuptools import namespaces
 import setuptools
 
-__metaclass__ = type
-
 
 class develop(namespaces.DevelopInstaller, easy_install):
     """Set up package for development"""
 
     description = "install package in 'development mode'"
 
     user_options = easy_install.user_options + [
@@ -104,15 +100,15 @@
             raise DistutilsOptionError(
                 "Can't get a consistent path to setup script from"
                 " installation directory", resolved,
                 pkg_resources.normalize_path(os.curdir))
         return path_to_setup
 
     def install_for_development(self):
-        if not six.PY2 and getattr(self.distribution, 'use_2to3', False):
+        if getattr(self.distribution, 'use_2to3', False):
             # If we run 2to3 we can not do this inplace:
 
             # Ensure metadata is up-to-date
             self.reinitialize_command('build_py', inplace=0)
             self.run_command('build_py')
             bpy_cmd = self.get_finalized_command("build_py")
             build_path = pkg_resources.normalize_path(bpy_cmd.build_lib)
@@ -135,15 +131,14 @@
             # Without 2to3 inplace works fine:
             self.run_command('egg_info')
 
             # Build extensions in-place
             self.reinitialize_command('build_ext', inplace=1)
             self.run_command('build_ext')
 
-        self.install_site_py()  # ensure that target dir is site-safe
         if setuptools.bootstrap_install_from:
             self.easy_install(setuptools.bootstrap_install_from)
             setuptools.bootstrap_install_from = None
 
         self.install_namespaces()
 
         # create an .egg-link in the installation dir, pointing to our egg
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/dist_info.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/easy_install.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/easy_install.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,49 +34,44 @@
 import warnings
 import site
 import struct
 import contextlib
 import subprocess
 import shlex
 import io
+import configparser
 
 
 from sysconfig import get_config_vars, get_path
 
 from setuptools import SetuptoolsDeprecationWarning
 
-from setuptools.extern import six
-from setuptools.extern.six.moves import configparser, map
-
 from setuptools import Command
 from setuptools.sandbox import run_setup
-from setuptools.py27compat import rmtree_safe
 from setuptools.command import setopt
 from setuptools.archive_util import unpack_archive
 from setuptools.package_index import (
     PackageIndex, parse_requirement_arg, URL_SCHEME,
 )
 from setuptools.command import bdist_egg, egg_info
 from setuptools.wheel import Wheel
 from pkg_resources import (
     yield_lines, normalize_path, resource_string, ensure_directory,
     get_distribution, find_distributions, Environment, Requirement,
     Distribution, PathMetadata, EggMetadata, WorkingSet, DistributionNotFound,
     VersionConflict, DEVELOP_DIST,
 )
-import pkg_resources.py31compat
-
-__metaclass__ = type
+import pkg_resources
 
 # Turn on PEP440Warnings
 warnings.filterwarnings("default", category=pkg_resources.PEP440Warning)
 
 __all__ = [
     'samefile', 'easy_install', 'PthDistributions', 'extract_wininst_cfg',
-    'main', 'get_exe_prefixes',
+    'get_exe_prefixes',
 ]
 
 
 def is_64bit():
     return struct.calcsize("P") == 8
 
 
@@ -92,36 +87,24 @@
     if use_samefile:
         return os.path.samefile(p1, p2)
     norm_p1 = os.path.normpath(os.path.normcase(p1))
     norm_p2 = os.path.normpath(os.path.normcase(p2))
     return norm_p1 == norm_p2
 
 
-if six.PY2:
-
-    def _to_bytes(s):
-        return s
+def _to_bytes(s):
+    return s.encode('utf8')
 
-    def isascii(s):
-        try:
-            six.text_type(s, 'ascii')
-            return True
-        except UnicodeError:
-            return False
-else:
 
-    def _to_bytes(s):
-        return s.encode('utf8')
-
-    def isascii(s):
-        try:
-            s.encode('ascii')
-            return True
-        except UnicodeError:
-            return False
+def isascii(s):
+    try:
+        s.encode('ascii')
+        return True
+    except UnicodeError:
+        return False
 
 
 def _one_liner(text):
     return textwrap.dedent(text).strip().replace('\n', '; ')
 
 
 class easy_install(Command):
@@ -201,15 +184,14 @@
         self.no_find_links = None
 
         # Options not specifiable via command line
         self.package_index = None
         self.pth_file = self.always_copy_from = None
         self.site_dirs = None
         self.installed_projects = {}
-        self.sitepy_installed = False
         # Always read easy_install options, even if we are subclassed, or have
         # an independent instance created.  This ensures that defaults will
         # always come from the standard configuration file(s)' "easy_install"
         # section, even if this is a "develop" or "install" command, or some
         # other embedding.
         self._dry_run = None
         self.verbose = self.distribution.verbose
@@ -240,15 +222,15 @@
         """
         ver = '{}.{}'.format(*sys.version_info)
         dist = get_distribution('setuptools')
         tmpl = 'setuptools {dist.version} from {dist.location} (Python {ver})'
         print(tmpl.format(**locals()))
         raise SystemExit()
 
-    def finalize_options(self):
+    def finalize_options(self):  # noqa: C901  # is too complex (25)  # FIXME
         self.version and self._render_version()
 
         py_version = sys.version.split()[0]
         prefix, exec_prefix = get_config_vars('prefix', 'exec_prefix')
 
         self.config_vars = {
             'dist_name': self.distribution.get_name(),
@@ -338,30 +320,32 @@
         if self.package_index is None:
             self.package_index = self.create_index(
                 self.index_url, search_path=self.shadow_path, hosts=hosts,
             )
         self.local_index = Environment(self.shadow_path + sys.path)
 
         if self.find_links is not None:
-            if isinstance(self.find_links, six.string_types):
+            if isinstance(self.find_links, str):
                 self.find_links = self.find_links.split()
         else:
             self.find_links = []
         if self.local_snapshots_ok:
             self.package_index.scan_egg_links(self.shadow_path + sys.path)
         if not self.no_find_links:
             self.package_index.add_find_links(self.find_links)
         self.set_undefined_options('install_lib', ('optimize', 'optimize'))
         if not isinstance(self.optimize, int):
             try:
                 self.optimize = int(self.optimize)
                 if not (0 <= self.optimize <= 2):
                     raise ValueError
-            except ValueError:
-                raise DistutilsOptionError("--optimize must be 0, 1, or 2")
+            except ValueError as e:
+                raise DistutilsOptionError(
+                    "--optimize must be 0, 1, or 2"
+                ) from e
 
         if self.editable and not self.build_directory:
             raise DistutilsArgError(
                 "Must specify a build directory (-b) when using --editable"
             )
         if not self.args:
             raise DistutilsArgError(
@@ -449,15 +433,15 @@
         except Exception:
             pid = random.randint(0, sys.maxsize)
         return os.path.join(self.install_dir, "test-easy-install-%s" % pid)
 
     def warn_deprecated_options(self):
         pass
 
-    def check_site_dir(self):
+    def check_site_dir(self):  # noqa: C901  # is too complex (12)  # FIXME
         """Verify that self.install_dir is .pth-capable dir, if needed"""
 
         instdir = normalize_path(self.install_dir)
         pth_file = os.path.join(instdir, 'easy-install.pth')
 
         if not os.path.exists(instdir):
             try:
@@ -490,20 +474,16 @@
 
         if is_site_dir:
             if self.pth_file is None:
                 self.pth_file = PthDistributions(pth_file, self.all_site_dirs)
         else:
             self.pth_file = None
 
-        if instdir not in map(normalize_path, _pythonpath()):
-            # only PYTHONPATH dirs need a site.py, so pretend it's there
-            self.sitepy_installed = True
-        elif self.multi_version and not os.path.exists(pth_file):
-            self.sitepy_installed = True  # don't need site.py in this case
-            self.pth_file = None  # and don't create a .pth file
+        if self.multi_version and not os.path.exists(pth_file):
+            self.pth_file = None  # don't create a .pth file
         self.install_dir = instdir
 
     __cant_write_msg = textwrap.dedent("""
         can't create or remove files in install directory
 
         The following error occurred while trying to add or remove files in the
         installation directory:
@@ -560,15 +540,15 @@
             f.write('OK')
             f.close()
             """) + '\n'
         try:
             if ok_exists:
                 os.unlink(ok_file)
             dirname = os.path.dirname(ok_file)
-            pkg_resources.py31compat.makedirs(dirname, exist_ok=True)
+            os.makedirs(dirname, exist_ok=True)
             f = open(pth_file, 'w')
         except (OSError, IOError):
             self.cant_write_to_target()
         else:
             try:
                 f.write(tmpl.format(**locals()))
                 f.close()
@@ -649,20 +629,17 @@
     @contextlib.contextmanager
     def _tmpdir(self):
         tmpdir = tempfile.mkdtemp(prefix=u"easy_install-")
         try:
             # cast to str as workaround for #709 and #710 and #712
             yield str(tmpdir)
         finally:
-            os.path.exists(tmpdir) and rmtree(rmtree_safe(tmpdir))
+            os.path.exists(tmpdir) and rmtree(tmpdir)
 
     def easy_install(self, spec, deps=False):
-        if not self.editable:
-            self.install_site_py()
-
         with self._tmpdir() as tmpdir:
             if not isinstance(spec, Requirement):
                 if URL_SCHEME(spec):
                     # It's a url, download it to tmpdir and process
                     self.not_editable(spec)
                     dl = self.package_index.download(spec, tmpdir)
                     return self.install_item(None, dl, tmpdir, deps, True)
@@ -732,15 +709,18 @@
         # it's the caller's problem if they supply a bad name!
         scheme = INSTALL_SCHEMES[name]
         for key in SCHEME_KEYS:
             attrname = 'install_' + key
             if getattr(self, attrname) is None:
                 setattr(self, attrname, scheme[key])
 
-    def process_distribution(self, requirement, dist, deps=True, *info):
+    # FIXME: 'easy_install.process_distribution' is too complex (12)
+    def process_distribution(  # noqa: C901
+            self, requirement, dist, deps=True, *info,
+    ):
         self.update_pth(dist)
         self.package_index.add(dist)
         if dist in self.local_index[dist.key]:
             self.local_index.remove(dist)
         self.local_index.add(dist)
         self.install_egg_scripts(dist)
         self.installed_projects[dist.key] = dist
@@ -761,17 +741,17 @@
             requirement = Requirement(str(distreq))
         log.info("Processing dependencies for %s", requirement)
         try:
             distros = WorkingSet([]).resolve(
                 [requirement], self.local_index, self.easy_install
             )
         except DistributionNotFound as e:
-            raise DistutilsError(str(e))
+            raise DistutilsError(str(e)) from e
         except VersionConflict as e:
-            raise DistutilsError(e.report())
+            raise DistutilsError(e.report()) from e
         if self.always_copy or self.always_copy_from:
             # Force all the relevant distros to be copied or activated
             for dist in distros:
                 if dist.key not in self.installed_projects:
                     self.easy_install(dist.as_requirement())
         log.info("Finished processing dependencies for %s", requirement)
 
@@ -856,20 +836,27 @@
             os.unlink(target)
         with open(target, "w" + mode) as f:
             f.write(contents)
         chmod(target, 0o777 - mask)
 
     def install_eggs(self, spec, dist_filename, tmpdir):
         # .egg dirs or files are already built, so just return them
-        if dist_filename.lower().endswith('.egg'):
-            return [self.install_egg(dist_filename, tmpdir)]
-        elif dist_filename.lower().endswith('.exe'):
-            return [self.install_exe(dist_filename, tmpdir)]
-        elif dist_filename.lower().endswith('.whl'):
-            return [self.install_wheel(dist_filename, tmpdir)]
+        installer_map = {
+            '.egg': self.install_egg,
+            '.exe': self.install_exe,
+            '.whl': self.install_wheel,
+        }
+        try:
+            install_dist = installer_map[
+                dist_filename.lower()[-4:]
+            ]
+        except KeyError:
+            pass
+        else:
+            return [install_dist(dist_filename, tmpdir)]
 
         # Anything else, try to extract and build
         setup_base = tmpdir
         if os.path.isfile(dist_filename) and not dist_filename.endswith('.py'):
             unpack_archive(dist_filename, tmpdir, self.unpack_progress)
         elif os.path.isdir(dist_filename):
             setup_base = os.path.abspath(dist_filename)
@@ -906,15 +893,16 @@
         if os.path.isdir(egg_path):
             metadata = PathMetadata(egg_path, os.path.join(egg_path,
                                                            'EGG-INFO'))
         else:
             metadata = EggMetadata(zipimport.zipimporter(egg_path))
         return Distribution.from_filename(egg_path, metadata=metadata)
 
-    def install_egg(self, egg_path, tmpdir):
+    # FIXME: 'easy_install.install_egg' is too complex (11)
+    def install_egg(self, egg_path, tmpdir):  # noqa: C901
         destination = os.path.join(
             self.install_dir,
             os.path.basename(egg_path),
         )
         destination = os.path.abspath(destination)
         if not self.dry_run:
             ensure_directory(destination)
@@ -1005,15 +993,16 @@
         # Build .egg file from tmpdir
         bdist_egg.make_zipfile(
             egg_path, egg_tmp, verbose=self.verbose, dry_run=self.dry_run,
         )
         # install the .egg
         return self.install_egg(egg_path, tmpdir)
 
-    def exe_to_egg(self, dist_filename, egg_tmp):
+    # FIXME: 'easy_install.exe_to_egg' is too complex (12)
+    def exe_to_egg(self, dist_filename, egg_tmp):  # noqa: C901
         """Extract a bdist_wininst to the directories an egg would use"""
         # Check for .pth file and set up prefix translations
         prefixes = get_exe_prefixes(dist_filename)
         to_compile = []
         native_libs = []
         top_level = {}
 
@@ -1152,15 +1141,17 @@
             args.insert(0, '-n')
         log.info(
             "Running %s %s", setup_script[len(setup_base) + 1:], ' '.join(args)
         )
         try:
             run_setup(setup_script, args)
         except SystemExit as v:
-            raise DistutilsError("Setup script exited with %s" % (v.args[0],))
+            raise DistutilsError(
+                "Setup script exited with %s" % (v.args[0],)
+            ) from v
 
     def build_and_install(self, setup_script, setup_base):
         args = ['bdist_egg', '--dist-dir']
 
         dist_dir = tempfile.mkdtemp(
             prefix='egg-dist-tmp-', dir=os.path.dirname(setup_script)
         )
@@ -1195,56 +1186,60 @@
         fetch_directives = (
             'find_links', 'site_dirs', 'index_url', 'optimize', 'allow_hosts',
         )
         fetch_options = {}
         for key, val in ei_opts.items():
             if key not in fetch_directives:
                 continue
-            fetch_options[key.replace('_', '-')] = val[1]
+            fetch_options[key] = val[1]
         # create a settings dictionary suitable for `edit_config`
         settings = dict(easy_install=fetch_options)
         cfg_filename = os.path.join(base, 'setup.cfg')
         setopt.edit_config(cfg_filename, settings)
 
-    def update_pth(self, dist):
+    def update_pth(self, dist):  # noqa: C901  # is too complex (11)  # FIXME
         if self.pth_file is None:
             return
 
         for d in self.pth_file[dist.key]:  # drop old entries
-            if self.multi_version or d.location != dist.location:
-                log.info("Removing %s from easy-install.pth file", d)
-                self.pth_file.remove(d)
-                if d.location in self.shadow_path:
-                    self.shadow_path.remove(d.location)
+            if not self.multi_version and d.location == dist.location:
+                continue
+
+            log.info("Removing %s from easy-install.pth file", d)
+            self.pth_file.remove(d)
+            if d.location in self.shadow_path:
+                self.shadow_path.remove(d.location)
 
         if not self.multi_version:
             if dist.location in self.pth_file.paths:
                 log.info(
                     "%s is already the active version in easy-install.pth",
                     dist,
                 )
             else:
                 log.info("Adding %s to easy-install.pth file", dist)
                 self.pth_file.add(dist)  # add new entry
                 if dist.location not in self.shadow_path:
                     self.shadow_path.append(dist.location)
 
-        if not self.dry_run:
+        if self.dry_run:
+            return
 
-            self.pth_file.save()
+        self.pth_file.save()
 
-            if dist.key == 'setuptools':
-                # Ensure that setuptools itself never becomes unavailable!
-                # XXX should this check for latest version?
-                filename = os.path.join(self.install_dir, 'setuptools.pth')
-                if os.path.islink(filename):
-                    os.unlink(filename)
-                f = open(filename, 'wt')
-                f.write(self.pth_file.make_relative(dist.location) + '\n')
-                f.close()
+        if dist.key != 'setuptools':
+            return
+
+        # Ensure that setuptools itself never becomes unavailable!
+        # XXX should this check for latest version?
+        filename = os.path.join(self.install_dir, 'setuptools.pth')
+        if os.path.islink(filename):
+            os.unlink(filename)
+        with open(filename, 'wt') as f:
+            f.write(self.pth_file.make_relative(dist.location) + '\n')
 
     def unpack_progress(self, src, dst):
         # Progress filter for unpacking
         log.debug("Unpacking %s to %s", src, dst)
         return dst  # only unpack-and-compile skips files for dry run
 
     def unpack_and_compile(self, egg_path, destination):
@@ -1313,52 +1308,20 @@
 
           https://setuptools.readthedocs.io/en/latest/easy_install.html#custom-installation-locations
 
 
         Please make the appropriate changes for your system and try again.
         """).strip()
 
-    def install_site_py(self):
-        """Make sure there's a site.py in the target dir, if needed"""
-
-        if self.sitepy_installed:
-            return  # already did it, or don't need to
-
-        sitepy = os.path.join(self.install_dir, "site.py")
-        source = resource_string("setuptools", "site-patch.py")
-        source = source.decode('utf-8')
-        current = ""
-
-        if os.path.exists(sitepy):
-            log.debug("Checking existing site.py in %s", self.install_dir)
-            with io.open(sitepy) as strm:
-                current = strm.read()
-
-            if not current.startswith('def __boot():'):
-                raise DistutilsError(
-                    "%s is not a setuptools-generated site.py; please"
-                    " remove it." % sitepy
-                )
-
-        if current != source:
-            log.info("Creating %s", sitepy)
-            if not self.dry_run:
-                ensure_directory(sitepy)
-                with io.open(sitepy, 'w', encoding='utf-8') as strm:
-                    strm.write(source)
-            self.byte_compile([sitepy])
-
-        self.sitepy_installed = True
-
     def create_home_path(self):
         """Create directories under ~."""
         if not self.user:
             return
         home = convert_path(os.path.expanduser("~"))
-        for name, path in six.iteritems(self.config_vars):
+        for name, path in self.config_vars.items():
             if path.startswith(home) and not os.path.isdir(path):
                 self.debug_print("os.makedirs('%s', 0o700)" % path)
                 os.makedirs(path, 0o700)
 
     INSTALL_SCHEMES = dict(
         posix=dict(
             install_dir='$base/lib/python$py_version_short/site-packages',
@@ -1409,66 +1372,71 @@
     # start with PYTHONPATH
     sitedirs.extend(_pythonpath())
 
     prefixes = [sys.prefix]
     if sys.exec_prefix != sys.prefix:
         prefixes.append(sys.exec_prefix)
     for prefix in prefixes:
-        if prefix:
-            if sys.platform in ('os2emx', 'riscos'):
-                sitedirs.append(os.path.join(prefix, "Lib", "site-packages"))
-            elif os.sep == '/':
-                sitedirs.extend([
-                    os.path.join(
-                        prefix,
-                        "lib",
-                        "python{}.{}".format(*sys.version_info),
-                        "site-packages",
-                    ),
-                    os.path.join(prefix, "lib", "site-python"),
-                ])
-            else:
-                sitedirs.extend([
+        if not prefix:
+            continue
+
+        if sys.platform in ('os2emx', 'riscos'):
+            sitedirs.append(os.path.join(prefix, "Lib", "site-packages"))
+        elif os.sep == '/':
+            sitedirs.extend([
+                os.path.join(
                     prefix,
-                    os.path.join(prefix, "lib", "site-packages"),
-                ])
-            if sys.platform == 'darwin':
-                # for framework builds *only* we add the standard Apple
-                # locations. Currently only per-user, but /Library and
-                # /Network/Library could be added too
-                if 'Python.framework' in prefix:
-                    home = os.environ.get('HOME')
-                    if home:
-                        home_sp = os.path.join(
-                            home,
-                            'Library',
-                            'Python',
-                            '{}.{}'.format(*sys.version_info),
-                            'site-packages',
-                        )
-                        sitedirs.append(home_sp)
+                    "lib",
+                    "python{}.{}".format(*sys.version_info),
+                    "site-packages",
+                ),
+                os.path.join(prefix, "lib", "site-python"),
+            ])
+        else:
+            sitedirs.extend([
+                prefix,
+                os.path.join(prefix, "lib", "site-packages"),
+            ])
+        if sys.platform != 'darwin':
+            continue
+
+        # for framework builds *only* we add the standard Apple
+        # locations. Currently only per-user, but /Library and
+        # /Network/Library could be added too
+        if 'Python.framework' not in prefix:
+            continue
+
+        home = os.environ.get('HOME')
+        if not home:
+            continue
+
+        home_sp = os.path.join(
+            home,
+            'Library',
+            'Python',
+            '{}.{}'.format(*sys.version_info),
+            'site-packages',
+        )
+        sitedirs.append(home_sp)
     lib_paths = get_path('purelib'), get_path('platlib')
-    for site_lib in lib_paths:
-        if site_lib not in sitedirs:
-            sitedirs.append(site_lib)
+
+    sitedirs.extend(s for s in lib_paths if s not in sitedirs)
 
     if site.ENABLE_USER_SITE:
         sitedirs.append(site.USER_SITE)
 
-    try:
+    with contextlib.suppress(AttributeError):
         sitedirs.extend(site.getsitepackages())
-    except AttributeError:
-        pass
 
     sitedirs = list(map(normalize_path, sitedirs))
 
     return sitedirs
 
 
-def expand_paths(inputs):
+def expand_paths(inputs):  # noqa: C901  # is too complex (11)  # FIXME
     """Yield sys.path directories that might contain "old-style" packages"""
 
     seen = {}
 
     for dirname in inputs:
         dirname = normalize_path(dirname)
         if dirname in seen:
@@ -1492,21 +1460,26 @@
             # Read the .pth file
             f = open(os.path.join(dirname, name))
             lines = list(yield_lines(f))
             f.close()
 
             # Yield existing non-dupe, non-import directory lines from it
             for line in lines:
-                if not line.startswith("import"):
-                    line = normalize_path(line.rstrip())
-                    if line not in seen:
-                        seen[line] = 1
-                        if not os.path.isdir(line):
-                            continue
-                        yield line, os.listdir(line)
+                if line.startswith("import"):
+                    continue
+
+                line = normalize_path(line.rstrip())
+                if line in seen:
+                    continue
+
+                seen[line] = 1
+                if not os.path.isdir(line):
+                    continue
+
+                yield line, os.listdir(line)
 
 
 def extract_wininst_cfg(dist_filename):
     """Extract configuration data from a bdist_wininst .exe
 
     Returns a configparser.RawConfigParser, or None
     """
@@ -1531,15 +1504,15 @@
         try:
             part = f.read(cfglen)
             # Read up to the first null byte.
             config = part.split(b'\0', 1)[0]
             # Now the config is in bytes, but for RawConfigParser, it should
             #  be text, so decode it.
             config = config.decode(sys.getfilesystemencoding())
-            cfg.readfp(six.StringIO(config))
+            cfg.readfp(io.StringIO(config))
         except configparser.Error:
             return None
         if not cfg.has_section('metadata') or not cfg.has_section('Setup'):
             return None
         return cfg
 
     finally:
@@ -1566,17 +1539,15 @@
                     prefixes.insert(0, ('/'.join(parts[:2]), 'EGG-INFO/'))
                     break
             if len(parts) != 2 or not name.endswith('.pth'):
                 continue
             if name.endswith('-nspkg.pth'):
                 continue
             if parts[0].upper() in ('PURELIB', 'PLATLIB'):
-                contents = z.read(name)
-                if not six.PY2:
-                    contents = contents.decode()
+                contents = z.read(name).decode()
                 for pth in yield_lines(contents):
                     pth = pth.strip().replace('\\', '/')
                     if not pth.startswith('import'):
                         prefixes.append((('%s/%s/' % (parts[0], pth)), ''))
     finally:
         z.close()
     prefixes = [(x.lower(), y) for x, y in prefixes]
@@ -1732,15 +1703,16 @@
 
 
 def auto_chmod(func, arg, exc):
     if func in [os.unlink, os.remove] and os.name == 'nt':
         chmod(arg, stat.S_IWRITE)
         return func(arg)
     et, ev, _ = sys.exc_info()
-    six.reraise(et, (ev[0], ev[1] + (" %s %s" % (func, arg))))
+    # TODO: This code doesn't make sense. What is it trying to do?
+    raise (ev[0], ev[1] + (" %s %s" % (func, arg)))
 
 
 def update_dist_caches(dist_path, fix_zipimporter_caches):
     """
     Fix any globally cached `dist_path` related data
 
     `dist_path` should be a path of a newly installed egg distribution (zipped
@@ -2068,25 +2040,46 @@
     """
     Encapsulates behavior around writing entry point scripts for console and
     gui apps.
     """
 
     template = textwrap.dedent(r"""
         # EASY-INSTALL-ENTRY-SCRIPT: %(spec)r,%(group)r,%(name)r
-        __requires__ = %(spec)r
         import re
         import sys
-        from pkg_resources import load_entry_point
+
+        # for compatibility with easy_install; see #2198
+        __requires__ = %(spec)r
+
+        try:
+            from importlib.metadata import distribution
+        except ImportError:
+            try:
+                from importlib_metadata import distribution
+            except ImportError:
+                from pkg_resources import load_entry_point
+
+
+        def importlib_load_entry_point(spec, group, name):
+            dist_name, _, _ = spec.partition('==')
+            matches = (
+                entry_point
+                for entry_point in distribution(dist_name).entry_points
+                if entry_point.group == group and entry_point.name == name
+            )
+            return next(matches).load()
+
+
+        globals().setdefault('load_entry_point', importlib_load_entry_point)
+
 
         if __name__ == '__main__':
             sys.argv[0] = re.sub(r'(-script\.pyw?|\.exe)?$', '', sys.argv[0])
-            sys.exit(
-                load_entry_point(%(spec)r, %(group)r, %(name)r)()
-            )
-    """).lstrip()
+            sys.exit(load_entry_point(%(spec)r, %(group)r, %(name)r)())
+        """).lstrip()
 
     command_spec_class = CommandSpec
 
     @classmethod
     def get_script_args(cls, dist, executable=None, wininst=False):
         # for backward compatibility
         warnings.warn("Use get_args", EasyInstallDeprecationWarning)
@@ -2196,15 +2189,15 @@
         header = cls._adjust_header(type_, header)
         blockers = [name + x for x in old]
         yield name + ext, header + script_text, 't', blockers
 
     @classmethod
     def _adjust_header(cls, type_, orig_header):
         """
-        Make sure 'pythonw' is used for gui and and 'python' is used for
+        Make sure 'pythonw' is used for gui and 'python' is used for
         console (regardless of what sys.executable is).
         """
         pattern = 'pythonw.exe'
         repl = 'python.exe'
         if type_ == 'gui':
             pattern, repl = repl, pattern
         pattern_ob = re.compile(re.escape(pattern), re.IGNORECASE)
@@ -2274,81 +2267,24 @@
     else:
         launcher_fn = launcher_fn.replace(".", "-32.")
     return resource_string('setuptools', launcher_fn)
 
 
 def load_launcher_manifest(name):
     manifest = pkg_resources.resource_string(__name__, 'launcher manifest.xml')
-    if six.PY2:
-        return manifest % vars()
-    else:
-        return manifest.decode('utf-8') % vars()
+    return manifest.decode('utf-8') % vars()
 
 
 def rmtree(path, ignore_errors=False, onerror=auto_chmod):
     return shutil.rmtree(path, ignore_errors, onerror)
 
 
 def current_umask():
     tmp = os.umask(0o022)
     os.umask(tmp)
     return tmp
 
 
-def bootstrap():
-    # This function is called when setuptools*.egg is run using /bin/sh
-    import setuptools
-
-    argv0 = os.path.dirname(setuptools.__path__[0])
-    sys.argv[0] = argv0
-    sys.argv.append(argv0)
-    main()
-
-
-def main(argv=None, **kw):
-    from setuptools import setup
-    from setuptools.dist import Distribution
-
-    class DistributionWithoutHelpCommands(Distribution):
-        common_usage = ""
-
-        def _show_help(self, *args, **kw):
-            with _patch_usage():
-                Distribution._show_help(self, *args, **kw)
-
-    if argv is None:
-        argv = sys.argv[1:]
-
-    with _patch_usage():
-        setup(
-            script_args=['-q', 'easy_install', '-v'] + argv,
-            script_name=sys.argv[0] or 'easy_install',
-            distclass=DistributionWithoutHelpCommands,
-            **kw
-        )
-
-
-@contextlib.contextmanager
-def _patch_usage():
-    import distutils.core
-    USAGE = textwrap.dedent("""
-        usage: %(script)s [options] requirement_or_url ...
-           or: %(script)s --help
-        """).lstrip()
-
-    def gen_usage(script_name):
-        return USAGE % dict(
-            script=os.path.basename(script_name),
-        )
-
-    saved = distutils.core.gen_usage
-    distutils.core.gen_usage = gen_usage
-    try:
-        yield
-    finally:
-        distutils.core.gen_usage = saved
-
-
 class EasyInstallDeprecationWarning(SetuptoolsDeprecationWarning):
     """
     Warning for EasyInstall deprecations, bypassing suppression.
     """
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/egg_info.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/egg_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 
 from distutils.filelist import FileList as _FileList
 from distutils.errors import DistutilsInternalError
 from distutils.util import convert_path
 from distutils import log
 import distutils.errors
 import distutils.filelist
+import functools
 import os
 import re
 import sys
 import io
 import warnings
 import time
 import collections
 
-from setuptools.extern import six
-from setuptools.extern.six.moves import map
-
 from setuptools import Command
 from setuptools.command.sdist import sdist
 from setuptools.command.sdist import walk_revctrl
 from setuptools.command.setopt import edit_config
 from setuptools.command import bdist_egg
 from pkg_resources import (
     parse_requirements, safe_name, parse_version,
@@ -30,15 +28,15 @@
 import setuptools.unicode_utils as unicode_utils
 from setuptools.glob import glob
 
 from setuptools.extern import packaging
 from setuptools import SetuptoolsDeprecationWarning
 
 
-def translate_pattern(glob):
+def translate_pattern(glob):  # noqa: C901  # is too complex (14)  # FIXME
     """
     Translate a file path glob like '*.txt' in to a regular expression.
     This differs from fnmatch.translate which allows wildcards to match
     directory separators. It also knows about '**/' which matches any number of
     directories.
     """
     pat = ''
@@ -122,20 +120,25 @@
     tag_date = None
 
     @property
     def name(self):
         return safe_name(self.distribution.get_name())
 
     def tagged_version(self):
-        version = self.distribution.get_version()
-        # egg_info may be called more than once for a distribution,
-        # in which case the version string already contains all tags.
-        if self.vtags and version.endswith(self.vtags):
-            return safe_version(version)
-        return safe_version(version + self.vtags)
+        return safe_version(self._maybe_tag(self.distribution.get_version()))
+
+    def _maybe_tag(self, version):
+        """
+        egg_info may be called more than once for a distribution,
+        in which case the version string already contains all tags.
+        """
+        return (
+            version if self.vtags and version.endswith(self.vtags)
+            else version + self.vtags
+        )
 
     def tags(self):
         version = ''
         if self.tag_build:
             version += self.tag_build
         if self.tag_date:
             version += time.strftime("-%Y%m%d")
@@ -204,19 +207,19 @@
             is_version = isinstance(parsed_version, packaging.version.Version)
             spec = (
                 "%s==%s" if is_version else "%s===%s"
             )
             list(
                 parse_requirements(spec % (self.egg_name, self.egg_version))
             )
-        except ValueError:
+        except ValueError as e:
             raise distutils.errors.DistutilsOptionError(
                 "Invalid distribution name or version syntax: %s-%s" %
                 (self.egg_name, self.egg_version)
-            )
+            ) from e
 
         if self.egg_base is None:
             dirs = self.distribution.package_dir
             self.egg_base = (dirs or {}).get('', os.curdir)
 
         self.ensure_dirname('egg_base')
         self.egg_info = to_filename(self.egg_name) + '.egg-info'
@@ -263,16 +266,15 @@
     def write_file(self, what, filename, data):
         """Write `data` to `filename` (if not a dry run) after announcing it
 
         `what` is used in a log message to identify what is being written
         to the file.
         """
         log.info("writing %s to %s", what, filename)
-        if not six.PY2:
-            data = data.encode("utf-8")
+        data = data.encode("utf-8")
         if not self.dry_run:
             f = open(filename, 'wb')
             f.write(data)
             f.close()
 
     def delete_file(self, filename):
         """Delete `filename` (if not a dry run) after announcing it"""
@@ -327,78 +329,82 @@
         # Parse the line: split it up, make sure the right number of words
         # is there, and return the relevant words.  'action' is always
         # defined: it's the first word of the line.  Which of the other
         # three are defined depends on the action; it'll be either
         # patterns, (dir and patterns), or (dir_pattern).
         (action, patterns, dir, dir_pattern) = self._parse_template_line(line)
 
+        action_map = {
+            'include': self.include,
+            'exclude': self.exclude,
+            'global-include': self.global_include,
+            'global-exclude': self.global_exclude,
+            'recursive-include': functools.partial(
+                self.recursive_include, dir,
+            ),
+            'recursive-exclude': functools.partial(
+                self.recursive_exclude, dir,
+            ),
+            'graft': self.graft,
+            'prune': self.prune,
+        }
+        log_map = {
+            'include': "warning: no files found matching '%s'",
+            'exclude': (
+                "warning: no previously-included files found "
+                "matching '%s'"
+            ),
+            'global-include': (
+                "warning: no files found matching '%s' "
+                "anywhere in distribution"
+            ),
+            'global-exclude': (
+                "warning: no previously-included files matching "
+                "'%s' found anywhere in distribution"
+            ),
+            'recursive-include': (
+                "warning: no files found matching '%s' "
+                "under directory '%s'"
+            ),
+            'recursive-exclude': (
+                "warning: no previously-included files matching "
+                "'%s' found under directory '%s'"
+            ),
+            'graft': "warning: no directories found matching '%s'",
+            'prune': "no previously-included directories found matching '%s'",
+        }
+
+        try:
+            process_action = action_map[action]
+        except KeyError:
+            raise DistutilsInternalError(
+                "this cannot happen: invalid action '{action!s}'".
+                format(action=action),
+            )
+
         # OK, now we know that the action is valid and we have the
         # right number of words on the line for that action -- so we
         # can proceed with minimal error-checking.
-        if action == 'include':
-            self.debug_print("include " + ' '.join(patterns))
-            for pattern in patterns:
-                if not self.include(pattern):
-                    log.warn("warning: no files found matching '%s'", pattern)
-
-        elif action == 'exclude':
-            self.debug_print("exclude " + ' '.join(patterns))
-            for pattern in patterns:
-                if not self.exclude(pattern):
-                    log.warn(("warning: no previously-included files "
-                              "found matching '%s'"), pattern)
-
-        elif action == 'global-include':
-            self.debug_print("global-include " + ' '.join(patterns))
-            for pattern in patterns:
-                if not self.global_include(pattern):
-                    log.warn(("warning: no files found matching '%s' "
-                              "anywhere in distribution"), pattern)
-
-        elif action == 'global-exclude':
-            self.debug_print("global-exclude " + ' '.join(patterns))
-            for pattern in patterns:
-                if not self.global_exclude(pattern):
-                    log.warn(("warning: no previously-included files matching "
-                              "'%s' found anywhere in distribution"),
-                             pattern)
-
-        elif action == 'recursive-include':
-            self.debug_print("recursive-include %s %s" %
-                             (dir, ' '.join(patterns)))
-            for pattern in patterns:
-                if not self.recursive_include(dir, pattern):
-                    log.warn(("warning: no files found matching '%s' "
-                              "under directory '%s'"),
-                             pattern, dir)
-
-        elif action == 'recursive-exclude':
-            self.debug_print("recursive-exclude %s %s" %
-                             (dir, ' '.join(patterns)))
-            for pattern in patterns:
-                if not self.recursive_exclude(dir, pattern):
-                    log.warn(("warning: no previously-included files matching "
-                              "'%s' found under directory '%s'"),
-                             pattern, dir)
-
-        elif action == 'graft':
-            self.debug_print("graft " + dir_pattern)
-            if not self.graft(dir_pattern):
-                log.warn("warning: no directories found matching '%s'",
-                         dir_pattern)
-
-        elif action == 'prune':
-            self.debug_print("prune " + dir_pattern)
-            if not self.prune(dir_pattern):
-                log.warn(("no previously-included directories found "
-                          "matching '%s'"), dir_pattern)
 
-        else:
-            raise DistutilsInternalError(
-                "this cannot happen: invalid action '%s'" % action)
+        action_is_recursive = action.startswith('recursive-')
+        if action in {'graft', 'prune'}:
+            patterns = [dir_pattern]
+        extra_log_args = (dir, ) if action_is_recursive else ()
+        log_tmpl = log_map[action]
+
+        self.debug_print(
+            ' '.join(
+                [action] +
+                ([dir] if action_is_recursive else []) +
+                patterns,
+            )
+        )
+        for pattern in patterns:
+            if not process_action(pattern):
+                log.warn(log_tmpl, pattern, *extra_log_args)
 
     def _remove_files(self, predicate):
         """
         Remove all files from the file list that match the predicate.
         Return True if any matching files were removed
         """
         found = False
@@ -643,15 +649,15 @@
         return line + '\n'
     lines = map(append_cr, lines)
     stream.writelines(lines)
 
 
 def write_requirements(cmd, basename, filename):
     dist = cmd.distribution
-    data = six.StringIO()
+    data = io.StringIO()
     _write_requirements(data, dist.install_requires)
     extras_require = dist.extras_require or {}
     for extra in sorted(extras_require):
         data.write('\n[{extra}]\n'.format(**vars()))
         _write_requirements(data, extras_require[extra])
     cmd.write_or_delete_file("requirements", filename, data.getvalue())
 
@@ -683,20 +689,20 @@
         value = '\n'.join(value) + '\n'
     cmd.write_or_delete_file(argname, filename, value, force)
 
 
 def write_entries(cmd, basename, filename):
     ep = cmd.distribution.entry_points
 
-    if isinstance(ep, six.string_types) or ep is None:
+    if isinstance(ep, str) or ep is None:
         data = ep
     elif ep is not None:
         data = []
         for section, contents in sorted(ep.items()):
-            if not isinstance(contents, six.string_types):
+            if not isinstance(contents, str):
                 contents = EntryPoint.parse_group(section, contents)
                 contents = '\n'.join(sorted(map(str, contents.values())))
             data.append('[%s]\n%s\n\n' % (section, contents))
         data = ''.join(data)
 
     cmd.write_or_delete_file('entry points', filename, data, True)
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/install.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/install_egg_info.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/install_lib.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/install_scripts.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/install_scripts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from distutils import log
 import distutils.command.install_scripts as orig
+from distutils.errors import DistutilsModuleError
 import os
 import sys
 
 from pkg_resources import Distribution, PathMetadata, ensure_directory
 
 
 class install_scripts(orig.install_scripts):
@@ -31,15 +32,15 @@
             ei_cmd.egg_name, ei_cmd.egg_version,
         )
         bs_cmd = self.get_finalized_command('build_scripts')
         exec_param = getattr(bs_cmd, 'executable', None)
         try:
             bw_cmd = self.get_finalized_command("bdist_wininst")
             is_wininst = getattr(bw_cmd, '_is_running', False)
-        except ImportError:
+        except (ImportError, DistutilsModuleError):
             is_wininst = False
         writer = ei.ScriptWriter
         if is_wininst:
             exec_param = "python.exe"
             writer = ei.WindowsScriptWriter
         if exec_param == sys.executable:
             # In case the path to the Python executable contains a space, wrap
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/launcher manifest.xml` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/py36compat.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/py36compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 from glob import glob
 from distutils.util import convert_path
 from distutils.command import sdist
 
-from setuptools.extern.six.moves import filter
-
 
 class sdist_add_defaults:
     """
     Mix-in providing forward-compatibility for functionality as found in
     distutils on Python 3.7.
 
     Do not edit the code in this class except to update functionality
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/rotate.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/rotate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from distutils.util import convert_path
 from distutils import log
 from distutils.errors import DistutilsOptionError
 import os
 import shutil
 
-from setuptools.extern import six
-
 from setuptools import Command
 
 
 class rotate(Command):
     """Delete older distributions"""
 
     description = "delete older distributions, keeping N newest files"
@@ -32,17 +30,17 @@
                 "Must specify one or more (comma-separated) match patterns "
                 "(e.g. '.zip' or '.egg')"
             )
         if self.keep is None:
             raise DistutilsOptionError("Must specify number of files to keep")
         try:
             self.keep = int(self.keep)
-        except ValueError:
-            raise DistutilsOptionError("--keep must be an integer")
-        if isinstance(self.match, six.string_types):
+        except ValueError as e:
+            raise DistutilsOptionError("--keep must be an integer") from e
+        if isinstance(self.match, str):
             self.match = [
                 convert_path(p.strip()) for p in self.match.split(',')
             ]
         self.set_undefined_options('bdist', ('dist_dir', 'dist_dir'))
 
     def run(self):
         self.run_command("egg_info")
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/saveopts.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/sdist.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/sdist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from distutils import log
 import distutils.command.sdist as orig
 import os
 import sys
 import io
 import contextlib
+from glob import iglob
 
-from setuptools.extern import six, ordered_set
+from setuptools.extern import ordered_set
 
 from .py36compat import sdist_add_defaults
 
 import pkg_resources
 
 _default_revctrl = list
 
@@ -94,42 +95,16 @@
             pass
         try:
             yield
         finally:
             if orig_val is not NoValue:
                 setattr(os, 'link', orig_val)
 
-    def __read_template_hack(self):
-        # This grody hack closes the template file (MANIFEST.in) if an
-        #  exception occurs during read_template.
-        # Doing so prevents an error when easy_install attempts to delete the
-        #  file.
-        try:
-            orig.sdist.read_template(self)
-        except Exception:
-            _, _, tb = sys.exc_info()
-            tb.tb_next.tb_frame.f_locals['template'].close()
-            raise
-
-    # Beginning with Python 2.7.2, 3.1.4, and 3.2.1, this leaky file handle
-    #  has been fixed, so only override the method if we're using an earlier
-    #  Python.
-    has_leaky_handle = (
-        sys.version_info < (2, 7, 2)
-        or (3, 0) <= sys.version_info < (3, 1, 4)
-        or (3, 2) <= sys.version_info < (3, 2, 1)
-    )
-    if has_leaky_handle:
-        read_template = __read_template_hack
-
     def _add_defaults_optional(self):
-        if six.PY2:
-            sdist_add_defaults._add_defaults_optional(self)
-        else:
-            super()._add_defaults_optional()
+        super()._add_defaults_optional()
         if os.path.isfile('pyproject.toml'):
             self.filelist.append('pyproject.toml')
 
     def _add_defaults_python(self):
         """getting python files"""
         if self.distribution.has_pure_modules():
             build_py = self.get_finalized_command('build_py')
@@ -154,18 +129,15 @@
             os.path.join(src_dir, name)
             for _, src_dir, _, filenames in data_files
             for name in filenames
         )
 
     def _add_defaults_data_files(self):
         try:
-            if six.PY2:
-                sdist_add_defaults._add_defaults_data_files(self)
-            else:
-                super()._add_defaults_data_files()
+            super()._add_defaults_data_files()
         except TypeError:
             log.warn("data_files contains unexpected objects")
 
     def check_readme(self):
         for f in self.READMES:
             if os.path.exists(f):
                 return
@@ -203,50 +175,61 @@
         fill in 'self.filelist', the list of files to include in the source
         distribution.
         """
         log.info("reading manifest file '%s'", self.manifest)
         manifest = open(self.manifest, 'rb')
         for line in manifest:
             # The manifest must contain UTF-8. See #303.
-            if not six.PY2:
-                try:
-                    line = line.decode('UTF-8')
-                except UnicodeDecodeError:
-                    log.warn("%r not UTF-8 decodable -- skipping" % line)
-                    continue
+            try:
+                line = line.decode('UTF-8')
+            except UnicodeDecodeError:
+                log.warn("%r not UTF-8 decodable -- skipping" % line)
+                continue
             # ignore comments and blank lines
             line = line.strip()
             if line.startswith('#') or not line:
                 continue
             self.filelist.append(line)
         manifest.close()
 
     def check_license(self):
         """Checks if license_file' or 'license_files' is configured and adds any
         valid paths to 'self.filelist'.
         """
-
-        files = ordered_set.OrderedSet()
-
         opts = self.distribution.get_option_dict('metadata')
 
-        # ignore the source of the value
-        _, license_file = opts.get('license_file', (None, None))
-
-        if license_file is None:
-            log.debug("'license_file' option was not specified")
-        else:
-            files.add(license_file)
-
+        files = ordered_set.OrderedSet()
         try:
-            files.update(self.distribution.metadata.license_files)
+            license_files = self.distribution.metadata.license_files
         except TypeError:
             log.warn("warning: 'license_files' option is malformed")
+            license_files = ordered_set.OrderedSet()
+        patterns = license_files if isinstance(license_files, ordered_set.OrderedSet) \
+            else ordered_set.OrderedSet(license_files)
+
+        if 'license_file' in opts:
+            log.warn(
+                "warning: the 'license_file' option is deprecated, "
+                "use 'license_files' instead")
+            patterns.append(opts['license_file'][1])
+
+        if 'license_file' not in opts and 'license_files' not in opts:
+            # Default patterns match the ones wheel uses
+            # See https://wheel.readthedocs.io/en/stable/user_guide.html
+            # -> 'Including license files in the generated wheel file'
+            patterns = ('LICEN[CS]E*', 'COPYING*', 'NOTICE*', 'AUTHORS*')
+
+        for pattern in patterns:
+            for path in iglob(pattern):
+                if path.endswith('~'):
+                    log.debug(
+                        "ignoring license file '%s' as it looks like a backup",
+                        path)
+                    continue
 
-        for f in files:
-            if not os.path.exists(f):
-                log.warn(
-                    "warning: Failed to find the configured license file '%s'",
-                    f)
-                files.remove(f)
+                if path not in files and os.path.isfile(path):
+                    log.info(
+                        "adding license file '%s' (matched pattern '%s')",
+                        path, pattern)
+                    files.add(path)
 
-        self.filelist.extend(files)
+        self.filelist.extend(sorted(files))
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/setopt.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/setopt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from distutils.util import convert_path
 from distutils import log
 from distutils.errors import DistutilsOptionError
 import distutils
 import os
-
-from setuptools.extern.six.moves import configparser
+import configparser
 
 from setuptools import Command
 
 __all__ = ['config_file', 'edit_config', 'option_base', 'setopt']
 
 
 def config_file(kind="local"):
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/test.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,20 @@
 import contextlib
 import itertools
 import unittest
 from distutils.errors import DistutilsError, DistutilsOptionError
 from distutils import log
 from unittest import TestLoader
 
-from setuptools.extern import six
-from setuptools.extern.six.moves import map, filter
-
 from pkg_resources import (resource_listdir, resource_exists, normalize_path,
                            working_set, _namespace_packages, evaluate_marker,
                            add_activation_listener, require, EntryPoint)
 from setuptools import Command
 from .build_py import _unique_everseen
 
-__metaclass__ = type
-
 
 class ScanningLoader(TestLoader):
 
     def __init__(self):
         TestLoader.__init__(self)
         self._visited = set()
 
@@ -125,16 +120,15 @@
         Backward compatibility for project_on_sys_path context.
         """
         with self.project_on_sys_path():
             func()
 
     @contextlib.contextmanager
     def project_on_sys_path(self, include_dists=[]):
-        with_2to3 = not six.PY2 and getattr(
-            self.distribution, 'use_2to3', False)
+        with_2to3 = getattr(self.distribution, 'use_2to3', False)
 
         if with_2to3:
             # If we run 2to3 we can not do this inplace:
 
             # Ensure metadata is up-to-date
             self.reinitialize_command('build_py', inplace=0)
             self.run_command('build_py')
@@ -237,15 +231,15 @@
             with self.project_on_sys_path():
                 self.run_tests()
 
     def run_tests(self):
         # Purge modules under test from sys.modules. The test loader will
         # re-import them from the build location. Required when 2to3 is used
         # with namespace packages.
-        if not six.PY2 and getattr(self.distribution, 'use_2to3', False):
+        if getattr(self.distribution, 'use_2to3', False):
             module = self.test_suite.split('.')[0]
             if module in _namespace_packages:
                 del_modules = []
                 if module in sys.modules:
                     del_modules.append(module)
                 module += '.'
                 for name in sys.modules:
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/command/upload_docs.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/command/upload_docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # -*- coding: utf-8 -*-
 """upload_docs
 
 Implements a Distutils 'upload_docs' subcommand (upload documentation to
-PyPI's pythonhosted.org).
+sites other than PyPi such as devpi).
 """
 
 from base64 import standard_b64encode
 from distutils import log
 from distutils.errors import DistutilsOptionError
 import os
 import socket
 import zipfile
 import tempfile
 import shutil
 import itertools
 import functools
-
-from setuptools.extern import six
-from setuptools.extern.six.moves import http_client, urllib
+import http.client
+import urllib.parse
 
 from pkg_resources import iter_entry_points
 from .upload import upload
 
 
 def _encode(s):
-    errors = 'strict' if six.PY2 else 'surrogateescape'
-    return s.encode('utf-8', errors)
+    return s.encode('utf-8', 'surrogateescape')
 
 
 class upload_docs(upload):
     # override the default repository as upload_docs isn't
     # supported by Warehouse (and won't be).
     DEFAULT_REPOSITORY = 'https://pypi.python.org/pypi/'
 
-    description = 'Upload documentation to PyPI'
+    description = 'Upload documentation to sites other than PyPi such as devpi'
 
     user_options = [
         ('repository=', 'r',
          "url of repository [default: %s]" % upload.DEFAULT_REPOSITORY),
         ('show-response', None,
          'display full response text from server'),
         ('upload-dir=', None, 'directory to upload'),
@@ -57,23 +55,23 @@
         self.target_dir = None
 
     def finalize_options(self):
         upload.finalize_options(self)
         if self.upload_dir is None:
             if self.has_sphinx():
                 build_sphinx = self.get_finalized_command('build_sphinx')
-                self.target_dir = build_sphinx.builder_target_dir
+                self.target_dir = dict(build_sphinx.builder_target_dirs)['html']
             else:
                 build = self.get_finalized_command('build')
                 self.target_dir = os.path.join(build.build_base, 'docs')
         else:
             self.ensure_dirname('upload_dir')
             self.target_dir = self.upload_dir
         if 'pypi.python.org' in self.repository:
-            log.warn("Upload_docs command is deprecated. Use RTD instead.")
+            log.warn("Upload_docs command is deprecated for PyPi. Use RTD instead.")
         self.announce('Using upload directory %s' % self.target_dir)
 
     def create_zipfile(self, filename):
         zip_file = zipfile.ZipFile(filename, "w")
         try:
             self.mkpath(self.target_dir)  # just in case
             for root, dirs, files in os.walk(self.target_dir):
@@ -148,34 +146,32 @@
         data = {
             ':action': 'doc_upload',
             'name': meta.get_name(),
             'content': (os.path.basename(filename), content),
         }
         # set up the authentication
         credentials = _encode(self.username + ':' + self.password)
-        credentials = standard_b64encode(credentials)
-        if not six.PY2:
-            credentials = credentials.decode('ascii')
+        credentials = standard_b64encode(credentials).decode('ascii')
         auth = "Basic " + credentials
 
         body, ct = self._build_multipart(data)
 
         msg = "Submitting documentation to %s" % (self.repository)
         self.announce(msg, log.INFO)
 
         # build the Request
         # We can't use urllib2 since we need to send the Basic
         # auth right with the first request
         schema, netloc, url, params, query, fragments = \
             urllib.parse.urlparse(self.repository)
         assert not params and not query and not fragments
         if schema == 'http':
-            conn = http_client.HTTPConnection(netloc)
+            conn = http.client.HTTPConnection(netloc)
         elif schema == 'https':
-            conn = http_client.HTTPSConnection(netloc)
+            conn = http.client.HTTPSConnection(netloc)
         else:
             raise AssertionError("unsupported schema " + schema)
 
         data = ''
         try:
             conn.connect()
             conn.putrequest("POST", url)
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/config.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import absolute_import, unicode_literals
 import ast
 import io
 import os
 import sys
 
 import warnings
 import functools
@@ -11,18 +10,14 @@
 from functools import partial
 from functools import wraps
 import contextlib
 
 from distutils.errors import DistutilsOptionError, DistutilsFileError
 from setuptools.extern.packaging.version import LegacyVersion, parse
 from setuptools.extern.packaging.specifiers import SpecifierSet
-from setuptools.extern.six import string_types, PY3
-
-
-__metaclass__ = type
 
 
 class StaticModule:
     """
     Attempt to load the module by the name
     """
     def __init__(self, name):
@@ -38,17 +33,18 @@
             return next(
                 ast.literal_eval(statement.value)
                 for statement in self.module.body
                 if isinstance(statement, ast.Assign)
                 for target in statement.targets
                 if isinstance(target, ast.Name) and target.id == attr
             )
-        except Exception:
+        except Exception as e:
             raise AttributeError(
-                "{self.name} has no attribute {attr}".format(**locals()))
+                "{self.name} has no attribute {attr}".format(**locals())
+            ) from e
 
 
 @contextlib.contextmanager
 def patch_path(path):
     """
     Add path to front of sys.path for the duration of the context.
     """
@@ -319,15 +315,15 @@
             file: README.rst, CHANGELOG.md, src/file.txt
 
         :param str value:
         :rtype: str
         """
         include_directive = 'file:'
 
-        if not isinstance(value, string_types):
+        if not isinstance(value, str):
             return value
 
         if not value.startswith(include_directive):
             return value
 
         spec = value[len(include_directive):]
         filepaths = (os.path.abspath(path.strip()) for path in spec.split(','))
@@ -554,15 +550,15 @@
             return version
 
         version = self._parse_attr(value, self.package_dir)
 
         if callable(version):
             version = version()
 
-        if not isinstance(version, string_types):
+        if not isinstance(version, str):
             if hasattr(version, '__iter__'):
                 version = '.'.join(map(str, version))
             else:
                 version = '%s' % version
 
         return version
 
@@ -574,14 +570,15 @@
     @property
     def parsers(self):
         """Metadata item name to parser function mapping."""
         parse_list = self._parse_list
         parse_list_semicolon = partial(self._parse_list, separator=';')
         parse_bool = self._parse_bool
         parse_dict = self._parse_dict
+        parse_cmdclass = self._parse_cmdclass
 
         return {
             'zip_safe': parse_bool,
             'use_2to3': parse_bool,
             'include_package_data': parse_bool,
             'package_dir': parse_dict,
             'use_2to3_fixers': parse_list,
@@ -594,14 +591,30 @@
             'install_requires': parse_list_semicolon,
             'setup_requires': parse_list_semicolon,
             'tests_require': parse_list_semicolon,
             'packages': self._parse_packages,
             'entry_points': self._parse_file,
             'py_modules': parse_list,
             'python_requires': SpecifierSet,
+            'cmdclass': parse_cmdclass,
+        }
+
+    def _parse_cmdclass(self, value):
+        def resolve_class(qualified_class_name):
+            idx = qualified_class_name.rfind('.')
+            class_name = qualified_class_name[idx+1:]
+            pkg_name = qualified_class_name[:idx]
+
+            module = __import__(pkg_name)
+
+            return getattr(module, class_name)
+
+        return {
+            k: resolve_class(v)
+            for k, v in self._parse_dict(value).items()
         }
 
     def _parse_packages(self, value):
         """Parses `packages` option value.
 
         :param value:
         :rtype: list
@@ -609,17 +622,14 @@
         find_directives = ['find:', 'find_namespace:']
         trimmed_value = value.strip()
 
         if trimmed_value not in find_directives:
             return self._parse_list(value)
 
         findns = trimmed_value == find_directives[1]
-        if findns and not PY3:
-            raise DistutilsOptionError(
-                'find_namespace: directive is unsupported on Python < 3.3')
 
         # Read function arguments from a dedicated section.
         find_kwargs = self.parse_section_packages__find(
             self.sections.get('packages.find', {}))
 
         if findns:
             from setuptools import find_namespace_packages as find_packages
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/dep_util.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/depends.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/depends.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import sys
 import marshal
 import contextlib
+import dis
 from distutils.version import StrictVersion
 
-from .py33compat import Bytecode
-
-from .py27compat import find_module, PY_COMPILED, PY_FROZEN, PY_SOURCE
-from . import py27compat
+from ._imp import find_module, PY_COMPILED, PY_FROZEN, PY_SOURCE
+from . import _imp
 
 
 __all__ = [
     'Require', 'find_module', 'get_module_constant', 'extract_constant'
 ]
 
 
@@ -107,20 +106,20 @@
         return None
 
     with maybe_close(f):
         if kind == PY_COMPILED:
             f.read(8)  # skip magic & date
             code = marshal.load(f)
         elif kind == PY_FROZEN:
-            code = py27compat.get_frozen_object(module, paths)
+            code = _imp.get_frozen_object(module, paths)
         elif kind == PY_SOURCE:
             code = compile(f.read(), path, 'exec')
         else:
             # Not something we can parse; we'll have to import it.  :(
-            imported = py27compat.get_module(module, paths, info)
+            imported = _imp.get_module(module, paths, info)
             return getattr(imported, symbol, None)
 
     return extract_constant(code, symbol, default)
 
 
 def extract_constant(code, symbol, default=-1):
     """Extract the constant value of 'symbol' from 'code'
@@ -142,15 +141,15 @@
 
     STORE_NAME = 90
     STORE_GLOBAL = 97
     LOAD_CONST = 100
 
     const = default
 
-    for byte_code in Bytecode(code):
+    for byte_code in dis.Bytecode(code):
         op = byte_code.opcode
         arg = byte_code.arg
 
         if op == LOAD_CONST:
             const = code.co_consts[arg]
         elif arg == name_idx and (op == STORE_NAME or op == STORE_GLOBAL):
             return const
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/dist.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/dist.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 import os
 import warnings
 import numbers
 import distutils.log
 import distutils.core
 import distutils.cmd
 import distutils.dist
+import distutils.command
 from distutils.util import strtobool
 from distutils.debug import DEBUG
 from distutils.fancy_getopt import translate_longopt
 import itertools
 
 from collections import defaultdict
 from email import message_from_file
 
 from distutils.errors import DistutilsOptionError, DistutilsSetupError
 from distutils.util import rfc822_escape
 from distutils.version import StrictVersion
 
-from setuptools.extern import six
 from setuptools.extern import packaging
 from setuptools.extern import ordered_set
-from setuptools.extern.six.moves import map, filter, filterfalse
 
 from . import SetuptoolsDeprecationWarning
 
 import setuptools
+import setuptools.command
 from setuptools import windows_support
 from setuptools.monkey import get_unpatched
 from setuptools.config import parse_configuration
 import pkg_resources
 
 __import__('setuptools.extern.packaging.specifiers')
 __import__('setuptools.extern.packaging.version')
@@ -116,31 +116,36 @@
         self.obsoletes = _read_list('obsoletes')
     else:
         self.requires = None
         self.provides = None
         self.obsoletes = None
 
 
+def single_line(val):
+    # quick and dirty validation for description pypa/setuptools#1390
+    if '\n' in val:
+        # TODO after 2021-07-31: Replace with `raise ValueError("newlines not allowed")`
+        warnings.warn("newlines not allowed and will break in the future")
+        val = val.replace('\n', ' ')
+    return val
+
+
 # Based on Python 3.5 version
-def write_pkg_file(self, file):
+def write_pkg_file(self, file):  # noqa: C901  # is too complex (14)  # FIXME
     """Write the PKG-INFO format data to a file object.
     """
     version = self.get_metadata_version()
 
-    if six.PY2:
-        def write_field(key, value):
-            file.write("%s: %s\n" % (key, self._encode_field(value)))
-    else:
-        def write_field(key, value):
-            file.write("%s: %s\n" % (key, value))
+    def write_field(key, value):
+        file.write("%s: %s\n" % (key, value))
 
     write_field('Metadata-Version', str(version))
     write_field('Name', self.get_name())
     write_field('Version', self.get_version())
-    write_field('Summary', self.get_description())
+    write_field('Summary', single_line(self.get_description()))
     write_field('Home-page', self.get_url())
 
     if version < StrictVersion('1.2'):
         write_field('Author', self.get_contact())
         write_field('Author-email', self.get_contact_email())
     else:
         optional_fields = (
@@ -200,33 +205,33 @@
 sequence = tuple, list
 
 
 def check_importable(dist, attr, value):
     try:
         ep = pkg_resources.EntryPoint.parse('x=' + value)
         assert not ep.extras
-    except (TypeError, ValueError, AttributeError, AssertionError):
+    except (TypeError, ValueError, AttributeError, AssertionError) as e:
         raise DistutilsSetupError(
             "%r must be importable 'module:attrs' string (got %r)"
             % (attr, value)
-        )
+        ) from e
 
 
 def assert_string_list(dist, attr, value):
     """Verify that value is a string list"""
     try:
         # verify that value is a list or tuple to exclude unordered
         # or single-use iterables
         assert isinstance(value, (list, tuple))
         # verify that elements of value are strings
         assert ''.join(value) != value
-    except (TypeError, ValueError, AttributeError, AssertionError):
+    except (TypeError, ValueError, AttributeError, AssertionError) as e:
         raise DistutilsSetupError(
             "%r must be a list of strings (got %r)" % (attr, value)
-        )
+        ) from e
 
 
 def check_nsp(dist, attr, value):
     """Verify that namespace packages are valid"""
     ns_packages = value
     assert_string_list(dist, attr, ns_packages)
     for nsp in ns_packages:
@@ -243,20 +248,20 @@
             )
 
 
 def check_extras(dist, attr, value):
     """Verify that extras_require mapping is valid"""
     try:
         list(itertools.starmap(_check_extra, value.items()))
-    except (TypeError, ValueError, AttributeError):
+    except (TypeError, ValueError, AttributeError) as e:
         raise DistutilsSetupError(
             "'extras_require' must be a dictionary whose values are "
             "strings or lists of strings containing valid project/version "
             "requirement specifiers."
-        )
+        ) from e
 
 
 def _check_extra(extra, reqs):
     name, sep, marker = extra.partition(':')
     if marker and pkg_resources.invalid_marker(marker):
         raise DistutilsSetupError("Invalid environment marker: " + marker)
     list(pkg_resources.parse_requirements(reqs))
@@ -276,50 +281,54 @@
         if isinstance(value, (dict, set)):
             raise TypeError("Unordered types are not allowed")
     except (TypeError, ValueError) as error:
         tmpl = (
             "{attr!r} must be a string or list of strings "
             "containing valid project/version requirement specifiers; {error}"
         )
-        raise DistutilsSetupError(tmpl.format(attr=attr, error=error))
+        raise DistutilsSetupError(
+            tmpl.format(attr=attr, error=error)
+        ) from error
 
 
 def check_specifier(dist, attr, value):
     """Verify that value is a valid version specifier"""
     try:
         packaging.specifiers.SpecifierSet(value)
-    except packaging.specifiers.InvalidSpecifier as error:
+    except (packaging.specifiers.InvalidSpecifier, AttributeError) as error:
         tmpl = (
             "{attr!r} must be a string "
             "containing valid version specifiers; {error}"
         )
-        raise DistutilsSetupError(tmpl.format(attr=attr, error=error))
+        raise DistutilsSetupError(
+            tmpl.format(attr=attr, error=error)
+        ) from error
 
 
 def check_entry_points(dist, attr, value):
     """Verify that entry_points map is parseable"""
     try:
         pkg_resources.EntryPoint.parse_map(value)
     except ValueError as e:
-        raise DistutilsSetupError(e)
+        raise DistutilsSetupError(e) from e
 
 
 def check_test_suite(dist, attr, value):
-    if not isinstance(value, six.string_types):
+    if not isinstance(value, str):
         raise DistutilsSetupError("test_suite must be a string")
 
 
 def check_package_data(dist, attr, value):
     """Verify that value is a dictionary of package names to glob lists"""
     if not isinstance(value, dict):
         raise DistutilsSetupError(
             "{!r} must be a dictionary mapping package names to lists of "
             "string wildcard patterns".format(attr))
     for k, v in value.items():
-        if not isinstance(k, six.string_types):
+        if not isinstance(k, str):
             raise DistutilsSetupError(
                 "keys of {!r} dict must be strings (got {!r})"
                 .format(attr, k)
             )
         assert_string_list(dist, 'values of {!r} dict'.format(attr), v)
 
 
@@ -529,15 +538,15 @@
 
         def is_simple_req(req):
             return not req.marker
 
         spec_inst_reqs = getattr(self, 'install_requires', None) or ()
         inst_reqs = list(pkg_resources.parse_requirements(spec_inst_reqs))
         simple_reqs = filter(is_simple_req, inst_reqs)
-        complex_reqs = filterfalse(is_simple_req, inst_reqs)
+        complex_reqs = itertools.filterfalse(is_simple_req, inst_reqs)
         self.install_requires = list(map(str, simple_reqs))
 
         for r in complex_reqs:
             self._tmp_extras_require[':' + str(r.marker)].append(r)
         self.extras_require = dict(
             (k, [str(r) for r in map(self._clean_req, v)])
             for k, v in self._tmp_extras_require.items()
@@ -546,97 +555,114 @@
     def _clean_req(self, req):
         """
         Given a Requirement, remove environment markers and return it.
         """
         req.marker = None
         return req
 
-    def _parse_config_files(self, filenames=None):
+    # FIXME: 'Distribution._parse_config_files' is too complex (14)
+    def _parse_config_files(self, filenames=None):  # noqa: C901
         """
         Adapted from distutils.dist.Distribution.parse_config_files,
         this method provides the same functionality in subtly-improved
         ways.
         """
-        from setuptools.extern.six.moves.configparser import ConfigParser
+        from configparser import ConfigParser
 
         # Ignore install directory options if we have a venv
-        if not six.PY2 and sys.prefix != sys.base_prefix:
-            ignore_options = [
-                'install-base', 'install-platbase', 'install-lib',
-                'install-platlib', 'install-purelib', 'install-headers',
-                'install-scripts', 'install-data', 'prefix', 'exec-prefix',
-                'home', 'user', 'root']
-        else:
-            ignore_options = []
+        ignore_options = [] if sys.prefix == sys.base_prefix else [
+            'install-base', 'install-platbase', 'install-lib',
+            'install-platlib', 'install-purelib', 'install-headers',
+            'install-scripts', 'install-data', 'prefix', 'exec-prefix',
+            'home', 'user', 'root',
+        ]
 
         ignore_options = frozenset(ignore_options)
 
         if filenames is None:
             filenames = self.find_config_files()
 
         if DEBUG:
             self.announce("Distribution.parse_config_files():")
 
         parser = ConfigParser()
+        parser.optionxform = str
         for filename in filenames:
             with io.open(filename, encoding='utf-8') as reader:
                 if DEBUG:
                     self.announce("  reading {filename}".format(**locals()))
-                (parser.readfp if six.PY2 else parser.read_file)(reader)
+                parser.read_file(reader)
             for section in parser.sections():
                 options = parser.options(section)
                 opt_dict = self.get_option_dict(section)
 
                 for opt in options:
-                    if opt != '__name__' and opt not in ignore_options:
-                        val = self._try_str(parser.get(section, opt))
-                        opt = opt.replace('-', '_')
-                        opt_dict[opt] = (filename, val)
+                    if opt == '__name__' or opt in ignore_options:
+                        continue
+
+                    val = parser.get(section, opt)
+                    opt = self.warn_dash_deprecation(opt, section)
+                    opt = self.make_option_lowercase(opt, section)
+                    opt_dict[opt] = (filename, val)
 
             # Make the ConfigParser forget everything (so we retain
             # the original filenames that options come from)
             parser.__init__()
 
+        if 'global' not in self.command_options:
+            return
+
         # If there was a "global" section in the config file, use it
         # to set Distribution options.
 
-        if 'global' in self.command_options:
-            for (opt, (src, val)) in self.command_options['global'].items():
-                alias = self.negative_opt.get(opt)
-                try:
-                    if alias:
-                        setattr(self, alias, not strtobool(val))
-                    elif opt in ('verbose', 'dry_run'):  # ugh!
-                        setattr(self, opt, strtobool(val))
-                    else:
-                        setattr(self, opt, val)
-                except ValueError as msg:
-                    raise DistutilsOptionError(msg)
-
-    @staticmethod
-    def _try_str(val):
-        """
-        On Python 2, much of distutils relies on string values being of
-        type 'str' (bytes) and not unicode text. If the value can be safely
-        encoded to bytes using the default encoding, prefer that.
-
-        Why the default encoding? Because that value can be implicitly
-        decoded back to text if needed.
+        for (opt, (src, val)) in self.command_options['global'].items():
+            alias = self.negative_opt.get(opt)
+            if alias:
+                val = not strtobool(val)
+            elif opt in ('verbose', 'dry_run'):  # ugh!
+                val = strtobool(val)
 
-        Ref #1653
-        """
-        if not six.PY2:
-            return val
-        try:
-            return val.encode()
-        except UnicodeEncodeError:
-            pass
-        return val
+            try:
+                setattr(self, alias or opt, val)
+            except ValueError as e:
+                raise DistutilsOptionError(e) from e
+
+    def warn_dash_deprecation(self, opt, section):
+        if section in (
+            'options.extras_require', 'options.data_files',
+        ):
+            return opt
+
+        underscore_opt = opt.replace('-', '_')
+        commands = distutils.command.__all__ + setuptools.command.__all__
+        if (not section.startswith('options') and section != 'metadata'
+                and section not in commands):
+            return underscore_opt
+
+        if '-' in opt:
+            warnings.warn(
+                "Usage of dash-separated '%s' will not be supported in future "
+                "versions. Please use the underscore name '%s' instead"
+                % (opt, underscore_opt))
+        return underscore_opt
+
+    def make_option_lowercase(self, opt, section):
+        if section != 'metadata' or opt.islower():
+            return opt
+
+        lowercase_opt = opt.lower()
+        warnings.warn(
+            "Usage of uppercase key '%s' in '%s' will be deprecated in future "
+            "versions. Please use lowercase '%s' instead"
+            % (opt, section, lowercase_opt)
+        )
+        return lowercase_opt
 
-    def _set_command_options(self, command_obj, option_dict=None):
+    # FIXME: 'Distribution._set_command_options' is too complex (14)
+    def _set_command_options(self, command_obj, option_dict=None):  # noqa: C901
         """
         Set the options for 'command_obj' from 'option_dict'.  Basically
         this means copying elements of a dictionary ('option_dict') to
         attributes of an instance ('command').
 
         'command_obj' must be a Command instance.  If 'option_dict' is not
         supplied, uses the standard option dictionary for this command
@@ -661,27 +687,27 @@
                 bool_opts = []
             try:
                 neg_opt = command_obj.negative_opt
             except AttributeError:
                 neg_opt = {}
 
             try:
-                is_string = isinstance(value, six.string_types)
+                is_string = isinstance(value, str)
                 if option in neg_opt and is_string:
                     setattr(command_obj, neg_opt[option], not strtobool(value))
                 elif option in bool_opts and is_string:
                     setattr(command_obj, option, strtobool(value))
                 elif hasattr(command_obj, option):
                     setattr(command_obj, option, value)
                 else:
                     raise DistutilsOptionError(
                         "error in %s: command '%s' has no such option '%s'"
                         % (source, command_name, option))
-            except ValueError as msg:
-                raise DistutilsOptionError(msg)
+            except ValueError as e:
+                raise DistutilsOptionError(e) from e
 
     def parse_config_files(self, filenames=None, ignore_option_errors=False):
         """Parses configuration files from various levels
         and loads configuration.
 
         """
         self._parse_config_files(filenames=filenames)
@@ -839,18 +865,18 @@
         """Handle 'exclude()' for list/tuple attrs without a special handler"""
         if not isinstance(value, sequence):
             raise DistutilsSetupError(
                 "%s: setting must be a list or tuple (%r)" % (name, value)
             )
         try:
             old = getattr(self, name)
-        except AttributeError:
+        except AttributeError as e:
             raise DistutilsSetupError(
                 "%s: No such distribution setting" % name
-            )
+            ) from e
         if old is not None and not isinstance(old, sequence):
             raise DistutilsSetupError(
                 name + ": this setting cannot be changed via include/exclude"
             )
         elif old:
             setattr(self, name, [item for item in old if item not in value])
 
@@ -859,18 +885,18 @@
 
         if not isinstance(value, sequence):
             raise DistutilsSetupError(
                 "%s: setting must be a list (%r)" % (name, value)
             )
         try:
             old = getattr(self, name)
-        except AttributeError:
+        except AttributeError as e:
             raise DistutilsSetupError(
                 "%s: No such distribution setting" % name
-            )
+            ) from e
         if old is None:
             setattr(self, name, value)
         elif not isinstance(old, sequence):
             raise DistutilsSetupError(
                 name + ": this setting cannot be changed via include/exclude"
             )
         else:
@@ -995,15 +1021,15 @@
         """If there were any non-global "display-only" options
         (--help-commands or the metadata display options) on the command
         line, display the requested info and return true; else return
         false.
         """
         import sys
 
-        if six.PY2 or self.help_commands:
+        if self.help_commands:
             return _Distribution.handle_display_options(self, option_order)
 
         # Stdout may be StringIO (e.g. in tests)
         if not isinstance(sys.stdout, io.TextIOWrapper):
             return _Distribution.handle_display_options(self, option_order)
 
         # Don't wrap stdout if utf-8 is already the encoding. Provides
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/errors.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/extension.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import re
 import functools
 import distutils.core
 import distutils.errors
 import distutils.extension
 
-from setuptools.extern.six.moves import map
-
 from .monkey import get_unpatched
 
 
 def _have_cython():
     """
     Return True if Cython can be imported.
     """
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/extern/__init__.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import importlib.util
 import sys
 
 
 class VendorImporter:
     """
     A PEP 302 meta path importer for finding optionally-vendored
     or otherwise naturally-installed packages from root_name.
@@ -16,25 +17,18 @@
     def search_path(self):
         """
         Search first the vendor package then as a natural package.
         """
         yield self.vendor_pkg + '.'
         yield ''
 
-    def find_module(self, fullname, path=None):
-        """
-        Return self when fullname starts with root_name and the
-        target module is one vendored through this importer.
-        """
+    def _module_matches_namespace(self, fullname):
+        """Figure out if the target module is vendored."""
         root, base, target = fullname.partition(self.root_name + '.')
-        if root:
-            return
-        if not any(map(target.startswith, self.vendored_names)):
-            return
-        return self
+        return not root and any(map(target.startswith, self.vendored_names))
 
     def load_module(self, fullname):
         """
         Iterate over the search path to locate and load fullname.
         """
         root, base, target = fullname.partition(self.root_name + '.')
         for prefix in self.search_path:
@@ -50,17 +44,30 @@
             raise ImportError(
                 "The '{target}' package is required; "
                 "normally this is bundled with this package so if you get "
                 "this warning, consult the packager of your "
                 "distribution.".format(**locals())
             )
 
+    def create_module(self, spec):
+        return self.load_module(spec.name)
+
+    def exec_module(self, module):
+        pass
+
+    def find_spec(self, fullname, path=None, target=None):
+        """Return a module spec for vendored names."""
+        return (
+            importlib.util.spec_from_loader(fullname, self)
+            if self._module_matches_namespace(fullname) else None
+        )
+
     def install(self):
         """
         Install this importer into sys.meta_path if not already present.
         """
         if self not in sys.meta_path:
             sys.meta_path.append(self)
 
 
-names = 'six', 'packaging', 'pyparsing', 'ordered_set',
-VendorImporter(__name__, names, 'setuptools._vendor').install()
+names = 'packaging', 'pyparsing', 'appdirs'
+VendorImporter(__name__, names).install()
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/glob.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/glob.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,44 +43,37 @@
         s = next(it)  # skip empty string
         assert not s
     return it
 
 
 def _iglob(pathname, recursive):
     dirname, basename = os.path.split(pathname)
+    glob_in_dir = glob2 if recursive and _isrecursive(basename) else glob1
+
     if not has_magic(pathname):
         if basename:
             if os.path.lexists(pathname):
                 yield pathname
         else:
             # Patterns ending with a slash should match only directories
             if os.path.isdir(dirname):
                 yield pathname
         return
+
     if not dirname:
-        if recursive and _isrecursive(basename):
-            for x in glob2(dirname, basename):
-                yield x
-        else:
-            for x in glob1(dirname, basename):
-                yield x
+        yield from glob_in_dir(dirname, basename)
         return
     # `os.path.split()` returns the argument itself as a dirname if it is a
     # drive or UNC path.  Prevent an infinite recursion if a drive or UNC path
     # contains magic characters (i.e. r'\\?\C:').
     if dirname != pathname and has_magic(dirname):
         dirs = _iglob(dirname, recursive)
     else:
         dirs = [dirname]
-    if has_magic(basename):
-        if recursive and _isrecursive(basename):
-            glob_in_dir = glob2
-        else:
-            glob_in_dir = glob1
-    else:
+    if not has_magic(basename):
         glob_in_dir = glob0
     for dirname in dirs:
         for name in glob_in_dir(dirname, basename):
             yield os.path.join(dirname, name)
 
 
 # These 2 helper functions non-recursively glob inside a literal directory.
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/gui-32.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/gui-64.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/gui.exe` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/launch.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/launch.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         __file__=script_name,
         __name__='__main__',
         __doc__=None,
     )
     sys.argv[:] = sys.argv[1:]
 
     open_ = getattr(tokenize, 'open', open)
-    script = open_(script_name).read()
+    with open_(script_name) as fid:
+        script = fid.read()
     norm_script = script.replace('\\r\\n', '\\n')
     code = compile(norm_script, script_name, 'exec')
     exec(code, namespace)
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/lib2to3_ex.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """
 Customized Mixin2to3 support:
 
  - adds support for converting doctests
-
-
-This module raises an ImportError on Python 2.
 """
 
 import warnings
 from distutils.util import Mixin2to3 as _Mixin2to3
 from distutils import log
 from lib2to3.refactor import RefactoringTool, get_fixers_from_package
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/monkey.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/monkey.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import distutils.filelist
 import platform
 import types
 import functools
 from importlib import import_module
 import inspect
 
-from setuptools.extern import six
-
 import setuptools
 
 __all__ = []
 """
 Everything is private. Contact the project team
 if you think you need this functionality.
 """
@@ -33,15 +31,15 @@
     if platform.python_implementation() == "Jython":
         return (cls,) + cls.__bases__
     return inspect.getmro(cls)
 
 
 def get_unpatched(item):
     lookup = (
-        get_unpatched_class if isinstance(item, six.class_types) else
+        get_unpatched_class if isinstance(item, type) else
         get_unpatched_function if isinstance(item, types.FunctionType) else
         lambda item: None
     )
     return lookup(item)
 
 
 def get_unpatched_class(cls):
@@ -134,15 +132,15 @@
     Patch functions in distutils to use standalone Microsoft Visual C++
     compilers.
     """
     # import late to avoid circular imports on Python < 3.5
     msvc = import_module('setuptools.msvc')
 
     if platform.system() != 'Windows':
-        # Compilers only availables on Microsoft Windows
+        # Compilers only available on Microsoft Windows
         return
 
     def patch_params(mod_name, func_name):
         """
         Prepare the parameters for patch_func to patch indicated function.
         """
         repl_prefix = 'msvc9_' if 'msvc9' in mod_name else 'msvc14_'
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/msvc.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/msvc.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,26 +20,25 @@
 """
 
 import json
 from io import open
 from os import listdir, pathsep
 from os.path import join, isfile, isdir, dirname
 import sys
+import contextlib
 import platform
 import itertools
 import subprocess
 import distutils.errors
 from setuptools.extern.packaging.version import LegacyVersion
 
-from setuptools.extern.six.moves import filterfalse
-
 from .monkey import get_unpatched
 
 if platform.system() == 'Windows':
-    from setuptools.extern.six.moves import winreg
+    import winreg
     from os import environ
 else:
     # Mock winreg and environ so the module can be imported on this platform.
 
     class winreg:
         HKEY_USERS = None
         HKEY_CURRENT_USER = None
@@ -273,15 +272,15 @@
         out = subprocess.check_output(
             'cmd /u /c "{}" {} && set'.format(vcvarsall, plat_spec),
             stderr=subprocess.STDOUT,
         ).decode('utf-16le', errors='replace')
     except subprocess.CalledProcessError as exc:
         raise distutils.errors.DistutilsPlatformError(
             "Error executing {}".format(exc.cmd)
-        )
+        ) from exc
 
     env = {
         key.lower(): value
         for key, _, value in
         (line.partition('=') for line in out.splitlines())
         if key and value
     }
@@ -336,15 +335,15 @@
     as to what action will resolve it.
     """
     # Error if MSVC++ directory not found or environment not set
     message = exc.args[0]
 
     if "vcvarsall" in message.lower() or "visual c" in message.lower():
         # Special error message if MSVC++ not installed
-        tmpl = 'Microsoft Visual C++ {version:0.1f} is required.'
+        tmpl = 'Microsoft Visual C++ {version:0.1f} or greater is required.'
         message = tmpl.format(**locals())
         msdownload = 'www.microsoft.com/download/details.aspx?id=%d'
         if version == 9.0:
             if arch.lower().find('ia64') > -1:
                 # For VC++ 9.0, if IA64 support is needed, redirect user
                 # to Windows SDK 7.0.
                 # Note: No download link available from Microsoft.
@@ -356,16 +355,17 @@
                 message += ' Get it from http://aka.ms/vcpython27'
         elif version == 10.0:
             # For VC++ 10.0 Redirect user to Windows SDK 7.1
             message += ' Get it with "Microsoft Windows SDK 7.1": '
             message += msdownload % 8279
         elif version >= 14.0:
             # For VC++ 14.X Redirect user to latest Visual C++ Build Tools
-            message += (' Get it with "Build Tools for Visual Studio": '
-                        r'https://visualstudio.microsoft.com/downloads/')
+            message += (' Get it with "Microsoft C++ Build Tools": '
+                        r'https://visualstudio.microsoft.com'
+                        r'/visual-cpp-build-tools/')
 
     exc.args = (message, )
 
 
 class PlatformInfo:
     """
     Current and Target Architectures information.
@@ -639,30 +639,35 @@
         Return
         ------
         str
             value
         """
         key_read = winreg.KEY_READ
         openkey = winreg.OpenKey
+        closekey = winreg.CloseKey
         ms = self.microsoft
         for hkey in self.HKEYS:
+            bkey = None
             try:
                 bkey = openkey(hkey, ms(key), 0, key_read)
             except (OSError, IOError):
                 if not self.pi.current_is_x86():
                     try:
                         bkey = openkey(hkey, ms(key, True), 0, key_read)
                     except (OSError, IOError):
                         continue
                 else:
                     continue
             try:
                 return winreg.QueryValueEx(bkey, name)[0]
             except (OSError, IOError):
                 pass
+            finally:
+                if bkey:
+                    closekey(bkey)
 
 
 class SystemInfo:
     """
     Microsoft Windows and Visual Studio related system information.
 
     Parameters
@@ -716,35 +721,31 @@
         ------
         list of float
             Versions
         """
         ms = self.ri.microsoft
         vckeys = (self.ri.vc, self.ri.vc_for_python, self.ri.vs)
         vs_vers = []
-        for hkey in self.ri.HKEYS:
-            for key in vckeys:
-                try:
-                    bkey = winreg.OpenKey(hkey, ms(key), 0, winreg.KEY_READ)
-                except (OSError, IOError):
-                    continue
+        for hkey, key in itertools.product(self.ri.HKEYS, vckeys):
+            try:
+                bkey = winreg.OpenKey(hkey, ms(key), 0, winreg.KEY_READ)
+            except (OSError, IOError):
+                continue
+            with bkey:
                 subkeys, values, _ = winreg.QueryInfoKey(bkey)
                 for i in range(values):
-                    try:
+                    with contextlib.suppress(ValueError):
                         ver = float(winreg.EnumValue(bkey, i)[0])
                         if ver not in vs_vers:
                             vs_vers.append(ver)
-                    except ValueError:
-                        pass
                 for i in range(subkeys):
-                    try:
+                    with contextlib.suppress(ValueError):
                         ver = float(winreg.EnumKey(bkey, i))
                         if ver not in vs_vers:
                             vs_vers.append(ver)
-                    except ValueError:
-                        pass
         return sorted(vs_vers)
 
     def find_programdata_vs_vers(self):
         r"""
         Find Visual studio 2017+ versions from information in
         "C:\ProgramData\Microsoft\VisualStudio\Packages\_Instances".
 
@@ -916,16 +917,16 @@
         Return
         ------
         str
             version
         """
         return self._use_last_dir_name(join(self.WindowsSdkDir, 'lib'))
 
-    @property
-    def WindowsSdkDir(self):
+    @property  # noqa: C901
+    def WindowsSdkDir(self):  # noqa: C901  # is too complex (12)  # FIXME
         """
         Microsoft Windows SDK directory.
 
         Return
         ------
         str
             path
@@ -1810,15 +1811,15 @@
         _unique_everseen('AAAABBBCCDAABBB') --> A B C D
 
         _unique_everseen('ABBCcAD', str.lower) --> A B C D
         """
         seen = set()
         seen_add = seen.add
         if key is None:
-            for element in filterfalse(seen.__contains__, iterable):
+            for element in itertools.filterfalse(seen.__contains__, iterable):
                 seen_add(element)
                 yield element
         else:
             for element in iterable:
                 k = key(element)
                 if k not in seen:
                     seen_add(k)
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/namespaces.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/namespaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 from distutils import log
 import itertools
 
-from setuptools.extern.six.moves import map
-
 
 flatten = itertools.chain.from_iterable
 
 
 class Installer:
 
     nspkg_ext = '-nspkg.pth'
@@ -68,16 +66,14 @@
     )
     "additional line(s) when a parent package is indicated"
 
     def _get_root(self):
         return "sys._getframe(1).f_locals['sitedir']"
 
     def _gen_nspkg_line(self, pkg):
-        # ensure pkg is not a unicode string under Python 2.7
-        pkg = str(pkg)
         pth = tuple(pkg.split('.'))
         root = self._get_root()
         tmpl_lines = self._nspkg_tmpl
         parent, sep, child = pkg.rpartition('.')
         if parent:
             tmpl_lines += self._nspkg_tmpl_multi
         return ';'.join(tmpl_lines) % locals() + '\n'
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/package_index.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/package_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """PyPI and direct package downloading"""
 import sys
 import os
 import re
+import io
 import shutil
 import socket
 import base64
 import hashlib
 import itertools
 import warnings
+import configparser
+import html
+import http.client
+import urllib.parse
+import urllib.request
+import urllib.error
 from functools import wraps
 
-from setuptools.extern import six
-from setuptools.extern.six.moves import urllib, http_client, configparser, map
-
 import setuptools
 from pkg_resources import (
     CHECKOUT_DIST, Distribution, BINARY_DIST, normalize_path, SOURCE_DIST,
     Environment, find_distributions, safe_name, safe_version,
     to_filename, Requirement, DEVELOP_DIST, EGG_DIST,
 )
 from setuptools import ssl_support
 from distutils import log
 from distutils.errors import DistutilsError
 from fnmatch import translate
-from setuptools.py27compat import get_all_headers
-from setuptools.py33compat import unescape
 from setuptools.wheel import Wheel
 
-__metaclass__ = type
-
 EGG_FRAGMENT = re.compile(r'^egg=([-A-Za-z0-9_.+!]+)$')
 HREF = re.compile(r"""href\s*=\s*['"]?([^'"> ]+)""", re.I)
 PYPI_MD5 = re.compile(
     r'<a href="([^"#]+)">([^<]+)</a>\n\s+\(<a (?:title="MD5 hash"\n\s+)'
     r'href="[^?]+\?:action=show_md5&amp;digest=([0-9a-f]{32})">md5</a>\)'
 )
 URL_SCHEME = re.compile('([-+.a-z0-9]{2,}):', re.I).match
@@ -49,18 +49,18 @@
 user_agent = _tmpl.format(
     py_major='{}.{}'.format(*sys.version_info), setuptools=setuptools)
 
 
 def parse_requirement_arg(spec):
     try:
         return Requirement.parse(spec)
-    except ValueError:
+    except ValueError as e:
         raise DistutilsError(
             "Not a URL, existing file, or requirement spec: %r" % (spec,)
-        )
+        ) from e
 
 
 def parse_bdist_wininst(name):
     """Return (base,pyversion) or (None,None) for possible .exe name"""
 
     lower = name.lower()
     base, py_ver, plat = None, None, None
@@ -187,15 +187,15 @@
 def unique_everseen(iterable, key=None):
     "List unique elements, preserving order. Remember all elements ever seen."
     # unique_everseen('AAAABBBCCDAABBB') --> A B C D
     # unique_everseen('ABBCcAD', str.lower) --> A B C D
     seen = set()
     seen_add = seen.add
     if key is None:
-        for element in six.moves.filterfalse(seen.__contains__, iterable):
+        for element in itertools.filterfalse(seen.__contains__, iterable):
             seen_add(element)
             yield element
     else:
         for element in iterable:
             k = key(element)
             if k not in seen:
                 seen_add(k)
@@ -316,15 +316,16 @@
             and (ca_bundle or ssl_support.find_ca_bundle())
         )
         if use_ssl:
             self.opener = ssl_support.opener_for(ca_bundle)
         else:
             self.opener = urllib.request.urlopen
 
-    def process_url(self, url, retrieve=False):
+    # FIXME: 'PackageIndex.process_url' is too complex (14)
+    def process_url(self, url, retrieve=False):  # noqa: C901
         """Evaluate a URL as a possible download, and maybe retrieve it"""
         if url in self.scanned_urls and not retrieve:
             return
         self.scanned_urls[url] = True
         if not URL_SCHEME(url):
             self.process_filename(url)
             return
@@ -424,57 +425,61 @@
         egg_path, setup_path = lines
 
         for dist in find_distributions(os.path.join(path, egg_path)):
             dist.location = os.path.join(path, *lines)
             dist.precedence = SOURCE_DIST
             self.add(dist)
 
+    def _scan(self, link):
+        # Process a URL to see if it's for a package page
+        NO_MATCH_SENTINEL = None, None
+        if not link.startswith(self.index_url):
+            return NO_MATCH_SENTINEL
+
+        parts = list(map(
+            urllib.parse.unquote, link[len(self.index_url):].split('/')
+        ))
+        if len(parts) != 2 or '#' in parts[1]:
+            return NO_MATCH_SENTINEL
+
+        # it's a package page, sanitize and index it
+        pkg = safe_name(parts[0])
+        ver = safe_version(parts[1])
+        self.package_pages.setdefault(pkg.lower(), {})[link] = True
+        return to_filename(pkg), to_filename(ver)
+
     def process_index(self, url, page):
         """Process the contents of a PyPI page"""
 
-        def scan(link):
-            # Process a URL to see if it's for a package page
-            if link.startswith(self.index_url):
-                parts = list(map(
-                    urllib.parse.unquote, link[len(self.index_url):].split('/')
-                ))
-                if len(parts) == 2 and '#' not in parts[1]:
-                    # it's a package page, sanitize and index it
-                    pkg = safe_name(parts[0])
-                    ver = safe_version(parts[1])
-                    self.package_pages.setdefault(pkg.lower(), {})[link] = True
-                    return to_filename(pkg), to_filename(ver)
-            return None, None
-
         # process an index page into the package-page index
         for match in HREF.finditer(page):
             try:
-                scan(urllib.parse.urljoin(url, htmldecode(match.group(1))))
+                self._scan(urllib.parse.urljoin(url, htmldecode(match.group(1))))
             except ValueError:
                 pass
 
-        pkg, ver = scan(url)  # ensure this page is in the page index
-        if pkg:
-            # process individual package page
-            for new_url in find_external_links(url, page):
-                # Process the found URL
-                base, frag = egg_info_for_url(new_url)
-                if base.endswith('.py') and not frag:
-                    if ver:
-                        new_url += '#egg=%s-%s' % (pkg, ver)
-                    else:
-                        self.need_version_info(url)
-                self.scan_url(new_url)
-
-            return PYPI_MD5.sub(
-                lambda m: '<a href="%s#md5=%s">%s</a>' % m.group(1, 3, 2), page
-            )
-        else:
+        pkg, ver = self._scan(url)  # ensure this page is in the page index
+        if not pkg:
             return ""  # no sense double-scanning non-package pages
 
+        # process individual package page
+        for new_url in find_external_links(url, page):
+            # Process the found URL
+            base, frag = egg_info_for_url(new_url)
+            if base.endswith('.py') and not frag:
+                if ver:
+                    new_url += '#egg=%s-%s' % (pkg, ver)
+                else:
+                    self.need_version_info(url)
+            self.scan_url(new_url)
+
+        return PYPI_MD5.sub(
+            lambda m: '<a href="%s#md5=%s">%s</a>' % m.group(1, 3, 2), page
+        )
+
     def need_version_info(self, url):
         self.scan_all(
             "Page at %s links to .py file(s) without version info; an index "
             "scan is required.", url
         )
 
     def scan_all(self, msg=None, *args):
@@ -587,15 +592,15 @@
             elif os.path.exists(spec):
                 # Existing file or directory, just return it
                 return spec
             else:
                 spec = parse_requirement_arg(spec)
         return getattr(self.fetch_distribution(spec, tmpdir), 'location', None)
 
-    def fetch_distribution(
+    def fetch_distribution(  # noqa: C901  # is too complex (14)  # FIXME
             self, requirement, tmpdir, force_scan=False, source=False,
             develop_ok=False, local_index=None):
         """Obtain a distribution suitable for fulfilling `requirement`
 
         `requirement` must be a ``pkg_resources.Requirement`` instance.
         If necessary, or if the `force_scan` flag is set, the requirement is
         searched for in the (online) package index as well as the locally
@@ -736,15 +741,15 @@
                 )
             headers = fp.info()
             blocknum = 0
             bs = self.dl_blocksize
             size = -1
             if "content-length" in headers:
                 # Some servers return multiple Content-Length headers :(
-                sizes = get_all_headers(headers, 'Content-Length')
+                sizes = headers.get_all('Content-Length')
                 size = max(map(int, sizes))
                 self.reporthook(url, filename, blocknum, bs, size)
             with open(filename, 'wb') as tfp:
                 while True:
                     block = fp.read(bs)
                     if block:
                         checker.feed(block)
@@ -758,48 +763,49 @@
         finally:
             if fp:
                 fp.close()
 
     def reporthook(self, url, filename, blocknum, blksize, size):
         pass  # no-op
 
-    def open_url(self, url, warning=None):
+    # FIXME:
+    def open_url(self, url, warning=None):  # noqa: C901  # is too complex (12)
         if url.startswith('file:'):
             return local_open(url)
         try:
             return open_with_auth(url, self.opener)
-        except (ValueError, http_client.InvalidURL) as v:
+        except (ValueError, http.client.InvalidURL) as v:
             msg = ' '.join([str(arg) for arg in v.args])
             if warning:
                 self.warn(warning, msg)
             else:
-                raise DistutilsError('%s %s' % (url, msg))
+                raise DistutilsError('%s %s' % (url, msg)) from v
         except urllib.error.HTTPError as v:
             return v
         except urllib.error.URLError as v:
             if warning:
                 self.warn(warning, v.reason)
             else:
                 raise DistutilsError("Download error for %s: %s"
-                                     % (url, v.reason))
-        except http_client.BadStatusLine as v:
+                                     % (url, v.reason)) from v
+        except http.client.BadStatusLine as v:
             if warning:
                 self.warn(warning, v.line)
             else:
                 raise DistutilsError(
                     '%s returned a bad status line. The server might be '
                     'down, %s' %
                     (url, v.line)
-                )
-        except (http_client.HTTPException, socket.error) as v:
+                ) from v
+        except (http.client.HTTPException, socket.error) as v:
             if warning:
                 self.warn(warning, v)
             else:
                 raise DistutilsError("Download error for %s: %s"
-                                     % (url, v))
+                                     % (url, v)) from v
 
     def _download_url(self, scheme, url, tmpdir):
         # Determine download filename
         #
         name, fragment = egg_info_for_url(url)
         if name:
             while '..' in name:
@@ -936,15 +942,15 @@
 # This pattern matches a character entity reference (a decimal numeric
 # references, a hexadecimal numeric reference, or a named reference).
 entity_sub = re.compile(r'&(#(\d+|x[\da-fA-F]+)|[\w.:-]+);?').sub
 
 
 def decode_entity(match):
     what = match.group(0)
-    return unescape(what)
+    return html.unescape(what)
 
 
 def htmldecode(text):
     """
     Decode HTML entities in the given text.
 
     >>> htmldecode(
@@ -968,16 +974,15 @@
         return _socket_timeout
 
     return _socket_timeout
 
 
 def _encode_auth(auth):
     """
-    A function compatible with Python 2.3-3.3 that will encode
-    auth from a URL suitable for an HTTP header.
+    Encode auth from a URL suitable for an HTTP header.
     >>> str(_encode_auth('username%3Apassword'))
     'dXNlcm5hbWU6cGFzc3dvcmQ='
 
     Long auth strings should not cause a newline to be inserted.
     >>> long_auth = 'username:' + 'password'*10
     >>> chr(10) in str(_encode_auth(long_auth))
     False
@@ -1052,15 +1057,15 @@
 
     parsed = urllib.parse.urlparse(url)
     scheme, netloc, path, params, query, frag = parsed
 
     # Double scheme does not raise on macOS as revealed by a
     # failing test. We would expect "nonnumeric port". Refs #20.
     if netloc.endswith(':'):
-        raise http_client.InvalidURL("nonnumeric port: ''")
+        raise http.client.InvalidURL("nonnumeric port: ''")
 
     if scheme in ('http', 'https'):
         auth, address = _splituser(netloc)
     else:
         auth = None
 
     if not auth:
@@ -1132,9 +1137,9 @@
                 "</head><body>{files}</body></html>")
             body = tmpl.format(url=url, files='\n'.join(files))
         status, message = 200, "OK"
     else:
         status, message, body = 404, "Path not found", "Not found"
 
     headers = {'content-type': 'text/html'}
-    body_stream = six.StringIO(body)
+    body_stream = io.StringIO(body)
     return urllib.error.HTTPError(url, status, message, headers, body_stream)
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/sandbox.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/sandbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 import operator
 import functools
 import itertools
 import re
 import contextlib
 import pickle
 import textwrap
+import builtins
 
-from setuptools.extern import six
-from setuptools.extern.six.moves import builtins, map
-
-import pkg_resources.py31compat
+import pkg_resources
 from distutils.errors import DistutilsError
 from pkg_resources import working_set
 
 if sys.platform.startswith('java'):
     import org.python.modules.posix.PosixModule as _os
 else:
     _os = sys.modules[os.name]
@@ -66,15 +64,15 @@
 
 
 @contextlib.contextmanager
 def override_temp(replacement):
     """
     Monkey-patch tempfile.tempdir with replacement, ensuring it exists
     """
-    pkg_resources.py31compat.makedirs(replacement, exist_ok=True)
+    os.makedirs(replacement, exist_ok=True)
 
     saved = tempfile.tempdir
 
     tempfile.tempdir = replacement
 
     try:
         yield
@@ -134,15 +132,15 @@
     def resume(self):
         "restore and re-raise any exception"
 
         if '_saved' not in vars(self):
             return
 
         type, exc = map(pickle.loads, self._saved)
-        six.reraise(type, exc, self._tb)
+        raise exc.with_traceback(self._tb)
 
 
 @contextlib.contextmanager
 def save_modules():
     """
     Context in which imported modules are saved.
 
@@ -181,24 +179,33 @@
 
 
 @contextlib.contextmanager
 def setup_context(setup_dir):
     temp_dir = os.path.join(setup_dir, 'temp')
     with save_pkg_resources_state():
         with save_modules():
-            hide_setuptools()
             with save_path():
+                hide_setuptools()
                 with save_argv():
                     with override_temp(temp_dir):
                         with pushd(setup_dir):
                             # ensure setuptools commands are available
                             __import__('setuptools')
                             yield
 
 
+_MODULES_TO_HIDE = {
+    'setuptools',
+    'distutils',
+    'pkg_resources',
+    'Cython',
+    '_distutils_hack',
+}
+
+
 def _needs_hiding(mod_name):
     """
     >>> _needs_hiding('setuptools')
     True
     >>> _needs_hiding('pkg_resources')
     True
     >>> _needs_hiding('setuptools_plugin')
@@ -208,25 +215,29 @@
     >>> _needs_hiding('distutils')
     True
     >>> _needs_hiding('os')
     False
     >>> _needs_hiding('Cython')
     True
     """
-    pattern = re.compile(r'(setuptools|pkg_resources|distutils|Cython)(\.|$)')
-    return bool(pattern.match(mod_name))
+    base_module = mod_name.split('.', 1)[0]
+    return base_module in _MODULES_TO_HIDE
 
 
 def hide_setuptools():
     """
     Remove references to setuptools' modules from sys.modules to allow the
     invocation to import the most appropriate setuptools. This technique is
     necessary to avoid issues such as #315 where setuptools upgrading itself
     would fail to find a function declared in the metadata.
     """
+    _distutils_hack = sys.modules.get('_distutils_hack', None)
+    if _distutils_hack is not None:
+        _distutils_hack.remove_shim()
+
     modules = filter(_needs_hiding, sys.modules)
     _clear_modules(modules)
 
 
 def run_setup(setup_script, args):
     """Run a distutils setup script, sandboxed in its directory"""
     setup_dir = os.path.abspath(os.path.dirname(setup_script))
@@ -234,23 +245,16 @@
         try:
             sys.argv[:] = [setup_script] + list(args)
             sys.path.insert(0, setup_dir)
             # reset to include setup dir, w/clean callback list
             working_set.__init__()
             working_set.callbacks.append(lambda dist: dist.activate())
 
-            # __file__ should be a byte string on Python 2 (#712)
-            dunder_file = (
-                setup_script
-                if isinstance(setup_script, str) else
-                setup_script.encode(sys.getfilesystemencoding())
-            )
-
             with DirectorySandbox(setup_dir):
-                ns = dict(__file__=dunder_file, __name__='__main__')
+                ns = dict(__file__=setup_script, __name__='__main__')
                 _execfile(setup_script, ns)
         except SystemExit as v:
             if v.args and v.args[0]:
                 raise
             # Normal exit, just return
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/ssl_support.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/ssl_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import socket
 import atexit
 import re
 import functools
+import urllib.request
+import http.client
 
-from setuptools.extern.six.moves import urllib, http_client, map, filter
 
 from pkg_resources import ResolutionError, ExtractionError
 
 try:
     import ssl
 except ImportError:
     ssl = None
@@ -27,15 +28,15 @@
 /System/Library/OpenSSL/certs/cert.pem
 /usr/local/share/certs/ca-root-nss.crt
 /etc/ssl/ca-bundle.pem
 """.strip().split()
 
 try:
     HTTPSHandler = urllib.request.HTTPSHandler
-    HTTPSConnection = http_client.HTTPSConnection
+    HTTPSConnection = http.client.HTTPSConnection
 except AttributeError:
     HTTPSHandler = HTTPSConnection = object
 
 is_available = ssl is not None and object not in (
     HTTPSHandler, HTTPSConnection)
 
 
@@ -51,15 +52,15 @@
 
 if not CertificateError:
 
     class CertificateError(ValueError):
         pass
 
 
-if not match_hostname:
+if not match_hostname:  # noqa: C901  # 'If 59' is too complex (21)  # FIXME
 
     def _dnsname_match(dn, hostname, max_wildcards=1):
         """Matching according to RFC 6125, section 6.4.3
 
         https://tools.ietf.org/html/rfc6125#section-6.4.3
         """
         pats = []
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/unicode_utils.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/unicode_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import unicodedata
 import sys
 
-from setuptools.extern import six
-
 
 # HFS Plus uses decomposed UTF-8
 def decompose(path):
-    if isinstance(path, six.text_type):
+    if isinstance(path, str):
         return unicodedata.normalize('NFD', path)
     try:
         path = path.decode('utf-8')
         path = unicodedata.normalize('NFD', path)
         path = path.encode('utf-8')
     except UnicodeError:
         pass  # Not UTF-8
@@ -19,15 +17,15 @@
 
 def filesys_decode(path):
     """
     Ensure that the given path is decoded,
     NONE when no expected encoding works
     """
 
-    if isinstance(path, six.text_type):
+    if isinstance(path, str):
         return path
 
     fs_enc = sys.getfilesystemencoding() or 'utf-8'
     candidates = fs_enc, 'utf-8'
 
     for enc in candidates:
         try:
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/wheel.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,17 @@
 import zipfile
 
 import pkg_resources
 import setuptools
 from pkg_resources import parse_version
 from setuptools.extern.packaging.tags import sys_tags
 from setuptools.extern.packaging.utils import canonicalize_name
-from setuptools.extern.six import PY3
 from setuptools.command.egg_info import write_requirements
 
 
-__metaclass__ = type
-
-
 WHEEL_NAME = re.compile(
     r"""^(?P<project_name>.+?)-(?P<version>\d.*?)
     ((-(?P<build>\d.*?))?-(?P<py_version>.+?)-(?P<abi>.+?)-(?P<platform>.+?)
     )\.whl$""",
     re.VERBOSE).match
 
 NAMESPACE_PACKAGE_INIT = \
@@ -108,15 +104,15 @@
         self._move_data_entries(destination_eggdir, dist_data)
         self._fix_namespace_packages(egg_info, destination_eggdir)
 
     @staticmethod
     def _convert_metadata(zf, destination_eggdir, dist_info, egg_info):
         def get_metadata(name):
             with zf.open(posixpath.join(dist_info, name)) as fp:
-                value = fp.read().decode('utf-8') if PY3 else fp.read()
+                value = fp.read().decode('utf-8')
                 return email.parser.Parser().parsestr(value)
 
         wheel_metadata = get_metadata('WHEEL')
         # Check wheel format version is supported.
         wheel_version = parse_version(wheel_metadata.get('Wheel-Version'))
         wheel_v1 = (
             parse_version('1.0') <= wheel_version < parse_version('2.0dev0')
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools/windows_support.py` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/LICENSE` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (C) 2016 Jason R Coombs <jaraco@jaraco.com>
+Copyright Jason R. Coombs
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/METADATA` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 Metadata-Version: 2.1
 Name: setuptools
-Version: 47.1.0
+Version: 56.0.0
 Summary: Easily download, build, install, upgrade, and uninstall Python packages
 Home-page: https://github.com/pypa/setuptools
 Author: Python Packaging Authority
 Author-email: distutils-sig@python.org
 License: UNKNOWN
 Project-URL: Documentation, https://setuptools.readthedocs.io/
 Keywords: CPAN PyPI distutils eggs package management
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
-Description-Content-Type: text/x-rst; charset=UTF-8
+Requires-Python: >=3.6
 Provides-Extra: certs
 Requires-Dist: certifi (==2016.9.26) ; extra == 'certs'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
-Requires-Dist: jaraco.packaging (>=6.1) ; extra == 'docs'
+Requires-Dist: jaraco.packaging (>=8.2) ; extra == 'docs'
 Requires-Dist: rst.linker (>=1.9) ; extra == 'docs'
 Requires-Dist: pygments-github-lexers (==0.0.5) ; extra == 'docs'
+Requires-Dist: sphinx-inline-tabs ; extra == 'docs'
 Provides-Extra: ssl
 Requires-Dist: wincertstore (==0.2) ; (sys_platform == "win32") and extra == 'ssl'
-Provides-Extra: tests
-Requires-Dist: mock ; extra == 'tests'
-Requires-Dist: pytest-flake8 ; extra == 'tests'
-Requires-Dist: virtualenv (>=13.0.0) ; extra == 'tests'
-Requires-Dist: pytest-virtualenv (>=1.2.7) ; extra == 'tests'
-Requires-Dist: pytest (>=3.7) ; extra == 'tests'
-Requires-Dist: wheel ; extra == 'tests'
-Requires-Dist: coverage (>=4.5.1) ; extra == 'tests'
-Requires-Dist: pytest-cov (>=2.5.1) ; extra == 'tests'
-Requires-Dist: pip (>=19.1) ; extra == 'tests'
-Requires-Dist: futures ; (python_version == "2.7") and extra == 'tests'
-Requires-Dist: flake8-2020 ; (python_version >= "3.6") and extra == 'tests'
-Requires-Dist: paver ; (python_version >= "3.6") and extra == 'tests'
+Provides-Extra: testing
+Requires-Dist: pytest (>=4.6) ; extra == 'testing'
+Requires-Dist: pytest-checkdocs (>=2.4) ; extra == 'testing'
+Requires-Dist: pytest-flake8 ; extra == 'testing'
+Requires-Dist: pytest-cov ; extra == 'testing'
+Requires-Dist: pytest-enabler (>=1.0.1) ; extra == 'testing'
+Requires-Dist: mock ; extra == 'testing'
+Requires-Dist: flake8-2020 ; extra == 'testing'
+Requires-Dist: virtualenv (>=13.0.0) ; extra == 'testing'
+Requires-Dist: pytest-virtualenv (>=1.2.7) ; extra == 'testing'
+Requires-Dist: wheel ; extra == 'testing'
+Requires-Dist: paver ; extra == 'testing'
+Requires-Dist: pip (>=19.1) ; extra == 'testing'
+Requires-Dist: jaraco.envs ; extra == 'testing'
+Requires-Dist: pytest-xdist ; extra == 'testing'
+Requires-Dist: sphinx ; extra == 'testing'
+Requires-Dist: jaraco.path (>=3.2.0) ; extra == 'testing'
+Requires-Dist: pytest-black (>=0.3.7) ; (platform_python_implementation != "PyPy" and python_version < "3.10") and extra == 'testing'
+Requires-Dist: pytest-mypy ; (platform_python_implementation != "PyPy" and python_version < "3.10") and extra == 'testing'
 
 .. image:: https://img.shields.io/pypi/v/setuptools.svg
    :target: `PyPI link`_
 
 .. image:: https://img.shields.io/pypi/pyversions/setuptools.svg
    :target: `PyPI link`_
 
 .. _PyPI link: https://pypi.org/project/setuptools
 
-.. image:: https://dev.azure.com/jaraco/setuptools/_apis/build/status/pypa.setuptools?branchName=master
-   :target: https://dev.azure.com/jaraco/setuptools/_build/latest?definitionId=1&branchName=master
-
-.. image:: https://img.shields.io/travis/pypa/setuptools/master.svg?label=Linux%20CI&logo=travis&logoColor=white
-   :target: https://travis-ci.org/pypa/setuptools
-
-.. image:: https://img.shields.io/appveyor/ci/pypa/setuptools/master.svg?label=Windows%20CI&logo=appveyor&logoColor=white
-   :target: https://ci.appveyor.com/project/pypa/setuptools/branch/master
+.. image:: https://github.com/pypa/setuptools/workflows/tests/badge.svg
+   :target: https://github.com/pypa/setuptools/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
 
 .. image:: https://img.shields.io/readthedocs/setuptools/latest.svg
     :target: https://setuptools.readthedocs.io
 
 .. image:: https://img.shields.io/codecov/c/github/pypa/setuptools/master.svg?logo=codecov&logoColor=white
    :target: https://codecov.io/gh/pypa/setuptools
 
@@ -81,29 +81,34 @@
 
 Questions and comments should be directed to the `distutils-sig
 mailing list <http://mail.python.org/pipermail/distutils-sig/>`_.
 Bug reports and especially tested patches may be
 submitted directly to the `bug tracker
 <https://github.com/pypa/setuptools/issues>`_.
 
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
+
+Code of Conduct
+===============
+
+Everyone interacting in the setuptools project's codebases, issue trackers,
+chat rooms, and mailing lists is expected to follow the
+`PSF Code of Conduct <https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md>`_.
 
 
 For Enterprise
 ==============
 
 Available as part of the Tidelift Subscription.
 
 Setuptools and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-setuptools?utm_source=pypi-setuptools&utm_medium=referral&utm_campaign=github>`_.
 
-Code of Conduct
-===============
 
-Everyone interacting in the setuptools project's codebases, issue trackers,
-chat rooms, and mailing lists is expected to follow the
-`PyPA Code of Conduct <https://www.pypa.io/en/latest/code-of-conduct/>`_.
+Security Contact
+================
+
+To report a security vulnerability, please use the
+`Tidelift security contact <https://tidelift.com/security>`_.
+Tidelift will coordinate the fix and disclosure.
```

### Comparing `klvm_rs-0.6.1/venv/lib/python3.7/site-packages/setuptools-47.1.0.dist-info/entry_points.txt` & `klvm_rs-0.7.0/venv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-[console_scripts]
-easy_install = setuptools.command.easy_install:main
-easy_install-3.8 = setuptools.command.easy_install:main
-
 [distutils.commands]
 alias = setuptools.command.alias:alias
 bdist_egg = setuptools.command.bdist_egg:bdist_egg
 bdist_rpm = setuptools.command.bdist_rpm:bdist_rpm
-bdist_wininst = setuptools.command.bdist_wininst:bdist_wininst
 build_clib = setuptools.command.build_clib:build_clib
 build_ext = setuptools.command.build_ext:build_ext
 build_py = setuptools.command.build_py:build_py
 develop = setuptools.command.develop:develop
 dist_info = setuptools.command.dist_info:dist_info
 easy_install = setuptools.command.easy_install:easy_install
 egg_info = setuptools.command.egg_info:egg_info
@@ -59,10 +54,7 @@
 top_level.txt = setuptools.command.egg_info:write_toplevel_names
 
 [setuptools.finalize_distribution_options]
 2to3_doctests = setuptools.dist:Distribution._finalize_2to3_doctests
 keywords = setuptools.dist:Distribution._finalize_setup_keywords
 parent_finalize = setuptools.dist:_Distribution.finalize_options
 
-[setuptools.installation]
-eggsecutable = setuptools.command.easy_install:bootstrap
-
```

### Comparing `klvm_rs-0.6.1/wheel/Cargo.toml` & `klvm_rs-0.7.0/wheel/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "klvm_rs"
-version = "0.6.1"
+version = "0.7.0"
 authors = ["Richard Kiss <him@richardkiss.com>"]
 edition = "2021"
 license = "Apache-2.0"
 description = "Implementation of `klvm` for Chik Network's cryptocurrency"
 homepage = "https://github.com/Chik-Network/klvm_rs/"
 repository = "https://github.com/Chik-Network/klvm_rs/"
 readme = "README.md"
@@ -12,11 +12,11 @@
 [lib]
 name = "klvm_rs"
 crate-type = ["cdylib"]
 path = "src/lib.rs"
 
 [dependencies]
 klvmr = { path = ".." }
-pyo3 = { version = "=0.18.3", features = ["abi3-py37", "extension-module"] }
+pyo3 = { version = "=0.18.3", features = ["abi3-py38", "extension-module"] }
 
 [features]
 openssl = ["klvmr/openssl"]
```

### Comparing `klvm_rs-0.6.1/wheel/README.md` & `klvm_rs-0.7.0/wheel/README.md`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/at.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/at.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/casts.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/casts.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/chik_dialect.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/chik_dialect.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/curry_and_treehash.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/curry_and_treehash.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/de.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/de.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/klvm_rs.pyi` & `klvm_rs-0.7.0/wheel/python/klvm_rs/klvm_rs.pyi`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/klvm_storage.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/klvm_storage.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/klvm_tree.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/klvm_tree.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/program.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/program.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/replace.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/replace.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/ser.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/ser.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/klvm_rs/tree_hash.py` & `klvm_rs-0.7.0/wheel/python/klvm_rs/tree_hash.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/tests/test_apis.py` & `klvm_rs-0.7.0/wheel/python/tests/test_apis.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/tests/test_curry_and_treehash.py` & `klvm_rs-0.7.0/wheel/python/tests/test_curry_and_treehash.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/python/tests/test_program.py` & `klvm_rs-0.7.0/wheel/python/tests/test_program.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     # there's garbage at the end of the top-level list
     # `(a (q . 1) (c (q . 1) (q . 1)) (q . 0x1337))`
     plus = Program.fromhex("ff02ffff0101ffff04ffff0101ffff010180ffff0182133780")
     assert plus.uncurry() == (plus, None)
 
 
 def test_uncurry_not_pair():
-    # the second item in the list is expected to be a pair, with a qoute
+    # the second item in the list is expected to be a pair, with a quote
     # `(a 1 (c (q . 1) (q . 1)))`
     plus = Program.fromhex("ff02ff01ffff04ffff0101ffff01018080")
     assert plus.uncurry() == (plus, None)
 
 
 def test_uncurry_args_garbage():
     # there's garbage at the end of the args list
```

### Comparing `klvm_rs-0.6.1/wheel/python/tests/test_serialize.py` & `klvm_rs-0.7.0/wheel/python/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/src/adapt_response.rs` & `klvm_rs-0.7.0/wheel/src/adapt_response.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/src/api.rs` & `klvm_rs-0.7.0/wheel/src/api.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/wheel/src/lazy_node.rs` & `klvm_rs-0.7.0/wheel/src/lazy_node.rs`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/Cargo.lock` & `klvm_rs-0.7.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -761,15 +761,15 @@
  "serde",
  "serde_json",
  "sha1",
 ]
 
 [[package]]
 name = "klvm_rs"
-version = "0.6.1"
+version = "0.7.0"
 dependencies = [
  "klvmr",
  "pyo3",
 ]
 
 [[package]]
 name = "klvm_rs-fuzz"
@@ -777,26 +777,26 @@
 dependencies = [
  "klvmr",
  "libfuzzer-sys",
 ]
 
 [[package]]
 name = "klvm_wasm"
-version = "0.3.2"
+version = "0.7.0"
 dependencies = [
  "getrandom",
  "js-sys",
  "klvmr",
  "wasm-bindgen",
  "wasm-bindgen-test",
 ]
 
 [[package]]
 name = "klvmr"
-version = "0.6.1"
+version = "0.7.0"
 dependencies = [
  "chik-bls 0.4.0",
  "criterion",
  "hex",
  "hex-literal",
  "k256",
  "lazy_static",
```

### Comparing `klvm_rs-0.6.1/Cargo.toml` & `klvm_rs-0.7.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["wheel"]
 
 [package]
 name = "klvmr"
-version = "0.6.1"
+version = "0.7.0"
 authors = ["Richard Kiss <him@richardkiss.com>"]
 edition = "2021"
 license = "Apache-2.0"
 description = "Implementation of `klvm` for Chik Network's cryptocurrency"
 homepage = "https://github.com/Chik-Network/klvm_rs/"
 repository = "https://github.com/Chik-Network/klvm_rs/"
 readme = "README.md"
```

### Comparing `klvm_rs-0.6.1/python/klvm_rs/klvm_rs.pyi` & `klvm_rs-0.7.0/python/klvm_rs/klvm_rs.pyi`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/klvm_tree.py` & `klvm_rs-0.7.0/python/klvm_rs/klvm_tree.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/ser.py` & `klvm_rs-0.7.0/python/klvm_rs/ser.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/klvm_storage.py` & `klvm_rs-0.7.0/python/klvm_rs/klvm_storage.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/chik_dialect.py` & `klvm_rs-0.7.0/python/klvm_rs/chik_dialect.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/casts.py` & `klvm_rs-0.7.0/python/klvm_rs/casts.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/tree_hash.py` & `klvm_rs-0.7.0/python/klvm_rs/tree_hash.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/at.py` & `klvm_rs-0.7.0/python/klvm_rs/at.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/program.py` & `klvm_rs-0.7.0/python/klvm_rs/program.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/curry_and_treehash.py` & `klvm_rs-0.7.0/python/klvm_rs/curry_and_treehash.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/de.py` & `klvm_rs-0.7.0/python/klvm_rs/de.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/python/klvm_rs/replace.py` & `klvm_rs-0.7.0/python/klvm_rs/replace.py`

 * *Files identical despite different names*

### Comparing `klvm_rs-0.6.1/PKG-INFO` & `klvm_rs-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: klvm_rs
-Version: 0.6.1
+Version: 0.7.0
 Summary: Implementation of `klvm` for Chik Network's cryptocurrency
 Home-Page: https://github.com/Chik-Network/klvm_rs/
 Author: Richard Kiss <him@richardkiss.com>
 Author-email: Richard Kiss <him@richardkiss.com>
 License: Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/Chik-Network/klvm_rs/
```

