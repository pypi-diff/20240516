# Comparing `tmp/chik_rs-0.7.0.tar.gz` & `tmp/chik_rs-0.8.0.tar.gz`

## Comparing `chik_rs-0.7.0.tar` & `chik_rs-0.8.0.tar`

### file list

```diff
@@ -1,144 +1,147 @@
--rw-r--r--   0     1001      127      809 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/Cargo.toml
--rw-r--r--   0     1001      127     6975 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/docs/derive_macros.md
--rw-r--r--   0     1001      127     1067 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/error.rs
--rw-r--r--   0     1001      127    10932 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/from_klvm.rs
--rw-r--r--   0     1001      127     1742 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/klvm_decoder.rs
--rw-r--r--   0     1001      127     1518 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/klvm_encoder.rs
--rw-r--r--   0     1001      127     5612 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/lib.rs
--rw-r--r--   0     1001      127     3246 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/macros.rs
--rw-r--r--   0     1001      127     1026 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/match_byte.rs
--rw-r--r--   0     1001      127     8909 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/to_klvm.rs
--rw-r--r--   0     1001      127      670 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-traits/src/wrappers.rs
--rw-r--r--   0     1001      127     1151 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/Cargo.toml
--rw-r--r--   0     1001      127     7024 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/block_record.rs
--rw-r--r--   0     1001      127    17317 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/bytes.rs
--rw-r--r--   0     1001      127     4997 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/chik_protocol.rs
--rw-r--r--   0     1001      127     1194 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/classgroup.rs
--rw-r--r--   0     1001      127     4446 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/coin.rs
--rw-r--r--   0     1001      127      199 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/coin_spend.rs
--rw-r--r--   0     1001      127      182 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/coin_state.rs
--rw-r--r--   0     1001      127      397 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/end_of_sub_slot_bundle.rs
--rw-r--r--   0     1001      127      531 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/fee_estimate.rs
--rw-r--r--   0     1001      127     1983 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/foliage.rs
--rw-r--r--   0     1001      127     3226 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/full_node_protocol.rs
--rw-r--r--   0     1001      127     4342 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/fullblock.rs
--rw-r--r--   0     1001      127     4114 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/header_block.rs
--rw-r--r--   0     1001      127     1406 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/lazy_node.rs
--rw-r--r--   0     1001      127     1380 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/lib.rs
--rw-r--r--   0     1001      127      142 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/peer_info.rs
--rw-r--r--   0     1001      127      195 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/pool_target.rs
--rw-r--r--   0     1001      127    17472 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/program.rs
--rw-r--r--   0     1001      127      319 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/proof_of_space.rs
--rw-r--r--   0     1001      127     1967 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/reward_chain_block.rs
--rw-r--r--   0     1001      127     1458 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/slots.rs
--rw-r--r--   0     1001      127     8260 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/spend_bundle.rs
--rw-r--r--   0     1001      127      449 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/sub_epoch_summary.rs
--rw-r--r--   0     1001      127     2343 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/unfinished_block.rs
--rw-r--r--   0     1001      127     1856 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/unfinished_header_block.rs
--rw-r--r--   0     1001      127      338 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/vdf.rs
--rw-r--r--   0     1001      127     4071 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/wallet_protocol.rs
--rw-r--r--   0     1001      127     2361 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-protocol/src/weight_proof.rs
--rw-r--r--   0     1001      127      454 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik_py_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      127    16368 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik_py_streamable_macro/src/lib.rs
--rw-r--r--   0     1001      127      471 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/Cargo.toml
--rw-r--r--   0     1001      127     2069 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/src/curried_program.rs
--rw-r--r--   0     1001      127     1899 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/src/curry_tree_hash.rs
--rw-r--r--   0     1001      127      806 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/src/lib.rs
--rw-r--r--   0     1001      127     9836 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-utils/src/tree_hash.rs
--rw-r--r--   0     1001      127      625 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/Cargo.toml
--rw-r--r--   0     1001      127      839 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/chik_error.rs
--rw-r--r--   0     1001      127     2346 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/from_json_dict.rs
--rw-r--r--   0     1001      127     2484 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/int.rs
--rw-r--r--   0     1001      127      457 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/lib.rs
--rw-r--r--   0     1001      127    20419 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/streamable.rs
--rw-r--r--   0     1001      127     1892 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-traits/src/to_json_dict.rs
--rw-r--r--   0     1001      127      415 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/Cargo.toml
--rw-r--r--   0     1001      127    10152 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/from_klvm.rs
--rw-r--r--   0     1001      127     2602 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/helpers.rs
--rw-r--r--   0     1001      127      603 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/lib.rs
--rw-r--r--   0     1001      127     1217 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/macros.rs
--rw-r--r--   0     1001      127     7548 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/klvm-derive/src/to_klvm.rs
--rw-r--r--   0     1001      127      516 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      127     9355 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik_streamable_macro/src/lib.rs
--rw-r--r--   0     1001      127      759 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/Cargo.toml
--rw-r--r--   0     1001      127     6089 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/derive_synthetic.rs
--rw-r--r--   0     1001      127      114 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/lib.rs
--rw-r--r--   0     1001      127      710 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/proof.rs
--rw-r--r--   0     1001      127    11363 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/cat.rs
--rw-r--r--   0     1001      127     4507 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/did.rs
--rw-r--r--   0     1001      127    13636 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/nft.rs
--rw-r--r--   0     1001      127     2711 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/offer.rs
--rw-r--r--   0     1001      127     4717 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/singleton.rs
--rw-r--r--   0     1001      127     3082 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles/standard.rs
--rw-r--r--   0     1001      127      427 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-wallet/src/puzzles.rs
--rw-r--r--   0     1001      127     1471 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/Cargo.toml
--rw-r--r--   0     1001      127     4313 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/README.md
--rw-r--r--   0     1001      127     2275 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/benches/merkle-set.rs
--rw-r--r--   0     1001      127     3186 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/benches/run-generator.rs
--rw-r--r--   0     1001      127     2182 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/benches/tree-hash.rs
--rw-r--r--   0     1001      127      266 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/allocator.rs
--rw-r--r--   0     1001      127     4085 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/consensus_constants.rs
--rw-r--r--   0     1001      127     1228 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/error.rs
--rw-r--r--   0     1001      127    17250 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/fast_forward.rs
--rw-r--r--   0     1001      127     3068 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/coin_id.rs
--rw-r--r--   0     1001      127     5714 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/condition_sanitizers.rs
--rw-r--r--   0     1001      127   189253 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/conditions.rs
--rw-r--r--   0     1001      127     1751 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/flags.rs
--rw-r--r--   0     1001      127     6428 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs
--rw-r--r--   0     1001      127     9647 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/messages.rs
--rw-r--r--   0     1001      127      506 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/mod.rs
--rw-r--r--   0     1001      127    11894 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/opcodes.rs
--rw-r--r--   0     1001      127     5299 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/owned_conditions.rs
--rw-r--r--   0     1001      127     6795 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/run_block_generator.rs
--rw-r--r--   0     1001      127     2004 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/run_puzzle.rs
--rw-r--r--   0     1001      127     2944 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/sanitize_int.rs
--rw-r--r--   0     1001      127    10908 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/solution_generator.rs
--rw-r--r--   0     1001      127      471 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/spend_visitor.rs
--rw-r--r--   0     1001      127     9411 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/test_generators.rs
--rw-r--r--   0     1001      127    14899 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/gen/validation_error.rs
--rw-r--r--   0     1001      127     3133 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/generator_rom.rs
--rw-r--r--   0     1001      127      202 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/lib.rs
--rw-r--r--   0     1001      127    17854 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/merkle_set.rs
--rw-r--r--   0     1001      127    32196 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-consensus/src/merkle_tree.rs
--rw-r--r--   0     1001      127     1267 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/Cargo.toml
--rw-r--r--   0     1001      127     2115 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/README.md
--rw-r--r--   0     1001      127     1389 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/benches/derive_key.rs
--rw-r--r--   0     1001      127     1356 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/benches/parse.rs
--rw-r--r--   0     1001      127      828 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/benches/sign.rs
--rw-r--r--   0     1001      127     1023 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/benches/verify.rs
--rw-r--r--   0     1001      127       78 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/derivable_key.rs
--rw-r--r--   0     1001      127     1500 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/derive_keys.rs
--rw-r--r--   0     1001      127     1114 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/error.rs
--rw-r--r--   0     1001      127     4267 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/gtelement.rs
--rw-r--r--   0     1001      127      565 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/lib.rs
--rw-r--r--   0     1001      127     4484 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/mnemonic.rs
--rw-r--r--   0     1001      127    26579 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/public_key.rs
--rw-r--r--   0     1001      127    19133 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/secret_key.rs
--rw-r--r--   0     1001      127    41458 2024-05-15 07:54:39.000000 chik_rs-0.7.0/crates/chik-bls/src/signature.rs
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 chik_rs-0.7.0/wheel/Cargo.toml
--rw-r--r--   0     1001      127       77 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/README.md
--rw-r--r--   0     1001      127    15905 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/generate_type_stubs.py
--rw-r--r--   0     1001      127        0 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/py.typed
--rw-r--r--   0     1001      127       23 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/__init__.py
--rw-r--r--   0     1001      127   154338 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/chik_rs.pyi
--rw-r--r--   0     1001      127        0 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/py.typed
--rw-r--r--   0     1001      127     2708 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/sized_byte_class.py
--rw-r--r--   0     1001      127      385 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/sized_bytes.py
--rw-r--r--   0     1001      127     1629 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/sized_ints.py
--rw-r--r--   0     1001      127     3974 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/python/chik_rs/struct_stream.py
--rw-r--r--   0     1001      127      364 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/adapt_response.rs
--rw-r--r--   0     1001      127    18714 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/api.rs
--rw-r--r--   0     1001      127      158 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/lib.rs
--rw-r--r--   0     1001      127     3832 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/run_generator.rs
--rw-r--r--   0     1001      127     1788 2024-05-15 07:54:39.000000 chik_rs-0.7.0/wheel/src/run_program.rs
--rw-r--r--   0     1001      127    70689 2024-05-15 07:54:39.000000 chik_rs-0.7.0/Cargo.lock
--rw-r--r--   0        0        0     2015 1970-01-01 00:00:00.000000 chik_rs-0.7.0/Cargo.toml
--rw-r--r--   0        0        0      209 1970-01-01 00:00:00.000000 chik_rs-0.7.0/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/py.typed
--rw-r--r--   0     1001      127     3974 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/struct_stream.py
--rw-r--r--   0     1001      127      385 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/sized_bytes.py
--rw-r--r--   0     1001      127       23 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/__init__.py
--rw-r--r--   0     1001      127     1629 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/sized_ints.py
--rw-r--r--   0     1001      127     2708 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/sized_byte_class.py
--rw-r--r--   0     1001      127   154338 2024-05-15 07:54:39.000000 chik_rs-0.7.0/python/chik_rs/chik_rs.pyi
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 chik_rs-0.7.0/PKG-INFO
+-rw-r--r--   0     1001      127     1372 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/Cargo.toml
+-rw-r--r--   0     1001      127     2115 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/README.md
+-rw-r--r--   0     1001      127     2797 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/benches/cache.rs
+-rw-r--r--   0     1001      127     1389 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/benches/derive_key.rs
+-rw-r--r--   0     1001      127     1356 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/benches/parse.rs
+-rw-r--r--   0     1001      127      828 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/benches/sign.rs
+-rw-r--r--   0     1001      127     2016 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/benches/verify.rs
+-rw-r--r--   0     1001      127     8777 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/cached_bls.rs
+-rw-r--r--   0     1001      127       78 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/derivable_key.rs
+-rw-r--r--   0     1001      127     1500 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/derive_keys.rs
+-rw-r--r--   0     1001      127     1114 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/error.rs
+-rw-r--r--   0     1001      127     4619 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/gtelement.rs
+-rw-r--r--   0     1001      127      636 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/lib.rs
+-rw-r--r--   0     1001      127     4484 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/mnemonic.rs
+-rw-r--r--   0     1001      127    26545 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/public_key.rs
+-rw-r--r--   0     1001      127    19147 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/secret_key.rs
+-rw-r--r--   0     1001      127    44458 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-bls/src/signature.rs
+-rw-r--r--   0     1001      127      516 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      127     9371 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik_streamable_macro/src/lib.rs
+-rw-r--r--   0     1001      127      555 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-utils/Cargo.toml
+-rw-r--r--   0     1001      127     2069 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-utils/src/curried_program.rs
+-rw-r--r--   0     1001      127     1909 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-utils/src/curry_tree_hash.rs
+-rw-r--r--   0     1001      127     2624 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-utils/src/hash_encoder.rs
+-rw-r--r--   0     1001      127      849 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-utils/src/lib.rs
+-rw-r--r--   0     1001      127    10970 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-utils/src/tree_hash.rs
+-rw-r--r--   0     1001      127      415 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-derive/Cargo.toml
+-rw-r--r--   0     1001      127    10152 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-derive/src/from_klvm.rs
+-rw-r--r--   0     1001      127     2602 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-derive/src/helpers.rs
+-rw-r--r--   0     1001      127      603 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-derive/src/lib.rs
+-rw-r--r--   0     1001      127     1217 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-derive/src/macros.rs
+-rw-r--r--   0     1001      127     7548 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-derive/src/to_klvm.rs
+-rw-r--r--   0     1001      127     1528 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/Cargo.toml
+-rw-r--r--   0     1001      127     4313 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/README.md
+-rw-r--r--   0     1001      127     2274 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/benches/merkle-set.rs
+-rw-r--r--   0     1001      127     3186 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/benches/run-generator.rs
+-rw-r--r--   0     1001      127     2182 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/benches/tree-hash.rs
+-rw-r--r--   0     1001      127      266 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/allocator.rs
+-rw-r--r--   0     1001      127     4085 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/consensus_constants.rs
+-rw-r--r--   0     1001      127     1370 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/error.rs
+-rw-r--r--   0     1001      127    17402 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/fast_forward.rs
+-rw-r--r--   0     1001      127     3068 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/coin_id.rs
+-rw-r--r--   0     1001      127     5714 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/condition_sanitizers.rs
+-rw-r--r--   0     1001      127   189253 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/conditions.rs
+-rw-r--r--   0     1001      127     1751 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/flags.rs
+-rw-r--r--   0     1001      127     6426 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs
+-rw-r--r--   0     1001      127     9647 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/messages.rs
+-rw-r--r--   0     1001      127      506 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/mod.rs
+-rw-r--r--   0     1001      127    11894 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/opcodes.rs
+-rw-r--r--   0     1001      127     5466 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/owned_conditions.rs
+-rw-r--r--   0     1001      127     6807 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/run_block_generator.rs
+-rw-r--r--   0     1001      127     2004 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/run_puzzle.rs
+-rw-r--r--   0     1001      127     2944 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/sanitize_int.rs
+-rw-r--r--   0     1001      127    10868 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/solution_generator.rs
+-rw-r--r--   0     1001      127      471 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/spend_visitor.rs
+-rw-r--r--   0     1001      127     9411 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/test_generators.rs
+-rw-r--r--   0     1001      127    14899 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/gen/validation_error.rs
+-rw-r--r--   0     1001      127     3133 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/generator_rom.rs
+-rw-r--r--   0     1001      127      202 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/lib.rs
+-rw-r--r--   0     1001      127    17854 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/merkle_set.rs
+-rw-r--r--   0     1001      127    32195 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-consensus/src/merkle_tree.rs
+-rw-r--r--   0     1001      127      454 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik_py_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      127    16368 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik_py_streamable_macro/src/lib.rs
+-rw-r--r--   0     1001      127     1220 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/Cargo.toml
+-rw-r--r--   0     1001      127     7024 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/block_record.rs
+-rw-r--r--   0     1001      127    17592 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/bytes.rs
+-rw-r--r--   0     1001      127     5494 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/chik_protocol.rs
+-rw-r--r--   0     1001      127     1194 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/classgroup.rs
+-rw-r--r--   0     1001      127     4462 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/coin.rs
+-rw-r--r--   0     1001      127      199 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/coin_spend.rs
+-rw-r--r--   0     1001      127      198 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/coin_state.rs
+-rw-r--r--   0     1001      127      397 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/end_of_sub_slot_bundle.rs
+-rw-r--r--   0     1001      127      531 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/fee_estimate.rs
+-rw-r--r--   0     1001      127     1983 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/foliage.rs
+-rw-r--r--   0     1001      127     3492 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/full_node_protocol.rs
+-rw-r--r--   0     1001      127     4342 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/fullblock.rs
+-rw-r--r--   0     1001      127     4114 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/header_block.rs
+-rw-r--r--   0     1001      127     1406 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/lazy_node.rs
+-rw-r--r--   0     1001      127     1423 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/lib.rs
+-rw-r--r--   0     1001      127      142 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/peer_info.rs
+-rw-r--r--   0     1001      127      195 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/pool_target.rs
+-rw-r--r--   0     1001      127    17486 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/program.rs
+-rw-r--r--   0     1001      127      319 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/proof_of_space.rs
+-rw-r--r--   0     1001      127     1967 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/reward_chain_block.rs
+-rw-r--r--   0     1001      127     1458 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/slots.rs
+-rw-r--r--   0     1001      127     8244 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/spend_bundle.rs
+-rw-r--r--   0     1001      127      449 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/sub_epoch_summary.rs
+-rw-r--r--   0     1001      127     2343 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/unfinished_block.rs
+-rw-r--r--   0     1001      127     1856 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/unfinished_header_block.rs
+-rw-r--r--   0     1001      127      338 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/vdf.rs
+-rw-r--r--   0     1001      127     6158 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/wallet_protocol.rs
+-rw-r--r--   0     1001      127     2361 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-protocol/src/weight_proof.rs
+-rw-r--r--   0     1001      127      475 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-traits/Cargo.toml
+-rw-r--r--   0     1001      127      839 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-traits/src/chik_error.rs
+-rw-r--r--   0     1001      127     2346 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-traits/src/from_json_dict.rs
+-rw-r--r--   0     1001      127     2484 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-traits/src/int.rs
+-rw-r--r--   0     1001      127      457 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-traits/src/lib.rs
+-rw-r--r--   0     1001      127    20419 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-traits/src/streamable.rs
+-rw-r--r--   0     1001      127     1892 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-traits/src/to_json_dict.rs
+-rw-r--r--   0     1001      127      809 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/Cargo.toml
+-rw-r--r--   0     1001      127     6975 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/docs/derive_macros.md
+-rw-r--r--   0     1001      127     1067 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/error.rs
+-rw-r--r--   0     1001      127    10932 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/from_klvm.rs
+-rw-r--r--   0     1001      127     1742 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/klvm_decoder.rs
+-rw-r--r--   0     1001      127     1518 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/klvm_encoder.rs
+-rw-r--r--   0     1001      127     5612 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/lib.rs
+-rw-r--r--   0     1001      127     3246 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/macros.rs
+-rw-r--r--   0     1001      127     1026 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/match_byte.rs
+-rw-r--r--   0     1001      127     8909 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/to_klvm.rs
+-rw-r--r--   0     1001      127      670 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/klvm-traits/src/wrappers.rs
+-rw-r--r--   0     1001      127      883 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/Cargo.toml
+-rw-r--r--   0     1001      127     6407 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/derive_synthetic.rs
+-rw-r--r--   0     1001      127      114 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/lib.rs
+-rw-r--r--   0     1001      127      789 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/proof.rs
+-rw-r--r--   0     1001      127    14594 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/cat.rs
+-rw-r--r--   0     1001      127     4690 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/did.rs
+-rw-r--r--   0     1001      127    14167 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/nft.rs
+-rw-r--r--   0     1001      127     4011 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/offer.rs
+-rw-r--r--   0     1001      127     5065 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/singleton.rs
+-rw-r--r--   0     1001      127     3146 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/standard.rs
+-rw-r--r--   0     1001      127      427 2024-05-16 03:29:09.000000 chik_rs-0.8.0/crates/chik-puzzles/src/puzzles.rs
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 chik_rs-0.8.0/wheel/Cargo.toml
+-rw-r--r--   0     1001      127       78 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/README.md
+-rw-r--r--   0     1001      127    16321 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/generate_type_stubs.py
+-rw-r--r--   0     1001      127        0 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/py.typed
+-rw-r--r--   0     1001      127       23 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/python/chik_rs/__init__.py
+-rw-r--r--   0     1001      127   170298 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/python/chik_rs/chik_rs.pyi
+-rw-r--r--   0     1001      127        0 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/python/chik_rs/py.typed
+-rw-r--r--   0     1001      127     2708 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/python/chik_rs/sized_byte_class.py
+-rw-r--r--   0     1001      127      385 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/python/chik_rs/sized_bytes.py
+-rw-r--r--   0     1001      127     1629 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/python/chik_rs/sized_ints.py
+-rw-r--r--   0     1001      127     3974 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/python/chik_rs/struct_stream.py
+-rw-r--r--   0     1001      127      364 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/src/adapt_response.rs
+-rw-r--r--   0     1001      127    19747 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/src/api.rs
+-rw-r--r--   0     1001      127      158 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/src/lib.rs
+-rw-r--r--   0     1001      127     3939 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/src/run_generator.rs
+-rw-r--r--   0     1001      127     1788 2024-05-16 03:29:09.000000 chik_rs-0.8.0/wheel/src/run_program.rs
+-rw-r--r--   0     1001      127    69312 2024-05-16 03:29:09.000000 chik_rs-0.8.0/Cargo.lock
+-rw-r--r--   0        0        0     2020 1970-01-01 00:00:00.000000 chik_rs-0.8.0/Cargo.toml
+-rw-r--r--   0        0        0      209 1970-01-01 00:00:00.000000 chik_rs-0.8.0/pyproject.toml
+-rw-r--r--   0     1001      127   170298 2024-05-16 03:29:09.000000 chik_rs-0.8.0/python/chik_rs/chik_rs.pyi
+-rw-r--r--   0     1001      127     1629 2024-05-16 03:29:09.000000 chik_rs-0.8.0/python/chik_rs/sized_ints.py
+-rw-r--r--   0     1001      127       23 2024-05-16 03:29:09.000000 chik_rs-0.8.0/python/chik_rs/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-16 03:29:09.000000 chik_rs-0.8.0/python/chik_rs/py.typed
+-rw-r--r--   0     1001      127     2708 2024-05-16 03:29:09.000000 chik_rs-0.8.0/python/chik_rs/sized_byte_class.py
+-rw-r--r--   0     1001      127      385 2024-05-16 03:29:09.000000 chik_rs-0.8.0/python/chik_rs/sized_bytes.py
+-rw-r--r--   0     1001      127     3974 2024-05-16 03:29:09.000000 chik_rs-0.8.0/python/chik_rs/struct_stream.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 chik_rs-0.8.0/PKG-INFO
```

### Comparing `chik_rs-0.7.0/crates/klvm-traits/Cargo.toml` & `chik_rs-0.8.0/crates/klvm-traits/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "klvm-traits"
-version = "0.7.0"
+version = "0.8.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Traits for encoding and decoding KLVM objects."
 authors = ["Brandon Haggstrom <b.haggstrom@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
@@ -14,16 +14,16 @@
 [features]
 derive = ["dep:klvm-derive"]
 chik-bls = ["dep:chik-bls"]
 py-bindings = ["dep:pyo3"]
 
 [dependencies]
 pyo3 = { version = ">=0.19.0", optional = true }
-klvmr = "0.6.1"
+klvmr = "0.7.0"
 klvm-derive = { version = "0.6.0", path = "../klvm-derive", optional = true }
-chik-bls = { version = "0.7.0", path = "../chik-bls", optional = true }
+chik-bls = { version = "0.8.0", path = "../chik-bls", optional = true }
 num-bigint = "0.4.3"
 thiserror = "1.0.44"
 
 [dev-dependencies]
 hex = "0.4.3"
 hex-literal = "0.4.1"
```

### Comparing `chik_rs-0.7.0/crates/klvm-traits/docs/derive_macros.md` & `chik_rs-0.8.0/crates/klvm-traits/docs/derive_macros.md`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/error.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/from_klvm.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/from_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/klvm_decoder.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/klvm_decoder.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/klvm_encoder.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/klvm_encoder.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/lib.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/macros.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/macros.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/match_byte.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/match_byte.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/to_klvm.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/to_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-traits/src/wrappers.rs` & `chik_rs-0.8.0/crates/klvm-traits/src/wrappers.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/Cargo.toml` & `chik_rs-0.8.0/crates/chik-protocol/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [package]
 name = "chik-protocol"
-version = "0.7.0"
+version = "0.8.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chik network protocol message types"
 authors = ["Arvid Norberg <arvid@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
 [features]
 py-bindings = ["dep:pyo3", "dep:chik_py_streamable_macro", "chik-traits/py-bindings", "chik-bls/py-bindings"]
+arbitrary = ["dep:arbitrary", "chik-bls/arbitrary"]
 
 [dependencies]
 pyo3 = { version = "0.19.0", features = ["multiple-pymethods", "num-bigint"], optional = true }
 sha2 = "0.10.8"
 hex = "0.4.3"
-chik_streamable_macro = { version = "0.6.0", path = "../chik_streamable_macro" }
+chik_streamable_macro = { version = "0.8.0", path = "../chik_streamable_macro" }
 chik_py_streamable_macro = { version = "0.7.0", path = "../chik_py_streamable_macro", optional = true }
-klvmr = "0.6.1"
-chik-traits = { version = "0.7.0", path = "../chik-traits" }
-klvm-traits = { version = "0.7.0", path = "../klvm-traits", features = ["derive"] }
-klvm-utils = { version = "0.7.0", path = "../klvm-utils" }
-chik-bls = { version = "0.7.0", path = "../chik-bls" }
-arbitrary = { version = "1.3.0", features = ["derive"] }
+klvmr = "0.7.0"
+chik-traits = { version = "0.8.0", path = "../chik-traits" }
+klvm-traits = { version = "0.8.0", path = "../klvm-traits", features = ["derive"] }
+klvm-utils = { version = "0.8.0", path = "../klvm-utils" }
+chik-bls = { version = "0.8.0", path = "../chik-bls" }
+arbitrary = { version = "1.3.0", features = ["derive"], optional = true }
 
 [dev-dependencies]
 rstest = "0.17.0"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/block_record.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/block_record.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/bytes.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/bytes.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use chik_traits::{chik_error, read_bytes, Streamable};
 use klvm_traits::{FromKlvm, FromKlvmError, KlvmDecoder, KlvmEncoder, ToKlvm, ToKlvmError};
+use klvm_utils::TreeHash;
 use sha2::{Digest, Sha256};
 use std::array::TryFromSliceError;
 use std::fmt;
 use std::io::Cursor;
 use std::ops::Deref;
 
 #[cfg(feature = "py-bindings")]
@@ -14,15 +15,15 @@
 use pyo3::exceptions::PyValueError;
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 #[cfg(feature = "py-bindings")]
 use pyo3::types::PyBytes;
 
 #[derive(Default, Clone, PartialEq, Eq, PartialOrd, Ord, Hash)]
-#[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 pub struct Bytes(Vec<u8>);
 
 impl Bytes {
     pub fn new(bytes: Vec<u8>) -> Self {
         Self(bytes)
     }
 
@@ -146,15 +147,15 @@
 
     fn deref(&self) -> &[u8] {
         &self.0
     }
 }
 
 #[derive(Clone, Copy, PartialEq, Eq, PartialOrd, Ord, Hash)]
-#[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 pub struct BytesImpl<const N: usize>([u8; N]);
 
 impl<const N: usize> BytesImpl<N> {
     pub fn new(bytes: [u8; N]) -> Self {
         Self(bytes)
     }
 
@@ -337,14 +338,26 @@
 }
 
 pub type Bytes32 = BytesImpl<32>;
 pub type Bytes48 = BytesImpl<48>;
 pub type Bytes96 = BytesImpl<96>;
 pub type Bytes100 = BytesImpl<100>;
 
+impl From<Bytes32> for TreeHash {
+    fn from(value: Bytes32) -> Self {
+        Self::new(value.0)
+    }
+}
+
+impl From<TreeHash> for Bytes32 {
+    fn from(value: TreeHash) -> Self {
+        Self(value.to_bytes())
+    }
+}
+
 #[cfg(feature = "py-bindings")]
 impl<const N: usize> ToPyObject for BytesImpl<N> {
     fn to_object(&self, py: Python) -> PyObject {
         PyBytes::new(py, &self.0).into()
     }
 }
```

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/chik_protocol.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/chik_protocol.rs`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use crate::Bytes;
 
 #[cfg(feature = "py-bindings")]
 use chik_py_streamable_macro::{PyJsonDict, PyStreamable};
 
 #[repr(u8)]
 #[cfg_attr(feature = "py-bindings", derive(PyJsonDict, PyStreamable))]
-#[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[derive(Streamable, Hash, Debug, Copy, Clone, Eq, PartialEq)]
 pub enum ProtocolMessageTypes {
     // Shared protocol (all services)
     Handshake = 1,
 
     // Harvester protocol (harvester <-> farmer)
     HarvesterHandshake = 3,
@@ -115,14 +115,30 @@
     RequestSesInfo = 76,
     RespondSesInfo = 77,
     RequestBlockHeaders = 86,
     RejectBlockHeaders = 87,
     RespondBlockHeaders = 88,
     RequestFeeEstimates = 89,
     RespondFeeEstimates = 90,
+
+    // Unfinished block protocol
+    NewUnfinishedBlock2 = 92,
+    RequestUnfinishedBlock2 = 93,
+
+    // New wallet sync protocol
+    RequestRemovePuzzleSubscriptions = 94,
+    RespondRemovePuzzleSubscriptions = 95,
+    RequestRemoveCoinSubscriptions = 96,
+    RespondRemoveCoinSubscriptions = 97,
+    RequestPuzzleState = 98,
+    RespondPuzzleState = 99,
+    RejectPuzzleState = 100,
+    RequestCoinState = 101,
+    RespondCoinState = 102,
+    RejectCoinState = 103,
 }
 
 #[cfg(feature = "py-bindings")]
 impl chik_traits::ChikToPython for ProtocolMessageTypes {
     fn to_python<'a>(&self, py: pyo3::Python<'a>) -> pyo3::PyResult<&'a pyo3::PyAny> {
         Ok(pyo3::IntoPy::into_py(*self, py).into_ref(py))
     }
@@ -130,15 +146,15 @@
 
 pub trait ChikProtocolMessage {
     fn msg_type() -> ProtocolMessageTypes;
 }
 
 #[repr(u8)]
 #[cfg_attr(feature = "py-bindings", derive(PyJsonDict, PyStreamable))]
-#[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[derive(Streamable, Hash, Debug, Copy, Clone, Eq, PartialEq)]
 pub enum NodeType {
     FullNode = 1,
     Harvester = 2,
     Farmer = 3,
     Timelord = 4,
     Introducer = 5,
```

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/classgroup.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/classgroup.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/coin.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/coin.rs`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 };
 use sha2::{Digest, Sha256};
 
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
 #[streamable]
+#[derive(Copy)]
 pub struct Coin {
     parent_coin_info: Bytes32,
     puzzle_hash: Bytes32,
     amount: u64,
 }
 
 impl Coin {
```

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/fee_estimate.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/fee_estimate.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/foliage.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/foliage.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/full_node_protocol.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/full_node_protocol.rs`

 * *Files 6% similar despite different names*

```diff
@@ -161,7 +161,19 @@
 #[streamable(message)]
 pub struct RequestPeers {}
 
 #[streamable(message)]
 pub struct RespondPeers {
     peer_list: Vec<TimestampedPeerInfo>,
 }
+
+#[streamable(message)]
+pub struct NewUnfinishedBlock2 {
+    unfinished_reward_hash: Bytes32,
+    foliage_hash: Option<Bytes32>,
+}
+
+#[streamable(message)]
+pub struct RequestUnfinishedBlock2 {
+    unfinished_reward_hash: Bytes32,
+    foliage_hash: Option<Bytes32>,
+}
```

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/fullblock.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/fullblock.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/header_block.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/header_block.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/lazy_node.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/lazy_node.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/lib.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -47,13 +47,14 @@
 pub use crate::program::*;
 pub use crate::proof_of_space::*;
 pub use crate::reward_chain_block::*;
 pub use crate::slots::*;
 pub use crate::spend_bundle::*;
 pub use crate::sub_epoch_summary::*;
 pub use crate::unfinished_block::*;
+pub use crate::unfinished_header_block::*;
 pub use crate::vdf::*;
 pub use crate::wallet_protocol::*;
 pub use crate::weight_proof::*;
 
 #[cfg(feature = "py-bindings")]
 pub use crate::lazy_node::*;
```

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/program.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/program.rs`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     type Target = [u8];
 
     fn deref(&self) -> &[u8] {
         &self.0
     }
 }
 
-#[cfg(fuzzing)]
+#[cfg(feature = "arbitrary")]
 impl<'a> arbitrary::Arbitrary<'a> for Program {
     fn arbitrary(u: &mut arbitrary::Unstructured<'a>) -> arbitrary::Result<Self> {
         // generate an arbitrary KLVM structure. Not likely a valid program.
         let mut items_left = 1;
         let mut total_items = 0;
         let mut buf = Vec::<u8>::with_capacity(200);
```

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/reward_chain_block.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/reward_chain_block.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/slots.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/slots.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/spend_bundle.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/spend_bundle.rs`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     fn py_name(&self) -> Bytes32 {
         self.name()
     }
 
     fn removals(&self) -> Vec<Coin> {
         let mut ret = Vec::<Coin>::with_capacity(self.coin_spends.len());
         for cs in &self.coin_spends {
-            ret.push(cs.coin.clone());
+            ret.push(cs.coin);
         }
         ret
     }
 
     #[pyo3(name = "additions")]
     fn py_additions(&self) -> PyResult<Vec<Coin>> {
         self.additions()
@@ -185,15 +185,15 @@
             hex::decode("3333333333333333333333333333333333333333333333333333333333333333")
                 .unwrap()
                 .try_into()
                 .unwrap(),
             1,
         );
         let spend = CoinSpend::new(
-            test_coin.clone(),
+            test_coin,
             Program::new(vec![1_u8].into()),
             Program::new(solution.into()),
         );
         let bundle = SpendBundle::new(vec![spend], G2Element::default());
         body(test_coin, bundle);
     }
```

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/unfinished_block.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/unfinished_block.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/unfinished_header_block.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/unfinished_header_block.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-protocol/src/weight_proof.rs` & `chik_rs-0.8.0/crates/chik-protocol/src/weight_proof.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik_py_streamable_macro/src/lib.rs` & `chik_rs-0.8.0/crates/chik_py_streamable_macro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-utils/src/curried_program.rs` & `chik_rs-0.8.0/crates/klvm-utils/src/curried_program.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-utils/src/curry_tree_hash.rs` & `chik_rs-0.8.0/crates/klvm-utils/src/curry_tree_hash.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-use crate::{tree_hash_atom, tree_hash_pair};
+use crate::{tree_hash_atom, tree_hash_pair, TreeHash};
 
-pub fn curry_tree_hash(program_hash: [u8; 32], arg_hashes: &[[u8; 32]]) -> [u8; 32] {
+pub fn curry_tree_hash(program_hash: TreeHash, arg_hashes: &[TreeHash]) -> TreeHash {
     let nil = tree_hash_atom(&[]);
     let op_q = tree_hash_atom(&[1]);
     let op_a = tree_hash_atom(&[2]);
     let op_c = tree_hash_atom(&[4]);
 
     let quoted_program = tree_hash_pair(op_q, program_hash);
     let mut quoted_args = tree_hash_atom(&[1]);
```

### Comparing `chik_rs-0.7.0/crates/klvm-utils/src/lib.rs` & `chik_rs-0.8.0/crates/klvm-utils/src/lib.rs`

 * *Files 19% similar despite different names*

```diff
@@ -22,12 +22,14 @@
 //! let hex = hex::encode(node_to_bytes(a, ptr).unwrap());
 //!
 //! // (a (q . 1) (c (q . 42) (c (q . 75) 1)))
 //! assert_eq!(hex, "ff02ffff0101ffff04ffff012affff04ffff014bff01808080");
 
 mod curried_program;
 mod curry_tree_hash;
+mod hash_encoder;
 mod tree_hash;
 
 pub use curried_program::*;
 pub use curry_tree_hash::*;
+pub use hash_encoder::*;
 pub use tree_hash::*;
```

### Comparing `chik_rs-0.7.0/crates/klvm-utils/src/tree_hash.rs` & `chik_rs-0.8.0/crates/klvm-utils/src/tree_hash.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,91 @@
 use klvmr::allocator::{Allocator, NodePtr, SExp};
 use klvmr::serde::node_from_bytes_backrefs_record;
 use klvmr::sha2::{Digest, Sha256};
 use std::collections::{HashMap, HashSet};
-use std::io;
+use std::ops::Deref;
+use std::{fmt, io};
+
+#[derive(Clone, Copy, PartialEq, Eq, PartialOrd, Ord, Hash)]
+pub struct TreeHash([u8; 32]);
+
+impl TreeHash {
+    pub const fn new(hash: [u8; 32]) -> Self {
+        Self(hash)
+    }
+
+    pub const fn to_bytes(&self) -> [u8; 32] {
+        self.0
+    }
+
+    pub fn to_vec(&self) -> Vec<u8> {
+        self.0.to_vec()
+    }
+}
+
+impl fmt::Debug for TreeHash {
+    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+        write!(f, "TreeHash({})", self)
+    }
+}
+
+impl fmt::Display for TreeHash {
+    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
+        write!(f, "{}", hex::encode(self.0))
+    }
+}
+
+impl From<[u8; 32]> for TreeHash {
+    fn from(hash: [u8; 32]) -> Self {
+        Self::new(hash)
+    }
+}
+
+impl From<TreeHash> for [u8; 32] {
+    fn from(hash: TreeHash) -> [u8; 32] {
+        hash.0
+    }
+}
+
+impl AsRef<[u8]> for TreeHash {
+    fn as_ref(&self) -> &[u8] {
+        &self.0
+    }
+}
+
+impl Deref for TreeHash {
+    type Target = [u8];
+
+    fn deref(&self) -> &Self::Target {
+        &self.0
+    }
+}
 
 enum TreeOp {
     SExp(NodePtr),
     Cons,
     ConsAddCache(NodePtr),
 }
 
-pub fn tree_hash_atom(bytes: &[u8]) -> [u8; 32] {
+pub fn tree_hash_atom(bytes: &[u8]) -> TreeHash {
     let mut sha256 = Sha256::new();
     sha256.update([1]);
     sha256.update(bytes);
-    sha256.finalize().into()
+    TreeHash::new(sha256.finalize().into())
 }
 
-pub fn tree_hash_pair(first: [u8; 32], rest: [u8; 32]) -> [u8; 32] {
+pub fn tree_hash_pair(first: TreeHash, rest: TreeHash) -> TreeHash {
     let mut sha256 = Sha256::new();
     sha256.update([2]);
     sha256.update(first);
     sha256.update(rest);
-    sha256.finalize().into()
+    TreeHash::new(sha256.finalize().into())
 }
 
-pub fn tree_hash(a: &Allocator, node: NodePtr) -> [u8; 32] {
+pub fn tree_hash(a: &Allocator, node: NodePtr) -> TreeHash {
     let mut hashes = Vec::new();
     let mut ops = vec![TreeOp::SExp(node)];
 
     while let Some(op) = ops.pop() {
         match op {
             TreeOp::SExp(node) => match a.sexp(node) {
                 SExp::Atom => {
@@ -54,16 +110,16 @@
     hashes[0]
 }
 
 pub fn tree_hash_cached(
     a: &Allocator,
     node: NodePtr,
     backrefs: &HashSet<NodePtr>,
-    cache: &mut HashMap<NodePtr, [u8; 32]>,
-) -> [u8; 32] {
+    cache: &mut HashMap<NodePtr, TreeHash>,
+) -> TreeHash {
     let mut hashes = Vec::new();
     let mut ops = vec![TreeOp::SExp(node)];
 
     while let Some(op) = ops.pop() {
         match op {
             TreeOp::SExp(node) => match a.sexp(node) {
                 SExp::Atom => {
@@ -102,18 +158,18 @@
         }
     }
 
     assert!(hashes.len() == 1);
     hashes[0]
 }
 
-pub fn tree_hash_from_bytes(buf: &[u8]) -> io::Result<[u8; 32]> {
+pub fn tree_hash_from_bytes(buf: &[u8]) -> io::Result<TreeHash> {
     let mut a = Allocator::new();
     let (node, backrefs) = node_from_bytes_backrefs_record(&mut a, buf)?;
-    let mut cache = HashMap::<NodePtr, [u8; 32]>::new();
+    let mut cache = HashMap::<NodePtr, TreeHash>::new();
     Ok(tree_hash_cached(&a, node, &backrefs, &mut cache))
 }
 
 #[test]
 fn test_tree_hash() {
     let mut a = Allocator::new();
     let atom1 = a.new_atom(&[1, 2, 3]).unwrap();
@@ -123,38 +179,38 @@
     // test atom1 hash
     let atom1_hash = {
         let mut sha256 = Sha256::new();
         sha256.update([1_u8]);
         sha256.update([1, 2, 3]);
         let atom1_hash = sha256.finalize();
 
-        assert_eq!(tree_hash(&a, atom1), atom1_hash.as_slice());
+        assert_eq!(tree_hash(&a, atom1).as_ref(), atom1_hash.as_slice());
         atom1_hash
     };
 
     // test atom2 hash
     let atom2_hash = {
         let mut sha256 = Sha256::new();
         sha256.update([1_u8]);
         sha256.update([4, 5, 6]);
         let atom2_hash = sha256.finalize();
 
-        assert_eq!(tree_hash(&a, atom2), atom2_hash.as_slice());
+        assert_eq!(tree_hash(&a, atom2).as_ref(), atom2_hash.as_slice());
         atom2_hash
     };
 
     // test tree hash
     let root_hash = {
         let mut sha256 = Sha256::new();
         sha256.update([2_u8]);
         sha256.update(atom1_hash.as_slice());
         sha256.update(atom2_hash.as_slice());
         let root_hash = sha256.finalize();
 
-        assert_eq!(tree_hash(&a, root), root_hash.as_slice());
+        assert_eq!(tree_hash(&a, root).as_ref(), root_hash.as_slice());
         root_hash
     };
 
     let atom3 = a.new_atom(&[7, 8, 9]).unwrap();
     let root2 = a.new_pair(root, atom3).unwrap();
 
     let atom3_hash = {
@@ -167,15 +223,15 @@
     // test deeper tree hash
     {
         let mut sha256 = Sha256::new();
         sha256.update([2_u8]);
         sha256.update(root_hash.as_slice());
         sha256.update(atom3_hash.as_slice());
 
-        assert_eq!(tree_hash(&a, root2), sha256.finalize().as_slice());
+        assert_eq!(tree_hash(&a, root2).as_ref(), sha256.finalize().as_slice());
     }
 }
 
 #[test]
 fn test_tree_hash_from_bytes() {
     use klvmr::serde::{node_to_bytes, node_to_bytes_backrefs};
 
@@ -285,39 +341,39 @@
         let node = node_from_bytes_backrefs(&mut a, &generator).expect("node_from_bytes_backrefs");
         node_to_bytes_backrefs(&a, node).expect("node_to_bytes_backrefs")
     } else {
         generator
     };
 
     let mut a = Allocator::new();
-    let mut cache = HashMap::<NodePtr, [u8; 32]>::new();
+    let mut cache = HashMap::<NodePtr, TreeHash>::new();
     let (node, backrefs) = node_from_bytes_backrefs_record(&mut a, &generator)
         .expect("node_from_bytes_backrefs_records");
 
     let hash1 = tree_hash(&a, node);
     let hash2 = tree_hash_cached(&a, node, &backrefs, &mut cache);
     // for (key, value) in cache.iter() {
     //     println!("  {key:?}: {}", hex::encode(value));
     // }
     assert_eq!(hash1, hash2);
-    assert_eq!(hash1, hex::decode(expect).unwrap().as_slice());
+    assert_eq!(hash1.as_ref(), hex::decode(expect).unwrap().as_slice());
     assert!(!compressed || !backrefs.is_empty());
 }
 
 #[cfg(test)]
 fn test_sha256_atom(buf: &[u8]) {
     let hash = tree_hash_atom(buf);
 
     let mut hasher = Sha256::new();
     hasher.update([1_u8]);
     if !buf.is_empty() {
         hasher.update(buf);
     }
 
-    assert_eq!(hash, hasher.finalize().as_slice());
+    assert_eq!(hash.as_ref(), hasher.finalize().as_slice());
 }
 
 #[test]
 fn test_tree_hash_atom() {
     test_sha256_atom(&[]);
     for val in 0..255 {
         test_sha256_atom(&[val]);
```

### Comparing `chik_rs-0.7.0/crates/chik-traits/src/chik_error.rs` & `chik_rs-0.8.0/crates/chik-traits/src/chik_error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-traits/src/from_json_dict.rs` & `chik_rs-0.8.0/crates/chik-traits/src/from_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-traits/src/int.rs` & `chik_rs-0.8.0/crates/chik-traits/src/int.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-traits/src/streamable.rs` & `chik_rs-0.8.0/crates/chik-traits/src/streamable.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-traits/src/to_json_dict.rs` & `chik_rs-0.8.0/crates/chik-traits/src/to_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-derive/src/from_klvm.rs` & `chik_rs-0.8.0/crates/klvm-derive/src/from_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-derive/src/helpers.rs` & `chik_rs-0.8.0/crates/klvm-derive/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-derive/src/lib.rs` & `chik_rs-0.8.0/crates/klvm-derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-derive/src/macros.rs` & `chik_rs-0.8.0/crates/klvm-derive/src/macros.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/klvm-derive/src/to_klvm.rs` & `chik_rs-0.8.0/crates/klvm-derive/src/to_klvm.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik_streamable_macro/Cargo.toml` & `chik_rs-0.8.0/crates/chik_streamable_macro/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chik_streamable_macro"
-version = "0.6.0"
+version = "0.8.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Streamable derive macro for serializing/deserializing types in Chik protocol format"
 authors = ["Arvid Norberg <arvid@libtorrent.org>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
```

### Comparing `chik_rs-0.7.0/crates/chik_streamable_macro/src/lib.rs` & `chik_rs-0.8.0/crates/chik_streamable_macro/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -89,28 +89,28 @@
         panic!("only structs are supported");
     }
 
     let main_derives = quote! {
         #[derive(chik_streamable_macro::Streamable, Hash, Debug, Clone, Eq, PartialEq)]
     };
 
-    // If you're calling the macro from `chik-protocol`, enable Python bindings and fuzzing conditionally.
+    // If you're calling the macro from `chik-protocol`, enable Python bindings and arbitrary conditionally.
     // Otherwise, you're calling it from an external crate which doesn't have this infrastructure setup.
     // In that case, the caller can add these macros manually if they want to.
     let attrs = if matches!(found_crate, FoundCrate::Itself) {
         quote! {
             #[cfg_attr(
                 feature = "py-bindings", pyo3::pyclass(frozen), derive(
                     chik_py_streamable_macro::PyJsonDict,
                     chik_py_streamable_macro::PyStreamable,
                     chik_py_streamable_macro::PyGetters
                 )
             )]
             #main_derives
-            #[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+            #[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
         }
     } else {
         main_derives
     };
 
     quote! {
         #attrs
```

### Comparing `chik_rs-0.7.0/crates/chik-wallet/Cargo.toml` & `chik_rs-0.8.0/crates/chik-puzzles/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [package]
-name = "chik-wallet"
-version = "0.7.0"
+name = "chik-puzzles"
+version = "0.8.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chik primitives needed for building wallets."
 authors = ["Brandon Haggstrom <b.haggstrom@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
+[features]
+arbitrary = ["dep:arbitrary", "chik-protocol/arbitrary"]
+
 [dependencies]
-klvmr = "0.6.1"
+klvmr = "0.7.0"
 sha2 = "0.10.8"
 num-bigint = "0.4.3"
 hex-literal = "0.4.1"
-klvm-utils = { version = "0.7.0", path = "../klvm-utils" }
-klvm-traits = { version = "0.7.0", path = "../klvm-traits", features = ["chik-bls"] }
-chik-bls = { version = "0.7.0", path = "../chik-bls" }
-chik-protocol = { version = "0.7.0", path = "../chik-protocol" }
-arbitrary = "1.3.0"
+klvm-utils = { version = "0.8.0", path = "../klvm-utils" }
+klvm-traits = { version = "0.8.0", path = "../klvm-traits", features = ["chik-bls"] }
+chik-bls = { version = "0.8.0", path = "../chik-bls" }
+chik-protocol = { version = "0.8.0", path = "../chik-protocol" }
+arbitrary = { version = "1.3.0", features = ["derive"], optional = true }
 
 [dev-dependencies]
 hex = "0.4.3"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chik_rs-0.7.0/crates/chik-wallet/src/derive_synthetic.rs` & `chik_rs-0.8.0/crates/chik-puzzles/src/derive_synthetic.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 use chik_bls::{PublicKey, SecretKey};
 use hex_literal::hex;
 use num_bigint::BigInt;
 use sha2::{digest::FixedOutput, Digest, Sha256};
 
+use crate::standard::DEFAULT_HIDDEN_PUZZLE_HASH;
+
 const GROUP_ORDER_BYTES: [u8; 32] =
     hex!("73eda753299d7d483339d80809a1d80553bda402fffe5bfeffffffff00000001");
 
 pub trait DeriveSynthetic {
-    fn derive_synthetic(&self, hidden_puzzle_hash: &[u8; 32]) -> Self;
+    /// Derive a synthetic key that includes a custom hidden puzzle hash.
+    fn derive_synthetic_hidden(&self, hidden_puzzle_hash: &[u8; 32]) -> Self;
+
+    /// Derive a synthetic key that includes [`DEFAULT_HIDDEN_PUZZLE_HASH`].
+    /// The default hidden puzzle is `(=)`.
+    fn derive_synthetic(&self) -> Self
+    where
+        Self: Sized,
+    {
+        self.derive_synthetic_hidden(&DEFAULT_HIDDEN_PUZZLE_HASH.to_bytes())
+    }
 }
 
 impl DeriveSynthetic for PublicKey {
-    fn derive_synthetic(&self, hidden_puzzle_hash: &[u8; 32]) -> Self {
+    fn derive_synthetic_hidden(&self, hidden_puzzle_hash: &[u8; 32]) -> Self {
         self + &synthetic_offset(self, hidden_puzzle_hash).public_key()
     }
 }
 
 impl DeriveSynthetic for SecretKey {
-    fn derive_synthetic(&self, hidden_puzzle_hash: &[u8; 32]) -> Self {
+    fn derive_synthetic_hidden(&self, hidden_puzzle_hash: &[u8; 32]) -> Self {
         self + &synthetic_offset(&self.public_key(), hidden_puzzle_hash)
     }
 }
 
 pub fn mod_by_group_order(bytes: [u8; 32]) -> [u8; 32] {
     let value = BigInt::from_signed_bytes_be(bytes.as_slice());
     let group_order = BigInt::from_signed_bytes_be(&GROUP_ORDER_BYTES);
@@ -40,16 +52,14 @@
     hasher.update(hidden_puzzle_hash);
     let bytes: [u8; 32] = hasher.finalize_fixed().into();
     SecretKey::from_bytes(&mod_by_group_order(bytes)).unwrap()
 }
 
 #[cfg(test)]
 mod tests {
-    use crate::standard::DEFAULT_HIDDEN_PUZZLE_HASH;
-
     use super::*;
 
     use chik_bls::{derive_keys::master_to_wallet_unhardened_intermediate, DerivableKey};
     use hex::ToHex;
     use hex_literal::hex;
 
     #[test]
@@ -79,15 +89,15 @@
         .unwrap();
         let pk = sk.public_key();
         let intermediate = master_to_wallet_unhardened_intermediate(&pk);
 
         for (index, hex) in hex_keys.iter().enumerate() {
             let key = intermediate
                 .derive_unhardened(index as u32)
-                .derive_synthetic(&DEFAULT_HIDDEN_PUZZLE_HASH);
+                .derive_synthetic();
             assert_eq!(key.to_bytes().encode_hex::<String>(), *hex);
         }
     }
 
     #[test]
     fn test_synthetic_secret_keys() {
         let hex_keys = [
@@ -114,12 +124,12 @@
         ))
         .unwrap();
         let intermediate = master_to_wallet_unhardened_intermediate(&sk);
 
         for (index, hex) in hex_keys.iter().enumerate() {
             let key = intermediate
                 .derive_unhardened(index as u32)
-                .derive_synthetic(&DEFAULT_HIDDEN_PUZZLE_HASH);
+                .derive_synthetic();
             assert_eq!(key.to_bytes().encode_hex::<String>(), *hex);
         }
     }
 }
```

### Comparing `chik_rs-0.7.0/crates/chik-wallet/src/proof.rs` & `chik_rs-0.8.0/crates/chik-puzzles/src/proof.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 use chik_protocol::Bytes32;
 use klvm_traits::{FromKlvm, ToKlvm};
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
-#[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(untagged, tuple)]
 pub enum Proof {
     Lineage(LineageProof),
     Eve(EveProof),
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
-#[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(list)]
 pub struct LineageProof {
-    pub parent_coin_info: Bytes32,
-    pub inner_puzzle_hash: Bytes32,
-    pub amount: u64,
+    pub parent_parent_coin_id: Bytes32,
+    pub parent_inner_puzzle_hash: Bytes32,
+    pub parent_amount: u64,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
-#[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(list)]
 pub struct EveProof {
     pub parent_coin_info: Bytes32,
     pub amount: u64,
 }
```

### Comparing `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/did.rs` & `chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/did.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 use chik_protocol::Bytes32;
 use hex_literal::hex;
 use klvm_traits::{
     klvm_list, match_list, match_tuple, FromKlvm, FromKlvmError, KlvmDecoder, KlvmEncoder, Raw,
     ToKlvm, ToKlvmError,
 };
+use klvm_utils::TreeHash;
 
 use crate::singleton::SingletonStruct;
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(curry)]
 pub struct DidArgs<I, M> {
     pub inner_puzzle: I,
     pub recovery_did_list_hash: Bytes32,
     pub num_verifications_required: u64,
     pub singleton_struct: SingletonStruct,
     pub metadata: M,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 pub enum DidSolution<I> {
     InnerSpend(I),
 }
 
 impl<N, I> FromKlvm<N> for DidSolution<I>
 where
     I: FromKlvm<N>,
@@ -86,19 +89,19 @@
     808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff7effff04ff
     02ffff04ff09ff80808080ffff02ff7effff04ff02ffff04ff0dff8080808080
     ffff01ff0bffff0101ff058080ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [DID1 standard](https://chiklisp.com/dids) puzzle.
-pub const DID_INNER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const DID_INNER_PUZZLE_HASH: TreeHash = TreeHash::new(hex!(
     "
     33143d2bef64f14036742673afd158126b94284b4530a28c354fac202b0c910e
     "
-);
+));
 
 #[cfg(test)]
 mod tests {
     use klvmr::Allocator;
 
     use super::*;
```

### Comparing `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/nft.rs` & `chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/nft.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 use chik_protocol::Bytes32;
 use hex_literal::hex;
 use klvm_traits::{FromKlvm, FromKlvmError, KlvmDecoder, KlvmEncoder, Raw, ToKlvm, ToKlvmError};
+use klvm_utils::TreeHash;
 
 use crate::singleton::SingletonStruct;
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(curry)]
 pub struct NftIntermediateLauncherArgs {
     pub launcher_puzzle_hash: Bytes32,
     pub mint_number: usize,
     pub mint_total: usize,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(curry)]
 pub struct NftStateLayerArgs<I, M> {
     pub mod_hash: Bytes32,
     pub metadata: M,
     pub metadata_updater_puzzle_hash: Bytes32,
     pub inner_puzzle: I,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(list)]
 pub struct NftStateLayerSolution<I> {
     pub inner_solution: I,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(curry)]
 pub struct NftOwnershipLayerArgs<I, P> {
     pub mod_hash: Bytes32,
     pub current_owner: Option<Bytes32>,
     pub transfer_program: P,
     pub inner_puzzle: I,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(list)]
 pub struct NftOwnershipLayerSolution<I> {
     pub inner_solution: I,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(curry)]
 pub struct NftRoyaltyTransferPuzzleArgs {
     pub singleton_struct: SingletonStruct,
     pub royalty_puzzle_hash: Bytes32,
     pub trade_price_percentage: u16,
 }
 
 #[derive(Debug, Clone, PartialEq, Eq)]
-#[cfg_attr(fuzzing, derive(arbitrary::Arbitrary))]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 pub struct NftMetadata {
     pub edition_number: u64,
     pub edition_total: u64,
     pub data_uris: Vec<String>,
     pub data_hash: Option<Bytes32>,
     pub metadata_uris: Vec<String>,
     pub metadata_hash: Option<Bytes32>,
@@ -135,15 +142,15 @@
         ]);
 
         items.to_klvm(encoder)
     }
 }
 
 /// This is the puzzle reveal of the [NFT1 state layer](https://chiklisp.com/nfts) puzzle.
-pub static NFT_STATE_LAYER_PUZZLE: [u8; 827] = hex!(
+pub const NFT_STATE_LAYER_PUZZLE: [u8; 827] = hex!(
     "
     ff02ffff01ff02ff3effff04ff02ffff04ff05ffff04ffff02ff2fff5f80ffff
     04ff80ffff04ffff04ffff04ff0bffff04ff17ff808080ffff01ff808080ffff
     01ff8080808080808080ffff04ffff01ffffff0233ff04ff0101ffff02ff02ff
     ff03ff05ffff01ff02ff1affff04ff02ffff04ff0dffff04ffff0bff12ffff0b
     ff2cff1480ffff0bff12ffff0bff12ffff0bff2cff3c80ff0980ffff0bff12ff
     0bffff0bff2cff8080808080ff8080808080ffff010b80ff0180ffff0bff12ff
@@ -167,22 +174,22 @@
     02ff16ffff04ff02ffff04ff05ffff04ff27ffff04ffff0bff2cff82014f80ff
     ff04ffff02ff2effff04ff02ffff04ff818fff80808080ffff04ffff0bff2cff
     0580ff8080808080808080ff378080ff81af8080ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [NFT1 state layer](https://chiklisp.com/nfts) puzzle.
-pub static NFT_STATE_LAYER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const NFT_STATE_LAYER_PUZZLE_HASH: TreeHash = TreeHash::new(hex!(
     "
     a04d9f57764f54a43e4030befb4d80026e870519aaa66334aef8304f5d0393c2
     "
-);
+));
 
 /// This is the puzzle reveal of the [NFT1 ownership layer](https://chiklisp.com/nfts) puzzle.
-pub static NFT_OWNERSHIP_LAYER_PUZZLE: [u8; 1226] = hex!(
+pub const NFT_OWNERSHIP_LAYER_PUZZLE: [u8; 1226] = hex!(
     "
     ff02ffff01ff02ff26ffff04ff02ffff04ff05ffff04ff17ffff04ff0bffff04
     ffff02ff2fff5f80ff80808080808080ffff04ffff01ffffff82ad4cff0233ff
     ff3e04ff81f601ffffff0102ffff02ffff03ff05ffff01ff02ff2affff04ff02
     ffff04ff0dffff04ffff0bff32ffff0bff3cff3480ffff0bff32ffff0bff32ff
     ff0bff3cff2280ff0980ffff0bff32ff0bffff0bff3cff8080808080ff808080
     8080ffff010b80ff0180ff04ffff04ff38ffff04ffff02ff36ffff04ff02ffff
@@ -219,22 +226,22 @@
     04ff0bffff04ff81bfffff04ffff02ffff03ff82017fffff0182017fffff01ff
     02ff0bffff04ff17ffff04ff2fffff01ff808080808080ff0180ff8080808080
     808080ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [NFT1 ownership layer](https://chiklisp.com/nfts) puzzle.
-pub static NFT_OWNERSHIP_LAYER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const NFT_OWNERSHIP_LAYER_PUZZLE_HASH: TreeHash = TreeHash::new(hex!(
     "
     c5abea79afaa001b5427dfa0c8cf42ca6f38f5841b78f9b3c252733eb2de2726
     "
-);
+));
 
 /// This is the puzzle reveal of the [NFT1 royalty transfer](https://chiklisp.com/nfts) puzzle.
-pub static NFT_ROYALTY_TRANSFER_PUZZLE: [u8; 687] = hex!(
+pub const NFT_ROYALTY_TRANSFER_PUZZLE: [u8; 687] = hex!(
     "
     ff02ffff01ff02ffff03ff81bfffff01ff04ff82013fffff04ff80ffff04ffff
     02ffff03ffff22ff82013fffff20ffff09ff82013fff2f808080ffff01ff04ff
     ff04ff10ffff04ffff0bffff02ff2effff04ff02ffff04ff09ffff04ff8205bf
     ffff04ffff02ff3effff04ff02ffff04ffff04ff09ffff04ff82013fff1d8080
     ff80808080ff808080808080ff1580ff808080ffff02ff16ffff04ff02ffff04
     ff0bffff04ff17ffff04ff8202bfffff04ff15ff8080808080808080ffff01ff
@@ -254,56 +261,56 @@
     ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff3effff04ff02ffff04ff
     09ff80808080ffff02ff3effff04ff02ffff04ff0dff8080808080ffff01ff0b
     ffff0101ff058080ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [NFT1 royalty transfer](https://chiklisp.com/nfts) puzzle.
-pub static NFT_ROYALTY_TRANSFER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const NFT_ROYALTY_TRANSFER_PUZZLE_HASH: TreeHash = TreeHash::new(hex!(
     "
     025dee0fb1e9fa110302a7e9bfb6e381ca09618e2778b0184fa5c6b275cfce1f
     "
-);
+));
 
 /// This is the puzzle reveal of the [NFT1 metadata updater](https://chiklisp.com/nfts) puzzle.
-pub static NFT_METADATA_UPDATER_PUZZLE: [u8; 241] = hex!(
+pub const NFT_METADATA_UPDATER_PUZZLE: [u8; 241] = hex!(
     "
     ff02ffff01ff04ffff04ffff02ffff03ffff22ff27ff3780ffff01ff02ffff03
     ffff21ffff09ff27ffff01826d7580ffff09ff27ffff01826c7580ffff09ff27
     ffff01758080ffff01ff02ff02ffff04ff02ffff04ff05ffff04ff27ffff04ff
     37ff808080808080ffff010580ff0180ffff010580ff0180ffff04ff0bff8080
     80ffff01ff808080ffff04ffff01ff02ffff03ff05ffff01ff02ffff03ffff09
     ff11ff0b80ffff01ff04ffff04ff0bffff04ff17ff198080ff0d80ffff01ff04
     ff09ffff02ff02ffff04ff02ffff04ff0dffff04ff0bffff04ff17ff80808080
     80808080ff0180ff8080ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [NFT1 metadata updater](https://chiklisp.com/nfts) puzzle.
-pub static NFT_METADATA_UPDATER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const NFT_METADATA_UPDATER_PUZZLE_HASH: TreeHash = TreeHash::new(hex!(
     "
     fe8a4b4e27a2e29a4d3fc7ce9d527adbcaccbab6ada3903ccf3ba9a769d2d78b
     "
-);
+));
 
 /// This is the puzzle reveal of the [NFT1 intermediate launcher](https://chiklisp.com/nfts) puzzle.
-pub static NFT_INTERMEDIATE_LAUNCHER_PUZZLE: [u8; 65] = hex!(
+pub const NFT_INTERMEDIATE_LAUNCHER_PUZZLE: [u8; 65] = hex!(
     "
     ff02ffff01ff04ffff04ff04ffff04ff05ffff01ff01808080ffff04ffff04ff
     06ffff04ffff0bff0bff1780ff808080ff808080ffff04ffff01ff333cff0180
     80
     "
 );
 
 /// This is the puzzle hash of the [NFT1 intermediate launcher](https://chiklisp.com/nfts) puzzle.
-pub static NFT_INTERMEDIATE_LAUNCHER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const NFT_INTERMEDIATE_LAUNCHER_PUZZLE_HASH: TreeHash = TreeHash::new(hex!(
     "
     7a32d2d9571d3436791c0ad3d7fcfdb9c43ace2b0f0ff13f98d29f0cc093f445
     "
-);
+));
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     use crate::assert_puzzle_hash;
```

### Comparing `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/offer.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/generator_rom.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,42 @@
 use hex_literal::hex;
 
-/// This is the puzzle reveal of the [offer settlement payments](https://chiklisp.com/offers) puzzle.
-pub static SETTLEMENT_PAYMENTS_PUZZLE: [u8; 293] = hex!(
-    "
-    ff02ffff01ff02ff0affff04ff02ffff04ff03ff80808080ffff04ffff01ffff
-    333effff02ffff03ff05ffff01ff04ffff04ff0cffff04ffff02ff1effff04ff
-    02ffff04ff09ff80808080ff808080ffff02ff16ffff04ff02ffff04ff19ffff
-    04ffff02ff0affff04ff02ffff04ff0dff80808080ff808080808080ff8080ff
-    0180ffff02ffff03ff05ffff01ff02ffff03ffff15ff29ff8080ffff01ff04ff
-    ff04ff08ff0980ffff02ff16ffff04ff02ffff04ff0dffff04ff0bff80808080
-    8080ffff01ff088080ff0180ffff010b80ff0180ff02ffff03ffff07ff0580ff
-    ff01ff0bffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff
-    1effff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff01
-    80ff018080
-    "
-);
-
-/// This is the puzzle hash of the [offer settlement payments](https://chiklisp.com/offers) puzzle.
-pub static SETTLEMENT_PAYMENTS_PUZZLE_HASH: [u8; 32] = hex!(
-    "
-    cfbfdeed5c4ca2de3d0bf520b9cb4bb7743a359bd2e6a188d19ce7dffc21d3e7
-    "
-);
-
-/// This is the puzzle reveal of the old [offer settlement payments](https://chiklisp.com/offers) puzzle.
-///
-/// **Warning:**
-/// It is recommended not to use settlement payments v1 for anything other than backwards compatibility (e.g. offer compression).
-pub static SETTLEMENT_PAYMENTS_PUZZLE_V1: [u8; 267] = hex!(
-    "
-    ff02ffff01ff02ff0affff04ff02ffff04ff03ff80808080ffff04ffff01ffff
-    333effff02ffff03ff05ffff01ff04ffff04ff0cffff04ffff02ff1effff04ff
-    02ffff04ff09ff80808080ff808080ffff02ff16ffff04ff02ffff04ff19ffff
-    04ffff02ff0affff04ff02ffff04ff0dff80808080ff808080808080ff8080ff
-    0180ffff02ffff03ff05ffff01ff04ffff04ff08ff0980ffff02ff16ffff04ff
-    02ffff04ff0dffff04ff0bff808080808080ffff010b80ff0180ff02ffff03ff
-    ff07ff0580ffff01ff0bffff0102ffff02ff1effff04ff02ffff04ff09ff8080
-    8080ffff02ff1effff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101
-    ff058080ff0180ff018080
-    "
+// the generator ROM from:
+// https://github.com/Chik-Network/chik-blockchain/blob/main/chik/wallet/puzzles/rom_bootstrap_generator.clsp.hex
+pub const GENERATOR_ROM: [u8; 737] = hex!(
+    "
+    ff02ffff01ff02ff0cffff04ff02ffff04ffff02ff05ffff04ff08ffff04ff13
+    ff80808080ff80808080ffff04ffff01ffffff02ffff01ff05ffff02ff3effff
+    04ff02ffff04ff05ff8080808080ffff04ffff01ffffff81ff7fff81df81bfff
+    ffff02ffff03ffff09ff0bffff01818080ffff01ff04ff80ffff04ff05ff8080
+    80ffff01ff02ffff03ffff0aff0bff1880ffff01ff02ff1affff04ff02ffff04
+    ffff02ffff03ffff0aff0bff1c80ffff01ff02ffff03ffff0aff0bff1480ffff
+    01ff0880ffff01ff04ffff0effff18ffff011fff0b80ffff0cff05ff80ffff01
+    018080ffff04ffff0cff05ffff010180ff80808080ff0180ffff01ff04ffff18
+    ffff013fff0b80ffff04ff05ff80808080ff0180ff80808080ffff01ff04ff0b
+    ffff04ff05ff80808080ff018080ff0180ff04ffff0cff15ff80ff0980ffff04
+    ffff0cff15ff0980ff808080ffff04ffff04ff05ff1380ffff04ff2bff808080
+    ffff02ff16ffff04ff02ffff04ff09ffff04ffff02ff3effff04ff02ffff04ff
+    15ff80808080ff8080808080ff02ffff03ffff09ffff0cff05ff80ffff010180
+    ff1080ffff01ff02ff2effff04ff02ffff04ffff02ff3effff04ff02ffff04ff
+    ff0cff05ffff010180ff80808080ff80808080ffff01ff02ff12ffff04ff02ff
+    ff04ffff0cff05ffff010180ffff04ffff0cff05ff80ffff010180ff80808080
+    8080ff0180ff018080ff04ffff02ff16ffff04ff02ffff04ff09ff80808080ff
+    0d80ffff04ff09ffff04ffff02ff1effff04ff02ffff04ff15ff80808080ffff
+    04ff2dffff04ffff02ff15ff5d80ff7d80808080ffff02ffff03ff05ffff01ff
+    04ffff02ff0affff04ff02ffff04ff09ff80808080ffff02ff16ffff04ff02ff
+    ff04ff0dff8080808080ff8080ff0180ff02ffff03ffff07ff0580ffff01ff0b
+    ffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff1effff04
+    ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff0180
+    80"
 );
 
-/// This is the puzzle hash of the old [offer settlement payments](https://chiklisp.com/offers) puzzle.
-///
-/// **Warning:**
-/// It is recommended not to use settlement payments v1 for anything other than backwards compatibility (e.g. offer compression).
-pub static SETTLEMENT_PAYMENTS_PUZZLE_HASH_V1: [u8; 32] = hex!(
-    "
-    bae24162efbd568f89bc7a340798a6118df0189eb9e3f8697bcea27af99f8f79
-    "
+// the KLVM deserializer from:
+// https://github.com/Chik-Network/chik-blockchain/blob/main/chik/wallet/puzzles/chiklisp_deserialisation.clsp.hex
+pub const KLVM_DESERIALIZER: [u8; 471] = hex!(
+"
+ff02ffff01ff05ffff02ff3effff04ff02ffff04ff05ff8080808080ffff04ffff01ffffff81ff7fff81df81bfffffff02ffff03ffff09ff0bffff01818080ffff01ff04ff80ffff04ff05ff808080ffff01ff02ffff03ffff0aff0bff1880ffff01ff02ff1affff04ff02ffff04ffff02ffff03ffff0aff0bff1c80ffff01ff02ffff03ffff0aff0bff1480ffff01ff0880ffff01ff04ffff0effff18ffff011fff0b80ffff0cff05ff80ffff01018080ffff04ffff0cff05ffff010180ff80808080ff0180ffff01ff04ffff18ffff013fff0b80ffff04ff05ff80808080ff0180ff80808080ffff01ff04ff0bffff04ff05ff80808080ff018080ff0180ff04ffff0cff15ff80ff0980ffff04ffff0cff15ff0980ff808080ffff04ffff04ff05ff1380ffff04ff2bff808080ffff02ff16ffff04ff02ffff04ff09ffff04ffff02ff3effff04ff02ffff04ff15ff80808080ff8080808080ff02ffff03ffff09ffff0cff05ff80ffff010180ff1080ffff01ff02ff2effff04ff02ffff04ffff02ff3effff04ff02ffff04ffff0cff05ffff010180ff80808080ff80808080ffff01ff02ff12ffff04ff02ffff04ffff0cff05ffff010180ffff04ffff0cff05ff80ffff010180ff808080808080ff0180ff018080"
 );
 
-#[cfg(test)]
-mod tests {
-    use super::*;
-
-    use crate::assert_puzzle_hash;
-
-    #[test]
-    fn puzzle_hashes() {
-        assert_puzzle_hash!(SETTLEMENT_PAYMENTS_PUZZLE => SETTLEMENT_PAYMENTS_PUZZLE_HASH);
-        assert_puzzle_hash!(SETTLEMENT_PAYMENTS_PUZZLE_V1 => SETTLEMENT_PAYMENTS_PUZZLE_HASH_V1);
-    }
-}
+// constant from the main chik blockchain:
+// https://github.com/Chik-Network/chik-blockchain/blob/main/chik/consensus/default_constants.py
+pub const COST_PER_BYTE: u64 = 12000;
```

### Comparing `chik_rs-0.7.0/crates/chik-wallet/src/puzzles/singleton.rs` & `chik_rs-0.8.0/crates/chik-puzzles/src/puzzles/singleton.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 use chik_protocol::Bytes32;
 use hex_literal::hex;
 use klvm_traits::{FromKlvm, ToKlvm};
+use klvm_utils::TreeHash;
 
 use crate::Proof;
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(curry)]
 pub struct SingletonArgs<I> {
     pub singleton_struct: SingletonStruct,
     pub inner_puzzle: I,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(tuple)]
 pub struct SingletonStruct {
     pub mod_hash: Bytes32,
     pub launcher_id: Bytes32,
     pub launcher_puzzle_hash: Bytes32,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(list)]
 pub struct SingletonSolution<I> {
-    pub proof: Proof,
+    pub lineage_proof: Proof,
     pub amount: u64,
     pub inner_solution: I,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, ToKlvm, FromKlvm)]
+#[cfg_attr(feature = "arbitrary", derive(arbitrary::Arbitrary))]
 #[klvm(list)]
 pub struct LauncherSolution<T> {
     pub singleton_puzzle_hash: Bytes32,
     pub amount: u64,
     pub key_value_list: T,
 }
 
@@ -54,19 +59,19 @@
     ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff0effff04ff02ffff04ff
     09ff80808080ffff02ff0effff04ff02ffff04ff0dff8080808080ffff01ff0b
     ffff0101ff058080ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [singleton launcher](https://chiklisp.com/singletons#launcher) puzzle.
-pub const SINGLETON_LAUNCHER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const SINGLETON_LAUNCHER_PUZZLE_HASH: TreeHash = TreeHash::new(hex!(
     "
     eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9
     "
-);
+));
 
 /// This is the puzzle reveal of the [singleton](https://chiklisp.com/singletons) puzzle.
 pub const SINGLETON_TOP_LAYER_PUZZLE: [u8; 967] = hex!(
     "
     ff02ffff01ff02ffff03ffff18ff2fff3480ffff01ff04ffff04ff20ffff04ff
     2fff808080ffff04ffff02ff3effff04ff02ffff04ff05ffff04ffff02ff2aff
     ff04ff02ffff04ff27ffff04ffff02ffff03ff77ffff01ff02ff36ffff04ff02
@@ -98,19 +103,19 @@
     ff8080808080ffff01ff0bffff0101ff058080ff0180ff02ffff03ffff21ff17
     ffff09ff0bff158080ffff01ff04ff30ffff04ff0bff808080ffff01ff088080
     ff0180ff018080
     "
 );
 
 /// This is the puzzle hash of the [singleton](https://chiklisp.com/singletons) puzzle.
-pub const SINGLETON_TOP_LAYER_PUZZLE_HASH: [u8; 32] = hex!(
+pub const SINGLETON_TOP_LAYER_PUZZLE_HASH: TreeHash = TreeHash::new(hex!(
     "
     7faa3253bfddd1e0decb0906b2dc6247bbc4cf608f58345d173adb63e8b47c9f
     "
-);
+));
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     use crate::assert_puzzle_hash;
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/Cargo.toml` & `chik_rs-0.8.0/crates/chik-consensus/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [package]
 name = "chik-consensus"
-version = "0.7.0"
+version = "0.8.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "Utility functions and types used by the Chik blockchain full node"
 authors = ["Richard Kiss <him@richardkiss.com>", "Arvid Norberg <arvid@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
 [features]
 py-bindings = ["dep:pyo3", "dep:chik_py_streamable_macro"]
 
 [dependencies]
-klvmr = "0.6.1"
+klvmr = "0.7.0"
 hex = "0.4.3"
 pyo3 = { version = ">=0.19.0", optional = true }
 sha2 = "0.10.8"
-chik_streamable_macro = { version = "0.6.0", path = "../chik_streamable_macro" }
+chik_streamable_macro = { version = "0.8.0", path = "../chik_streamable_macro" }
 chik_py_streamable_macro = { version = "0.7.0", path = "../chik_py_streamable_macro", optional = true }
-klvm-utils = { version = "0.7.0", path = "../klvm-utils" }
-chik-traits = { version = "0.7.0", path = "../chik-traits" }
-klvm-traits = { version = "0.7.0", path = "../klvm-traits" }
+klvm-utils = { version = "0.8.0", path = "../klvm-utils" }
+chik-traits = { version = "0.8.0", path = "../chik-traits" }
+klvm-traits = { version = "0.8.0", path = "../klvm-traits" }
 klvm-derive = { version = "0.6.0", path = "../klvm-derive" }
-chik-protocol = { version = "0.7.0", path = "../chik-protocol" }
-chik-wallet = { version = "0.7.0", path = "../chik-wallet" }
+chik-protocol = { version = "0.8.0", path = "../chik-protocol" }
+chik-puzzles = { version = "0.8.0", path = "../chik-puzzles" }
+chik-bls = { version = "0.8.0", path = "../chik-bls" }
 hex-literal = "0.4.1"
 thiserror = "1.0.44"
 
 [dev-dependencies]
 num-traits = "0.2.15"
 rstest = "0.16.0"
 text-diff = "0.4.0"
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/README.md` & `chik_rs-0.8.0/crates/chik-consensus/README.md`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/benches/merkle-set.rs` & `chik_rs-0.8.0/crates/chik-consensus/benches/merkle-set.rs`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     let root = &tree.get_root();
     use std::iter::zip;
     group.bench_function("validate_merkle_proof", |b| {
         b.iter(|| {
             let start = Instant::now();
             for (p, leaf) in zip(&proofs, &leafs) {
                 let _ =
-                    black_box(validate_merkle_proof(&p, leaf, root).expect("expect valid proof"));
+                    black_box(validate_merkle_proof(p, leaf, root).expect("expect valid proof"));
             }
             start.elapsed()
         })
     });
 }
 
 criterion_group!(merkle_set, run);
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/benches/run-generator.rs` & `chik_rs-0.8.0/crates/chik-consensus/benches/run-generator.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/benches/tree-hash.rs` & `chik_rs-0.8.0/crates/chik-consensus/benches/tree-hash.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/consensus_constants.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/consensus_constants.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/error.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/error.rs`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
     #[error("Eval {0}")]
     Eval(#[from] EvalErr),
 
     #[error("Validation {0}")]
     Validation(#[from] ValidationErr),
 
+    #[error("BLS {0}")]
+    Bls(#[from] chik_bls::Error),
+
     #[error("not a singleton mod hash")]
     NotSingletonModHash,
 
     #[error("inner puzzle hash mismatch")]
     InnerPuzzleHashMismatch,
 
     #[error("puzzle hash mismatch")]
@@ -37,14 +40,17 @@
 
     #[error("parent coin mismatch")]
     ParentCoinMismatch,
 
     #[error("coin mismatch")]
     CoinMismatch,
 
+    #[error("expected lineage proof, found eve proof")]
+    ExpectedLineageProof,
+
     #[error("{0}")]
     Custom(String),
 }
 
 #[cfg(feature = "py-bindings")]
 impl std::convert::From<Error> for PyErr {
     fn from(err: Error) -> PyErr {
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/fast_forward.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/fast_forward.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,26 @@
 use crate::error::{Error, Result};
 use chik_protocol::Bytes32;
 use chik_protocol::Coin;
-use chik_wallet::singleton::SINGLETON_TOP_LAYER_PUZZLE_HASH;
+use chik_puzzles::singleton::{
+    SingletonArgs, SingletonSolution, SingletonStruct, SINGLETON_TOP_LAYER_PUZZLE_HASH,
+};
+use chik_puzzles::Proof;
 use klvm_traits::{FromKlvm, ToKlvm};
 use klvm_utils::CurriedProgram;
+use klvm_utils::TreeHash;
 use klvm_utils::{tree_hash, tree_hash_atom, tree_hash_pair};
 use klvmr::allocator::{Allocator, NodePtr};
 
-#[derive(FromKlvm, ToKlvm, Debug)]
-#[klvm(tuple)]
-pub struct SingletonStruct {
-    pub mod_hash: Bytes32,
-    pub launcher_id: Bytes32,
-    pub launcher_puzzle_hash: Bytes32,
-}
-
-#[derive(FromKlvm, ToKlvm, Debug)]
-#[klvm(curry)]
-pub struct SingletonArgs<I> {
-    pub singleton_struct: SingletonStruct,
-    pub inner_puzzle: I,
-}
-
-#[derive(FromKlvm, ToKlvm, Debug)]
-#[klvm(list)]
-pub struct LineageProof {
-    pub parent_parent_coin_id: Bytes32,
-    pub parent_inner_puzzle_hash: Bytes32,
-    pub parent_amount: u64,
-}
-
-#[derive(FromKlvm, ToKlvm, Debug)]
-#[klvm(list)]
-pub struct SingletonSolution<I> {
-    pub lineage_proof: LineageProof,
-    pub amount: u64,
-    pub inner_solution: I,
-}
-
 // TODO: replace this with a generic function to compute the hash of curried
 // puzzles
 const OP_QUOTE: u8 = 1;
 const OP_APPLY: u8 = 2;
 const OP_CONS: u8 = 4;
-fn curry_single_arg(arg_hash: [u8; 32], rest: [u8; 32]) -> [u8; 32] {
+fn curry_single_arg(arg_hash: TreeHash, rest: TreeHash) -> TreeHash {
     tree_hash_pair(
         tree_hash_atom(&[OP_CONS]),
         tree_hash_pair(
             tree_hash_pair(tree_hash_atom(&[OP_QUOTE]), arg_hash),
             tree_hash_pair(rest, tree_hash_atom(&[])),
         ),
     )
@@ -59,23 +32,23 @@
         tree_hash_pair(
             tree_hash_atom(&singleton_struct.launcher_id),
             tree_hash_atom(&singleton_struct.launcher_puzzle_hash),
         ),
     );
 
     let args_hash = tree_hash_atom(&[OP_QUOTE]);
-    let args_hash = curry_single_arg(inner_puzzle_hash.into(), args_hash);
+    let args_hash = curry_single_arg((*inner_puzzle_hash).into(), args_hash);
     let args_hash = curry_single_arg(singleton_struct_hash, args_hash);
 
     tree_hash_pair(
         tree_hash_atom(&[OP_APPLY]),
         tree_hash_pair(
             tree_hash_pair(
                 tree_hash_atom(&[OP_QUOTE]),
-                (&singleton_struct.mod_hash).into(),
+                singleton_struct.mod_hash.into(),
             ),
             tree_hash_pair(args_hash, tree_hash_atom(&[])),
         ),
     )
     .into()
 }
 
@@ -103,17 +76,24 @@
     if coin.puzzle_hash != new_parent.puzzle_hash || coin.puzzle_hash != new_coin.puzzle_hash {
         return Err(Error::PuzzleHashMismatch);
     }
 
     let singleton = CurriedProgram::<NodePtr, SingletonArgs<NodePtr>>::from_klvm(a, puzzle)?;
     let mut new_solution = SingletonSolution::<NodePtr>::from_klvm(a, solution)?;
 
+    let lineage_proof = match &mut new_solution.lineage_proof {
+        Proof::Lineage(proof) => proof,
+        _ => return Err(Error::ExpectedLineageProof),
+    };
+
     // this is the tree hash of the singleton top layer puzzle
     // the tree hash of singleton_top_layer_v1_1.clsp
-    if singleton.args.singleton_struct.mod_hash.as_ref() != SINGLETON_TOP_LAYER_PUZZLE_HASH {
+    if singleton.args.singleton_struct.mod_hash.as_ref()
+        != SINGLETON_TOP_LAYER_PUZZLE_HASH.to_bytes()
+    {
         return Err(Error::NotSingletonModHash);
     }
 
     // also make sure the actual mod-hash of this puzzle matches the
     // singleton_top_layer_v1_1.clsp
     let mod_hash = tree_hash(a, singleton.program);
     if mod_hash != SINGLETON_TOP_LAYER_PUZZLE_HASH {
@@ -125,47 +105,47 @@
     if coin.amount != new_solution.amount {
         return Err(Error::CoinAmountMismatch);
     }
 
     // given the parent's parent, the parent's inner puzzle and parent's amount,
     // we can compute the hash of the curried inner puzzle for our parent coin
     let parent_puzzle_hash = curry_and_treehash(
-        &new_solution.lineage_proof.parent_inner_puzzle_hash,
+        &lineage_proof.parent_inner_puzzle_hash,
         &singleton.args.singleton_struct,
     );
 
     // now that we know the parent coin's puzzle hash, we have all the pieces to
     // compute the coin being spent (before the fast-forward).
     let parent_coin = Coin {
-        parent_coin_info: new_solution.lineage_proof.parent_parent_coin_id,
+        parent_coin_info: lineage_proof.parent_parent_coin_id,
         puzzle_hash: parent_puzzle_hash,
-        amount: new_solution.lineage_proof.parent_amount,
+        amount: lineage_proof.parent_amount,
     };
 
     if parent_coin.coin_id() != coin.parent_coin_info {
         return Err(Error::ParentCoinMismatch);
     }
 
     let inner_puzzle_hash = tree_hash(a, singleton.args.inner_puzzle);
-    if inner_puzzle_hash != *new_solution.lineage_proof.parent_inner_puzzle_hash {
+    if inner_puzzle_hash != lineage_proof.parent_inner_puzzle_hash.into() {
         return Err(Error::InnerPuzzleHashMismatch);
     }
 
     let puzzle_hash = tree_hash(a, puzzle);
 
-    if puzzle_hash != *new_parent.puzzle_hash || puzzle_hash != *coin.puzzle_hash {
+    if puzzle_hash != new_parent.puzzle_hash.into() || puzzle_hash != coin.puzzle_hash.into() {
         // we can only fast-forward if the puzzle hash match the new coin
         // the spend is assumed to be valied already, so we don't check it
         // against the original coin being spent
         return Err(Error::PuzzleHashMismatch);
     }
 
     // update the solution to use the new parent coin's information
-    new_solution.lineage_proof.parent_parent_coin_id = new_parent.parent_coin_info;
-    new_solution.lineage_proof.parent_amount = new_parent.amount;
+    lineage_proof.parent_parent_coin_id = new_parent.parent_coin_info;
+    lineage_proof.parent_amount = new_parent.amount;
     new_solution.amount = new_coin.amount;
 
     let expected_new_parent = new_parent.coin_id();
 
     if new_coin.parent_coin_info != expected_new_parent {
         return Err(Error::CoinMismatch);
     }
@@ -358,15 +338,17 @@
             },
             Error::CoinAmountMismatch,
         );
     }
 
     fn parse_solution(a: &mut Allocator, solution: &[u8]) -> SingletonSolution<NodePtr> {
         let new_solution = node_from_bytes(a, solution).expect("parse solution");
-        SingletonSolution::from_klvm(a, new_solution).expect("parse solution")
+        let solution = SingletonSolution::from_klvm(a, new_solution).expect("parse solution");
+        assert!(matches!(solution.lineage_proof, Proof::Lineage(_)));
+        solution
     }
 
     fn serialize_solution(a: &mut Allocator, solution: &SingletonSolution<NodePtr>) -> Vec<u8> {
         let new_solution = solution.to_klvm(a).expect("to_klvm");
         node_to_bytes(a, new_solution).expect("serialize solution")
     }
 
@@ -388,16 +370,20 @@
 
     #[test]
     fn test_invalid_lineage_proof_parent() {
         run_ff_test(
             |a, _coin, _new_coin, _new_parent, _puzzle, solution| {
                 let mut new_solution = parse_solution(a, solution);
 
+                let Proof::Lineage(lineage_proof) = &mut new_solution.lineage_proof else {
+                    unreachable!();
+                };
+
                 // corrupt the lineage proof
-                new_solution.lineage_proof.parent_parent_coin_id = Bytes32::from(hex!(
+                lineage_proof.parent_parent_coin_id = Bytes32::from(hex!(
                     "fefefefefefefefefefefefefefefefefefefefefefefefefefefefefefefefe"
                 ));
 
                 *solution = serialize_solution(a, &new_solution);
             },
             Error::ParentCoinMismatch,
         );
@@ -405,31 +391,39 @@
 
     #[test]
     fn test_invalid_lineage_proof_parent_amount() {
         run_ff_test(
             |a, _coin, _new_coin, _new_parent, _puzzle, solution| {
                 let mut new_solution = parse_solution(a, solution);
 
+                let Proof::Lineage(lineage_proof) = &mut new_solution.lineage_proof else {
+                    unreachable!();
+                };
+
                 // corrupt the lineage proof
-                new_solution.lineage_proof.parent_amount = 11;
+                lineage_proof.parent_amount = 11;
 
                 *solution = serialize_solution(a, &new_solution);
             },
             Error::ParentCoinMismatch,
         );
     }
 
     #[test]
     fn test_invalid_lineage_proof_parent_inner_ph() {
         run_ff_test(
             |a, _coin, _new_coin, _new_parent, _puzzle, solution| {
                 let mut new_solution = parse_solution(a, solution);
 
+                let Proof::Lineage(lineage_proof) = &mut new_solution.lineage_proof else {
+                    unreachable!();
+                };
+
                 // corrupt the lineage proof
-                new_solution.lineage_proof.parent_inner_puzzle_hash = Bytes32::from(hex!(
+                lineage_proof.parent_inner_puzzle_hash = Bytes32::from(hex!(
                     "fefefefefefefefefefefefefefefefefefefefefefefefefefefefefefefefe"
                 ));
 
                 *solution = serialize_solution(a, &new_solution);
             },
             Error::ParentCoinMismatch,
         );
@@ -438,33 +432,37 @@
     #[test]
     fn test_invalid_lineage_proof_parent_inner_ph_with_coin() {
         run_ff_test(
             |a, coin, new_coin, new_parent, puzzle, solution| {
                 let mut new_solution = parse_solution(a, solution);
                 let singleton = parse_singleton(a, puzzle);
 
+                let Proof::Lineage(lineage_proof) = &mut new_solution.lineage_proof else {
+                    unreachable!();
+                };
+
                 // corrupt the lineage proof
-                new_solution.lineage_proof.parent_inner_puzzle_hash = Bytes32::from(hex!(
+                lineage_proof.parent_inner_puzzle_hash = Bytes32::from(hex!(
                     "fefefefefefefefefefefefefefefefefefefefefefefefefefefefefefefefe"
                 ));
 
                 // adjust the coins puzzle hashes to match
                 let parent_puzzle_hash = curry_and_treehash(
-                    &new_solution.lineage_proof.parent_inner_puzzle_hash,
+                    &lineage_proof.parent_inner_puzzle_hash,
                     &singleton.args.singleton_struct,
                 );
 
-                *solution = serialize_solution(a, &new_solution);
-
                 *new_parent = Coin {
-                    parent_coin_info: new_solution.lineage_proof.parent_parent_coin_id,
+                    parent_coin_info: lineage_proof.parent_parent_coin_id,
                     puzzle_hash: parent_puzzle_hash,
-                    amount: new_solution.lineage_proof.parent_amount,
+                    amount: lineage_proof.parent_amount,
                 };
 
+                *solution = serialize_solution(a, &new_solution);
+
                 new_coin.puzzle_hash = parent_puzzle_hash;
 
                 coin.parent_coin_info = new_parent.coin_id();
                 coin.puzzle_hash = parent_puzzle_hash;
             },
             Error::InnerPuzzleHashMismatch,
         );
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/coin_id.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/coin_id.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/condition_sanitizers.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/condition_sanitizers.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/conditions.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/conditions.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/flags.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/flags.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/get_puzzle_and_solution.rs`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         // we want to avoid having to compute the puzzle hash if we don't have to
         // so check parent and amount first
         if parent.as_ref() != find_parent.as_ref() || amount != find_amount {
             continue;
         }
 
         let puzzle_hash = tree_hash(a, puzzle);
-        if puzzle_hash != find_ph.as_ref() {
+        if puzzle_hash != find_ph.into() {
             continue;
         }
 
         // we found the coin!
         return Ok((puzzle, solution));
     }
     Err(ValidationErr(generator_result, ErrorCode::InvalidCondition))
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/messages.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/messages.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/opcodes.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/opcodes.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/owned_conditions.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/owned_conditions.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-use chik_protocol::{Bytes, Bytes32, Bytes48};
+use crate::error::Result;
+use chik_bls::PublicKey;
+use chik_protocol::{Bytes, Bytes32};
 use chik_streamable_macro::Streamable;
 use klvmr::{Allocator, NodePtr};
 
 use super::conditions::{Spend, SpendBundleConditions};
 
 #[cfg(feature = "py-bindings")]
 use chik_py_streamable_macro::{PyJsonDict, PyStreamable};
@@ -21,21 +23,21 @@
     pub height_relative: Option<u32>,
     pub seconds_relative: Option<u64>,
     pub before_height_relative: Option<u32>,
     pub before_seconds_relative: Option<u64>,
     pub birth_height: Option<u32>,
     pub birth_seconds: Option<u64>,
     pub create_coin: Vec<(Bytes32, u64, Option<Bytes>)>,
-    pub agg_sig_me: Vec<(Bytes48, Bytes)>,
-    pub agg_sig_parent: Vec<(Bytes48, Bytes)>,
-    pub agg_sig_puzzle: Vec<(Bytes48, Bytes)>,
-    pub agg_sig_amount: Vec<(Bytes48, Bytes)>,
-    pub agg_sig_puzzle_amount: Vec<(Bytes48, Bytes)>,
-    pub agg_sig_parent_amount: Vec<(Bytes48, Bytes)>,
-    pub agg_sig_parent_puzzle: Vec<(Bytes48, Bytes)>,
+    pub agg_sig_me: Vec<(PublicKey, Bytes)>,
+    pub agg_sig_parent: Vec<(PublicKey, Bytes)>,
+    pub agg_sig_puzzle: Vec<(PublicKey, Bytes)>,
+    pub agg_sig_amount: Vec<(PublicKey, Bytes)>,
+    pub agg_sig_puzzle_amount: Vec<(PublicKey, Bytes)>,
+    pub agg_sig_parent_amount: Vec<(PublicKey, Bytes)>,
+    pub agg_sig_parent_puzzle: Vec<(PublicKey, Bytes)>,
     pub flags: u32,
 }
 
 #[derive(Streamable, Hash, Debug, Clone, Eq, PartialEq)]
 #[cfg_attr(
     feature = "py-bindings",
     pyo3::pyclass(name = "SpendBundleConditions", get_all, frozen),
@@ -49,95 +51,98 @@
     pub seconds_absolute: u64,
     // when set, this is the lowest (i.e. most restrictive) of all
     // ASSERT_BEFORE_HEIGHT_ABSOLUTE conditions
     pub before_height_absolute: Option<u32>,
     // ASSERT_BEFORE_SECONDS_ABSOLUTE conditions
     pub before_seconds_absolute: Option<u64>,
     // Unsafe Agg Sig conditions (i.e. not tied to the spend generating it)
-    pub agg_sig_unsafe: Vec<(Bytes48, Bytes)>,
+    pub agg_sig_unsafe: Vec<(PublicKey, Bytes)>,
     pub cost: u64,
     // the sum of all values of all spent coins
     pub removal_amount: u128,
     // the sum of all amounts of CREATE_COIN conditions
     pub addition_amount: u128,
 }
 
 impl OwnedSpend {
-    pub fn from(a: &Allocator, spend: Spend) -> Self {
+    pub fn from(a: &Allocator, spend: Spend) -> Result<Self> {
         let mut create_coin =
             Vec::<(Bytes32, u64, Option<Bytes>)>::with_capacity(spend.create_coin.len());
         for c in spend.create_coin {
             create_coin.push((
                 c.puzzle_hash,
                 c.amount,
                 if c.hint != a.nil() {
                     Some(a.atom(c.hint).as_ref().into())
                 } else {
                     None
                 },
             ));
         }
 
-        Self {
+        Ok(Self {
             coin_id: *spend.coin_id,
             parent_id: a.atom(spend.parent_id).as_ref().try_into().unwrap(),
             puzzle_hash: a.atom(spend.puzzle_hash).as_ref().try_into().unwrap(),
             coin_amount: spend.coin_amount,
             height_relative: spend.height_relative,
             seconds_relative: spend.seconds_relative,
             before_height_relative: spend.before_height_relative,
             before_seconds_relative: spend.before_seconds_relative,
             birth_height: spend.birth_height,
             birth_seconds: spend.birth_seconds,
             create_coin,
-            agg_sig_me: convert_agg_sigs(a, &spend.agg_sig_me),
-            agg_sig_parent: convert_agg_sigs(a, &spend.agg_sig_parent),
-            agg_sig_puzzle: convert_agg_sigs(a, &spend.agg_sig_puzzle),
-            agg_sig_amount: convert_agg_sigs(a, &spend.agg_sig_amount),
-            agg_sig_puzzle_amount: convert_agg_sigs(a, &spend.agg_sig_puzzle_amount),
-            agg_sig_parent_amount: convert_agg_sigs(a, &spend.agg_sig_parent_amount),
-            agg_sig_parent_puzzle: convert_agg_sigs(a, &spend.agg_sig_parent_puzzle),
+            agg_sig_me: convert_agg_sigs(a, &spend.agg_sig_me)?,
+            agg_sig_parent: convert_agg_sigs(a, &spend.agg_sig_parent)?,
+            agg_sig_puzzle: convert_agg_sigs(a, &spend.agg_sig_puzzle)?,
+            agg_sig_amount: convert_agg_sigs(a, &spend.agg_sig_amount)?,
+            agg_sig_puzzle_amount: convert_agg_sigs(a, &spend.agg_sig_puzzle_amount)?,
+            agg_sig_parent_amount: convert_agg_sigs(a, &spend.agg_sig_parent_amount)?,
+            agg_sig_parent_puzzle: convert_agg_sigs(a, &spend.agg_sig_parent_puzzle)?,
             flags: spend.flags,
-        }
+        })
     }
 }
 
 impl OwnedSpendBundleConditions {
-    pub fn from(a: &Allocator, sb: SpendBundleConditions) -> Self {
+    pub fn from(a: &Allocator, sb: SpendBundleConditions) -> Result<Self> {
         let mut spends = Vec::<OwnedSpend>::new();
         for s in sb.spends {
-            spends.push(OwnedSpend::from(a, s));
+            spends.push(OwnedSpend::from(a, s)?);
         }
 
-        let mut agg_sigs = Vec::<(Bytes48, Bytes)>::with_capacity(sb.agg_sig_unsafe.len());
+        let mut agg_sigs = Vec::<(PublicKey, Bytes)>::with_capacity(sb.agg_sig_unsafe.len());
         for (pk, msg) in sb.agg_sig_unsafe {
             agg_sigs.push((
-                a.atom(pk).as_ref().try_into().unwrap(),
+                PublicKey::from_bytes(a.atom(pk).as_ref().try_into().unwrap())?,
                 a.atom(msg).as_ref().into(),
             ));
         }
 
-        Self {
+        Ok(Self {
             spends,
             reserve_fee: sb.reserve_fee,
             height_absolute: sb.height_absolute,
             seconds_absolute: sb.seconds_absolute,
             before_height_absolute: sb.before_height_absolute,
             before_seconds_absolute: sb.before_seconds_absolute,
             agg_sig_unsafe: agg_sigs,
             cost: sb.cost,
             removal_amount: sb.removal_amount,
             addition_amount: sb.addition_amount,
-        }
+        })
     }
 }
 
-fn convert_agg_sigs(a: &Allocator, agg_sigs: &[(NodePtr, NodePtr)]) -> Vec<(Bytes48, Bytes)> {
-    let mut ret = Vec::<(Bytes48, Bytes)>::new();
+fn convert_agg_sigs(
+    a: &Allocator,
+    agg_sigs: &[(NodePtr, NodePtr)],
+) -> Result<Vec<(PublicKey, Bytes)>> {
+    let mut ret = Vec::<(PublicKey, Bytes)>::new();
     for (pk, msg) in agg_sigs {
         ret.push((
-            a.atom(*pk).as_ref().try_into().unwrap(),
+            PublicKey::from_bytes(a.atom(*pk).as_ref().try_into().unwrap())?,
             a.atom(*msg).as_ref().into(),
         ));
     }
-    ret
+    Ok(ret)
 }
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/run_block_generator.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/run_block_generator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use crate::gen::conditions::{
     parse_spends, process_single_spend, validate_conditions, ParseState, SpendBundleConditions,
 };
 use crate::gen::flags::ALLOW_BACKREFS;
 use crate::gen::spend_visitor::SpendVisitor;
 use crate::gen::validation_error::{first, ErrorCode, ValidationErr};
 use crate::generator_rom::{COST_PER_BYTE, GENERATOR_ROM, KLVM_DESERIALIZER};
-use klvm_utils::tree_hash_cached;
+use klvm_utils::{tree_hash_cached, TreeHash};
 use klvmr::allocator::{Allocator, NodePtr};
 use klvmr::chik_dialect::ChikDialect;
 use klvmr::cost::Cost;
 use klvmr::reduction::Reduction;
 use klvmr::run_program::run_program;
 use klvmr::serde::{node_from_bytes, node_from_bytes_backrefs, node_from_bytes_backrefs_record};
 use std::collections::{HashMap, HashSet};
@@ -151,15 +151,15 @@
 
     // at this point all_spends is a list of:
     // (parent-coin-id puzzle-reveal amount solution . extra)
     // where extra may be nil, or additional extension data
 
     let mut ret = SpendBundleConditions::default();
     let mut state = ParseState::default();
-    let mut cache = HashMap::<NodePtr, [u8; 32]>::new();
+    let mut cache = HashMap::<NodePtr, TreeHash>::new();
 
     while let Some((spend, rest)) = a.next(all_spends) {
         all_spends = rest;
         // process the spend
         let [parent_id, puzzle, amount, solution, _spend_level_extra] =
             extract_n::<5>(a, spend, ErrorCode::InvalidCondition)?;
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/run_puzzle.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/run_puzzle.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/sanitize_int.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/sanitize_int.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/solution_generator.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/solution_generator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,16 @@
         let coin2: Coin = Coin::new(
             hex!("ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000").into(),
             hex!("d23da14695a188ae5708dd152263c4db883eb27edeb936178d4d988b8f3ce5fc").into(),
             18375000000000000000,
         );
 
         let result = solution_generator([
-            (coin1.clone(), PUZZLE1.as_ref(), SOLUTION1.as_ref()),
-            (coin2.clone(), PUZZLE2.as_ref(), SOLUTION2.as_ref()),
+            (coin1, PUZZLE1.as_ref(), SOLUTION1.as_ref()),
+            (coin2, PUZZLE2.as_ref(), SOLUTION2.as_ref()),
         ])
         .expect("solution_generator");
 
         assert_eq!(
             result,
             hex!(
                 "
@@ -190,15 +190,15 @@
             808080"
             )
         );
 
         let generator_output = run_generator(&result);
         assert_eq!(generator_output, EXPECTED_GENERATOR_OUTPUT);
 
-        let result = solution_generator([(coin2.clone(), PUZZLE2.as_ref(), SOLUTION2.as_ref())])
+        let result = solution_generator([(coin2, PUZZLE2.as_ref(), SOLUTION2.as_ref())])
             .expect("solution_generator");
 
         assert_eq!(
             result,
             hex!(
                 "
             ff01ffffffa0
@@ -230,16 +230,16 @@
         let coin2: Coin = Coin::new(
             hex!("ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000").into(),
             hex!("d23da14695a188ae5708dd152263c4db883eb27edeb936178d4d988b8f3ce5fc").into(),
             18375000000000000000,
         );
 
         let result = solution_generator_backrefs([
-            (coin1.clone(), PUZZLE1.as_ref(), SOLUTION1.as_ref()),
-            (coin2.clone(), PUZZLE2.as_ref(), SOLUTION2.as_ref()),
+            (coin1, PUZZLE1.as_ref(), SOLUTION1.as_ref()),
+            (coin2, PUZZLE2.as_ref(), SOLUTION2.as_ref()),
         ])
         .expect("solution_generator");
 
         assert_eq!(
             result,
             hex!(
                 "
```

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/test_generators.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/test_generators.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/gen/validation_error.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/gen/validation_error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/merkle_set.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/merkle_set.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-consensus/src/merkle_tree.rs` & `chik_rs-0.8.0/crates/chik-consensus/src/merkle_tree.rs`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
         for item in leafs {
             let Ok((included, proof)) = tree.generate_proof(item) else {
                 panic!("failed to generate proof");
             };
             assert!(included);
             let rebuilt = MerkleSet::from_proof(&proof).expect("failed to parse proof");
             assert_eq!(rebuilt.get_root(), root);
-            let (included, new_proof) = rebuilt.generate_proof(&item).unwrap();
+            let (included, new_proof) = rebuilt.generate_proof(item).unwrap();
             assert!(included);
             assert_eq!(new_proof, Vec::<u8>::new());
             assert_eq!(rebuilt.get_root(), root);
         }
 
         // === proofs-of-exclusion ===
         let mut rng = SmallRng::seed_from_u64(42);
```

### Comparing `chik_rs-0.7.0/crates/chik-bls/Cargo.toml` & `chik_rs-0.8.0/crates/chik-bls/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 [package]
 name = "chik-bls"
-version = "0.7.0"
+version = "0.8.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "BLS signature, verification and aggregation funcions for the Chik blockchain"
 authors = ["Arvid Norberg <arvid@chiknetwork.com>"]
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 
 [features]
 py-bindings = ["dep:pyo3", "chik_py_streamable_macro", "chik-traits/py-bindings"]
+arbitrary = ["dep:arbitrary"]
 
 [dependencies]
-chik-traits = { version = "0.7.0", path = "../chik-traits" }
+chik-traits = { version = "0.8.0", path = "../chik-traits" }
 chik_py_streamable_macro = { version = "0.7.0", path = "../chik_py_streamable_macro", optional = true }
 tiny-bip39 = "1.0.0"
 anyhow = "1.0.71"
 sha2 = "0.10.8"
 hkdf = "0.12.0"
 blst = { version = "0.3.11", git = "https://github.com/supranational/blst.git", rev = "0d46eefa45fc1e57aceb42bba0e84eab3a7a9725", features = ["portable"] }
 hex = "0.4.3"
 thiserror = "1.0.44"
 pyo3 = { version = "0.19.0", features = ["multiple-pymethods"], optional = true }
-arbitrary = { version = "1.3.0" }
+arbitrary = { version = "1.3.0" , optional = true}
+lru = "0.12.2"
+
 
 [dev-dependencies]
 rand = "0.8.5"
 criterion = "0.5.1"
 rstest = "0.17.0"
 
 [lib]
@@ -43,7 +46,11 @@
 [[bench]]
 name = "verify"
 harness = false
 
 [[bench]]
 name = "parse"
 harness = false
+
+[[bench]]
+name = "cache"
+harness = false
```

### Comparing `chik_rs-0.7.0/crates/chik-bls/README.md` & `chik_rs-0.8.0/crates/chik-bls/README.md`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-bls/benches/derive_key.rs` & `chik_rs-0.8.0/crates/chik-bls/benches/derive_key.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-bls/benches/parse.rs` & `chik_rs-0.8.0/crates/chik-bls/benches/parse.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-bls/benches/sign.rs` & `chik_rs-0.8.0/crates/chik-bls/benches/sign.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-bls/src/derive_keys.rs` & `chik_rs-0.8.0/crates/chik-bls/src/derive_keys.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-bls/src/error.rs` & `chik_rs-0.8.0/crates/chik-bls/src/error.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-bls/src/gtelement.rs` & `chik_rs-0.8.0/crates/chik-bls/src/gtelement.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 use chik_traits::chik_error::Result;
 use chik_traits::{read_bytes, Streamable};
 use sha2::{Digest, Sha256};
 use std::fmt;
 use std::hash::{Hash, Hasher};
 use std::io::Cursor;
 use std::mem::MaybeUninit;
-use std::ops::MulAssign;
+use std::ops::{Mul, MulAssign};
 
 #[cfg(feature = "py-bindings")]
 use chik_py_streamable_macro::PyStreamable;
 #[cfg(feature = "py-bindings")]
 use chik_traits::from_json_dict::FromJsonDict;
 #[cfg(feature = "py-bindings")]
 use chik_traits::to_json_dict::ToJsonDict;
 #[cfg(feature = "py-bindings")]
 use pyo3::exceptions::PyValueError;
 #[cfg(feature = "py-bindings")]
 use pyo3::{pyclass, pymethods, IntoPy, PyAny, PyObject, PyResult, Python};
 
-#[cfg_attr(feature = "py-bindings", pyclass, derive(PyStreamable, Clone))]
+#[cfg_attr(feature = "py-bindings", pyclass, derive(PyStreamable))]
+#[derive(Clone)]
 pub struct GTElement(pub(crate) blst_fp12);
 
 impl GTElement {
     const SIZE: usize = std::mem::size_of::<blst_fp12>();
 
     pub fn from_bytes(bytes: &[u8; Self::SIZE]) -> Self {
         let gt = unsafe {
@@ -89,14 +90,26 @@
     fn mul_assign(&mut self, rhs: &GTElement) {
         unsafe {
             blst_fp12_mul(&mut self.0, &self.0, &rhs.0);
         }
     }
 }
 
+impl Mul<&GTElement> for &GTElement {
+    type Output = GTElement;
+    fn mul(self, rhs: &GTElement) -> GTElement {
+        let gt = unsafe {
+            let mut gt = MaybeUninit::<blst_fp12>::uninit();
+            blst_fp12_mul(gt.as_mut_ptr(), &self.0, &rhs.0);
+            gt.assume_init()
+        };
+        GTElement(gt)
+    }
+}
+
 #[cfg(feature = "py-bindings")]
 impl ToJsonDict for GTElement {
     fn to_json_dict(&self, py: Python) -> pyo3::PyResult<PyObject> {
         let bytes = self.to_bytes();
         Ok(hex::encode(bytes).into_py(py))
     }
 }
```

### Comparing `chik_rs-0.7.0/crates/chik-bls/src/mnemonic.rs` & `chik_rs-0.8.0/crates/chik-bls/src/mnemonic.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/crates/chik-bls/src/public_key.rs` & `chik_rs-0.8.0/crates/chik-bls/src/public_key.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 use pyo3::{pyclass, pymethods, IntoPy, PyAny, PyObject, PyResult, Python};
 
 #[cfg_attr(
     feature = "py-bindings",
     pyclass(name = "G1Element"),
     derive(PyStreamable)
 )]
-#[derive(Clone, Default)]
+#[derive(Clone, Copy, Default)]
 pub struct PublicKey(pub(crate) blst_p1);
 
-#[cfg(fuzzing)]
+#[cfg(feature = "arbitrary")]
 impl<'a> arbitrary::Arbitrary<'a> for PublicKey {
     fn arbitrary(_u: &mut arbitrary::Unstructured<'a>) -> arbitrary::Result<Self> {
         // placeholder
         Ok(Self::default())
     }
 }
 
@@ -233,15 +233,15 @@
         self
     }
 }
 
 impl Neg for &PublicKey {
     type Output = PublicKey;
     fn neg(self) -> Self::Output {
-        let mut ret = self.clone();
+        let mut ret = *self;
         ret.negate();
         ret
     }
 }
 
 impl AddAssign<&PublicKey> for PublicKey {
     fn add_assign(&mut self, rhs: &PublicKey) {
@@ -250,15 +250,15 @@
         }
     }
 }
 
 impl SubAssign<&PublicKey> for PublicKey {
     fn sub_assign(&mut self, rhs: &PublicKey) {
         unsafe {
-            let mut neg = rhs.clone();
+            let mut neg = *rhs;
             blst_p1_cneg(&mut neg.0, true);
             blst_p1_add_or_double(&mut self.0, &self.0, &neg.0);
         }
     }
 }
 
 impl Add<&PublicKey> for &PublicKey {
@@ -625,27 +625,27 @@
         let mut data = [0u8; 32];
         for _i in 0..50 {
             // this integer may not exceed the group order, so leave the top
             // byte as 0
             rng.fill(&mut data[1..]);
 
             let g1 = PublicKey::from_integer(&data);
-            let mut g1_neg = g1.clone();
+            let mut g1_neg = g1;
             g1_neg.negate();
             assert!(g1_neg != g1);
 
             g1_neg.negate();
             assert!(g1_neg == g1);
         }
     }
 
     #[test]
     fn test_negate_infinity() {
         let g1 = PublicKey::default();
-        let mut g1_neg = g1.clone();
+        let mut g1_neg = g1;
         // negate on infinity is a no-op
         g1_neg.negate();
         assert!(g1_neg == g1);
     }
 
     #[test]
     fn test_negate() {
@@ -653,18 +653,18 @@
         let mut data = [0u8; 32];
         for _i in 0..50 {
             // this integer may not exceed the group order, so leave the top
             // byte as 0
             rng.fill(&mut data[1..]);
 
             let g1 = PublicKey::from_integer(&data);
-            let mut g1_neg = g1.clone();
+            let mut g1_neg = g1;
             g1_neg.negate();
 
-            let mut g1_double = g1.clone();
+            let mut g1_double = g1;
             // adding the negative undoes adding the positive
             g1_double += &g1;
             assert!(g1_double != g1);
             g1_double += &g1_neg;
             assert!(g1_double == g1);
         }
     }
@@ -675,15 +675,15 @@
         let mut data = [0u8; 32];
         for _i in 0..50 {
             // this integer may not exceed the group order, so leave the top
             // byte as 0
             rng.fill(&mut data[1..]);
 
             let mut g1 = PublicKey::from_integer(&data);
-            let mut g1_double = g1.clone();
+            let mut g1_double = g1;
             g1_double += &g1;
             assert!(g1_double != g1);
             // scalar multiply by 2 is the same as adding oneself
             g1.scalar_multiply(&[2]);
             assert!(g1_double == g1);
         }
     }
```

### Comparing `chik_rs-0.7.0/crates/chik-bls/src/secret_key.rs` & `chik_rs-0.8.0/crates/chik-bls/src/secret_key.rs`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     feature = "py-bindings",
     pyclass(frozen, name = "PrivateKey"),
     derive(PyStreamable)
 )]
 #[derive(PartialEq, Eq, Clone)]
 pub struct SecretKey(pub(crate) blst_scalar);
 
-#[cfg(fuzzing)]
+#[cfg(feature = "arbitrary")]
 impl<'a> arbitrary::Arbitrary<'a> for SecretKey {
     fn arbitrary(u: &mut arbitrary::Unstructured<'a>) -> arbitrary::Result<Self> {
         let mut seed = [0_u8; 32];
         let _ = u.fill_buffer(seed.as_mut_slice());
         Ok(Self::from_seed(&seed))
     }
 }
```

### Comparing `chik_rs-0.7.0/crates/chik-bls/src/signature.rs` & `chik_rs-0.8.0/crates/chik-bls/src/signature.rs`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     feature = "py-bindings",
     pyclass(name = "G2Element"),
     derive(PyStreamable)
 )]
 #[derive(Clone, Default)]
 pub struct Signature(pub(crate) blst_p2);
 
-#[cfg(fuzzing)]
+#[cfg(feature = "arbitrary")]
 impl<'a> arbitrary::Arbitrary<'a> for Signature {
     fn arbitrary(_u: &mut arbitrary::Unstructured<'a>) -> arbitrary::Result<Self> {
         // placeholder
         Ok(Self::default())
     }
 }
 
@@ -284,14 +284,19 @@
     }
 
     pub fn __iadd__(&mut self, rhs: &Self) {
         *self += rhs;
     }
 }
 
+// validate a series of public keys (G1 points) and G2 points. These points are
+// paired and the resulting GT points are multiplied. If the resulting GT point
+// is the identity, the function returns true, otherwise false. To validate an
+// aggregate signature, include the G1 generator and the signature as one of the
+// pairs.
 pub fn aggregate_pairing<G1: Borrow<PublicKey>, G2: Borrow<Signature>, I>(data: I) -> bool
 where
     I: IntoIterator<Item = (G1, G2)>,
 {
     let mut data = data.into_iter().peekable();
     if data.peek().is_none() {
         return true;
@@ -357,26 +362,30 @@
             0,
         );
         p2.assume_init()
     };
     Signature(p2)
 }
 
+// aggregate the signatures into a single one. It can then be validated using
+// aggregate_verify()
 pub fn aggregate<Sig: Borrow<Signature>, I>(sigs: I) -> Signature
 where
     I: IntoIterator<Item = Sig>,
 {
     let mut ret = Signature::default();
 
     for s in sigs.into_iter() {
         ret.aggregate(s.borrow());
     }
     ret
 }
 
+// verify a signature given a single public key and message using the augmented
+// scheme, i.e. the public key is pre-pended to the message before hashed to G2.
 pub fn verify<Msg: AsRef<[u8]>>(sig: &Signature, key: &PublicKey, msg: Msg) -> bool {
     unsafe {
         let mut pubkey_affine = MaybeUninit::<blst_p1_affine>::uninit();
         let mut sig_affine = MaybeUninit::<blst_p2_affine>::uninit();
 
         blst_p1_to_affine(pubkey_affine.as_mut_ptr(), &key.0);
         blst_p2_to_affine(sig_affine.as_mut_ptr(), &sig.0);
@@ -396,14 +405,17 @@
             0,
         );
 
         err == BLST_ERROR::BLST_SUCCESS
     }
 }
 
+// verify an aggregate signature given all public keys and messages.
+// Messages will been augmented with the public key.
+// returns true if the signature is valid.
 pub fn aggregate_verify<Pk: Borrow<PublicKey>, Msg: Borrow<[u8]>, I>(
     sig: &Signature,
     data: I,
 ) -> bool
 where
     I: IntoIterator<Item = (Pk, Msg)>,
 {
@@ -471,14 +483,39 @@
 
     unsafe {
         blst_pairing_commit(ctx);
         blst_pairing_finalverify(ctx, &sig_gt)
     }
 }
 
+// verify an aggregate signature by pre-paired public keys and messages.
+// Messages having been augmented and hashed to G2 and then paired with the G1
+// public key.
+// returns true if the signature is valid.
+pub fn aggregate_verify_gt<Gt: Borrow<GTElement>, I>(sig: &Signature, data: I) -> bool
+where
+    I: IntoIterator<Item = Gt>,
+{
+    if !sig.is_valid() {
+        return false;
+    }
+
+    let mut data = data.into_iter();
+    let Some(agg) = data.next() else {
+        return *sig == Signature::default();
+    };
+
+    let mut agg = agg.borrow().clone();
+    for gt in data {
+        agg *= gt.borrow();
+    }
+
+    agg == sig.pair(&PublicKey::generator())
+}
+
 // Signs msg using sk without augmenting the message with the public key. This
 // function is used when the caller augments the message with some other public
 // key
 pub fn sign_raw<Msg: AsRef<[u8]>>(sk: &SecretKey, msg: Msg) -> Signature {
     let p2 = unsafe {
         let mut p2 = MaybeUninit::<blst_p2>::uninit();
         blst_hash_to_g2(
@@ -492,14 +529,16 @@
         );
         blst_sign_pk_in_g1(p2.as_mut_ptr(), p2.as_ptr(), &sk.0);
         p2.assume_init()
     };
     Signature(p2)
 }
 
+// Signs msg using sk using the augmented scheme, meaning the public key is
+// pre-pended to msg befire signing.
 pub fn sign<Msg: AsRef<[u8]>>(sk: &SecretKey, msg: Msg) -> Signature {
     let mut aug_msg = sk.public_key().to_bytes().to_vec();
     aug_msg.extend_from_slice(msg.as_ref());
     sign_raw(sk, aug_msg)
 }
 
 #[cfg(test)]
@@ -653,20 +692,20 @@
         let mut agg2 = Signature::default();
         let mut sigs = Vec::<Signature>::new();
         let mut data = Vec::<(PublicKey, &[u8])>::new();
         let mut pairs = Vec::<(PublicKey, Signature)>::new();
         for idx in 0..4 {
             let derived = sk.derive_hardened(idx as u32);
             let pk = derived.public_key();
-            data.push((pk.clone(), msg));
+            data.push((pk, msg));
             let sig = sign(&derived, msg);
             agg1.aggregate(&sig);
             agg2 += &sig;
             sigs.push(sig);
-            pairs.push((pk.clone(), aug_msg_to_g2(&pk, msg)));
+            pairs.push((pk, aug_msg_to_g2(&pk, msg)));
         }
         let agg3 = aggregate(&sigs);
         let agg4 = &sigs[0] + &sigs[1] + &sigs[2] + &sigs[3];
 
         assert_eq!(agg1.to_bytes(), <[u8; 96]>::from_hex("87bce2c588f4257e2792d929834548c7d3af679272cb4f8e1d24cf4bf584dd287aa1d9f5e53a86f288190db45e1d100d0a5e936079a66a709b5f35394cf7d52f49dd963284cb5241055d54f8cf48f61bc1037d21cae6c025a7ea5e9f4d289a18").unwrap());
         assert_eq!(agg1, agg2);
         assert_eq!(agg1, agg3);
@@ -680,28 +719,66 @@
 
         pairs.push((-PublicKey::generator(), agg1));
         assert!(aggregate_pairing(pairs.clone()));
         // order does not matter
         assert!(aggregate_pairing(pairs.into_iter().rev()));
     }
 
+    #[rstest]
+    fn test_aggregate_gt_signature(#[values(0, 1, 2, 3, 4, 5, 100)] num_keys: usize) {
+        let sk_hex = "52d75c4707e39595b27314547f9723e5530c01198af3fc5849d9a7af65631efb";
+        let sk = SecretKey::from_bytes(&<[u8; 32]>::from_hex(sk_hex).unwrap()).unwrap();
+        let msg = b"foobar";
+        let mut agg = Signature::default();
+        let mut gts = Vec::<GTElement>::new();
+        let mut pks = Vec::<PublicKey>::new();
+        for idx in 0..num_keys {
+            let derived = sk.derive_hardened(idx as u32);
+            let pk = derived.public_key();
+            let sig = sign(&derived, msg);
+            agg.aggregate(&sig);
+            gts.push(aug_msg_to_g2(&pk, msg).pair(&pk));
+            pks.push(pk);
+        }
+
+        assert!(aggregate_verify_gt(&agg, &gts));
+        assert!(aggregate_verify(&agg, pks.iter().map(|pk| (pk, &msg[..]))));
+
+        // the order of the GTElements does not matter
+        for _ in 0..num_keys {
+            gts.rotate_right(1);
+            pks.rotate_right(1);
+            assert!(aggregate_verify_gt(&agg, &gts));
+            assert!(aggregate_verify(&agg, pks.iter().map(|pk| (pk, &msg[..]))));
+        }
+        for _ in 0..num_keys {
+            gts.rotate_right(1);
+            pks.rotate_right(1);
+            assert!(!aggregate_verify_gt(&agg, &gts[1..]));
+            assert!(!aggregate_verify(
+                &agg,
+                pks[1..].iter().map(|pk| (pk, &msg[..]))
+            ));
+        }
+    }
+
     #[test]
     fn test_aggregate_duplicate_signature() {
         let sk_hex = "52d75c4707e39595b27314547f9723e5530c01198af3fc5849d9a7af65631efb";
         let sk = SecretKey::from_bytes(&<[u8; 32]>::from_hex(sk_hex).unwrap()).unwrap();
         let msg = b"foobar";
         let mut agg = Signature::default();
         let mut data = Vec::<(PublicKey, &[u8])>::new();
         let mut pairs = Vec::<(PublicKey, Signature)>::new();
         for _idx in 0..2 {
             let pk = sk.public_key();
-            data.push((pk.clone(), msg));
+            data.push((pk, msg));
             agg.aggregate(&sign(&sk, *msg));
 
-            pairs.push((pk.clone(), aug_msg_to_g2(&pk, msg)));
+            pairs.push((pk, aug_msg_to_g2(&pk, msg)));
         }
 
         assert_eq!(agg.to_bytes(), <[u8; 96]>::from_hex("a1cca6540a4a06d096cb5b5fc76af5fd099476e70b623b8c6e4cf02ffde94fc0f75f4e17c67a9e350940893306798a3519368b02dc3464b7270ea4ca233cfa85a38da9e25c9314e81270b54d1e773a2ec5c3e14c62dac7abdebe52f4688310d3").unwrap());
 
         assert!(aggregate_verify(&agg, data));
 
         pairs.push((-PublicKey::generator(), agg));
```

### Comparing `chik_rs-0.7.0/wheel/Cargo.toml` & `chik_rs-0.8.0/wheel/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [package]
 name = "chik_rs"
-version = "0.7.0"
+version = "0.8.0"
 authors = ["Richard Kiss <him@richardkiss.com>"]
 edition = "2021"
 license = "Apache-2.0"
 description = "Code useful for implementing chik consensus."
 homepage = "https://github.com/Chik-Network/chik_rs"
 repository = "https://github.com/Chik-Network/chik_rs"
 readme = "README.md"
 
 [lib]
 name = "chik_rs"
 crate-type = ["cdylib"]
 path = "src/lib.rs"
 
 [dependencies]
-klvmr = "0.6.1"
+klvmr = "0.7.0"
 hex = "0.4.3"
 sha2 = "0.10.8"
 pyo3 = { version = "=0.19.0", features = ["multiple-pymethods"] }
-chik-consensus = { version = "0.7.0", path = "../crates/chik-consensus", features = ["py-bindings"] }
-chik-bls = { version = "0.7.0", path = "../crates/chik-bls", features = ["py-bindings"]  }
-chik-protocol = { version = "0.7.0", path = "../crates/chik-protocol", features = ["py-bindings"]  }
-chik-traits = { version = "0.7.0", path = "../crates/chik-traits", features = ["py-bindings"]  }
-klvm-traits = { version = "0.7.0", path = "../crates/klvm-traits", features = ["derive", "py-bindings"] }
-klvm-utils = { version = "0.7.0", path = "../crates/klvm-utils" }
+chik-consensus = { version = "0.8.0", path = "../crates/chik-consensus", features = ["py-bindings"] }
+chik-bls = { version = "0.8.0", path = "../crates/chik-bls", features = ["py-bindings"]  }
+chik-protocol = { version = "0.8.0", path = "../crates/chik-protocol", features = ["py-bindings"]  }
+chik-traits = { version = "0.8.0", path = "../crates/chik-traits", features = ["py-bindings"]  }
+klvm-traits = { version = "0.8.0", path = "../crates/klvm-traits", features = ["derive", "py-bindings"] }
+klvm-utils = { version = "0.8.0", path = "../crates/klvm-utils" }
 chik_py_streamable_macro = { version = "0.7.0", path = "../crates/chik_py_streamable_macro" }
-chik_streamable_macro = { version = "=0.6.0", path = "../crates/chik_streamable_macro" }
+chik_streamable_macro = { version = "0.8.0", path = "../crates/chik_streamable_macro" }
```

### Comparing `chik_rs-0.7.0/wheel/generate_type_stubs.py` & `chik_rs-0.8.0/wheel/generate_type_stubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from glob import glob
 
 output_file = Path(__file__).parent.resolve() / "python" / "chik_rs" / "chik_rs.pyi"
 crates_dir = Path(__file__).parent.parent.resolve() / "crates"
 input_dir = crates_dir / "chik-protocol" / "src"
 
 # enums are exposed to python as int
-enums = set(["NodeType", "ProtocolMessageTypes"])
+enums = set(["NodeType", "ProtocolMessageTypes", "RejectStateReason"])
 
 
 def transform_type(m: str) -> str:
     n, t = m.split(":")
     if "List[" in t:
         t = t.replace("List[", "Sequence[")
     elif "bytes32" == t.strip():
@@ -193,14 +193,19 @@
         "weight: uint128",
         "header_hash: bytes32",
         "total_iters: uint128",
         "log_string: str",
         "is_transaction_block: bool",
         "first_in_sub_slot: bool",
     ],
+    "UnfinishedHeaderBlock": [
+        "prev_header_hash: bytes32",
+        "header_hash: bytes32",
+        "total_iters: uint128",
+    ],
     "RewardChainBlock": [
         "def get_unfinished(self) -> RewardChainBlockUnfinished: ...",
     ],
     "SubSlotData": [
         "def is_end_of_slot(self) -> bool: ...",
         "def is_challenge(self) -> bool: ...",
     ],
@@ -329,14 +334,20 @@
     pair: Optional[Tuple[LazyNode, LazyNode]]
     atom: Optional[bytes]
 
 def serialized_length(program: ReadableBuffer) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
 def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
+class BLSCache:
+    def __init__(self, cache_size: Optional[int] = 50000) -> None: ...
+    def len(self) -> int: ...
+    def aggregate_verify(self, pks: List[G1Element], msgs: List[bytes], sig: G2Element) -> bool: ...
+    
+
 class AugSchemeMPL:
     @staticmethod
     def sign(pk: PrivateKey, msg: bytes, prepend_pk: Optional[G1Element] = None) -> G2Element: ...
     @staticmethod
     def aggregate(sigs: Sequence[G2Element]) -> G2Element: ...
     @staticmethod
     def verify(pk: G1Element, msg: bytes, sig: G2Element) -> bool: ...
@@ -428,36 +439,36 @@
             "height_relative: Optional[int]",
             "seconds_relative: Optional[int]",
             "before_height_relative: Optional[int]",
             "before_seconds_relative: Optional[int]",
             "birth_height: Optional[int]",
             "birth_seconds: Optional[int]",
             "create_coin: List[Tuple[bytes, int, Optional[bytes]]]",
-            "agg_sig_me: List[Tuple[bytes, bytes]]",
-            "agg_sig_parent: List[Tuple[bytes, bytes]]",
-            "agg_sig_puzzle: List[Tuple[bytes, bytes]]",
-            "agg_sig_amount: List[Tuple[bytes, bytes]]",
-            "agg_sig_puzzle_amount: List[Tuple[bytes, bytes]]",
-            "agg_sig_parent_amount: List[Tuple[bytes, bytes]]",
-            "agg_sig_parent_puzzle: List[Tuple[bytes, bytes]]",
+            "agg_sig_me: List[Tuple[G1Element, bytes]]",
+            "agg_sig_parent: List[Tuple[G1Element, bytes]]",
+            "agg_sig_puzzle: List[Tuple[G1Element, bytes]]",
+            "agg_sig_amount: List[Tuple[G1Element, bytes]]",
+            "agg_sig_puzzle_amount: List[Tuple[G1Element, bytes]]",
+            "agg_sig_parent_amount: List[Tuple[G1Element, bytes]]",
+            "agg_sig_parent_puzzle: List[Tuple[G1Element, bytes]]",
             "flags: int",
         ],
     )
 
     print_class(
         file,
         "SpendBundleConditions",
         [
             "spends: List[Spend]",
             "reserve_fee: int",
             "height_absolute: int",
             "seconds_absolute: int",
             "before_height_absolute: Optional[int]",
             "before_seconds_absolute: Optional[int]",
-            "agg_sig_unsafe: List[Tuple[bytes, bytes]]",
+            "agg_sig_unsafe: List[Tuple[G1Element, bytes]]",
             "cost: int",
             "removal_amount: int",
             "addition_amount: int",
         ],
     )
 
     for item in classes:
```

### Comparing `chik_rs-0.7.0/wheel/python/chik_rs/chik_rs.pyi` & `chik_rs-0.8.0/wheel/python/chik_rs/chik_rs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,20 @@
     pair: Optional[Tuple[LazyNode, LazyNode]]
     atom: Optional[bytes]
 
 def serialized_length(program: ReadableBuffer) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
 def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
+class BLSCache:
+    def __init__(self, cache_size: Optional[int] = 50000) -> None: ...
+    def len(self) -> int: ...
+    def aggregate_verify(self, pks: List[G1Element], msgs: List[bytes], sig: G2Element) -> bool: ...
+    
+
 class AugSchemeMPL:
     @staticmethod
     def sign(pk: PrivateKey, msg: bytes, prepend_pk: Optional[G1Element] = None) -> G2Element: ...
     @staticmethod
     def aggregate(sigs: Sequence[G2Element]) -> G2Element: ...
     @staticmethod
     def verify(pk: G1Element, msg: bytes, sig: G2Element) -> bool: ...
@@ -234,42 +240,42 @@
     height_relative: Optional[int]
     seconds_relative: Optional[int]
     before_height_relative: Optional[int]
     before_seconds_relative: Optional[int]
     birth_height: Optional[int]
     birth_seconds: Optional[int]
     create_coin: List[Tuple[bytes, int, Optional[bytes]]]
-    agg_sig_me: List[Tuple[bytes, bytes]]
-    agg_sig_parent: List[Tuple[bytes, bytes]]
-    agg_sig_puzzle: List[Tuple[bytes, bytes]]
-    agg_sig_amount: List[Tuple[bytes, bytes]]
-    agg_sig_puzzle_amount: List[Tuple[bytes, bytes]]
-    agg_sig_parent_amount: List[Tuple[bytes, bytes]]
-    agg_sig_parent_puzzle: List[Tuple[bytes, bytes]]
+    agg_sig_me: List[Tuple[G1Element, bytes]]
+    agg_sig_parent: List[Tuple[G1Element, bytes]]
+    agg_sig_puzzle: List[Tuple[G1Element, bytes]]
+    agg_sig_amount: List[Tuple[G1Element, bytes]]
+    agg_sig_puzzle_amount: List[Tuple[G1Element, bytes]]
+    agg_sig_parent_amount: List[Tuple[G1Element, bytes]]
+    agg_sig_parent_puzzle: List[Tuple[G1Element, bytes]]
     flags: int
     def __init__(
         self,
         coin_id: bytes,
         parent_id: bytes,
         puzzle_hash: bytes,
         coin_amount: int,
         height_relative: Optional[int],
         seconds_relative: Optional[int],
         before_height_relative: Optional[int],
         before_seconds_relative: Optional[int],
         birth_height: Optional[int],
         birth_seconds: Optional[int],
         create_coin: Sequence[Tuple[bytes, int, Optional[bytes]]],
-        agg_sig_me: Sequence[Tuple[bytes, bytes]],
-        agg_sig_parent: Sequence[Tuple[bytes, bytes]],
-        agg_sig_puzzle: Sequence[Tuple[bytes, bytes]],
-        agg_sig_amount: Sequence[Tuple[bytes, bytes]],
-        agg_sig_puzzle_amount: Sequence[Tuple[bytes, bytes]],
-        agg_sig_parent_amount: Sequence[Tuple[bytes, bytes]],
-        agg_sig_parent_puzzle: Sequence[Tuple[bytes, bytes]],
+        agg_sig_me: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_parent: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_puzzle: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_amount: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_puzzle_amount: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_parent_amount: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_parent_puzzle: Sequence[Tuple[G1Element, bytes]],
         flags: int
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> Spend: ...
     def __copy__(self) -> Spend: ...
@@ -293,43 +299,43 @@
         height_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         seconds_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         before_height_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         before_seconds_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         birth_height: Union[ Optional[int], _Unspec] = _Unspec(),
         birth_seconds: Union[ Optional[int], _Unspec] = _Unspec(),
         create_coin: Union[ List[Tuple[bytes, int, Optional[bytes]]], _Unspec] = _Unspec(),
-        agg_sig_me: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_parent: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_puzzle: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_amount: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_puzzle_amount: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_parent_amount: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_parent_puzzle: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
+        agg_sig_me: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_parent: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_puzzle: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_amount: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_puzzle_amount: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_parent_amount: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_parent_puzzle: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
         flags: Union[ int, _Unspec] = _Unspec()) -> Spend: ...
 
 class SpendBundleConditions:
     spends: List[Spend]
     reserve_fee: int
     height_absolute: int
     seconds_absolute: int
     before_height_absolute: Optional[int]
     before_seconds_absolute: Optional[int]
-    agg_sig_unsafe: List[Tuple[bytes, bytes]]
+    agg_sig_unsafe: List[Tuple[G1Element, bytes]]
     cost: int
     removal_amount: int
     addition_amount: int
     def __init__(
         self,
         spends: Sequence[Spend],
         reserve_fee: int,
         height_absolute: int,
         seconds_absolute: int,
         before_height_absolute: Optional[int],
         before_seconds_absolute: Optional[int],
-        agg_sig_unsafe: Sequence[Tuple[bytes, bytes]],
+        agg_sig_unsafe: Sequence[Tuple[G1Element, bytes]],
         cost: int,
         removal_amount: int,
         addition_amount: int
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
@@ -350,15 +356,15 @@
     def from_json_dict(json_dict: Any) -> SpendBundleConditions: ...
     def replace(self, *, spends: Union[ List[Spend], _Unspec] = _Unspec(),
         reserve_fee: Union[ int, _Unspec] = _Unspec(),
         height_absolute: Union[ int, _Unspec] = _Unspec(),
         seconds_absolute: Union[ int, _Unspec] = _Unspec(),
         before_height_absolute: Union[ Optional[int], _Unspec] = _Unspec(),
         before_seconds_absolute: Union[ Optional[int], _Unspec] = _Unspec(),
-        agg_sig_unsafe: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
+        agg_sig_unsafe: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
         cost: Union[ int, _Unspec] = _Unspec(),
         removal_amount: Union[ int, _Unspec] = _Unspec(),
         addition_amount: Union[ int, _Unspec] = _Unspec()) -> SpendBundleConditions: ...
 
 class BlockRecord:
     header_hash: bytes32
     prev_hash: bytes32
@@ -1692,14 +1698,72 @@
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
     def to_json_dict(self) -> Any: ...
     @staticmethod
     def from_json_dict(json_dict: Any) -> RespondPeers: ...
     def replace(self, *, peer_list: Union[ List[TimestampedPeerInfo], _Unspec] = _Unspec()) -> RespondPeers: ...
 
+class NewUnfinishedBlock2:
+    unfinished_reward_hash: bytes32
+    foliage_hash: Optional[bytes32]
+    def __init__(
+        self,
+        unfinished_reward_hash: bytes,
+        foliage_hash: Optional[bytes32]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> NewUnfinishedBlock2: ...
+    def __copy__(self) -> NewUnfinishedBlock2: ...
+    @staticmethod
+    def from_bytes(bytes) -> NewUnfinishedBlock2: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> NewUnfinishedBlock2: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[NewUnfinishedBlock2, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> NewUnfinishedBlock2: ...
+    def replace(self, *, unfinished_reward_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        foliage_hash: Union[ Optional[bytes32], _Unspec] = _Unspec()) -> NewUnfinishedBlock2: ...
+
+class RequestUnfinishedBlock2:
+    unfinished_reward_hash: bytes32
+    foliage_hash: Optional[bytes32]
+    def __init__(
+        self,
+        unfinished_reward_hash: bytes,
+        foliage_hash: Optional[bytes32]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestUnfinishedBlock2: ...
+    def __copy__(self) -> RequestUnfinishedBlock2: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestUnfinishedBlock2: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestUnfinishedBlock2: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestUnfinishedBlock2, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestUnfinishedBlock2: ...
+    def replace(self, *, unfinished_reward_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        foliage_hash: Union[ Optional[bytes32], _Unspec] = _Unspec()) -> RequestUnfinishedBlock2: ...
+
 class FullBlock:
     finished_sub_slots: List[EndOfSubSlotBundle]
     reward_chain_block: RewardChainBlock
     challenge_chain_sp_proof: Optional[VDFProof]
     challenge_chain_ip_proof: VDFProof
     reward_chain_sp_proof: Optional[VDFProof]
     reward_chain_ip_proof: VDFProof
@@ -2380,14 +2444,17 @@
     finished_sub_slots: List[EndOfSubSlotBundle]
     reward_chain_block: RewardChainBlockUnfinished
     challenge_chain_sp_proof: Optional[VDFProof]
     reward_chain_sp_proof: Optional[VDFProof]
     foliage: Foliage
     foliage_transaction_block: Optional[FoliageTransactionBlock]
     transactions_filter: bytes
+    prev_header_hash: bytes32
+    header_hash: bytes32
+    total_iters: uint128
     def __init__(
         self,
         finished_sub_slots: Sequence[EndOfSubSlotBundle],
         reward_chain_block: RewardChainBlockUnfinished,
         challenge_chain_sp_proof: Optional[VDFProof],
         reward_chain_sp_proof: Optional[VDFProof],
         foliage: Foliage,
@@ -3464,14 +3531,345 @@
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
     def to_json_dict(self) -> Any: ...
     @staticmethod
     def from_json_dict(json_dict: Any) -> RespondFeeEstimates: ...
     def replace(self, *, estimates: Union[ FeeEstimateGroup, _Unspec] = _Unspec()) -> RespondFeeEstimates: ...
 
+class RequestRemovePuzzleSubscriptions:
+    puzzle_hashes: Optional[List[bytes32]]
+    def __init__(
+        self,
+        puzzle_hashes: Optional[Sequence[bytes32]]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestRemovePuzzleSubscriptions: ...
+    def __copy__(self) -> RequestRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestRemovePuzzleSubscriptions, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestRemovePuzzleSubscriptions: ...
+    def replace(self, *, puzzle_hashes: Union[ Optional[List[bytes32]], _Unspec] = _Unspec()) -> RequestRemovePuzzleSubscriptions: ...
+
+class RespondRemovePuzzleSubscriptions:
+    puzzle_hashes: List[bytes32]
+    def __init__(
+        self,
+        puzzle_hashes: Sequence[bytes32]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RespondRemovePuzzleSubscriptions: ...
+    def __copy__(self) -> RespondRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def from_bytes(bytes) -> RespondRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RespondRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondRemovePuzzleSubscriptions, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RespondRemovePuzzleSubscriptions: ...
+    def replace(self, *, puzzle_hashes: Union[ List[bytes32], _Unspec] = _Unspec()) -> RespondRemovePuzzleSubscriptions: ...
+
+class RequestRemoveCoinSubscriptions:
+    coin_ids: Optional[List[bytes32]]
+    def __init__(
+        self,
+        coin_ids: Optional[Sequence[bytes32]]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestRemoveCoinSubscriptions: ...
+    def __copy__(self) -> RequestRemoveCoinSubscriptions: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestRemoveCoinSubscriptions: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestRemoveCoinSubscriptions: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestRemoveCoinSubscriptions, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestRemoveCoinSubscriptions: ...
+    def replace(self, *, coin_ids: Union[ Optional[List[bytes32]], _Unspec] = _Unspec()) -> RequestRemoveCoinSubscriptions: ...
+
+class RespondRemoveCoinSubscriptions:
+    coin_ids: List[bytes32]
+    def __init__(
+        self,
+        coin_ids: Sequence[bytes32]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RespondRemoveCoinSubscriptions: ...
+    def __copy__(self) -> RespondRemoveCoinSubscriptions: ...
+    @staticmethod
+    def from_bytes(bytes) -> RespondRemoveCoinSubscriptions: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RespondRemoveCoinSubscriptions: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondRemoveCoinSubscriptions, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RespondRemoveCoinSubscriptions: ...
+    def replace(self, *, coin_ids: Union[ List[bytes32], _Unspec] = _Unspec()) -> RespondRemoveCoinSubscriptions: ...
+
+class CoinStateFilters:
+    include_spent: bool
+    include_unspent: bool
+    include_hinted: bool
+    min_amount: uint64
+    def __init__(
+        self,
+        include_spent: bool,
+        include_unspent: bool,
+        include_hinted: bool,
+        min_amount: uint64
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> CoinStateFilters: ...
+    def __copy__(self) -> CoinStateFilters: ...
+    @staticmethod
+    def from_bytes(bytes) -> CoinStateFilters: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> CoinStateFilters: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[CoinStateFilters, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> CoinStateFilters: ...
+    def replace(self, *, include_spent: Union[ bool, _Unspec] = _Unspec(),
+        include_unspent: Union[ bool, _Unspec] = _Unspec(),
+        include_hinted: Union[ bool, _Unspec] = _Unspec(),
+        min_amount: Union[ uint64, _Unspec] = _Unspec()) -> CoinStateFilters: ...
+
+class RequestPuzzleState:
+    puzzle_hashes: List[bytes32]
+    previous_height: Optional[uint32]
+    header_hash: bytes32
+    filters: CoinStateFilters
+    subscribe_when_finished: bool
+    def __init__(
+        self,
+        puzzle_hashes: Sequence[bytes32],
+        previous_height: Optional[uint32],
+        header_hash: bytes,
+        filters: CoinStateFilters,
+        subscribe_when_finished: bool
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestPuzzleState: ...
+    def __copy__(self) -> RequestPuzzleState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestPuzzleState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestPuzzleState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestPuzzleState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestPuzzleState: ...
+    def replace(self, *, puzzle_hashes: Union[ List[bytes32], _Unspec] = _Unspec(),
+        previous_height: Union[ Optional[uint32], _Unspec] = _Unspec(),
+        header_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        filters: Union[ CoinStateFilters, _Unspec] = _Unspec(),
+        subscribe_when_finished: Union[ bool, _Unspec] = _Unspec()) -> RequestPuzzleState: ...
+
+class RespondPuzzleState:
+    puzzle_hashes: List[bytes32]
+    height: uint32
+    header_hash: bytes32
+    is_finished: bool
+    coin_states: List[CoinState]
+    def __init__(
+        self,
+        puzzle_hashes: Sequence[bytes32],
+        height: uint32,
+        header_hash: bytes,
+        is_finished: bool,
+        coin_states: Sequence[CoinState]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RespondPuzzleState: ...
+    def __copy__(self) -> RespondPuzzleState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RespondPuzzleState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RespondPuzzleState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondPuzzleState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RespondPuzzleState: ...
+    def replace(self, *, puzzle_hashes: Union[ List[bytes32], _Unspec] = _Unspec(),
+        height: Union[ uint32, _Unspec] = _Unspec(),
+        header_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        is_finished: Union[ bool, _Unspec] = _Unspec(),
+        coin_states: Union[ List[CoinState], _Unspec] = _Unspec()) -> RespondPuzzleState: ...
+
+class RejectPuzzleState:
+    reason: int
+    def __init__(
+        self,
+        reason: int
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RejectPuzzleState: ...
+    def __copy__(self) -> RejectPuzzleState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RejectPuzzleState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RejectPuzzleState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectPuzzleState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RejectPuzzleState: ...
+    def replace(self, *, reason: Union[ int, _Unspec] = _Unspec()) -> RejectPuzzleState: ...
+
+class RequestCoinState:
+    coin_ids: List[bytes32]
+    previous_height: Optional[uint32]
+    header_hash: bytes32
+    subscribe: bool
+    def __init__(
+        self,
+        coin_ids: Sequence[bytes32],
+        previous_height: Optional[uint32],
+        header_hash: bytes,
+        subscribe: bool
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestCoinState: ...
+    def __copy__(self) -> RequestCoinState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestCoinState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestCoinState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestCoinState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestCoinState: ...
+    def replace(self, *, coin_ids: Union[ List[bytes32], _Unspec] = _Unspec(),
+        previous_height: Union[ Optional[uint32], _Unspec] = _Unspec(),
+        header_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        subscribe: Union[ bool, _Unspec] = _Unspec()) -> RequestCoinState: ...
+
+class RespondCoinState:
+    coin_ids: List[bytes32]
+    coin_states: List[CoinState]
+    def __init__(
+        self,
+        coin_ids: Sequence[bytes32],
+        coin_states: Sequence[CoinState]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RespondCoinState: ...
+    def __copy__(self) -> RespondCoinState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RespondCoinState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RespondCoinState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondCoinState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RespondCoinState: ...
+    def replace(self, *, coin_ids: Union[ List[bytes32], _Unspec] = _Unspec(),
+        coin_states: Union[ List[CoinState], _Unspec] = _Unspec()) -> RespondCoinState: ...
+
+class RejectCoinState:
+    reason: int
+    def __init__(
+        self,
+        reason: int
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RejectCoinState: ...
+    def __copy__(self) -> RejectCoinState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RejectCoinState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RejectCoinState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectCoinState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RejectCoinState: ...
+    def replace(self, *, reason: Union[ int, _Unspec] = _Unspec()) -> RejectCoinState: ...
+
 class SubEpochData:
     reward_chain_hash: bytes32
     num_blocks_overflow: uint8
     new_sub_slot_iters: Optional[uint64]
     new_difficulty: Optional[uint64]
     def __init__(
         self,
```

### Comparing `chik_rs-0.7.0/wheel/python/chik_rs/sized_byte_class.py` & `chik_rs-0.8.0/wheel/python/chik_rs/sized_byte_class.py`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/wheel/python/chik_rs/sized_ints.py` & `chik_rs-0.8.0/wheel/python/chik_rs/sized_ints.py`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/wheel/python/chik_rs/struct_stream.py` & `chik_rs-0.8.0/wheel/python/chik_rs/struct_stream.py`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/wheel/src/api.rs` & `chik_rs-0.8.0/wheel/src/api.rs`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,37 @@
 use chik_consensus::gen::run_puzzle::run_puzzle as native_run_puzzle;
 use chik_consensus::gen::solution_generator::solution_generator as native_solution_generator;
 use chik_consensus::gen::solution_generator::solution_generator_backrefs as native_solution_generator_backrefs;
 use chik_consensus::merkle_set::compute_merkle_set_root as compute_merkle_root_impl;
 use chik_consensus::merkle_tree::{validate_merkle_proof, MerkleSet};
 use chik_protocol::{
     BlockRecord, Bytes32, ChallengeBlockInfo, ChallengeChainSubSlot, ClassgroupElement, Coin,
-    CoinSpend, CoinState, CoinStateUpdate, EndOfSubSlotBundle, Foliage, FoliageBlockData,
-    FoliageTransactionBlock, FullBlock, HeaderBlock, InfusedChallengeChainSubSlot, NewCompactVDF,
-    NewPeak, NewPeakWallet, NewSignagePointOrEndOfSubSlot, NewTransaction, NewUnfinishedBlock,
+    CoinSpend, CoinState, CoinStateFilters, CoinStateUpdate, EndOfSubSlotBundle, Foliage,
+    FoliageBlockData, FoliageTransactionBlock, FullBlock, HeaderBlock,
+    InfusedChallengeChainSubSlot, NewCompactVDF, NewPeak, NewPeakWallet,
+    NewSignagePointOrEndOfSubSlot, NewTransaction, NewUnfinishedBlock, NewUnfinishedBlock2,
     PoolTarget, Program, ProofBlockHeader, ProofOfSpace, PuzzleSolutionResponse, RecentChainData,
     RegisterForCoinUpdates, RegisterForPhUpdates, RejectAdditionsRequest, RejectBlock,
-    RejectBlockHeaders, RejectBlocks, RejectHeaderBlocks, RejectHeaderRequest,
-    RejectPuzzleSolution, RejectRemovalsRequest, RequestAdditions, RequestBlock,
-    RequestBlockHeader, RequestBlockHeaders, RequestBlocks, RequestChildren, RequestCompactVDF,
-    RequestFeeEstimates, RequestHeaderBlocks, RequestMempoolTransactions, RequestPeers,
-    RequestProofOfWeight, RequestPuzzleSolution, RequestRemovals, RequestSesInfo,
+    RejectBlockHeaders, RejectBlocks, RejectCoinState, RejectHeaderBlocks, RejectHeaderRequest,
+    RejectPuzzleSolution, RejectPuzzleState, RejectRemovalsRequest, RequestAdditions, RequestBlock,
+    RequestBlockHeader, RequestBlockHeaders, RequestBlocks, RequestChildren, RequestCoinState,
+    RequestCompactVDF, RequestFeeEstimates, RequestHeaderBlocks, RequestMempoolTransactions,
+    RequestPeers, RequestProofOfWeight, RequestPuzzleSolution, RequestPuzzleState, RequestRemovals,
+    RequestRemoveCoinSubscriptions, RequestRemovePuzzleSubscriptions, RequestSesInfo,
     RequestSignagePointOrEndOfSubSlot, RequestTransaction, RequestUnfinishedBlock,
-    RespondAdditions, RespondBlock, RespondBlockHeader, RespondBlockHeaders, RespondBlocks,
-    RespondChildren, RespondCompactVDF, RespondEndOfSubSlot, RespondFeeEstimates,
-    RespondHeaderBlocks, RespondPeers, RespondProofOfWeight, RespondPuzzleSolution,
-    RespondRemovals, RespondSesInfo, RespondSignagePoint, RespondToCoinUpdates, RespondToPhUpdates,
-    RespondTransaction, RespondUnfinishedBlock, RewardChainBlock, RewardChainBlockUnfinished,
-    RewardChainSubSlot, SendTransaction, SpendBundle, SubEpochChallengeSegment, SubEpochData,
-    SubEpochSegments, SubEpochSummary, SubSlotData, SubSlotProofs, TimestampedPeerInfo,
-    TransactionAck, TransactionsInfo, UnfinishedBlock, VDFInfo, VDFProof, WeightProof,
+    RequestUnfinishedBlock2, RespondAdditions, RespondBlock, RespondBlockHeader,
+    RespondBlockHeaders, RespondBlocks, RespondChildren, RespondCoinState, RespondCompactVDF,
+    RespondEndOfSubSlot, RespondFeeEstimates, RespondHeaderBlocks, RespondPeers,
+    RespondProofOfWeight, RespondPuzzleSolution, RespondPuzzleState, RespondRemovals,
+    RespondRemoveCoinSubscriptions, RespondRemovePuzzleSubscriptions, RespondSesInfo,
+    RespondSignagePoint, RespondToCoinUpdates, RespondToPhUpdates, RespondTransaction,
+    RespondUnfinishedBlock, RewardChainBlock, RewardChainBlockUnfinished, RewardChainSubSlot,
+    SendTransaction, SpendBundle, SubEpochChallengeSegment, SubEpochData, SubEpochSegments,
+    SubEpochSummary, SubSlotData, SubSlotProofs, TimestampedPeerInfo, TransactionAck,
+    TransactionsInfo, UnfinishedBlock, UnfinishedHeaderBlock, VDFInfo, VDFProof, WeightProof,
 };
 use klvm_utils::tree_hash_from_bytes;
 use klvmr::{ENABLE_BLS_OPS_OUTSIDE_GUARD, ENABLE_FIXED_DIV, LIMIT_HEAP, NO_UNKNOWN_OPS};
 use pyo3::buffer::PyBuffer;
 use pyo3::exceptions::{PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
@@ -58,15 +62,16 @@
 use klvmr::reduction::Reduction;
 use klvmr::run_program;
 use klvmr::serde::node_to_bytes;
 use klvmr::serde::{node_from_bytes, node_from_bytes_backrefs};
 use klvmr::ChikDialect;
 
 use chik_bls::{
-    hash_to_g2 as native_hash_to_g2, DerivableKey, GTElement, PublicKey, SecretKey, Signature,
+    hash_to_g2 as native_hash_to_g2, BLSCache, DerivableKey, GTElement, PublicKey, SecretKey,
+    Signature,
 };
 
 #[pyfunction]
 pub fn compute_merkle_set_root<'p>(
     py: Python<'p>,
     values: Vec<&'p PyBytes>,
 ) -> PyResult<&'p PyBytes> {
@@ -178,15 +183,15 @@
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<OwnedSpendBundleConditions> {
     let mut a = make_allocator(LIMIT_HEAP);
     let conds = native_run_puzzle::<MempoolVisitor>(
         &mut a, puzzle, solution, parent_id, amount, max_cost, flags,
     )?;
-    Ok(OwnedSpendBundleConditions::from(&a, conds))
+    Ok(OwnedSpendBundleConditions::from(&a, conds)?)
 }
 
 // this is like a CoinSpend but with references to the puzzle and solution,
 // rather than owning them
 type CoinSpendRef<'a> = (Coin, &'a [u8], &'a [u8]);
 
 fn convert_list_of_tuples(spends: &PyAny) -> PyResult<Vec<CoinSpendRef>> {
@@ -447,26 +452,38 @@
     m.add_class::<RespondBlockHeaders>()?;
     m.add_class::<RejectBlockHeaders>()?;
     m.add_class::<RequestBlockHeaders>()?;
     m.add_class::<RequestHeaderBlocks>()?;
     m.add_class::<RejectHeaderBlocks>()?;
     m.add_class::<RespondHeaderBlocks>()?;
     m.add_class::<HeaderBlock>()?;
+    m.add_class::<UnfinishedHeaderBlock>()?;
     m.add_class::<CoinState>()?;
     m.add_class::<RegisterForPhUpdates>()?;
     m.add_class::<RespondToPhUpdates>()?;
     m.add_class::<RegisterForCoinUpdates>()?;
     m.add_class::<RespondToCoinUpdates>()?;
     m.add_class::<CoinStateUpdate>()?;
     m.add_class::<RequestChildren>()?;
     m.add_class::<RespondChildren>()?;
     m.add_class::<RequestSesInfo>()?;
     m.add_class::<RespondSesInfo>()?;
     m.add_class::<RequestFeeEstimates>()?;
     m.add_class::<RespondFeeEstimates>()?;
+    m.add_class::<RequestRemovePuzzleSubscriptions>()?;
+    m.add_class::<RespondRemovePuzzleSubscriptions>()?;
+    m.add_class::<RequestRemoveCoinSubscriptions>()?;
+    m.add_class::<RespondRemoveCoinSubscriptions>()?;
+    m.add_class::<CoinStateFilters>()?;
+    m.add_class::<RequestPuzzleState>()?;
+    m.add_class::<RespondPuzzleState>()?;
+    m.add_class::<RejectPuzzleState>()?;
+    m.add_class::<RequestCoinState>()?;
+    m.add_class::<RespondCoinState>()?;
+    m.add_class::<RejectCoinState>()?;
 
     // full node protocol
     m.add_class::<NewPeak>()?;
     m.add_class::<NewTransaction>()?;
     m.add_class::<RequestTransaction>()?;
     m.add_class::<RespondTransaction>()?;
     m.add_class::<RequestProofOfWeight>()?;
@@ -486,14 +503,16 @@
     m.add_class::<RespondEndOfSubSlot>()?;
     m.add_class::<RequestMempoolTransactions>()?;
     m.add_class::<NewCompactVDF>()?;
     m.add_class::<RequestCompactVDF>()?;
     m.add_class::<RespondCompactVDF>()?;
     m.add_class::<RequestPeers>()?;
     m.add_class::<RespondPeers>()?;
+    m.add_class::<NewUnfinishedBlock2>()?;
+    m.add_class::<RequestUnfinishedBlock2>()?;
 
     // facilities from klvm_rs
 
     m.add_function(wrap_pyfunction!(run_chik_program, m)?)?;
     m.add("NO_UNKNOWN_OPS", NO_UNKNOWN_OPS)?;
     m.add("LIMIT_HEAP", LIMIT_HEAP)?;
     m.add("ENABLE_BLS_OPS_OUTSIDE_GUARD", ENABLE_BLS_OPS_OUTSIDE_GUARD)?;
@@ -506,10 +525,11 @@
     // facilities from chik-bls
 
     m.add_class::<PublicKey>()?;
     m.add_class::<Signature>()?;
     m.add_class::<GTElement>()?;
     m.add_class::<SecretKey>()?;
     m.add_class::<AugSchemeMPL>()?;
+    m.add_class::<BLSCache>()?;
 
     Ok(())
 }
```

### Comparing `chik_rs-0.7.0/wheel/src/run_generator.rs` & `chik_rs-0.8.0/wheel/src/run_generator.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use chik_consensus::allocator::make_allocator;
 use chik_consensus::gen::conditions::{EmptyVisitor, MempoolVisitor};
 use chik_consensus::gen::flags::ANALYZE_SPENDS;
 use chik_consensus::gen::owned_conditions::OwnedSpendBundleConditions;
 use chik_consensus::gen::run_block_generator::run_block_generator as native_run_block_generator;
 use chik_consensus::gen::run_block_generator::run_block_generator2 as native_run_block_generator2;
-use chik_consensus::gen::validation_error::ValidationErr;
+use chik_consensus::gen::validation_error::{ErrorCode, ValidationErr};
 
 use klvmr::cost::Cost;
 
 use pyo3::buffer::PyBuffer;
 use pyo3::prelude::*;
 use pyo3::types::PyList;
 
@@ -45,22 +45,20 @@
     } else {
         native_run_block_generator::<_, MempoolVisitor>
     };
 
     Ok(
         match run_block(&mut allocator, program, &refs, max_cost, flags) {
             Ok(spend_bundle_conds) => {
-                // everything was successful
-                (
-                    None,
-                    Some(OwnedSpendBundleConditions::from(
-                        &allocator,
-                        spend_bundle_conds,
-                    )),
-                )
+                let conds = OwnedSpendBundleConditions::from(&allocator, spend_bundle_conds);
+                match conds {
+                    // everything was successful
+                    Ok(c) => (None, Some(c)),
+                    Err(_) => (Some(ErrorCode::InvalidPublicKey.into()), None),
+                }
             }
             Err(ValidationErr(_, error_code)) => {
                 // a validation error occurred
                 (Some(error_code.into()), None)
             }
         },
     )
@@ -99,22 +97,20 @@
     } else {
         native_run_block_generator2::<_, MempoolVisitor>
     };
 
     Ok(
         match run_block(&mut allocator, program, &refs, max_cost, flags) {
             Ok(spend_bundle_conds) => {
-                // everything was successful
-                (
-                    None,
-                    Some(OwnedSpendBundleConditions::from(
-                        &allocator,
-                        spend_bundle_conds,
-                    )),
-                )
+                let conds = OwnedSpendBundleConditions::from(&allocator, spend_bundle_conds);
+                match conds {
+                    // everything was successful
+                    Ok(c) => (None, Some(c)),
+                    Err(_) => (Some(ErrorCode::InvalidPublicKey.into()), None),
+                }
             }
             Err(ValidationErr(_, error_code)) => {
                 // a validation error occurred
                 (Some(error_code.into()), None)
             }
         },
     )
```

### Comparing `chik_rs-0.7.0/wheel/src/run_program.rs` & `chik_rs-0.8.0/wheel/src/run_program.rs`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/Cargo.lock` & `chik_rs-0.8.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,65 +15,64 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.7"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77c3a9648d43b9cd48db467b3f87fdd6e146bcc88ab0180006cef2179fe11d01"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstream"
-version = "0.3.2"
+version = "0.6.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
- "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7079075b41f533b8c61d2a4d073c4676e1f8b249ff94a393b0595db304e0dd87"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
 name = "anstyle-parse"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
 dependencies = [
@@ -87,27 +86,27 @@
 checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "1.0.2"
+version = "3.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c677ab05e09154296dd37acecd46420c17b9713e8366facafa8fc0885167cf4c"
+checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
 dependencies = [
  "anstyle",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.75"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4668cab20f66d8d020e1fbc0ebe47217433c1b6c8f2040faf858554e394ace6"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "arbitrary"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2d098ff73c1ca148721f37baad5ea6a465a13f9573aba8641fbbbae8164a54e"
 dependencies = [
@@ -151,23 +150,23 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -178,17 +177,17 @@
 name = "base16ct"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
 [[package]]
 name = "base64"
-version = "0.21.5"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35636a1494ede3b646cc98f74f8e62c773a38a659ebc777a2cf26b9b74171df9"
+checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
@@ -196,17 +195,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
@@ -232,63 +231,64 @@
  "glob",
  "threadpool",
  "zeroize",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chik"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
- "chik-bls 0.7.0",
+ "chik-bls 0.8.0",
  "chik-client",
  "chik-consensus",
  "chik-protocol",
+ "chik-puzzles",
  "chik-ssl",
- "chik-traits 0.7.0",
- "chik-wallet",
+ "chik-traits 0.8.0",
  "klvm-traits",
  "klvm-utils",
 ]
 
 [[package]]
 name = "chik-bls"
 version = "0.4.0"
@@ -304,63 +304,65 @@
  "sha2",
  "thiserror",
  "tiny-bip39",
 ]
 
 [[package]]
 name = "chik-bls"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
  "anyhow",
  "arbitrary",
  "blst",
- "chik-traits 0.7.0",
+ "chik-traits 0.8.0",
  "chik_py_streamable_macro",
  "criterion",
  "hex",
  "hkdf",
+ "lru",
  "pyo3",
  "rand",
  "rstest 0.17.0",
  "sha2",
  "thiserror",
  "tiny-bip39",
 ]
 
 [[package]]
 name = "chik-bls-fuzz"
 version = "0.0.0"
 dependencies = [
- "chik-bls 0.7.0",
+ "chik-bls 0.8.0",
  "libfuzzer-sys",
  "pyo3",
 ]
 
 [[package]]
 name = "chik-client"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
  "chik-protocol",
- "chik-traits 0.7.0",
+ "chik-traits 0.8.0",
  "futures-util",
  "thiserror",
  "tokio",
  "tokio-tungstenite",
  "tungstenite",
 ]
 
 [[package]]
 name = "chik-consensus"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
+ "chik-bls 0.8.0",
  "chik-protocol",
- "chik-traits 0.7.0",
- "chik-wallet",
+ "chik-puzzles",
+ "chik-traits 0.8.0",
  "chik_py_streamable_macro",
- "chik_streamable_macro 0.6.0",
+ "chik_streamable_macro 0.8.0",
  "criterion",
  "hex",
  "hex-literal",
  "klvm-derive",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
@@ -375,76 +377,103 @@
 
 [[package]]
 name = "chik-fuzz"
 version = "0.6.0"
 dependencies = [
  "chik-consensus",
  "chik-protocol",
- "chik-traits 0.7.0",
+ "chik-traits 0.8.0",
  "hex-literal",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "libfuzzer-sys",
 ]
 
 [[package]]
 name = "chik-protocol"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
  "arbitrary",
- "chik-bls 0.7.0",
- "chik-traits 0.7.0",
+ "chik-bls 0.8.0",
+ "chik-traits 0.8.0",
  "chik_py_streamable_macro",
- "chik_streamable_macro 0.6.0",
+ "chik_streamable_macro 0.8.0",
  "hex",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "pyo3",
  "rstest 0.17.0",
  "sha2",
 ]
 
 [[package]]
 name = "chik-protocol-fuzz"
-version = "0.0.0"
+version = "0.8.0"
 dependencies = [
  "arbitrary",
  "chik-protocol",
- "chik-traits 0.7.0",
+ "chik-traits 0.8.0",
  "hex",
  "klvm-traits",
  "klvmr",
  "libfuzzer-sys",
  "sha2",
 ]
 
 [[package]]
+name = "chik-puzzles"
+version = "0.8.0"
+dependencies = [
+ "arbitrary",
+ "chik-bls 0.8.0",
+ "chik-protocol",
+ "hex",
+ "hex-literal",
+ "klvm-traits",
+ "klvm-utils",
+ "klvmr",
+ "num-bigint",
+ "sha2",
+]
+
+[[package]]
+name = "chik-puzzles-fuzz"
+version = "0.8.0"
+dependencies = [
+ "chik-puzzles",
+ "klvm-traits",
+ "klvmr",
+ "libfuzzer-sys",
+ "pyo3",
+]
+
+[[package]]
 name = "chik-ssl"
 version = "0.7.0"
 dependencies = [
  "lazy_static",
  "rand",
  "rcgen",
  "rsa",
  "thiserror",
  "time",
 ]
 
 [[package]]
 name = "chik-tools"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
  "blocking-threadpool",
- "chik-bls 0.7.0",
+ "chik-bls 0.8.0",
  "chik-consensus",
  "chik-protocol",
- "chik-traits 0.7.0",
- "chik-wallet",
+ "chik-puzzles",
+ "chik-traits 0.8.0",
  "clap",
  "hex",
  "hex-literal",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "rusqlite",
@@ -461,71 +490,42 @@
  "hex",
  "sha2",
  "thiserror",
 ]
 
 [[package]]
 name = "chik-traits"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
- "chik_py_streamable_macro",
- "chik_streamable_macro 0.6.0",
- "hex",
+ "chik_streamable_macro 0.8.0",
  "pyo3",
  "sha2",
  "thiserror",
 ]
 
 [[package]]
-name = "chik-wallet"
-version = "0.7.0"
-dependencies = [
- "arbitrary",
- "chik-bls 0.7.0",
- "chik-protocol",
- "hex",
- "hex-literal",
- "klvm-traits",
- "klvm-utils",
- "klvmr",
- "num-bigint",
- "sha2",
-]
-
-[[package]]
-name = "chik-wallet-fuzz"
-version = "0.6.0"
-dependencies = [
- "chik-wallet",
- "klvm-traits",
- "klvmr",
- "libfuzzer-sys",
- "pyo3",
-]
-
-[[package]]
 name = "chik_py_streamable_macro"
 version = "0.7.0"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "chik_rs"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
- "chik-bls 0.7.0",
+ "chik-bls 0.8.0",
  "chik-consensus",
  "chik-protocol",
- "chik-traits 0.7.0",
+ "chik-traits 0.8.0",
  "chik_py_streamable_macro",
- "chik_streamable_macro 0.6.0",
+ "chik_streamable_macro 0.8.0",
  "hex",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "pyo3",
  "sha2",
 ]
@@ -535,134 +535,118 @@
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b16474a430c84912f86b6454d6f5fe09ee67d33b3ddf6519ff0cb561f3bd29e"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "chik_streamable_macro"
-version = "0.6.0"
+version = "0.8.0"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "chik_wasm"
-version = "0.2.7"
+version = "0.8.0"
 dependencies = [
- "chik-consensus",
- "getrandom",
- "js-sys",
  "wasm-bindgen",
- "wasm-bindgen-test",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
+checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
+checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
+checksum = "57663b653d948a338bfb3eeba9bb2fd5fcfaecb9e199e87e1eda4d9e8b240fd9"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.9"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bba77a07e4489fb41bd90e8d4201c3eb246b3c2c9ea2ba0bddd6c1d1df87db7d"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
- "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.9"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c9b4a88bb4bc35d3d6f65a21b0f0bafe9c894fa00978de242c555ec28bea1c0"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstream",
  "anstyle",
- "bitflags 1.3.2",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.2"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.5.1"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd7cc57abe963c6d3b9d8be5b06ba7c8957a930305ca90304f24ef040aa6f961"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
-name = "console_error_panic_hook"
-version = "0.1.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
-dependencies = [
- "cfg-if",
- "wasm-bindgen",
-]
-
-[[package]]
 name = "const-oid"
-version = "0.9.5"
+version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28c122c3980598d243d63d9a704629a2d748d101f278052ff068be5a4423ab6f"
+checksum = "c2459377285ad874054d797f3ccebf984978aa39129f6eafde5cdc8315b612f8"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce420fe07aecd3e67c5f910618fe65e94158f6dcc0adf44e00d69ce2bdfe0fd0"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "criterion"
 version = "0.5.1"
@@ -697,52 +681,53 @@
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.11"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176dc175b78f56c0f321911d9c8eb2b77a78a4860b9c19db83835fea1a46649b"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
- "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.15"
+version = "0.9.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
- "autocfg",
- "cfg-if",
  "crossbeam-utils",
- "memoffset",
- "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "crypto-bigint"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0dc92fb57ca44df6db8059111ab3af99a63d5d0f8375d9972e319a379c6bab76"
 dependencies = [
  "generic-array",
  "rand_core",
@@ -764,17 +749,17 @@
 name = "data-encoding"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
 
 [[package]]
 name = "der"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fffa369a668c8af7dbf8b5e56c9f744fbd399949ed171606040001947de40b1c"
+checksum = "f55bf8e7b65898637379c1b74eb1551107c8294ed26d855ceb9fd1a09cfc9bc0"
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
@@ -789,30 +774,30 @@
  "num-bigint",
  "num-traits",
  "rusticata-macros",
 ]
 
 [[package]]
 name = "deranged"
-version = "0.3.10"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eb30d70a07a3b04884d2677f06bec33509dc67ca60d92949e5535352d3191dc"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "derive_arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -827,15 +812,15 @@
 name = "displaydoc"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "ecdsa"
 version = "0.16.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee27f32b5c5292967d2d4a9d7f1e0b0aed2c15daded5a60300e4abb9d8020bca"
@@ -846,17 +831,17 @@
  "rfc6979",
  "signature",
  "spki",
 ]
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "elliptic-curve"
 version = "0.13.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6043086bf7973472e0c7dff2142ea0b680d30e18d9cc40f267efbf222bd47"
 dependencies = [
@@ -877,24 +862,14 @@
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
-name = "errno"
-version = "0.3.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
-dependencies = [
- "libc",
- "windows-sys 0.52.0",
-]
-
-[[package]]
 name = "fallible-iterator"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2acce4a10f12dc2fb14a218589d4f1f62ef011b2d0cc4b3cb1bba8e94da14649"
 
 [[package]]
 name = "fallible-streaming-iterator"
@@ -925,94 +900,94 @@
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0290714b38af9b4a7b094b8a37086d1b4e61f2df9122c3cad2577669145335"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff4dd66668b557604244583e3e1e1eada8c5c2e96a6d0d6653ede395b78bbacb"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb1d22c66e66d9d72e1758f0bd7d4fd0bee04cad842ee34587d68c07e45d088c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f4fb8693db0cf099eadcca0efe2a5a22e4550f98ed16aba6c48700da29597bc"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bf34a163b5c4c52d0478a4d757da8fb65cabef42ba90515efee0f6f9fa45aaa"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53b153fd91e4b0147f4aced87be237c98248656bb01050b96bf3ee89220a8ddb"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e36d3378ee38c2a36ad710c5d30c2911d752cb941c00c72dbabfb786a7970817"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efd193069b0ddadc69c46389b740bbccdd97203899b48d09c5f7969591d6bae2"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-timer"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e64b03909df88034c26dc1547e8970b91f98bdb65165d6a4e9110d94263dbb2c"
+checksum = "f288b0a4f20f9a56b5d1da57e2227c661b7b16168e2f72365f57b63326e29b24"
 
 [[package]]
 name = "futures-util"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a19526d624e703a3179b3d322efec918b6246ea0fa51d41124525f00f1cc8104"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -1040,23 +1015,21 @@
 checksum = "14dbbfd5c71d70241ecf9e6f13737f7b5ce823821063188d7e46c41d371eebd5"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.11"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe9006bed769170c11f845cf00c7c1e9092aeb3f268e007c3e760ac68008070f"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
- "js-sys",
  "libc",
  "wasi",
- "wasm-bindgen",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
@@ -1076,17 +1049,21 @@
  "ff",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
 name = "half"
-version = "1.8.2"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
+dependencies = [
+ "cfg-if",
+ "crunchy",
+]
 
 [[package]]
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 dependencies = [
@@ -1101,23 +1078,23 @@
 checksum = "e8094feaf31ff591f651a2664fb9cfd92bba7a60ce3197265e9482ebe753c8f7"
 dependencies = [
  "hashbrown",
 ]
 
 [[package]]
 name = "heck"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -1125,17 +1102,17 @@
 name = "hex-literal"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fe2267d4ed49bc07b63801559be28c718ea06c4738b7a03c94df7386d2cde46"
 
 [[package]]
 name = "hkdf"
-version = "0.12.3"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "791a029f6b9fc27657f6f188ec6e5e43f6911f6f878e0dc5501396e09809d437"
+checksum = "7b5f8eb2ad728638ea2c7d47a21db23b7b58a72ed6a38256b8a1849f15fbbdf7"
 dependencies = [
  "hmac",
 ]
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
@@ -1143,17 +1120,17 @@
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "http"
-version = "1.0.0"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b32afd38673a8016f7c9ae69e5af41a58f81b1d31689040f2f1959594ce194ea"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -1170,65 +1147,65 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.1.0"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inventory"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0508c56cfe9bfd5dfeb0c22ab9a6abfda2f27bdca422132e494266351ed8d83c"
+checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.9"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
  "hermit-abi",
- "rustix",
- "windows-sys 0.48.0",
+ "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.27"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c37f63953c4c63420ed5fd3d6d398c719489b9f872b9fa683262f8edd363c7d"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.64"
@@ -1236,17 +1213,17 @@
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "k256"
-version = "0.13.2"
+version = "0.13.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f01b677d82ef7a676aa37e099defd83a28e15687112cafdd112d60236b6115b"
+checksum = "956ff9b67e26e1a6a866cb758f12c6f8746208489e3e4a4b5580802f2f0a587b"
 dependencies = [
  "cfg-if",
  "ecdsa",
  "elliptic-curve",
  "once_cell",
  "sha2",
  "signature",
@@ -1264,58 +1241,57 @@
 
 [[package]]
 name = "klvm-derive"
 version = "0.6.0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "klvm-traits"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
- "chik-bls 0.7.0",
+ "chik-bls 0.8.0",
  "hex",
  "hex-literal",
  "klvm-derive",
  "klvmr",
  "num-bigint",
  "pyo3",
  "thiserror",
 ]
 
 [[package]]
 name = "klvm-utils"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
  "hex",
  "klvm-traits",
  "klvmr",
  "rstest 0.16.0",
 ]
 
 [[package]]
 name = "klvm-utils-fuzz"
-version = "0.6.0"
+version = "0.8.0"
 dependencies = [
- "chik-consensus",
  "chik-fuzz",
  "klvm-traits",
  "klvm-utils",
  "klvmr",
  "libfuzzer-sys",
 ]
 
 [[package]]
 name = "klvmr"
-version = "0.6.1"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22cf3a3ac2edf86a94974b94056cedaee92be3b6b0fc2c0ab1afaafb96bf9a4c"
+checksum = "9637930ee2c56fb327289c00922f52963b2d3804a2209c68cdb1db2fb2800934"
 dependencies = [
  "chik-bls 0.4.0",
  "hex-literal",
  "k256",
  "lazy_static",
  "num-bigint",
  "num-integer",
@@ -1331,17 +1307,17 @@
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 dependencies = [
  "spin",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.151"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "302d7ab3130588088d277783b1e2d2e10c9e9e4a16dd9050e6ec93fb3e7048f4"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libfuzzer-sys"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a96cfd5557eb82f2b83fed4955246c988d331975a002961b07c81584d107e7f7"
 dependencies = [
@@ -1364,61 +1340,64 @@
 dependencies = [
  "cc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
-name = "linux-raw-sys"
-version = "0.4.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4cd1a83af159aa67994778be9070f0ae1bd732942279cabb14f86f986a21456"
-
-[[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
+
+[[package]]
+name = "lru"
+version = "0.12.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3262e75e648fce39813cb56ac41f3c3e3f65217ebf3844d818d1f9398cfb0dc"
+dependencies = [
+ "hashbrown",
+]
 
 [[package]]
 name = "memchr"
-version = "2.6.4"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -1438,17 +1417,17 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
@@ -1465,39 +1444,44 @@
  "num-traits",
  "rand",
  "smallvec",
  "zeroize",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.43"
+version = "0.1.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
+checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -1507,17 +1491,17 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "oid-registry"
 version = "0.6.1"
@@ -1581,17 +1565,17 @@
 checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "pem"
-version = "3.0.2"
+version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3163d2912b7c3b52d651a055f2c7eec9ba5cd22d26ef75b8dd3a59980b185923"
+checksum = "8e459365e590736a54c3fa561947c84837534b8e9af6fc5bf781307e82658fae"
 dependencies = [
  "base64",
  "serde",
 ]
 
 [[package]]
 name = "pem-rfc7468"
@@ -1606,17 +1590,17 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1639,17 +1623,17 @@
 dependencies = [
  "der",
  "spki",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.27"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "plotters"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
 dependencies = [
@@ -1704,17 +1688,17 @@
 dependencies = [
  "once_cell",
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.70"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39278fbbf5fb4f646ce651690877f89d1c5811a3d4acb27700c1cb3cdb78fd3b"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.0"
@@ -1775,17 +1759,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1814,27 +1798,27 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.8.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c27db03db7734835b3f53954b534c91069375ce6ccaa2e065441e07d9b6cdb1"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.12.0"
+version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ce3fb6ad83f861aac485e76e1985cd109d9a3713802152be56c3b1f0e0658ed"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "rcgen"
@@ -1856,40 +1840,40 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rfc6979"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8dd2a808d456c4a54e300a23e9f5a67e122c3024119acbfd73e3bf664491cb2"
 dependencies = [
@@ -1986,15 +1970,15 @@
 
 [[package]]
 name = "rusqlite"
 version = "0.30.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a78046161564f5e7cd9008aff3b2990b3850dc8e0349119b98e8f251e099f24d"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "fallible-iterator",
  "fallible-streaming-iterator",
  "hashlink",
  "libsqlite3-sys",
  "smallvec",
 ]
 
@@ -2025,48 +2009,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "faf0c4a6ece9950b9abdb62b1cfcf2a68b3b67a10ba445b3bb85be2a293d0632"
 dependencies = [
  "nom",
 ]
 
 [[package]]
-name = "rustix"
-version = "0.38.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72e572a5e8ca657d7366229cdde4bd14c4eb5499a9573d4d366fe1b599daa316"
-dependencies = [
- "bitflags 2.4.1",
- "errno",
- "libc",
- "linux-raw-sys",
- "windows-sys 0.52.0",
-]
-
-[[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "scoped-tls"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1cf6437eb19a8f4a6cc0f7dca544973b0b78843adbfeb3683d1a94a0024a294"
-
-[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "sec1"
@@ -2080,43 +2045,43 @@
  "pkcs8",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.20"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "836fa6a3e1e547f9a2c4040802ec865b5d85f4014efe00555d7090a3dcaa1090"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.193"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25dd9975e68d0cb5aa1120c288333fc98731bd1dd12f561e468ea4728c042b89"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.193"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43576ca501357b9b071ac53cdc7da8ef0cbd9493d8df094cd821777ea6e894d3"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.108"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1c7e3eac408d115102c4c24ad393e0821bb3a5df4d506a80f85f7a742a526b"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2158,26 +2123,26 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
@@ -2190,17 +2155,17 @@
 dependencies = [
  "base64ct",
  "der",
 ]
 
 [[package]]
 name = "strsim"
-version = "0.10.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
@@ -2213,17 +2178,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.40"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13fa70a4ee923979ffb522cacce59d34421ebdea5625e1073c4326ef9d2dd42e"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2236,17 +2201,17 @@
  "quote",
  "syn 1.0.109",
  "unicode-xid",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.12"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "term"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2077e54d38055cf1ca0fd7933a2e00cd3ec8f6fed352b2a377f06dcdaaf3281"
 dependencies = [
@@ -2262,67 +2227,69 @@
 dependencies = [
  "getopts",
  "term",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.50"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a7210f5c9a7156bb50aa36aed4c95afb51df0df00713949448cf9e97d382d2"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.50"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266b2e40bc00e5a6c09c3584011e08b06f123c00362c92b975ba9843aaaa14b8"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "threadpool"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
 dependencies = [
  "num_cpus",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.30"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4a34ab300f2dee6e562c10a046fc05e358b29f9bf92277f30c3c8d82275f6f5"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
+ "num-conv",
  "powerfmt",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.15"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ad70d68dba9e1f8aceda7aa6711965dfec1cac869f311a51bd08b3a2ccbce20"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
+ "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tiny-bip39"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2364,17 +2331,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.35.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "841d45b238a16291a4e1584e61820b8ae57d696cc5015c459c229ccc6990cc1c"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "pin-project-lite",
  "socket2",
@@ -2433,38 +2400,38 @@
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.14"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f2528f27a9eb2b21e69c95319b30bd0efd85d09c379741b0f78ea1d86be2416"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
@@ -2513,17 +2480,17 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
@@ -2548,31 +2515,19 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
-name = "wasm-bindgen-futures"
-version = "0.4.37"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
-dependencies = [
- "cfg-if",
- "js-sys",
- "wasm-bindgen",
- "web-sys",
-]
-
-[[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
@@ -2582,50 +2537,26 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
-name = "wasm-bindgen-test"
-version = "0.3.37"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e6e302a7ea94f83a6d09e78e7dc7d9ca7b186bc2829c24a22d0753efd680671"
-dependencies = [
- "console_error_panic_hook",
- "js-sys",
- "scoped-tls",
- "wasm-bindgen",
- "wasm-bindgen-futures",
- "wasm-bindgen-test-macro",
-]
-
-[[package]]
-name = "wasm-bindgen-test-macro"
-version = "0.3.37"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecb993dd8c836930ed130e020e77d9b2e65dd0fbab1b67c790b0f5d80b11a575"
-dependencies = [
- "proc-macro2",
- "quote",
-]
-
-[[package]]
 name = "web-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
@@ -2657,19 +2588,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi 0.3.9",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
@@ -2685,15 +2616,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2705,116 +2636,123 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.5.26"
+version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b67b5f0a4e7a27a64c651977932b9dc5667ca7fc31ac44b03ed37a0cf42fdfff"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "x509-parser"
 version = "0.15.1"
@@ -2840,30 +2778,30 @@
 checksum = "e17bb3549cc1321ae1296b9cdc2698e2b6cb1992adfa19a8c72e5b7a738f44cd"
 dependencies = [
  "time",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.31"
+version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c4061bedbb353041c12f413700357bec76df2c7e2ca8e4df8bac24c6bf68e3d"
+checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.31"
+version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3c129550b3e6de3fd0ba67ba5c81818f9805e58b8d7fee80a3a59d2c9fc601a"
+checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
@@ -2875,22 +2813,22 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.40",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.12.3+zstd.1.5.2"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
+checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
 version = "6.0.6"
@@ -2899,14 +2837,14 @@
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `chik_rs-0.7.0/Cargo.toml` & `chik_rs-0.8.0/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["wheel"]
 
 [package]
 name = "chik"
-version = "0.7.0"
+version = "0.8.0"
 edition = "2021"
 license = "Apache-2.0"
 description = "A meta-crate that exports all of the Chik crates in the workspace."
 authors = [
     "Richard Kiss <him@richardkiss.com>",
     "Arvid Norberg <arvid@chiknetwork.com>",
     "Brandon Haggstrom <b.haggstrom@chiknetwork.com>"
@@ -19,39 +19,39 @@
 default = [
     "bls",
     "client",
     "consensus",
     "protocol",
     "ssl",
     "traits",
-    "wallet",
+    "puzzles",
     "klvm-traits",
     "klvm-utils"
 ]
 
 bls = ["dep:chik-bls"]
 client = ["dep:chik-client"]
 consensus = ["dep:chik-consensus"]
 protocol = ["dep:chik-protocol"]
 ssl = ["dep:chik-ssl"]
 traits = ["dep:chik-traits"]
-wallet = ["dep:chik-wallet"]
+puzzles = ["dep:chik-puzzles"]
 klvm-traits = ["dep:klvm-traits"]
 klvm-utils = ["dep:klvm-utils"]
 
 [dependencies]
-chik-bls = { path = "./crates/chik-bls", version = "0.7.0", optional = true }
-chik-client = { path = "./crates/chik-client", version = "0.7.0", optional = true }
-chik-consensus = { path = "./crates/chik-consensus", version = "0.7.0", optional = true }
-chik-protocol = { path = "./crates/chik-protocol", version = "0.7.0", optional = true }
+chik-bls = { path = "./crates/chik-bls", version = "0.8.0", optional = true }
+chik-client = { path = "./crates/chik-client", version = "0.8.0", optional = true }
+chik-consensus = { path = "./crates/chik-consensus", version = "0.8.0", optional = true }
+chik-protocol = { path = "./crates/chik-protocol", version = "0.8.0", optional = true }
 chik-ssl = { path = "./crates/chik-ssl", version = "0.7.0", optional = true }
-chik-traits = { path = "./crates/chik-traits", version = "0.7.0", optional = true }
-chik-wallet = { path = "./crates/chik-wallet", version = "0.7.0", optional = true }
-klvm-traits = { path = "./crates/klvm-traits", version = "0.7.0", optional = true }
-klvm-utils = { path = "./crates/klvm-utils", version = "0.7.0", optional = true }
+chik-traits = { path = "./crates/chik-traits", version = "0.8.0", optional = true }
+chik-puzzles = { path = "./crates/chik-puzzles", version = "0.8.0", optional = true }
+klvm-traits = { path = "./crates/klvm-traits", version = "0.8.0", optional = true }
+klvm-utils = { path = "./crates/klvm-utils", version = "0.8.0", optional = true }
 
 [profile.release]
 lto = "thin"
 
 # This is also necessary in `wheel/Cargo.toml` to make sure the `wheel` crate builds as well.
 # Pin the `blst` dependency to the correct revision, since the fix has not been properly released yet.
 [patch.crates-io]
```

### Comparing `chik_rs-0.7.0/python/chik_rs/struct_stream.py` & `chik_rs-0.8.0/python/chik_rs/struct_stream.py`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/python/chik_rs/sized_ints.py` & `chik_rs-0.8.0/python/chik_rs/sized_ints.py`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/python/chik_rs/sized_byte_class.py` & `chik_rs-0.8.0/python/chik_rs/sized_byte_class.py`

 * *Files identical despite different names*

### Comparing `chik_rs-0.7.0/python/chik_rs/chik_rs.pyi` & `chik_rs-0.8.0/python/chik_rs/chik_rs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,20 @@
     pair: Optional[Tuple[LazyNode, LazyNode]]
     atom: Optional[bytes]
 
 def serialized_length(program: ReadableBuffer) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
 def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
+class BLSCache:
+    def __init__(self, cache_size: Optional[int] = 50000) -> None: ...
+    def len(self) -> int: ...
+    def aggregate_verify(self, pks: List[G1Element], msgs: List[bytes], sig: G2Element) -> bool: ...
+    
+
 class AugSchemeMPL:
     @staticmethod
     def sign(pk: PrivateKey, msg: bytes, prepend_pk: Optional[G1Element] = None) -> G2Element: ...
     @staticmethod
     def aggregate(sigs: Sequence[G2Element]) -> G2Element: ...
     @staticmethod
     def verify(pk: G1Element, msg: bytes, sig: G2Element) -> bool: ...
@@ -234,42 +240,42 @@
     height_relative: Optional[int]
     seconds_relative: Optional[int]
     before_height_relative: Optional[int]
     before_seconds_relative: Optional[int]
     birth_height: Optional[int]
     birth_seconds: Optional[int]
     create_coin: List[Tuple[bytes, int, Optional[bytes]]]
-    agg_sig_me: List[Tuple[bytes, bytes]]
-    agg_sig_parent: List[Tuple[bytes, bytes]]
-    agg_sig_puzzle: List[Tuple[bytes, bytes]]
-    agg_sig_amount: List[Tuple[bytes, bytes]]
-    agg_sig_puzzle_amount: List[Tuple[bytes, bytes]]
-    agg_sig_parent_amount: List[Tuple[bytes, bytes]]
-    agg_sig_parent_puzzle: List[Tuple[bytes, bytes]]
+    agg_sig_me: List[Tuple[G1Element, bytes]]
+    agg_sig_parent: List[Tuple[G1Element, bytes]]
+    agg_sig_puzzle: List[Tuple[G1Element, bytes]]
+    agg_sig_amount: List[Tuple[G1Element, bytes]]
+    agg_sig_puzzle_amount: List[Tuple[G1Element, bytes]]
+    agg_sig_parent_amount: List[Tuple[G1Element, bytes]]
+    agg_sig_parent_puzzle: List[Tuple[G1Element, bytes]]
     flags: int
     def __init__(
         self,
         coin_id: bytes,
         parent_id: bytes,
         puzzle_hash: bytes,
         coin_amount: int,
         height_relative: Optional[int],
         seconds_relative: Optional[int],
         before_height_relative: Optional[int],
         before_seconds_relative: Optional[int],
         birth_height: Optional[int],
         birth_seconds: Optional[int],
         create_coin: Sequence[Tuple[bytes, int, Optional[bytes]]],
-        agg_sig_me: Sequence[Tuple[bytes, bytes]],
-        agg_sig_parent: Sequence[Tuple[bytes, bytes]],
-        agg_sig_puzzle: Sequence[Tuple[bytes, bytes]],
-        agg_sig_amount: Sequence[Tuple[bytes, bytes]],
-        agg_sig_puzzle_amount: Sequence[Tuple[bytes, bytes]],
-        agg_sig_parent_amount: Sequence[Tuple[bytes, bytes]],
-        agg_sig_parent_puzzle: Sequence[Tuple[bytes, bytes]],
+        agg_sig_me: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_parent: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_puzzle: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_amount: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_puzzle_amount: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_parent_amount: Sequence[Tuple[G1Element, bytes]],
+        agg_sig_parent_puzzle: Sequence[Tuple[G1Element, bytes]],
         flags: int
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> Spend: ...
     def __copy__(self) -> Spend: ...
@@ -293,43 +299,43 @@
         height_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         seconds_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         before_height_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         before_seconds_relative: Union[ Optional[int], _Unspec] = _Unspec(),
         birth_height: Union[ Optional[int], _Unspec] = _Unspec(),
         birth_seconds: Union[ Optional[int], _Unspec] = _Unspec(),
         create_coin: Union[ List[Tuple[bytes, int, Optional[bytes]]], _Unspec] = _Unspec(),
-        agg_sig_me: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_parent: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_puzzle: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_amount: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_puzzle_amount: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_parent_amount: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
-        agg_sig_parent_puzzle: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
+        agg_sig_me: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_parent: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_puzzle: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_amount: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_puzzle_amount: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_parent_amount: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
+        agg_sig_parent_puzzle: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
         flags: Union[ int, _Unspec] = _Unspec()) -> Spend: ...
 
 class SpendBundleConditions:
     spends: List[Spend]
     reserve_fee: int
     height_absolute: int
     seconds_absolute: int
     before_height_absolute: Optional[int]
     before_seconds_absolute: Optional[int]
-    agg_sig_unsafe: List[Tuple[bytes, bytes]]
+    agg_sig_unsafe: List[Tuple[G1Element, bytes]]
     cost: int
     removal_amount: int
     addition_amount: int
     def __init__(
         self,
         spends: Sequence[Spend],
         reserve_fee: int,
         height_absolute: int,
         seconds_absolute: int,
         before_height_absolute: Optional[int],
         before_seconds_absolute: Optional[int],
-        agg_sig_unsafe: Sequence[Tuple[bytes, bytes]],
+        agg_sig_unsafe: Sequence[Tuple[G1Element, bytes]],
         cost: int,
         removal_amount: int,
         addition_amount: int
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
@@ -350,15 +356,15 @@
     def from_json_dict(json_dict: Any) -> SpendBundleConditions: ...
     def replace(self, *, spends: Union[ List[Spend], _Unspec] = _Unspec(),
         reserve_fee: Union[ int, _Unspec] = _Unspec(),
         height_absolute: Union[ int, _Unspec] = _Unspec(),
         seconds_absolute: Union[ int, _Unspec] = _Unspec(),
         before_height_absolute: Union[ Optional[int], _Unspec] = _Unspec(),
         before_seconds_absolute: Union[ Optional[int], _Unspec] = _Unspec(),
-        agg_sig_unsafe: Union[ List[Tuple[bytes, bytes]], _Unspec] = _Unspec(),
+        agg_sig_unsafe: Union[ List[Tuple[G1Element, bytes]], _Unspec] = _Unspec(),
         cost: Union[ int, _Unspec] = _Unspec(),
         removal_amount: Union[ int, _Unspec] = _Unspec(),
         addition_amount: Union[ int, _Unspec] = _Unspec()) -> SpendBundleConditions: ...
 
 class BlockRecord:
     header_hash: bytes32
     prev_hash: bytes32
@@ -1692,14 +1698,72 @@
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
     def to_json_dict(self) -> Any: ...
     @staticmethod
     def from_json_dict(json_dict: Any) -> RespondPeers: ...
     def replace(self, *, peer_list: Union[ List[TimestampedPeerInfo], _Unspec] = _Unspec()) -> RespondPeers: ...
 
+class NewUnfinishedBlock2:
+    unfinished_reward_hash: bytes32
+    foliage_hash: Optional[bytes32]
+    def __init__(
+        self,
+        unfinished_reward_hash: bytes,
+        foliage_hash: Optional[bytes32]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> NewUnfinishedBlock2: ...
+    def __copy__(self) -> NewUnfinishedBlock2: ...
+    @staticmethod
+    def from_bytes(bytes) -> NewUnfinishedBlock2: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> NewUnfinishedBlock2: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[NewUnfinishedBlock2, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> NewUnfinishedBlock2: ...
+    def replace(self, *, unfinished_reward_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        foliage_hash: Union[ Optional[bytes32], _Unspec] = _Unspec()) -> NewUnfinishedBlock2: ...
+
+class RequestUnfinishedBlock2:
+    unfinished_reward_hash: bytes32
+    foliage_hash: Optional[bytes32]
+    def __init__(
+        self,
+        unfinished_reward_hash: bytes,
+        foliage_hash: Optional[bytes32]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestUnfinishedBlock2: ...
+    def __copy__(self) -> RequestUnfinishedBlock2: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestUnfinishedBlock2: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestUnfinishedBlock2: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestUnfinishedBlock2, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestUnfinishedBlock2: ...
+    def replace(self, *, unfinished_reward_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        foliage_hash: Union[ Optional[bytes32], _Unspec] = _Unspec()) -> RequestUnfinishedBlock2: ...
+
 class FullBlock:
     finished_sub_slots: List[EndOfSubSlotBundle]
     reward_chain_block: RewardChainBlock
     challenge_chain_sp_proof: Optional[VDFProof]
     challenge_chain_ip_proof: VDFProof
     reward_chain_sp_proof: Optional[VDFProof]
     reward_chain_ip_proof: VDFProof
@@ -2380,14 +2444,17 @@
     finished_sub_slots: List[EndOfSubSlotBundle]
     reward_chain_block: RewardChainBlockUnfinished
     challenge_chain_sp_proof: Optional[VDFProof]
     reward_chain_sp_proof: Optional[VDFProof]
     foliage: Foliage
     foliage_transaction_block: Optional[FoliageTransactionBlock]
     transactions_filter: bytes
+    prev_header_hash: bytes32
+    header_hash: bytes32
+    total_iters: uint128
     def __init__(
         self,
         finished_sub_slots: Sequence[EndOfSubSlotBundle],
         reward_chain_block: RewardChainBlockUnfinished,
         challenge_chain_sp_proof: Optional[VDFProof],
         reward_chain_sp_proof: Optional[VDFProof],
         foliage: Foliage,
@@ -3464,14 +3531,345 @@
     def stream_to_bytes(self) -> bytes: ...
     def get_hash(self) -> bytes32: ...
     def to_json_dict(self) -> Any: ...
     @staticmethod
     def from_json_dict(json_dict: Any) -> RespondFeeEstimates: ...
     def replace(self, *, estimates: Union[ FeeEstimateGroup, _Unspec] = _Unspec()) -> RespondFeeEstimates: ...
 
+class RequestRemovePuzzleSubscriptions:
+    puzzle_hashes: Optional[List[bytes32]]
+    def __init__(
+        self,
+        puzzle_hashes: Optional[Sequence[bytes32]]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestRemovePuzzleSubscriptions: ...
+    def __copy__(self) -> RequestRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestRemovePuzzleSubscriptions, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestRemovePuzzleSubscriptions: ...
+    def replace(self, *, puzzle_hashes: Union[ Optional[List[bytes32]], _Unspec] = _Unspec()) -> RequestRemovePuzzleSubscriptions: ...
+
+class RespondRemovePuzzleSubscriptions:
+    puzzle_hashes: List[bytes32]
+    def __init__(
+        self,
+        puzzle_hashes: Sequence[bytes32]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RespondRemovePuzzleSubscriptions: ...
+    def __copy__(self) -> RespondRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def from_bytes(bytes) -> RespondRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RespondRemovePuzzleSubscriptions: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondRemovePuzzleSubscriptions, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RespondRemovePuzzleSubscriptions: ...
+    def replace(self, *, puzzle_hashes: Union[ List[bytes32], _Unspec] = _Unspec()) -> RespondRemovePuzzleSubscriptions: ...
+
+class RequestRemoveCoinSubscriptions:
+    coin_ids: Optional[List[bytes32]]
+    def __init__(
+        self,
+        coin_ids: Optional[Sequence[bytes32]]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestRemoveCoinSubscriptions: ...
+    def __copy__(self) -> RequestRemoveCoinSubscriptions: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestRemoveCoinSubscriptions: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestRemoveCoinSubscriptions: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestRemoveCoinSubscriptions, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestRemoveCoinSubscriptions: ...
+    def replace(self, *, coin_ids: Union[ Optional[List[bytes32]], _Unspec] = _Unspec()) -> RequestRemoveCoinSubscriptions: ...
+
+class RespondRemoveCoinSubscriptions:
+    coin_ids: List[bytes32]
+    def __init__(
+        self,
+        coin_ids: Sequence[bytes32]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RespondRemoveCoinSubscriptions: ...
+    def __copy__(self) -> RespondRemoveCoinSubscriptions: ...
+    @staticmethod
+    def from_bytes(bytes) -> RespondRemoveCoinSubscriptions: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RespondRemoveCoinSubscriptions: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondRemoveCoinSubscriptions, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RespondRemoveCoinSubscriptions: ...
+    def replace(self, *, coin_ids: Union[ List[bytes32], _Unspec] = _Unspec()) -> RespondRemoveCoinSubscriptions: ...
+
+class CoinStateFilters:
+    include_spent: bool
+    include_unspent: bool
+    include_hinted: bool
+    min_amount: uint64
+    def __init__(
+        self,
+        include_spent: bool,
+        include_unspent: bool,
+        include_hinted: bool,
+        min_amount: uint64
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> CoinStateFilters: ...
+    def __copy__(self) -> CoinStateFilters: ...
+    @staticmethod
+    def from_bytes(bytes) -> CoinStateFilters: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> CoinStateFilters: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[CoinStateFilters, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> CoinStateFilters: ...
+    def replace(self, *, include_spent: Union[ bool, _Unspec] = _Unspec(),
+        include_unspent: Union[ bool, _Unspec] = _Unspec(),
+        include_hinted: Union[ bool, _Unspec] = _Unspec(),
+        min_amount: Union[ uint64, _Unspec] = _Unspec()) -> CoinStateFilters: ...
+
+class RequestPuzzleState:
+    puzzle_hashes: List[bytes32]
+    previous_height: Optional[uint32]
+    header_hash: bytes32
+    filters: CoinStateFilters
+    subscribe_when_finished: bool
+    def __init__(
+        self,
+        puzzle_hashes: Sequence[bytes32],
+        previous_height: Optional[uint32],
+        header_hash: bytes,
+        filters: CoinStateFilters,
+        subscribe_when_finished: bool
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestPuzzleState: ...
+    def __copy__(self) -> RequestPuzzleState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestPuzzleState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestPuzzleState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestPuzzleState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestPuzzleState: ...
+    def replace(self, *, puzzle_hashes: Union[ List[bytes32], _Unspec] = _Unspec(),
+        previous_height: Union[ Optional[uint32], _Unspec] = _Unspec(),
+        header_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        filters: Union[ CoinStateFilters, _Unspec] = _Unspec(),
+        subscribe_when_finished: Union[ bool, _Unspec] = _Unspec()) -> RequestPuzzleState: ...
+
+class RespondPuzzleState:
+    puzzle_hashes: List[bytes32]
+    height: uint32
+    header_hash: bytes32
+    is_finished: bool
+    coin_states: List[CoinState]
+    def __init__(
+        self,
+        puzzle_hashes: Sequence[bytes32],
+        height: uint32,
+        header_hash: bytes,
+        is_finished: bool,
+        coin_states: Sequence[CoinState]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RespondPuzzleState: ...
+    def __copy__(self) -> RespondPuzzleState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RespondPuzzleState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RespondPuzzleState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondPuzzleState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RespondPuzzleState: ...
+    def replace(self, *, puzzle_hashes: Union[ List[bytes32], _Unspec] = _Unspec(),
+        height: Union[ uint32, _Unspec] = _Unspec(),
+        header_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        is_finished: Union[ bool, _Unspec] = _Unspec(),
+        coin_states: Union[ List[CoinState], _Unspec] = _Unspec()) -> RespondPuzzleState: ...
+
+class RejectPuzzleState:
+    reason: int
+    def __init__(
+        self,
+        reason: int
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RejectPuzzleState: ...
+    def __copy__(self) -> RejectPuzzleState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RejectPuzzleState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RejectPuzzleState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectPuzzleState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RejectPuzzleState: ...
+    def replace(self, *, reason: Union[ int, _Unspec] = _Unspec()) -> RejectPuzzleState: ...
+
+class RequestCoinState:
+    coin_ids: List[bytes32]
+    previous_height: Optional[uint32]
+    header_hash: bytes32
+    subscribe: bool
+    def __init__(
+        self,
+        coin_ids: Sequence[bytes32],
+        previous_height: Optional[uint32],
+        header_hash: bytes,
+        subscribe: bool
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RequestCoinState: ...
+    def __copy__(self) -> RequestCoinState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RequestCoinState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RequestCoinState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RequestCoinState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RequestCoinState: ...
+    def replace(self, *, coin_ids: Union[ List[bytes32], _Unspec] = _Unspec(),
+        previous_height: Union[ Optional[uint32], _Unspec] = _Unspec(),
+        header_hash: Union[ bytes32, _Unspec] = _Unspec(),
+        subscribe: Union[ bool, _Unspec] = _Unspec()) -> RequestCoinState: ...
+
+class RespondCoinState:
+    coin_ids: List[bytes32]
+    coin_states: List[CoinState]
+    def __init__(
+        self,
+        coin_ids: Sequence[bytes32],
+        coin_states: Sequence[CoinState]
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RespondCoinState: ...
+    def __copy__(self) -> RespondCoinState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RespondCoinState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RespondCoinState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RespondCoinState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RespondCoinState: ...
+    def replace(self, *, coin_ids: Union[ List[bytes32], _Unspec] = _Unspec(),
+        coin_states: Union[ List[CoinState], _Unspec] = _Unspec()) -> RespondCoinState: ...
+
+class RejectCoinState:
+    reason: int
+    def __init__(
+        self,
+        reason: int
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __richcmp__(self) -> Any: ...
+    def __deepcopy__(self) -> RejectCoinState: ...
+    def __copy__(self) -> RejectCoinState: ...
+    @staticmethod
+    def from_bytes(bytes) -> RejectCoinState: ...
+    @staticmethod
+    def from_bytes_unchecked(bytes) -> RejectCoinState: ...
+    @staticmethod
+    def parse_rust(ReadableBuffer, bool = False) -> Tuple[RejectCoinState, int]: ...
+    def to_bytes(self) -> bytes: ...
+    def __bytes__(self) -> bytes: ...
+    def stream_to_bytes(self) -> bytes: ...
+    def get_hash(self) -> bytes32: ...
+    def to_json_dict(self) -> Any: ...
+    @staticmethod
+    def from_json_dict(json_dict: Any) -> RejectCoinState: ...
+    def replace(self, *, reason: Union[ int, _Unspec] = _Unspec()) -> RejectCoinState: ...
+
 class SubEpochData:
     reward_chain_hash: bytes32
     num_blocks_overflow: uint8
     new_sub_slot_iters: Optional[uint64]
     new_difficulty: Optional[uint64]
     def __init__(
         self,
```

