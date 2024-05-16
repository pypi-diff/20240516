# Comparing `tmp/vyper-0.4.0rc3.tar.gz` & `tmp/vyper-0.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vyper-0.4.0rc3.tar", last modified: Wed May  8 16:11:14 2024, max compression
+gzip compressed data, was "vyper-0.4.0rc4.tar", last modified: Wed May 15 17:17:56 2024, max compression
```

## Comparing `vyper-0.4.0rc3.tar` & `vyper-0.4.0rc4.tar`

### file list

```diff
@@ -1,606 +1,607 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.832811 vyper-0.4.0rc3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.832811 vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/vip.md
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.832811 vyper-0.4.0rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/era-tester.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/ghcr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/release-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-08 16:11:14.904812 vyper-0.4.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/built-in-functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/compiler-exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/compiling-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/constants-and-vars.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/control-structures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/deploying-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/event-logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/installing-vyper.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/natspec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/scoping-and-declarations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/statements.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/structure-of-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/style-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/testing-contracts-brownie.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/testing-contracts-ethtester.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/testing-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/vyper-by-example.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/auctions/blind_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/auctions/simple_open_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/crowdfund.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/factory/Exchange.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/factory/Factory.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/market_maker/on_chain_market_maker.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/name_registry/name_registry.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/safe_remote_purchase/safe_remote_purchase.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/stock/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/stock/company.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/storage/advanced_storage.vy
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/storage/storage.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/tokens/ERC1155ownable.vy
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/tokens/ERC20.vy
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/tokens/ERC4626.vy
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/tokens/ERC721.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/voting/ballot.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/wallet/wallet.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/hooks/build
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/make.cmd
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/quicktest.sh
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-08 16:11:14.904812 vyper-0.4.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/tests/evm_backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/abi_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/base_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/pyevm_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/revm_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.824812 vyper-0.4.0rc3/tests/functional/builtins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.844812 vyper-0.4.0rc3/tests/functional/builtins/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_addmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_blobhash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)    20237 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_create_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ecrecover.py
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_is_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)    16628 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)    14884 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_unsafe_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.848812 vyper-0.4.0rc3/tests/functional/builtins/folding/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_addmod_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_floor_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_fold_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_keccak_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_powmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.848812 vyper-0.4.0rc3/tests/functional/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.848812 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_default_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_default_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_erc20_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    57029 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_self_call_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.848812 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_blobbasefee.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_block_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_blockhash.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.852812 vyper-0.4.0rc3/tests/functional/codegen/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.852812 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_private.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_pure.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.856812 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_break.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_for_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_range_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_address_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_assert_unreachable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_bytes_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_clampers.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_internal_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    27866 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_logging_bytes_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_logging_from_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_memory_alloc.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_memory_dealloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_reverting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_short_circuiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_string_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_transient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.856812 vyper-0.4.0rc3/tests/functional/codegen/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/integration/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/integration/test_crowdfund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/integration/test_escrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.856812 vyper-0.4.0rc3/tests/functional/codegen/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_flag_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_interface_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_module_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_module_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_stateless_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.856812 vyper-0.4.0rc3/tests/functional/codegen/storage_variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_setters.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_storage_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/test_call_graph_stability.py
--rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/test_selector_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/test_selector_table_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/codegen/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_decimals.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_division.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_exponents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_isqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_modulo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_signed_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_sqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_unsigned_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_array_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes_zero_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    48925 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_identifier_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    23216 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_node_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.824812 vyper-0.4.0rc3/tests/functional/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/auctions/test_blind_auction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/auctions/test_simple_open_auction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/company/
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/company/test_company.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/crowdfund/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/crowdfund/test_crowdfund_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/factory/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/market_maker/test_on_chain_market_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/name_registry/test_name_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/storage/test_advanced_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/storage/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.864812 vyper-0.4.0rc3/tests/functional/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc4626.py
--rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.864812 vyper-0.4.0rc3/tests/functional/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/voting/test_ballot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.864812 vyper-0.4.0rc3/tests/functional/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/wallet/test_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.864812 vyper-0.4.0rc3/tests/functional/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/grammar/test_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.872812 vyper-0.4.0rc3/tests/functional/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.872812 vyper-0.4.0rc3/tests/functional/syntax/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_argument_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_call_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_constancy_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_function_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_instantiation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_type_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_namespace_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_overflow_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_structure_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_syntax_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_undeclared_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.872812 vyper-0.4.0rc3/tests/functional/syntax/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/test_deploy_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/test_implements.py
--rw-r--r--   0 runner    (1001) docker     (127)    28241 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/test_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/functional/syntax/names/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/names/test_event_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/names/test_function_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/names/test_variable_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/functional/syntax/signatures/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/signatures/test_invalid_function_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/signatures/test_method_id_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_addmulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_address_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_ann_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_as_uint256.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_blockscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_bool_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_chainid.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_code_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_codehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_create_with_code_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_external_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_functions_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_immutables.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_invalids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_msg_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_nested_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_no_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_powmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_return_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_self_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_selfdestruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_tuple_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_unbalanced_return.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/abi_types/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/abi_types/test_invalid_abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/ast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/ast/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_compare_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_binop_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_binop_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_boolop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_unaryop.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_from_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_get_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_get_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_annotate_and_optimize_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_ast_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_metadata_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_source_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.824812 vyper-0.4.0rc3/tests/unit/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/cli/storage_layout/
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/storage_layout/test_storage_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/cli/vyper_compile/
--rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_compile/test_compile_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_compile/test_parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/cli/vyper_json/
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_compile_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_get_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_get_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_output_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/compiler/asm/
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/asm/test_asm_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/compiler/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_calldatacopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_optimize_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_repeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_with.py
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_bytecode_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_compile_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8697 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_sha3_32.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_source_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/compiler/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_convert_basicblock_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_dominator_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_duplicate_operands.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_liveness_simple_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_multi_entry_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_sccp.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_stack_at_external_return.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/tests/unit/semantics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/tests/unit/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/analysis/test_array_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/analysis/test_cyclic_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/analysis/test_for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/analysis/test_potential_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/test_storage_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/tests/unit/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_pure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_size_in_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_type_from_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_type_from_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/utils/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/vyper/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.888812 vyper-0.4.0rc3/vyper/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/grammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.888812 vyper-0.4.0rc3/vyper/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    91585 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.888812 vyper-0.4.0rc3/vyper/builtins/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC165.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC20.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC20Detailed.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC4626.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC721.vyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.888812 vyper-0.4.0rc3/vyper/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/compile_archive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13215 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/vyper_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/vyper_ir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15923 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/vyper_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.892812 vyper-0.4.0rc3/vyper/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/abi_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    42566 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    30724 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/external_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.892812 vyper-0.4.0rc3/vyper/codegen/function_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/function_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/function_definitions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/function_definitions/external_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/function_definitions/internal_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/ir_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/jumptable_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/keccak256_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/memory_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/return_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/self_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.892812 vyper-0.4.0rc3/vyper/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/output_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.892812 vyper-0.4.0rc3/vyper/evm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/evm/address_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/evm/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.896812 vyper-0.4.0rc3/vyper/ir/
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45899 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/s_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.896812 vyper-0.4.0rc3/vyper/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.896812 vyper-0.4.0rc3/vyper/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/constant_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/data_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/global_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/import_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/levenshtein_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37264 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/data_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/bytestrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    30949 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/subscriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/venom/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/dfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/dominators.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/dup_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/liveness.py
--rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/basicblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/ir_node_to_venom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/venom/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/base_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/mem2var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/remove_unused_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/venom/passes/sccp/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/sccp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/sccp/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/sccp/sccp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/simplify_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/stack_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/stack_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/venom_to_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 16:11:11.000000 vyper-0.4.0rc3/vyper/vyper_git_commithash.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21016 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.361787 vyper-0.4.0rc4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.297786 vyper-0.4.0rc4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.297786 vyper-0.4.0rc4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/ISSUE_TEMPLATE/vip.md
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.297786 vyper-0.4.0rc4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/workflows/era-tester.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/workflows/ghcr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-15 17:17:56.361787 vyper-0.4.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.301787 vyper-0.4.0rc4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.301787 vyper-0.4.0rc4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/built-in-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/compiler-exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/compiling-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/constants-and-vars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/control-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/deploying-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/event-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/installing-vyper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/natspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/scoping-and-declarations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/statements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/structure-of-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/style-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/testing-contracts-brownie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/testing-contracts-ethtester.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/testing-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/docs/vyper-by-example.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/auctions/blind_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/auctions/simple_open_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/crowdfund.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/factory/Exchange.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/factory/Factory.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/market_maker/on_chain_market_maker.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/name_registry/name_registry.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/safe_remote_purchase/safe_remote_purchase.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/stock/company.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/storage/advanced_storage.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/storage/storage.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/tokens/ERC1155ownable.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/tokens/ERC20.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/tokens/ERC4626.vy
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/tokens/ERC721.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/voting/ballot.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/examples/wallet/wallet.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/hooks/build
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/make.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/quicktest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 17:17:56.365787 vyper-0.4.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/tests/evm_backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/evm_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/evm_backends/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/evm_backends/abi_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/evm_backends/base_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/evm_backends/pyevm_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/evm_backends/revm_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.305786 vyper-0.4.0rc4/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.289786 vyper-0.4.0rc4/tests/functional/builtins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.309787 vyper-0.4.0rc4/tests/functional/builtins/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_addmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_blobhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20237 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_create_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_ecrecover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_is_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16628 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/codegen/test_unsafe_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.313787 vyper-0.4.0rc4/tests/functional/builtins/folding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_addmod_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_floor_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_fold_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_keccak_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/builtins/folding/test_powmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.313787 vyper-0.4.0rc4/tests/functional/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.313787 vyper-0.4.0rc4/tests/functional/codegen/calling_convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_default_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_default_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_erc20_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57029 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_self_call_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.313787 vyper-0.4.0rc4/tests/functional/codegen/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/environment_variables/test_blobbasefee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/environment_variables/test_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/environment_variables/test_blockhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/environment_variables/test_tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.317787 vyper-0.4.0rc4/tests/functional/codegen/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.317787 vyper-0.4.0rc4/tests/functional/codegen/features/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_pure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.317787 vyper-0.4.0rc4/tests/functional/codegen/features/iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_for_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_range_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_assert_unreachable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_bytes_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_clampers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_internal_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29735 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_logging_bytes_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_logging_from_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_memory_alloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_memory_dealloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_short_circuiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_string_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/features/test_transient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.321787 vyper-0.4.0rc4/tests/functional/codegen/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/integration/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/integration/test_crowdfund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/integration/test_escrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.321787 vyper-0.4.0rc4/tests/functional/codegen/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/test_flag_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/test_interface_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/test_module_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/test_module_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/modules/test_stateless_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.321787 vyper-0.4.0rc4/tests/functional/codegen/storage_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/storage_variables/test_getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/storage_variables/test_setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/storage_variables/test_storage_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/test_call_graph_stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/test_selector_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/test_selector_table_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.321787 vyper-0.4.0rc4/tests/functional/codegen/types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_decimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_exponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_isqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_modulo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_signed_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_unsigned_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_array_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_bytes_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_bytes_zero_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48925 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_identifier_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23216 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_node_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/codegen/types/test_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.293786 vyper-0.4.0rc4/tests/functional/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/auctions/test_blind_auction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/auctions/test_simple_open_auction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/company/
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/company/test_company.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/crowdfund/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/crowdfund/test_crowdfund_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/factory/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/market_maker/test_on_chain_market_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/name_registry/test_name_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/storage/test_advanced_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/storage/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/tokens/test_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/tokens/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/tokens/test_erc4626.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/tokens/test_erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/voting/test_ballot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/examples/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.325787 vyper-0.4.0rc4/tests/functional/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/grammar/test_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.333787 vyper-0.4.0rc4/tests/functional/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.333787 vyper-0.4.0rc4/tests/functional/syntax/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_argument_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_call_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_constancy_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_function_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_instantiation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_invalid_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_invalid_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_invalid_type_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_namespace_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_overflow_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_structure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_syntax_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_undeclared_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.337787 vyper-0.4.0rc4/tests/functional/syntax/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/modules/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/modules/test_deploy_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/modules/test_implements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28823 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/modules/test_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.337787 vyper-0.4.0rc4/tests/functional/syntax/names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/names/test_event_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/names/test_function_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/names/test_variable_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.337787 vyper-0.4.0rc4/tests/functional/syntax/signatures/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/signatures/test_invalid_function_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/signatures/test_method_id_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_addmulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_address_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_ann_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_as_uint256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_blockscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_bool_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_chainid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_code_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_codehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_create_with_code_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_external_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_functions_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_immutables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_invalids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_msg_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_nested_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_no_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_powmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_return_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_self_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_selfdestruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_tuple_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/functional/syntax/test_unbalanced_return.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.337787 vyper-0.4.0rc4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.337787 vyper-0.4.0rc4/tests/unit/abi_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/abi_types/test_invalid_abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.337787 vyper-0.4.0rc4/tests/unit/ast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.337787 vyper-0.4.0rc4/tests/unit/ast/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_compare_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_binop_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_binop_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_boolop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_unaryop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_from_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_get_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_get_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/nodes/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/test_annotate_and_optimize_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/test_ast_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/test_metadata_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/test_natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/ast/test_source_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.293786 vyper-0.4.0rc4/tests/unit/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.341787 vyper-0.4.0rc4/tests/unit/cli/storage_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/storage_layout/test_storage_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.341787 vyper-0.4.0rc4/tests/unit/cli/vyper_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/vyper_compile/test_compile_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/vyper_compile/test_parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.341787 vyper-0.4.0rc4/tests/unit/cli/vyper_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_compile_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_get_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_output_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.341787 vyper-0.4.0rc4/tests/unit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.341787 vyper-0.4.0rc4/tests/unit/compiler/asm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/asm/test_asm_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.341787 vyper-0.4.0rc4/tests/unit/compiler/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/ir/test_calldatacopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/ir/test_compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/ir/test_optimize_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/ir/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/ir/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_bytecode_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_compile_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_sha3_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/test_source_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.345787 vyper-0.4.0rc4/tests/unit/compiler/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_convert_basicblock_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_dominator_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_duplicate_operands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_liveness_simple_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_multi_entry_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_sccp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_stack_at_external_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/compiler/venom/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.345787 vyper-0.4.0rc4/tests/unit/semantics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.345787 vyper-0.4.0rc4/tests/unit/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/analysis/test_array_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/analysis/test_cyclic_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/analysis/test_for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/analysis/test_potential_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/test_storage_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.345787 vyper-0.4.0rc4/tests/unit/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/types/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/types/test_pure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/types/test_size_in_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/types/test_type_from_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/semantics/types/test_type_from_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.345787 vyper-0.4.0rc4/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/unit/utils/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.345787 vyper-0.4.0rc4/vyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.349787 vyper-0.4.0rc4/vyper/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.349787 vyper-0.4.0rc4/vyper/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91509 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.349787 vyper-0.4.0rc4/vyper/builtins/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/interfaces/IERC165.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/interfaces/IERC20.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/interfaces/IERC20Detailed.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/interfaces/IERC4626.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/builtins/interfaces/IERC721.vyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.349787 vyper-0.4.0rc4/vyper/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/cli/compile_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13322 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/cli/vyper_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/cli/vyper_ir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15875 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/cli/vyper_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.353787 vyper-0.4.0rc4/vyper/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/abi_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42566 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30724 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/external_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.353787 vyper-0.4.0rc4/vyper/codegen/function_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/function_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/function_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/function_definitions/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/function_definitions/internal_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/ir_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/jumptable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/keccak256_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/memory_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/return_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/self_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/codegen/stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.353787 vyper-0.4.0rc4/vyper/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/compiler/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/compiler/input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/compiler/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/compiler/output_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12134 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/compiler/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/compiler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/compiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.353787 vyper-0.4.0rc4/vyper/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/evm/address_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/evm/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.357787 vyper-0.4.0rc4/vyper/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45899 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ir/compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ir/optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/ir/s_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.357787 vyper-0.4.0rc4/vyper/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.357787 vyper-0.4.0rc4/vyper/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/constant_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/data_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/global_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/import_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/levenshtein_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37249 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37057 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/data_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.361787 vyper-0.4.0rc4/vyper/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/bytestrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31063 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/subscriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/semantics/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.361787 vyper-0.4.0rc4/vyper/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.361787 vyper-0.4.0rc4/vyper/venom/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/analysis/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/analysis/dfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/analysis/dominators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/analysis/dup_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/analysis/liveness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/basicblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/ir_node_to_venom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.361787 vyper-0.4.0rc4/vyper/venom/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/base_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/mem2var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/remove_unused_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.361787 vyper-0.4.0rc4/vyper/venom/passes/sccp/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/sccp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/sccp/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/sccp/sccp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/simplify_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/stack_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/passes/store_elimination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/stack_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/venom/venom_to_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 17:17:56.000000 vyper-0.4.0rc4/vyper/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 17:17:53.000000 vyper-0.4.0rc4/vyper/vyper_git_commithash.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 17:17:45.000000 vyper-0.4.0rc4/vyper/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:17:56.345787 vyper-0.4.0rc4/vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-15 17:17:56.000000 vyper-0.4.0rc4/vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21056 2024-05-15 17:17:56.000000 vyper-0.4.0rc4/vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:17:56.000000 vyper-0.4.0rc4/vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 17:17:56.000000 vyper-0.4.0rc4/vyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-15 17:17:56.000000 vyper-0.4.0rc4/vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 17:17:56.000000 vyper-0.4.0rc4/vyper.egg-info/top_level.txt
```

### Comparing `vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/bug.md` & `vyper-0.4.0rc4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/vip.md` & `vyper-0.4.0rc4/.github/ISSUE_TEMPLATE/vip.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/.github/workflows/build.yml` & `vyper-0.4.0rc4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/.github/workflows/codeql.yml` & `vyper-0.4.0rc4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/.github/workflows/era-tester.yml` & `vyper-0.4.0rc4/.github/workflows/era-tester.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/.github/workflows/ghcr.yml` & `vyper-0.4.0rc4/.github/workflows/ghcr.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/.github/workflows/pull-request.yaml` & `vyper-0.4.0rc4/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/.github/workflows/release-pypi.yml` & `vyper-0.4.0rc4/.github/workflows/release-pypi.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/.pre-commit-config.yaml` & `vyper-0.4.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/Dockerfile` & `vyper-0.4.0rc4/Dockerfile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/LICENSE` & `vyper-0.4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/Makefile` & `vyper-0.4.0rc4/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/PKG-INFO` & `vyper-0.4.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0rc3
+Version: 0.4.0rc4
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0rc3/README.md` & `vyper-0.4.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/SECURITY.md` & `vyper-0.4.0rc4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/Makefile` & `vyper-0.4.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/_templates/versions.html` & `vyper-0.4.0rc4/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/built-in-functions.rst` & `vyper-0.4.0rc4/docs/built-in-functions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/compiler-exceptions.rst` & `vyper-0.4.0rc4/docs/compiler-exceptions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/compiling-a-contract.rst` & `vyper-0.4.0rc4/docs/compiling-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/conf.py` & `vyper-0.4.0rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/constants-and-vars.rst` & `vyper-0.4.0rc4/docs/constants-and-vars.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/contributing.rst` & `vyper-0.4.0rc4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/control-structures.rst` & `vyper-0.4.0rc4/docs/control-structures.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/deploying-contracts.rst` & `vyper-0.4.0rc4/docs/deploying-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/event-logging.rst` & `vyper-0.4.0rc4/docs/event-logging.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/index.rst` & `vyper-0.4.0rc4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/installing-vyper.rst` & `vyper-0.4.0rc4/docs/installing-vyper.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/interfaces.rst` & `vyper-0.4.0rc4/docs/interfaces.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/logo.svg` & `vyper-0.4.0rc4/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/make.bat` & `vyper-0.4.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/natspec.rst` & `vyper-0.4.0rc4/docs/natspec.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/release-notes.rst` & `vyper-0.4.0rc4/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/resources.rst` & `vyper-0.4.0rc4/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/scoping-and-declarations.rst` & `vyper-0.4.0rc4/docs/scoping-and-declarations.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/statements.rst` & `vyper-0.4.0rc4/docs/statements.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/structure-of-a-contract.rst` & `vyper-0.4.0rc4/docs/structure-of-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/style-guide.rst` & `vyper-0.4.0rc4/docs/style-guide.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/testing-contracts-brownie.rst` & `vyper-0.4.0rc4/docs/testing-contracts-brownie.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/testing-contracts-ethtester.rst` & `vyper-0.4.0rc4/docs/testing-contracts-ethtester.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/testing-contracts.rst` & `vyper-0.4.0rc4/docs/testing-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/toctree.rst` & `vyper-0.4.0rc4/docs/toctree.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/types.rst` & `vyper-0.4.0rc4/docs/types.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/versioning.rst` & `vyper-0.4.0rc4/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/docs/vyper-by-example.rst` & `vyper-0.4.0rc4/docs/vyper-by-example.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/auctions/blind_auction.vy` & `vyper-0.4.0rc4/examples/auctions/blind_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/auctions/simple_open_auction.vy` & `vyper-0.4.0rc4/examples/auctions/simple_open_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/crowdfund.vy` & `vyper-0.4.0rc4/examples/crowdfund.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/factory/Exchange.vy` & `vyper-0.4.0rc4/examples/factory/Exchange.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/factory/Factory.vy` & `vyper-0.4.0rc4/examples/factory/Factory.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/market_maker/on_chain_market_maker.vy` & `vyper-0.4.0rc4/examples/market_maker/on_chain_market_maker.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/safe_remote_purchase/safe_remote_purchase.vy` & `vyper-0.4.0rc4/examples/safe_remote_purchase/safe_remote_purchase.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/stock/company.vy` & `vyper-0.4.0rc4/examples/stock/company.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/tokens/ERC1155ownable.vy` & `vyper-0.4.0rc4/examples/tokens/ERC1155ownable.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/tokens/ERC20.vy` & `vyper-0.4.0rc4/examples/tokens/ERC20.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/tokens/ERC4626.vy` & `vyper-0.4.0rc4/examples/tokens/ERC4626.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/tokens/ERC721.vy` & `vyper-0.4.0rc4/examples/tokens/ERC721.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/voting/ballot.vy` & `vyper-0.4.0rc4/examples/voting/ballot.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/examples/wallet/wallet.vy` & `vyper-0.4.0rc4/examples/wallet/wallet.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/make.cmd` & `vyper-0.4.0rc4/make.cmd`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/setup.cfg` & `vyper-0.4.0rc4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/setup.py` & `vyper-0.4.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/conftest.py` & `vyper-0.4.0rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/evm_backends/abi.py` & `vyper-0.4.0rc4/tests/evm_backends/abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/evm_backends/abi_contract.py` & `vyper-0.4.0rc4/tests/evm_backends/abi_contract.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/evm_backends/base_env.py` & `vyper-0.4.0rc4/tests/evm_backends/base_env.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/evm_backends/pyevm_env.py` & `vyper-0.4.0rc4/tests/evm_backends/pyevm_env.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/evm_backends/revm_env.py` & `vyper-0.4.0rc4/tests/evm_backends/revm_env.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_abi_decode.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_abi_encode.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_addmod.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_addmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_as_wei_value.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_bitwise.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_blobhash.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_blobhash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ceil.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_concat.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_convert.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_create_functions.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_create_functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ec.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_ec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ecrecover.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_ecrecover.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_empty.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_empty.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_extract32.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_floor.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_floor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_is_contract.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_is_contract.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_keccak256.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_length.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_length.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_method_id.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_minmax.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_minmax_value.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_mulmod.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_raw_call.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_send.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_sha256.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_sha256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_slice.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 _draw_1024_1 = st.integers(min_value=1, max_value=1024)
 _bytes_1024 = st.binary(min_size=0, max_size=1024)
 
 
 def _fail_contract(code, opt_level, exceptions):
     settings = Settings(optimize=opt_level)
     with pytest.raises(exceptions):
-        compile_code(code, settings)
+        compile_code(code, settings=settings)
 
 
 @pytest.mark.parametrize("use_literal_start", (True, False))
 @pytest.mark.parametrize("use_literal_length", (True, False))
 @pytest.mark.parametrize("opt_level", list(OptimizationLevel))
 @given(start=_draw_1024, length=_draw_1024, length_bound=_draw_1024_1, bytesdata=_bytes_1024)
 @settings(max_examples=100)
```

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_uint2str.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_uint2str.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_unary.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_unary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_unsafe_math.py` & `vyper-0.4.0rc4/tests/functional/builtins/codegen/test_unsafe_math.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_abs.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_addmod_mulmod.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_addmod_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_bitwise.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_floor_ceil.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_floor_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_fold_as_wei_value.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_fold_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_keccak_sha.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_keccak_sha.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_len.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_min_max.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_min_max.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/builtins/folding/test_powmod.py` & `vyper-0.4.0rc4/tests/functional/builtins/folding/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_default_function.py` & `vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_default_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_default_parameters.py` & `vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_default_parameters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_erc20_abi.py` & `vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_erc20_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_external_contract_calls.py` & `vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py` & `vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_return.py` & `vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_self_call_struct.py` & `vyper-0.4.0rc4/tests/functional/codegen/calling_convention/test_self_call_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_blobbasefee.py` & `vyper-0.4.0rc4/tests/functional/codegen/environment_variables/test_blobbasefee.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_blockhash.py` & `vyper-0.4.0rc4/tests/functional/codegen/environment_variables/test_blockhash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_nonreentrant.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_payable.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_private.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_private.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_public.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_pure.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_pure.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_view.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/decorators/test_view.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_break.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_break.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_continue.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_continue.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_for_in_list.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_for_in_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_for_range.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_range_in.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/iteration/test_range_in.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_assert.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_assert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_assert_unreachable.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_assert_unreachable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_assignment.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_assignment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_bytes_map_keys.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_bytes_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_clampers.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_clampers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_comparison.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_comparison.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_conditionals.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_constructor.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_constructor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_immutable.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_immutable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_init.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_internal_call.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_internal_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_logging.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -743,14 +743,89 @@
     c.ioo(b"moo4")
     ((topics, data),) = get_logs(c, raw=True)
     assert to_text(data) == "moo4"
 
     print("Passed raw log tests")
 
 
+def test_raw_log_topic_double_eval(get_contract, get_logs):
+    t1 = "0x1111111111111111111111111111111111111111111111111111111111111111"
+    code = f"""
+x: bytes32
+c: public(uint256)
+
+@internal
+def bar() -> bytes32:
+    self.c += 1
+    return {t1}
+
+@external
+def foo():
+    self.x = {t1}
+    raw_log([self.bar(), self.bar()], b"")
+
+    """
+
+    c = get_contract(code)
+    c.foo()
+
+    assert c.c() == 2
+
+
+def test_raw_log_with_topics_in_storage_locs(get_contract, get_logs):
+    t1 = "0x1111111111111111111111111111111111111111111111111111111111111111"
+    t2 = "0x2222222222222222222222222222222222222222222222222222222222222222"
+    code = f"""
+x: bytes32
+@external
+def foo():
+    self.x = {t1}
+    raw_log([self.x], b"")
+    y: bytes32 = {t2}
+    raw_log([y], b"")
+    """
+
+    c = get_contract(code)
+    c.foo()
+    logs = get_logs(c, raw=True)
+
+    assert len(logs) == 2
+    assert logs[0][0][0] == int(t1, 16).to_bytes(32, "big")
+    assert logs[1][0][0] == int(t2, 16).to_bytes(32, "big")
+
+
+def test_raw_log_with_topics_in_storage_locs2(get_contract, get_logs):
+    t1 = "0x1111111111111111111111111111111111111111111111111111111111111111"
+    t2 = "0x2222222222222222222222222222222222222222222222222222222222222222"
+    t3 = "0x3333333333333333333333333333333333333333333333333333333333333333"
+    t4 = "0x4444444444444444444444444444444444444444444444444444444444444444"
+    code = f"""
+x: bytes32
+x2: bytes32
+
+@external
+def foo():
+    self.x = {t1}
+    self.x2 = {t2}
+    y: bytes32 = {t3}
+    y2: bytes32 = {t4}
+    raw_log([self.x, y, self.x2, y2], b"")
+
+    raw_log([y, self.x], b"")
+    """
+
+    c = get_contract(code)
+    c.foo()
+    logs = get_logs(c, raw=True)
+
+    assert len(logs) == 2
+    assert logs[0][0] == [int(t, 16).to_bytes(32, "big") for t in [t1, t3, t2, t4]]
+    assert logs[1][0] == [int(t, 16).to_bytes(32, "big") for t in [t3, t1]]
+
+
 def test_raw_call_bytes32_data(get_logs, get_contract):
     code = """
 b: uint256
 
 @external
 def foo():
     a: uint256 = 1234
```

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_logging_bytes_extended.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_logging_bytes_extended.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_logging_from_call.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_logging_from_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_memory_dealloc.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_memory_dealloc.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_packing.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_packing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_reverting.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_reverting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_short_circuiting.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_short_circuiting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_string_map_keys.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_string_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_ternary.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/features/test_transient.py` & `vyper-0.4.0rc4/tests/functional/codegen/features/test_transient.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/integration/test_crowdfund.py` & `vyper-0.4.0rc4/tests/functional/codegen/integration/test_crowdfund.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/integration/test_escrow.py` & `vyper-0.4.0rc4/tests/functional/codegen/integration/test_escrow.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/modules/test_events.py` & `vyper-0.4.0rc4/tests/functional/codegen/modules/test_events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/modules/test_exports.py` & `vyper-0.4.0rc4/tests/functional/codegen/modules/test_exports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/modules/test_flag_imports.py` & `vyper-0.4.0rc4/tests/functional/codegen/modules/test_flag_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/modules/test_interface_imports.py` & `vyper-0.4.0rc4/tests/functional/codegen/modules/test_interface_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/modules/test_module_constants.py` & `vyper-0.4.0rc4/tests/functional/codegen/modules/test_module_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/modules/test_module_variables.py` & `vyper-0.4.0rc4/tests/functional/codegen/modules/test_module_variables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/modules/test_nonreentrant.py` & `vyper-0.4.0rc4/tests/functional/codegen/modules/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/modules/test_stateless_functions.py` & `vyper-0.4.0rc4/tests/functional/codegen/modules/test_stateless_functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_setters.py` & `vyper-0.4.0rc4/tests/functional/codegen/storage_variables/test_setters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_storage_variable.py` & `vyper-0.4.0rc4/tests/functional/codegen/storage_variables/test_storage_variable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/test_call_graph_stability.py` & `vyper-0.4.0rc4/tests/functional/codegen/test_call_graph_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/test_interfaces.py` & `vyper-0.4.0rc4/tests/functional/codegen/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/test_selector_table.py` & `vyper-0.4.0rc4/tests/functional/codegen/test_selector_table.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/test_selector_table_stability.py` & `vyper-0.4.0rc4/tests/functional/codegen/test_selector_table_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_constants.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_decimals.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_decimals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_division.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_division.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_exponents.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_exponents.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_isqrt.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_isqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_modulo.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_modulo.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_signed_ints.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_signed_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_sqrt.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_sqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_unsigned_ints.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/numbers/test_unsigned_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_array_indexing.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_array_indexing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes_literal.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_bytes_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes_zero_padding.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_bytes_zero_padding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_dynamic_array.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_flag.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_identifier_naming.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_identifier_naming.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_lists.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_lists.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_node_types.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_node_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_string.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_string_literal.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/codegen/types/test_struct.py` & `vyper-0.4.0rc4/tests/functional/codegen/types/test_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/auctions/test_blind_auction.py` & `vyper-0.4.0rc4/tests/functional/examples/auctions/test_blind_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/auctions/test_simple_open_auction.py` & `vyper-0.4.0rc4/tests/functional/examples/auctions/test_simple_open_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/company/test_company.py` & `vyper-0.4.0rc4/tests/functional/examples/company/test_company.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/crowdfund/test_crowdfund_example.py` & `vyper-0.4.0rc4/tests/functional/examples/crowdfund/test_crowdfund_example.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/factory/test_factory.py` & `vyper-0.4.0rc4/tests/functional/examples/factory/test_factory.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/market_maker/test_on_chain_market_maker.py` & `vyper-0.4.0rc4/tests/functional/examples/market_maker/test_on_chain_market_maker.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py` & `vyper-0.4.0rc4/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/storage/test_advanced_storage.py` & `vyper-0.4.0rc4/tests/functional/examples/storage/test_advanced_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/storage/test_storage.py` & `vyper-0.4.0rc4/tests/functional/examples/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc1155.py` & `vyper-0.4.0rc4/tests/functional/examples/tokens/test_erc1155.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc20.py` & `vyper-0.4.0rc4/tests/functional/examples/tokens/test_erc20.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc4626.py` & `vyper-0.4.0rc4/tests/functional/examples/tokens/test_erc4626.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc721.py` & `vyper-0.4.0rc4/tests/functional/examples/tokens/test_erc721.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/voting/test_ballot.py` & `vyper-0.4.0rc4/tests/functional/examples/voting/test_ballot.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/examples/wallet/test_wallet.py` & `vyper-0.4.0rc4/tests/functional/examples/wallet/test_wallet.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/grammar/test_grammar.py` & `vyper-0.4.0rc4/tests/functional/grammar/test_grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_argument_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_argument_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_call_violation.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_call_violation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_constancy_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_constancy_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_function_declaration_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_function_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_instantiation_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_instantiation_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_literal_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_invalid_literal_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_payable.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_invalid_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_reference.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_invalid_reference.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_type_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_invalid_type_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_namespace_collision.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_namespace_collision.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_overflow_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_overflow_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_structure_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_structure_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_syntax_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_type_mismatch_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_type_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_undeclared_definition.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_undeclared_definition.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_variable_declaration_exception.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_variable_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_vyper_exception_pos.py` & `vyper-0.4.0rc4/tests/functional/syntax/exceptions/test_vyper_exception_pos.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/modules/test_deploy_visibility.py` & `vyper-0.4.0rc4/tests/functional/syntax/modules/test_deploy_visibility.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/modules/test_exports.py` & `vyper-0.4.0rc4/tests/functional/syntax/modules/test_exports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/modules/test_implements.py` & `vyper-0.4.0rc4/tests/functional/syntax/modules/test_implements.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/modules/test_initializers.py` & `vyper-0.4.0rc4/tests/functional/syntax/modules/test_initializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1296,56 +1296,90 @@
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
     with pytest.raises(InitializerException) as e:
         compile_code(main, input_bundle=input_bundle)
     assert e.value._message == "`lib2` uses `lib1`, but it is not initialized with `lib1`"
     assert e.value._hint == "try importing lib1 first"
 
 
-def test_nonreentrant_exports(make_input_bundle):
+@pytest.fixture
+def nonreentrant_library_bundle(make_input_bundle):
+    # test simple case
     lib1 = """
 # lib1.vy
-@external
+@internal
 @nonreentrant
 def bar():
     pass
+
+# lib1.vy
+@external
+@nonreentrant
+def ext_bar():
+    pass
     """
-    main = """
+    # test case with recursion
+    lib2 = """
+@internal
+def bar():
+    self.baz()
+
+@external
+def ext_bar():
+    self.baz()
+
+@nonreentrant
+@internal
+def baz():
+    return
+    """
+    # test case with nested recursion
+    lib3 = """
 import lib1
+uses: lib1
+
+@internal
+def bar():
+    lib1.bar()
+
+@external
+def ext_bar():
+    lib1.bar()
+    """
+
+    return make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2, "lib3.vy": lib3})
 
-exports: lib1.bar  # line 4
+
+@pytest.mark.parametrize("lib", ("lib1", "lib2", "lib3"))
+def test_nonreentrant_exports(nonreentrant_library_bundle, lib):
+    main = f"""
+import {lib}
+
+exports: {lib}.ext_bar  # line 4
 
 @external
 def foo():
     pass
     """
-    input_bundle = make_input_bundle({"lib1.vy": lib1})
     with pytest.raises(ImmutableViolation) as e:
-        compile_code(main, input_bundle=input_bundle)
-    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
-    hint = "add `uses: lib1` or `initializes: lib1` as a top-level statement to your contract"
+        compile_code(main, input_bundle=nonreentrant_library_bundle)
+    assert e.value._message == f"Cannot access `{lib}` state!" + NONREENTRANT_NOTE
+    hint = f"add `uses: {lib}` or `initializes: {lib}` as a top-level statement to your contract"
     assert e.value._hint == hint
     assert e.value.annotations[0].lineno == 4
 
 
-def test_internal_nonreentrant_import(make_input_bundle):
-    lib1 = """
-# lib1.vy
-@internal
-@nonreentrant
-def bar():
-    pass
-    """
-    main = """
-import lib1
+@pytest.mark.parametrize("lib", ("lib1", "lib2", "lib3"))
+def test_internal_nonreentrant_import(nonreentrant_library_bundle, lib):
+    main = f"""
+import {lib}
 
 @external
 def foo():
-    lib1.bar()  # line 6
+    {lib}.bar()  # line 6
     """
-    input_bundle = make_input_bundle({"lib1.vy": lib1})
     with pytest.raises(ImmutableViolation) as e:
-        compile_code(main, input_bundle=input_bundle)
-    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
+        compile_code(main, input_bundle=nonreentrant_library_bundle)
+    assert e.value._message == f"Cannot access `{lib}` state!" + NONREENTRANT_NOTE
 
-    hint = "add `uses: lib1` or `initializes: lib1` as a top-level statement to your contract"
+    hint = f"add `uses: {lib}` or `initializes: {lib}` as a top-level statement to your contract"
     assert e.value._hint == hint
     assert e.value.annotations[0].lineno == 6
```

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/names/test_event_names.py` & `vyper-0.4.0rc4/tests/functional/syntax/names/test_event_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/names/test_function_names.py` & `vyper-0.4.0rc4/tests/functional/syntax/names/test_function_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/names/test_variable_names.py` & `vyper-0.4.0rc4/tests/functional/syntax/names/test_variable_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/signatures/test_invalid_function_decorators.py` & `vyper-0.4.0rc4/tests/functional/syntax/signatures/test_invalid_function_decorators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/signatures/test_method_id_conflicts.py` & `vyper-0.4.0rc4/tests/functional/syntax/signatures/test_method_id_conflicts.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_abi_decode.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_abi_encode.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_abs.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_addmulmod.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_addmulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_address_code.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_address_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_ann_assign.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_ann_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_as_uint256.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_as_uint256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_as_wei_value.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_block.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_blockscope.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_blockscope.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_bool.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_bool.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_bool_ops.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_bool_ops.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_bytes.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_chainid.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_chainid.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_code_size.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_code_size.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_codehash.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_codehash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_concat.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_constants.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_create_with_code_of.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_create_with_code_of.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_dynamic_array.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_external_calls.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_external_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_extract32.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_flag.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_for_range.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_functions_call.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_functions_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_immutables.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_immutables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_init.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_interfaces.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_invalids.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_invalids.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_keccak256.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_len.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_list.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_logging.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_method_id.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_minmax.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_minmax_value.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_msg_data.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_msg_data.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_nested_list.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_nested_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_no_none.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_no_none.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_powmod.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_print.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_print.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_public.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_raw_call.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_return_tuple.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_return_tuple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_self_balance.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_self_balance.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_selfdestruct.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_send.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_slice.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_string.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_structs.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_structs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_ternary.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_tuple_assign.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_tuple_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/functional/syntax/test_unbalanced_return.py` & `vyper-0.4.0rc4/tests/functional/syntax/test_unbalanced_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/abi_types/test_invalid_abi_types.py` & `vyper-0.4.0rc4/tests/unit/abi_types/test_invalid_abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_compare_nodes.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_compare_nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_binop_decimal.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_binop_decimal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_binop_int.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_binop_int.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_boolop.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_boolop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_compare.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_compare.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_subscript.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_subscript.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_unaryop.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_fold_unaryop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_from_node.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_from_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_get_children.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_get_children.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_get_descendants.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_get_descendants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/nodes/test_hex.py` & `vyper-0.4.0rc4/tests/unit/ast/nodes/test_hex.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/test_annotate_and_optimize_ast.py` & `vyper-0.4.0rc4/tests/unit/ast/test_annotate_and_optimize_ast.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/test_ast_dict.py` & `vyper-0.4.0rc4/tests/unit/ast/test_ast_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/test_metadata_journal.py` & `vyper-0.4.0rc4/tests/unit/ast/test_metadata_journal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/test_natspec.py` & `vyper-0.4.0rc4/tests/unit/ast/test_natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/test_parser.py` & `vyper-0.4.0rc4/tests/unit/ast/test_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/test_pre_parser.py` & `vyper-0.4.0rc4/tests/unit/ast/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/ast/test_source_annotation.py` & `vyper-0.4.0rc4/tests/unit/ast/test_source_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/cli/storage_layout/test_storage_layout.py` & `vyper-0.4.0rc4/tests/unit/cli/storage_layout/test_storage_layout.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/cli/storage_layout/test_storage_layout_overrides.py` & `vyper-0.4.0rc4/tests/unit/cli/storage_layout/test_storage_layout_overrides.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/cli/vyper_compile/test_compile_files.py` & `vyper-0.4.0rc4/tests/unit/cli/vyper_compile/test_compile_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     combined_keys = {
         "bytecode",
         "bytecode_runtime",
         "blueprint_bytecode",
         "abi",
         "source_map",
+        "source_map_runtime",
         "layout",
         "method_identifiers",
         "userdoc",
         "devdoc",
     }
     compile_data = compile_files(["bar.vy"], ["combined_json"])
```

### Comparing `vyper-0.4.0rc3/tests/unit/cli/vyper_compile/test_parse_args.py` & `vyper-0.4.0rc4/tests/unit/cli/vyper_compile/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_compile_json.py` & `vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_compile_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,20 +167,23 @@
             "abi": data["abi"],
             "devdoc": data["devdoc"],
             "interface": data["interface"],
             "ir": data["ir_dict"],
             "userdoc": data["userdoc"],
             "metadata": data["metadata"],
             "evm": {
-                "bytecode": {"object": data["bytecode"], "opcodes": data["opcodes"]},
+                "bytecode": {
+                    "object": data["bytecode"],
+                    "opcodes": data["opcodes"],
+                    "sourceMap": data["source_map"],
+                },
                 "deployedBytecode": {
                     "object": data["bytecode_runtime"],
                     "opcodes": data["opcodes_runtime"],
-                    "sourceMap": data["source_map"]["pc_pos_map_compressed"],
-                    "sourceMapFull": data["source_map_full"],
+                    "sourceMap": data["source_map_runtime"],
                 },
                 "methodIdentifiers": data["method_identifiers"],
             },
         }
 
 
 def test_compilation_targets(input_json):
@@ -262,24 +265,24 @@
     assert len(result["errors"]) == 1
     error = result["errors"][0]
     assert error["component"] == "compiler"
     assert error["type"] == "TypeMismatch"
 
 
 def test_source_ids_increment(input_json):
-    input_json["settings"]["outputSelection"] = {"*": ["ast", "evm.deployedBytecode.sourceMapFull"]}
+    input_json["settings"]["outputSelection"] = {"*": ["ast", "evm.deployedBytecode.sourceMap"]}
     result = compile_json(input_json)
 
     def get(filename, contractname):
         ast = result["sources"][filename]["ast"]
         ret = ast["source_id"]
 
         # grab it via source map to sanity check
         contract_info = result["contracts"][filename][contractname]["evm"]
-        pc_ast_map = contract_info["deployedBytecode"]["sourceMapFull"]["pc_ast_map"]
+        pc_ast_map = contract_info["deployedBytecode"]["sourceMap"]["pc_ast_map"]
         pc_item = next(iter(pc_ast_map.values()))
         source_id, node_id = pc_item
         assert ret == source_id
 
         return ret
 
     assert get("contracts/foo.vy", "foo") == 0
```

### Comparing `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_get_inputs.py` & `vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_get_inputs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_get_settings.py` & `vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_get_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_output_selection.py` & `vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_output_selection.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py` & `vyper-0.4.0rc4/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/asm/test_asm_optimizer.py` & `vyper-0.4.0rc4/tests/unit/compiler/asm/test_asm_optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/ir/test_compile_ir.py` & `vyper-0.4.0rc4/tests/unit/compiler/ir/test_compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/ir/test_optimize_ir.py` & `vyper-0.4.0rc4/tests/unit/compiler/ir/test_optimize_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/ir/test_with.py` & `vyper-0.4.0rc4/tests/unit/compiler/ir/test_with.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_abi.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_bytecode_runtime.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_bytecode_runtime.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_compile_code.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_compile_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_default_settings.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_default_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_input_bundle.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_input_bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,64 +52,64 @@
         filepaths.append(path)
 
     ib = FilesystemInputBundle([tmp_path, tmpdir, tmpdir2])
 
     file = ib.load_file("foo.vy")
 
     assert isinstance(file, FileInput)
-    assert file == FileInput(0, "foo.vy", filepaths[2], "contents 2")
+    assert file == FileInput(0, Path("foo.vy"), filepaths[2], "contents 2")
 
     with ib.search_path(tmpdir):
         file = ib.load_file("foo.vy")
 
         assert isinstance(file, FileInput)
-        assert file == FileInput(1, "foo.vy", filepaths[1], "contents 1")
+        assert file == FileInput(1, PurePath("foo.vy"), filepaths[1], "contents 1")
 
 
 # special rules for handling json files
 def test_load_abi(make_file, input_bundle, tmp_path):
     contents = json.dumps("some string")
 
     path = make_file("foo.json", contents)
 
     file = input_bundle.load_file("foo.json")
     assert isinstance(file, ABIInput)
-    assert file == ABIInput(0, "foo.json", path, contents, "some string")
+    assert file == ABIInput(0, PurePath("foo.json"), path, contents, "some string")
 
     # suffix doesn't matter
     path = make_file("foo.txt", contents)
     file = input_bundle.load_file("foo.txt")
     assert isinstance(file, ABIInput)
-    assert file == ABIInput(1, "foo.txt", path, contents, "some string")
+    assert file == ABIInput(1, PurePath("foo.txt"), path, contents, "some string")
 
 
 # check that unique paths give unique source ids
 def test_source_id_file_input(make_file, input_bundle, tmp_path):
     foopath = make_file("foo.vy", "contents")
     barpath = make_file("bar.vy", "contents 2")
 
     file = input_bundle.load_file("foo.vy")
     assert file.source_id == 0
-    assert file == FileInput(0, "foo.vy", foopath, "contents")
+    assert file == FileInput(0, PurePath("foo.vy"), foopath, "contents")
 
     file2 = input_bundle.load_file("bar.vy")
     # source id increments
     assert file2.source_id == 1
-    assert file2 == FileInput(1, "bar.vy", barpath, "contents 2")
+    assert file2 == FileInput(1, PurePath("bar.vy"), barpath, "contents 2")
 
     file3 = input_bundle.load_file("foo.vy")
     assert file3.source_id == 0
-    assert file3 == FileInput(0, "foo.vy", foopath, "contents")
+    assert file3 == FileInput(0, PurePath("foo.vy"), foopath, "contents")
 
     # test source id is stable across different search paths
     with working_directory(tmp_path):
         with input_bundle.search_path(Path(".")):
             file4 = input_bundle.load_file("foo.vy")
             assert file4.source_id == 0
-            assert file4 == FileInput(0, "foo.vy", foopath, "contents")
+            assert file4 == FileInput(0, PurePath("foo.vy"), foopath, "contents")
 
     # test source id is stable even when requested filename is different
     with working_directory(tmp_path.parent):
         with input_bundle.search_path(Path(".")):
             file5 = input_bundle.load_file(Path(tmp_path.stem) / "foo.vy")
             assert file5.source_id == 0
             assert file5 == FileInput(0, Path(tmp_path.stem) / "foo.vy", foopath, "contents")
@@ -122,30 +122,30 @@
 
     foopath = make_file("foo.json", contents)
 
     barpath = make_file("bar.json", contents2)
 
     file = input_bundle.load_file("foo.json")
     assert isinstance(file, ABIInput)
-    assert file == ABIInput(0, "foo.json", foopath, contents, "some string")
+    assert file == ABIInput(0, PurePath("foo.json"), foopath, contents, "some string")
 
     file2 = input_bundle.load_file("bar.json")
     assert isinstance(file2, ABIInput)
-    assert file2 == ABIInput(1, "bar.json", barpath, contents2, ["some list"])
+    assert file2 == ABIInput(1, PurePath("bar.json"), barpath, contents2, ["some list"])
 
     file3 = input_bundle.load_file("foo.json")
     assert file3.source_id == 0
-    assert file3 == ABIInput(0, "foo.json", foopath, contents, "some string")
+    assert file3 == ABIInput(0, PurePath("foo.json"), foopath, contents, "some string")
 
     # test source id is stable across different search paths
     with working_directory(tmp_path):
         with input_bundle.search_path(Path(".")):
             file4 = input_bundle.load_file("foo.json")
             assert file4.source_id == 0
-            assert file4 == ABIInput(0, "foo.json", foopath, contents, "some string")
+            assert file4 == ABIInput(0, PurePath("foo.json"), foopath, contents, "some string")
 
     # test source id is stable even when requested filename is different
     with working_directory(tmp_path.parent):
         with input_bundle.search_path(Path(".")):
             file5 = input_bundle.load_file(Path(tmp_path.stem) / "foo.json")
             assert file5.source_id == 0
             assert file5 == ABIInput(
@@ -155,22 +155,22 @@
 
 # test some pathological case where the file changes underneath
 def test_mutating_file_source_id(make_file, input_bundle, tmp_path):
     foopath = make_file("foo.vy", "contents")
 
     file = input_bundle.load_file("foo.vy")
     assert file.source_id == 0
-    assert file == FileInput(0, "foo.vy", foopath, "contents")
+    assert file == FileInput(0, PurePath("foo.vy"), foopath, "contents")
 
     foopath = make_file("foo.vy", "new contents")
 
     file = input_bundle.load_file("foo.vy")
     # source id hasn't changed, even though contents have
     assert file.source_id == 0
-    assert file == FileInput(0, "foo.vy", foopath, "new contents")
+    assert file == FileInput(0, PurePath("foo.vy"), foopath, "new contents")
 
 
 # test the os.normpath behavior of symlink
 # (slightly pathological, for illustration's sake)
 def test_load_file_symlink(make_file, input_bundle, tmp_path, tmp_path_factory):
     dir1 = tmp_path / "first"
     dir2 = tmp_path / "second"
```

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_opcodes.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_pre_parser.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_sha3_32.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_sha3_32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/test_source_map.py` & `vyper-0.4.0rc4/tests/unit/compiler/test_source_map.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/venom/test_convert_basicblock_simple.py` & `vyper-0.4.0rc4/tests/unit/compiler/venom/test_convert_basicblock_simple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/venom/test_dominator_tree.py` & `vyper-0.4.0rc4/tests/unit/compiler/venom/test_dominator_tree.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/venom/test_duplicate_operands.py` & `vyper-0.4.0rc4/tests/unit/compiler/venom/test_duplicate_operands.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/venom/test_make_ssa.py` & `vyper-0.4.0rc4/tests/unit/compiler/venom/test_make_ssa.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/venom/test_multi_entry_block.py` & `vyper-0.4.0rc4/tests/unit/compiler/venom/test_multi_entry_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/compiler/venom/test_sccp.py` & `vyper-0.4.0rc4/tests/unit/compiler/venom/test_sccp.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/analysis/test_array_index.py` & `vyper-0.4.0rc4/tests/unit/semantics/analysis/test_array_index.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/analysis/test_cyclic_function_calls.py` & `vyper-0.4.0rc4/tests/unit/semantics/analysis/test_cyclic_function_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/analysis/test_for_loop.py` & `vyper-0.4.0rc4/tests/unit/semantics/analysis/test_for_loop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/analysis/test_potential_types.py` & `vyper-0.4.0rc4/tests/unit/semantics/analysis/test_potential_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/conftest.py` & `vyper-0.4.0rc4/tests/unit/semantics/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/test_namespace.py` & `vyper-0.4.0rc4/tests/unit/semantics/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/test_storage_slots.py` & `vyper-0.4.0rc4/tests/unit/semantics/test_storage_slots.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/types/test_event.py` & `vyper-0.4.0rc4/tests/unit/semantics/types/test_event.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/types/test_pure_types.py` & `vyper-0.4.0rc4/tests/unit/semantics/types/test_pure_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/types/test_size_in_bytes.py` & `vyper-0.4.0rc4/tests/unit/semantics/types/test_size_in_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/types/test_type_from_abi.py` & `vyper-0.4.0rc4/tests/unit/semantics/types/test_type_from_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/unit/semantics/types/test_type_from_annotation.py` & `vyper-0.4.0rc4/tests/unit/semantics/types/test_type_from_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/tests/utils.py` & `vyper-0.4.0rc4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/__init__.py` & `vyper-0.4.0rc4/vyper/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/__main__.py` & `vyper-0.4.0rc4/vyper/__main__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/abi_types.py` & `vyper-0.4.0rc4/vyper/abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/README.md` & `vyper-0.4.0rc4/vyper/ast/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/grammar.lark` & `vyper-0.4.0rc4/vyper/ast/grammar.lark`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/grammar.py` & `vyper-0.4.0rc4/vyper/ast/grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/identifiers.py` & `vyper-0.4.0rc4/vyper/ast/identifiers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/metadata.py` & `vyper-0.4.0rc4/vyper/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/natspec.py` & `vyper-0.4.0rc4/vyper/ast/natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/nodes.py` & `vyper-0.4.0rc4/vyper/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/nodes.pyi` & `vyper-0.4.0rc4/vyper/ast/nodes.pyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/parse.py` & `vyper-0.4.0rc4/vyper/ast/parse.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/pre_parser.py` & `vyper-0.4.0rc4/vyper/ast/pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/utils.py` & `vyper-0.4.0rc4/vyper/ast/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ast/validation.py` & `vyper-0.4.0rc4/vyper/ast/validation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/builtins/_convert.py` & `vyper-0.4.0rc4/vyper/builtins/_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/builtins/_signatures.py` & `vyper-0.4.0rc4/vyper/builtins/_signatures.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/builtins/_utils.py` & `vyper-0.4.0rc4/vyper/builtins/_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/builtins/functions.py` & `vyper-0.4.0rc4/vyper/builtins/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1267,32 +1267,28 @@
 
         return [self._inputs[0][1], data_type]
 
     @process_inputs
     def build_IR(self, expr, args, kwargs, context):
         topics_length = len(expr.args[0].elements)
         topics = args[0].args
+        topics = [unwrap_location(topic) for topic in topics]
 
         # sanity check topics is a literal list
         assert args[0].value in ("~empty", "multi")
 
         data = args[1]
 
         log_op = "log" + str(topics_length)
 
         if data.typ == BYTES32_T:
             placeholder = context.new_internal_variable(BYTES32_T)
             log_ir = [log_op, placeholder, 32] + topics
             return IRnode.from_list(
-                [
-                    "seq",
-                    # TODO use make_setter
-                    ["mstore", placeholder, unwrap_location(data)],
-                    ensure_eval_once("raw_log", log_ir),
-                ]
+                ["seq", make_setter(placeholder, data), ensure_eval_once("raw_log", log_ir)]
             )
 
         input_buf = ensure_in_memory(data, context)
 
         log_ir = [log_op, ["add", "_sub", 32], ["mload", "_sub"], *topics]
         return IRnode.from_list(["with", "_sub", input_buf, ensure_eval_once("raw_log", log_ir)])
```

### Comparing `vyper-0.4.0rc3/vyper/builtins/interfaces/IERC20.vyi` & `vyper-0.4.0rc4/vyper/builtins/interfaces/IERC20.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/builtins/interfaces/IERC4626.vyi` & `vyper-0.4.0rc4/vyper/builtins/interfaces/IERC4626.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/builtins/interfaces/IERC721.vyi` & `vyper-0.4.0rc4/vyper/builtins/interfaces/IERC721.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/cli/compile_archive.py` & `vyper-0.4.0rc4/vyper/cli/compile_archive.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/cli/vyper_compile.py` & `vyper-0.4.0rc4/vyper/cli/vyper_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 format_options_help = """Format to print, one or more of:
 bytecode (default) - Deployable bytecode
 bytecode_runtime   - Bytecode at runtime
 blueprint_bytecode - Deployment bytecode for an ERC-5202 compatible blueprint
 abi                - ABI in JSON format
 abi_python         - ABI in python format
-source_map         - Vyper source map
+source_map         - Vyper source map of deployable bytecode
+source_map_runtime - Vyper source map of runtime bytecode
 method_identifiers - Dictionary of method signature to method identifier
 userdoc            - Natspec user documentation
 devdoc             - Natspec developer documentation
 metadata           - Contract metadata (intended for use by tooling developers)
 combined_json      - All of the above format options combined as single JSON output
 layout             - Storage layout of a Vyper contract
 ast                - AST (not yet annotated) in JSON format
@@ -48,14 +49,15 @@
 combined_json_outputs = [
     "bytecode",
     "bytecode_runtime",
     "blueprint_bytecode",
     "abi",
     "layout",
     "source_map",
+    "source_map_runtime",
     "method_identifiers",
     "userdoc",
     "devdoc",
 ]
 
 
 def _parse_cli_args():
```

### Comparing `vyper-0.4.0rc3/vyper/cli/vyper_ir.py` & `vyper-0.4.0rc4/vyper/cli/vyper_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/cli/vyper_json.py` & `vyper-0.4.0rc4/vyper/cli/vyper_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     "abi": "abi",
     "ast": "ast_dict",
     "annotated_ast": "annotated_ast_dict",
     "devdoc": "devdoc",
     "evm.methodIdentifiers": "method_identifiers",
     "evm.bytecode.object": "bytecode",
     "evm.bytecode.opcodes": "opcodes",
+    "evm.bytecode.sourceMap": "source_map",
     "evm.deployedBytecode.object": "bytecode_runtime",
     "evm.deployedBytecode.opcodes": "opcodes_runtime",
-    "evm.deployedBytecode.sourceMap": "source_map",
-    "evm.deployedBytecode.sourceMapFull": "source_map_full",
+    "evm.deployedBytecode.sourceMap": "source_map_runtime",
     "interface": "interface",
     "ir": "ir_dict",
     "ir_runtime": "ir_runtime_dict",
     "metadata": "metadata",
     "layout": "layout",
     "userdoc": "userdoc",
 }
@@ -231,15 +231,15 @@
 
         outputs = sorted(list(outputs))
 
         if path == "*":
             output_paths = [PurePath(path) for path in input_dict["sources"].keys()]
         else:
             output_paths = [PurePath(path)]
-            if str(output_paths[0]) not in input_dict["sources"]:
+            if output_paths[0].as_posix() not in input_dict["sources"]:
                 raise JSONError(f"outputSelection references unknown contract '{output_paths[0]}'")
 
         for output_path in output_paths:
             output_formats[output_path] = outputs
 
     return output_formats
 
@@ -313,15 +313,15 @@
     return res, warnings_dict
 
 
 # convert output of compile_input_dict to final output format
 def format_to_output_dict(compiler_data: dict) -> dict:
     output_dict: dict = {"compiler": f"vyper-{vyper.__version__}", "contracts": {}, "sources": {}}
     for path, data in compiler_data.items():
-        path = str(path)  # Path breaks json serializability
+        path = path.as_posix()  # Path breaks json serializability
         output_dict["sources"][path] = {"id": data["source_id"]}
 
         for k in ("ast_dict", "annotated_ast_dict"):
             if k in data:
                 # un-translate the key
                 k2 = k.removesuffix("_dict")
                 output_dict["sources"][path][k2] = data[k]["ast"]
@@ -337,32 +337,32 @@
             if key in data:
                 output_contracts[key] = data[key]
 
         if "method_identifiers" in data:
             output_contracts["evm"] = {"methodIdentifiers": data["method_identifiers"]}
 
         evm_keys = ("bytecode", "opcodes")
-        if any(i in data for i in evm_keys):
+        pc_maps_keys = ("source_map",)
+        if any(i in data for i in evm_keys + pc_maps_keys):
             evm = output_contracts.setdefault("evm", {}).setdefault("bytecode", {})
             if "bytecode" in data:
                 evm["object"] = data["bytecode"]
             if "opcodes" in data:
                 evm["opcodes"] = data["opcodes"]
+            if "source_map" in data:
+                evm["sourceMap"] = data["source_map"]
 
-        pc_maps_keys = ("source_map", "source_map_full")
-        if any(i + "_runtime" in data for i in evm_keys) or any(i in data for i in pc_maps_keys):
+        if any(i + "_runtime" in data for i in evm_keys + pc_maps_keys):
             evm = output_contracts.setdefault("evm", {}).setdefault("deployedBytecode", {})
             if "bytecode_runtime" in data:
                 evm["object"] = data["bytecode_runtime"]
             if "opcodes_runtime" in data:
                 evm["opcodes"] = data["opcodes_runtime"]
-            if "source_map" in data:
-                evm["sourceMap"] = data["source_map"]["pc_pos_map_compressed"]
-            if "source_map_full" in data:
-                evm["sourceMapFull"] = data["source_map_full"]
+            if "source_map_runtime" in data:
+                evm["sourceMap"] = data["source_map_runtime"]
 
     return output_dict
 
 
 # https://stackoverflow.com/a/49518779
 def _raise_on_duplicate_keys(ordered_pairs: list[tuple[Hashable, Any]]) -> dict:
     """
```

### Comparing `vyper-0.4.0rc3/vyper/codegen/abi_encoder.py` & `vyper-0.4.0rc4/vyper/codegen/abi_encoder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/arithmetic.py` & `vyper-0.4.0rc4/vyper/codegen/arithmetic.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/context.py` & `vyper-0.4.0rc4/vyper/codegen/context.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/core.py` & `vyper-0.4.0rc4/vyper/codegen/core.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/events.py` & `vyper-0.4.0rc4/vyper/codegen/events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/expr.py` & `vyper-0.4.0rc4/vyper/codegen/expr.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/external_call.py` & `vyper-0.4.0rc4/vyper/codegen/external_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/function_definitions/common.py` & `vyper-0.4.0rc4/vyper/codegen/function_definitions/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/function_definitions/external_function.py` & `vyper-0.4.0rc4/vyper/codegen/function_definitions/external_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/function_definitions/internal_function.py` & `vyper-0.4.0rc4/vyper/codegen/function_definitions/internal_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/ir_node.py` & `vyper-0.4.0rc4/vyper/codegen/ir_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/jumptable_utils.py` & `vyper-0.4.0rc4/vyper/codegen/jumptable_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/keccak256_helper.py` & `vyper-0.4.0rc4/vyper/codegen/keccak256_helper.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/memory_allocator.py` & `vyper-0.4.0rc4/vyper/codegen/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/module.py` & `vyper-0.4.0rc4/vyper/codegen/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/return_.py` & `vyper-0.4.0rc4/vyper/codegen/return_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/self_call.py` & `vyper-0.4.0rc4/vyper/codegen/self_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/codegen/stmt.py` & `vyper-0.4.0rc4/vyper/codegen/stmt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/compiler/README.md` & `vyper-0.4.0rc4/vyper/compiler/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/compiler/__init__.py` & `vyper-0.4.0rc4/vyper/compiler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "ir_runtime_dict": output.build_ir_runtime_dict_output,
     "method_identifiers": output.build_method_identifiers_output,
     "metadata": output.build_metadata_output,
     # requires assembly
     "abi": output.build_abi_output,
     "asm": output.build_asm_output,
     "source_map": output.build_source_map_output,
-    "source_map_full": output.build_source_map_output,
+    "source_map_runtime": output.build_source_map_runtime_output,
     # requires bytecode
     "bytecode": output.build_bytecode_output,
     "bytecode_runtime": output.build_bytecode_runtime_output,
     "blueprint_bytecode": output.build_blueprint_bytecode_output,
     "opcodes": output.build_opcodes_output,
     "opcodes_runtime": output.build_opcodes_runtime_output,
 }
@@ -101,16 +101,14 @@
 
     if output_formats is None:
         output_formats = ("bytecode",)
 
     # make IR output the same between runs
     codegen.reset_names()
 
-    # TODO: maybe at this point we might as well just pass a `FileInput`
-    # directly to `CompilerData`.
     compiler_data = CompilerData(
         file_input,
         input_bundle,
         settings=settings,
         integrity_sum=integrity_sum,
         storage_layout=storage_layout_override,
         show_gas_estimates=show_gas_estimates,
```

### Comparing `vyper-0.4.0rc3/vyper/compiler/input_bundle.py` & `vyper-0.4.0rc4/vyper/compiler/input_bundle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import contextlib
 import json
-import os
+import posixpath
 from dataclasses import asdict, dataclass, field
 from functools import cached_property
 from pathlib import Path, PurePath
 from typing import TYPE_CHECKING, Any, Iterator, Optional
 
 from vyper.exceptions import JSONError
 from vyper.utils import sha256sum
@@ -102,14 +102,16 @@
             self._source_id_counter += 1
 
         return self._source_ids[resolved_path]
 
     def load_file(self, path: PathLike | str) -> CompilerInput:
         # search path precedence
         tried = []
+        if isinstance(path, str):
+            path = PurePath(path)
         for sp in reversed(self.search_paths):
             # note from pathlib docs:
             # > If the argument is an absolute path, the previous path is ignored.
             # Path("/a") / Path("/b") => Path("/b")
             to_try = sp / path
 
             try:
@@ -183,17 +185,21 @@
             raise _NotFound(resolved_path)
 
         source_id = super()._generate_source_id(resolved_path)
 
         return FileInput(source_id, original_path, resolved_path, code)
 
 
-# wrap os.path.normpath, but return the same type as the input
+# wrap os.path.normpath, but return the same type as the input -
+# but use posixpath instead so that things work cross-platform.
 def _normpath(path):
-    return path.__class__(os.path.normpath(path))
+    cls = path.__class__
+    if not isinstance(path, str):
+        path = path.as_posix()
+    return cls(posixpath.normpath(path))
 
 
 # fake filesystem for "standard JSON" (aka solc-style) inputs. takes search
 # paths, and `load_file()` "reads" the file from the JSON input. Note that this
 # input bundle type never actually interacts with the filesystem -- it is
 # guaranteed to be pure!
 class JSONInputBundle(InputBundle):
@@ -251,15 +257,15 @@
     def _normalize_path(self, path: PurePath) -> PurePath:
         return _normpath(path)
 
     def _load_from_path(self, resolved_path: PurePath, original_path: PurePath) -> CompilerInput:
         # zipfile.BadZipFile: File is not a zip file
 
         try:
-            value = self.archive.read(str(resolved_path)).decode("utf-8")
+            value = self.archive.read(resolved_path.as_posix()).decode("utf-8")
         except KeyError:
             # zipfile literally raises KeyError if the file is not there
             raise _NotFound(resolved_path)
 
         source_id = super()._generate_source_id(resolved_path)
 
         return FileInput(source_id, original_path, resolved_path, value)
```

### Comparing `vyper-0.4.0rc3/vyper/compiler/output.py` & `vyper-0.4.0rc4/vyper/compiler/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -284,24 +284,21 @@
 
 
 def _build_node_identifier(ast_node):
     assert ast_node.module_node is not None, type(ast_node)
     return (ast_node.module_node.source_id, ast_node.node_id)
 
 
-def build_source_map_output(compiler_data: CompilerData) -> dict:
+def _build_source_map_output(compiler_data, bytecode, pc_maps):
     """
     Generate source map output in various formats. Note that integrations
     are encouraged to use pc_ast_map since the information it provides is
     a superset of the other formats, and the other types are included
     for legacy reasons.
     """
-    bytecode, pc_maps = compile_ir.assembly_to_evm(
-        compiler_data.assembly_runtime, insert_compiler_metadata=False
-    )
     # sort the pc maps alphabetically
     # CMC 2024-03-09 is this really necessary?
     out = {}
     for k in sorted(pc_maps.keys()):
         out[k] = pc_maps[k]
 
     ast_map = out.pop("pc_raw_ast_map")
@@ -318,14 +315,28 @@
     out["pc_pos_map"] = pc_pos_map
     out["pc_ast_map"] = node_id_map
     # hint to consumers what the fields in pc_ast_map mean
     out["pc_ast_map_item_keys"] = ("source_id", "node_id")
     return out
 
 
+def build_source_map_output(compiler_data: CompilerData) -> dict:
+    bytecode, pc_maps = compile_ir.assembly_to_evm(
+        compiler_data.assembly, insert_compiler_metadata=False
+    )
+    return _build_source_map_output(compiler_data, bytecode, pc_maps)
+
+
+def build_source_map_runtime_output(compiler_data: CompilerData) -> dict:
+    bytecode, pc_maps = compile_ir.assembly_to_evm(
+        compiler_data.assembly_runtime, insert_compiler_metadata=False
+    )
+    return _build_source_map_output(compiler_data, bytecode, pc_maps)
+
+
 # generate a solidity-style source map. this functionality is deprecated
 # in favor of pc_ast_map, and may not be maintained to the same level
 # as pc_ast_map.
 def _compress_source_map(ast_map, jump_map, bytecode_size):
     ret = []
 
     jump_map = jump_map.copy()
```

### Comparing `vyper-0.4.0rc3/vyper/compiler/output_bundle.py` & `vyper-0.4.0rc4/vyper/compiler/output_bundle.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,19 @@
     segments = []
     # replace ../../../a/b with 0/1/2/a/b
     for i, s in enumerate(PurePath(p).parts):
         if s == "..":
             segments.append(str(i))
         else:
             segments.append(s)
-    return str(PurePath(*segments))
+
+    # the way to get reliable paths which reproduce cross-platform is to use
+    # posix style paths.
+    # cf. https://stackoverflow.com/a/122485
+    return PurePath(*segments).as_posix()
 
 
 # data structure containing things that should be in an output bundle,
 # which is some container containing the information required to
 # reproduce a build
 @dataclass
 class OutputBundle:
@@ -54,26 +58,26 @@
         inputs: list[CompilerInput] = [
             t.compiler_input for t in self._imports if not _is_builtin(t.qualified_module_name)
         ]
         inputs.append(self.compiler_data.file_input)
 
         sources = {}
         for c in inputs:
-            path = os.path.relpath(str(c.resolved_path))
+            path = os.path.relpath(c.resolved_path)
             # note: there should be a 1:1 correspondence between
             # resolved_path and source_id, but for clarity use resolved_path
             # since it corresponds more directly to search path semantics.
             sources[_anonymize(path)] = c
 
         return sources
 
     @cached_property
     def compilation_target_path(self):
-        p = self.compiler_data.file_input.resolved_path
-        p = os.path.relpath(str(p))
+        p = PurePath(self.compiler_data.file_input.resolved_path)
+        p = os.path.relpath(p)
         return _anonymize(p)
 
     @cached_property
     def used_search_paths(self) -> list[str]:
         # report back which search paths were "actually used" in this
         # compilation run. this is useful mainly for aesthetic purposes,
         # because we don't need to see `/usr/lib/python` in the search path
@@ -251,10 +255,16 @@
     def write_compilation_target(self, targets: list[str]):
         self.archive.writestr("MANIFEST/compilation_targets", "\n".join(targets))
 
     def write_version(self, version: str):
         self.archive.writestr("MANIFEST/compiler_version", version)
 
     def output(self):
-        assert self.archive.testzip() is None
         self.archive.close()
+
+        # there is a race on windows where testzip() will return false
+        # before closing. close it and then reopen to run testzip()
+        s = zipfile.ZipFile(self._buf)
+        assert s.testzip() is None
+        del s  # garbage collector, cf. `__del__()` method.
+
         return self._buf.getvalue()
```

### Comparing `vyper-0.4.0rc3/vyper/compiler/phases.py` & `vyper-0.4.0rc4/vyper/compiler/phases.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
         return self.file_input.path
 
     @cached_property
     def _generate_ast(self):
         settings, ast = vy_ast.parse_to_ast_with_settings(
             self.source_code,
             self.source_id,
-            module_path=str(self.contract_path),
-            resolved_path=str(self.file_input.resolved_path),
+            module_path=self.contract_path.as_posix(),
+            resolved_path=self.file_input.resolved_path.as_posix(),
         )
 
         if self.original_settings:
             og_settings = self.original_settings
             settings = merge_settings(og_settings, settings)
             assert self.original_settings == og_settings  # be paranoid
         else:
```

### Comparing `vyper-0.4.0rc3/vyper/compiler/settings.py` & `vyper-0.4.0rc4/vyper/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/compiler/utils.py` & `vyper-0.4.0rc4/vyper/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/evm/address_space.py` & `vyper-0.4.0rc4/vyper/evm/address_space.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/evm/opcodes.py` & `vyper-0.4.0rc4/vyper/evm/opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/exceptions.py` & `vyper-0.4.0rc4/vyper/exceptions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ir/README.md` & `vyper-0.4.0rc4/vyper/ir/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ir/compile_ir.py` & `vyper-0.4.0rc4/vyper/ir/compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ir/optimizer.py` & `vyper-0.4.0rc4/vyper/ir/optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/ir/s_expressions.py` & `vyper-0.4.0rc4/vyper/ir/s_expressions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/README.md` & `vyper-0.4.0rc4/vyper/semantics/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/base.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/common.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/constant_folding.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/constant_folding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/data_positions.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/data_positions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/getters.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/global_.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/global_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/import_graph.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/import_graph.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/levenshtein_utils.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/levenshtein_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/local.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -910,22 +910,22 @@
                 # this should have been caught in
                 # `get_possible_types_from_node` but wasn't.
                 raise TypeCheckFailure(f"Expected {typ} but it is not a possible type", node)
 
         else:
             base_type = get_exact_type_from_node(node.value)
 
-        # get the correct type for the index, it might
-        # not be exactly base_type.key_type
-        # note: index_type is validated in types_from_Subscript
-        index_types = get_possible_types_from_node(node.slice)
-        index_type = index_types.pop()
+        if isinstance(base_type, HashMapT):
+            index_type = base_type.key_type
+        else:
+            # Arrays allow most int types as index: Take the least specific
+            index_type = get_possible_types_from_node(node.slice).pop()
 
-        self.visit(node.slice, index_type)
         self.visit(node.value, base_type)
+        self.visit(node.slice, index_type)
 
     def visit_Tuple(self, node: vy_ast.Tuple, typ: VyperType) -> None:
         if isinstance(typ, TYPE_T):
             # don't recurse; can't annotate AST children of type definition
             return
 
         # these guarantees should be provided by validate_expected_type
```

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/module.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -884,16 +884,16 @@
         # we couldn't get a relative path (cf. docs for Path.relative_to),
         # use the resolved path given to us by the InputBundle
         pass
 
     ret = vy_ast.parse_to_ast(
         file.source_code,
         source_id=file.source_id,
-        module_path=str(module_path),
-        resolved_path=str(file.resolved_path),
+        module_path=module_path.as_posix(),
+        resolved_path=file.resolved_path.as_posix(),
     )
     return ret
 
 
 # convert an import to a path (without suffix)
 def _import_to_path(level: int, module_str: str) -> PurePath:
     base_path = ""
```

### Comparing `vyper-0.4.0rc3/vyper/semantics/analysis/utils.py` & `vyper-0.4.0rc4/vyper/semantics/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/environment.py` & `vyper-0.4.0rc4/vyper/semantics/environment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/namespace.py` & `vyper-0.4.0rc4/vyper/semantics/namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/__init__.py` & `vyper-0.4.0rc4/vyper/semantics/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/base.py` & `vyper-0.4.0rc4/vyper/semantics/types/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/bytestrings.py` & `vyper-0.4.0rc4/vyper/semantics/types/bytestrings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/function.py` & `vyper-0.4.0rc4/vyper/semantics/types/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,19 @@
     def get_variable_writes(self):
         return self._variable_writes
 
     def get_variable_accesses(self):
         return self._variable_reads | self._variable_writes
 
     def uses_state(self):
-        return self.nonreentrant or uses_state(self.get_variable_accesses())
+        return (
+            self.nonreentrant
+            or uses_state(self.get_variable_accesses())
+            or any(f.nonreentrant for f in self.reachable_internal_functions)
+        )
 
     def get_used_modules(self):
         # _used_modules is populated during analysis
         return self._used_modules
 
     def mark_used_module(self, module_info):
         self._used_modules.add(module_info)
```

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/module.py` & `vyper-0.4.0rc4/vyper/semantics/types/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/primitives.py` & `vyper-0.4.0rc4/vyper/semantics/types/primitives.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/subscriptable.py` & `vyper-0.4.0rc4/vyper/semantics/types/subscriptable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/user.py` & `vyper-0.4.0rc4/vyper/semantics/types/user.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/semantics/types/utils.py` & `vyper-0.4.0rc4/vyper/semantics/types/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/utils.py` & `vyper-0.4.0rc4/vyper/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/README.md` & `vyper-0.4.0rc4/vyper/venom/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/__init__.py` & `vyper-0.4.0rc4/vyper/venom/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from vyper.venom.ir_node_to_venom import ir_node_to_venom
 from vyper.venom.passes.dft import DFTPass
 from vyper.venom.passes.make_ssa import MakeSSA
 from vyper.venom.passes.mem2var import Mem2Var
 from vyper.venom.passes.remove_unused_variables import RemoveUnusedVariablesPass
 from vyper.venom.passes.sccp import SCCP
 from vyper.venom.passes.simplify_cfg import SimplifyCFGPass
+from vyper.venom.passes.store_elimination import StoreElimination
 from vyper.venom.venom_to_assembly import VenomCompiler
 
 DEFAULT_OPT_LEVEL = OptimizationLevel.default()
 
 
 def generate_assembly_experimental(
     runtime_code: IRContext,
@@ -41,16 +42,17 @@
     # TODO: Add support for optimization levels
 
     ac = IRAnalysesCache(fn)
 
     SimplifyCFGPass(ac, fn).run_pass()
     Mem2Var(ac, fn).run_pass()
     MakeSSA(ac, fn).run_pass()
+    StoreElimination(ac, fn).run_pass()
+    MakeSSA(ac, fn).run_pass()
     SCCP(ac, fn).run_pass()
-
     SimplifyCFGPass(ac, fn).run_pass()
     RemoveUnusedVariablesPass(ac, fn).run_pass()
     DFTPass(ac, fn).run_pass()
 
 
 def generate_ir(ir: IRnode, optimize: OptimizationLevel) -> IRContext:
     # Convert "old" IR to "new" IR
```

### Comparing `vyper-0.4.0rc3/vyper/venom/analysis/analysis.py` & `vyper-0.4.0rc4/vyper/venom/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/analysis/cfg.py` & `vyper-0.4.0rc4/vyper/venom/analysis/cfg.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/analysis/dfg.py` & `vyper-0.4.0rc4/vyper/venom/analysis/dfg.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/analysis/dominators.py` & `vyper-0.4.0rc4/vyper/venom/analysis/dominators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/analysis/dup_requirements.py` & `vyper-0.4.0rc4/vyper/venom/analysis/dup_requirements.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/analysis/liveness.py` & `vyper-0.4.0rc4/vyper/venom/analysis/liveness.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/basicblock.py` & `vyper-0.4.0rc4/vyper/venom/basicblock.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/context.py` & `vyper-0.4.0rc4/vyper/venom/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,19 +49,27 @@
 
     def append_data(self, opcode: str, args: list[IROperand]) -> None:
         """
         Append data
         """
         self.data_segment.append(IRInstruction(opcode, args))  # type: ignore
 
+    def as_graph(self) -> str:
+        s = ["digraph G {"]
+        for fn in self.functions.values():
+            s.append(fn.as_graph(True))
+            s.append("\n")
+        s.append("}")
+        return "\n".join(s)
+
     def __repr__(self) -> str:
         s = ["IRContext:"]
         for fn in self.functions.values():
             s.append(fn.__repr__())
             s.append("\n")
 
         if len(self.data_segment) > 0:
-            s += "\nData segment:\n"
+            s.append("\nData segment:")
             for inst in self.data_segment:
-                s += f"{inst}\n"
+                s.append(f"{inst}")
 
         return "\n".join(s)
```

### Comparing `vyper-0.4.0rc3/vyper/venom/function.py` & `vyper-0.4.0rc4/vyper/venom/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,38 +210,49 @@
     def copy(self):
         new = IRFunction(self.name)
         new._basic_block_dict = self._basic_block_dict.copy()
         new.last_label = self.last_label
         new.last_variable = self.last_variable
         return new
 
-    def as_graph(self) -> str:
+    def as_graph(self, only_subgraph=False) -> str:
+        """
+        Return the function as a graphviz dot string. If only_subgraph is True, only return the
+        subgraph, not the full digraph -for embedding in a larger graph-
+        """
         import html
 
         def _make_label(bb):
             ret = '<<table border="1" cellborder="0" cellspacing="0">'
             ret += f'<tr><td align="left"><b>{html.escape(str(bb.label))}</b></td></tr>\n'
             for inst in bb.instructions:
                 ret += f'<tr ><td align="left">{html.escape(str(inst))}</td></tr>\n'
             ret += "</table>>"
 
             return ret
             # return f"{bb.label.value}:\n" + "\n".join([f"    {inst}" for inst in bb.instructions])
 
-        ret = "digraph G {\n"
+        ret = []
+
+        if not only_subgraph:
+            ret.append("digraph G {{")
+        ret.append(f'subgraph "{self.name}" {{')
 
         for bb in self.get_basic_blocks():
             for out_bb in bb.cfg_out:
-                ret += f'    "{bb.label.value}" -> "{out_bb.label.value}"\n'
+                ret.append(f'    "{bb.label.value}" -> "{out_bb.label.value}"')
 
         for bb in self.get_basic_blocks():
-            ret += f'    "{bb.label.value}" [shape=plaintext, '
-            ret += f'label={_make_label(bb)}, fontname="Courier" fontsize="8"]\n'
+            ret.append(f'    "{bb.label.value}" [shape=plaintext, ')
+            ret.append(f'label={_make_label(bb)}, fontname="Courier" fontsize="8"]')
+
+        ret.append("}\n")
+        if not only_subgraph:
+            ret.append("}\n")
 
-        ret += "}\n"
-        return ret
+        return "\n".join(ret)
 
     def __repr__(self) -> str:
         str = f"IRFunction: {self.name}\n"
         for bb in self.get_basic_blocks():
             str += f"{bb}\n"
         return str.strip()
```

### Comparing `vyper-0.4.0rc3/vyper/venom/ir_node_to_venom.py` & `vyper-0.4.0rc4/vyper/venom/ir_node_to_venom.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/base_pass.py` & `vyper-0.4.0rc4/vyper/venom/passes/base_pass.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/dft.py` & `vyper-0.4.0rc4/vyper/venom/passes/dft.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/make_ssa.py` & `vyper-0.4.0rc4/vyper/venom/passes/make_ssa.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,32 +63,14 @@
                 continue
 
             args.append(bb.label)  # type: ignore
             args.append(var)  # type: ignore
 
         basic_block.insert_instruction(IRInstruction("phi", args, var), 0)
 
-    def _add_phi(self, var: IRVariable, basic_block: IRBasicBlock) -> bool:
-        for inst in basic_block.instructions:
-            if inst.opcode == "phi" and inst.output is not None and inst.output.name == var.name:
-                return False
-
-        args: list[IROperand] = []
-        for bb in basic_block.cfg_in:
-            if bb == basic_block:
-                continue
-
-            args.append(bb.label)
-            args.append(var)
-
-        phi = IRInstruction("phi", args, var)
-        basic_block.instructions.insert(0, phi)
-
-        return True
-
     def _rename_vars(self, basic_block: IRBasicBlock):
         """
         Rename variables. This follows the placement of phi nodes.
         """
         outs = []
 
         # Pre-action
```

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/mem2var.py` & `vyper-0.4.0rc4/vyper/venom/passes/mem2var.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,11 @@
                     inst.output = IRVariable(var_name)
                     inst.operands = [inst.operands[0]]
                 elif inst.opcode == "mload":
                     inst.opcode = "store"
                     inst.operands = [IRVariable(var_name)]
                 elif inst.opcode == "return":
                     bb = inst.parent
-                    new_var = self.function.get_next_variable()
                     idx = bb.instructions.index(inst)
                     bb.insert_instruction(
-                        IRInstruction("mstore", [IRVariable(var_name), inst.operands[1]], new_var),
-                        idx,
+                        IRInstruction("mstore", [IRVariable(var_name), inst.operands[1]]), idx
                     )
-                    inst.operands[1] = new_var
```

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/normalization.py` & `vyper-0.4.0rc4/vyper/venom/passes/normalization.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/remove_unused_variables.py` & `vyper-0.4.0rc4/vyper/venom/passes/remove_unused_variables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/sccp/eval.py` & `vyper-0.4.0rc4/vyper/venom/passes/sccp/eval.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/sccp/sccp.py` & `vyper-0.4.0rc4/vyper/venom/passes/sccp/sccp.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,15 +164,17 @@
         in_vars: list[LatticeItem] = []
         for bb_label, var in inst.phi_operands:
             bb = self.fn.get_basic_block(bb_label.name)
             if bb not in self.cfg_in_exec[inst.parent]:
                 continue
             in_vars.append(self._lookup_from_lattice(var))
         value = reduce(_meet, in_vars, LatticeEnum.TOP)  # type: ignore
-        assert inst.output in self.lattice, "Got undefined var for phi"
+
+        if inst.output not in self.lattice:
+            return
 
         if value != self._lookup_from_lattice(inst.output):
             self._set_lattice(inst.output, value)
             self._add_ssa_work_items(inst)
 
     def _visit_expr(self, inst: IRInstruction):
         opcode = inst.opcode
@@ -323,34 +325,14 @@
 
         for i, op in enumerate(inst.operands):
             if isinstance(op, IRVariable):
                 lat = self.lattice[op]
                 if isinstance(lat, IRLiteral):
                     inst.operands[i] = lat
 
-    def _propagate_variables(self):
-        """
-        Copy elimination. #NOTE: Not working yet, but it's also not needed atm.
-        """
-        for bb in self.dom.dfs_walk:
-            for inst in bb.instructions:
-                if inst.opcode == "store":
-                    uses = self._get_uses(inst.output)
-                    remove_inst = True
-                    for usage_inst in uses:
-                        if usage_inst.opcode == "phi":
-                            remove_inst = False
-                            continue
-                        for i, op in enumerate(usage_inst.operands):
-                            if op == inst.output:
-                                usage_inst.operands[i] = inst.operands[0]
-                    if remove_inst:
-                        inst.opcode = "nop"
-                        inst.operands = []
-
 
 def _meet(x: LatticeItem, y: LatticeItem) -> LatticeItem:
     if x == LatticeEnum.TOP:
         return y
     if y == LatticeEnum.TOP or x == y:
         return x
     return LatticeEnum.BOTTOM
```

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/simplify_cfg.py` & `vyper-0.4.0rc4/vyper/venom/passes/simplify_cfg.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/passes/stack_reorder.py` & `vyper-0.4.0rc4/vyper/venom/passes/stack_reorder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/stack_model.py` & `vyper-0.4.0rc4/vyper/venom/stack_model.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper/venom/venom_to_assembly.py` & `vyper-0.4.0rc4/vyper/venom/venom_to_assembly.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc3/vyper.egg-info/PKG-INFO` & `vyper-0.4.0rc4/vyper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0rc3
+Version: 0.4.0rc4
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0rc3/vyper.egg-info/SOURCES.txt` & `vyper-0.4.0rc4/vyper.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -509,10 +509,11 @@
 vyper/venom/passes/dft.py
 vyper/venom/passes/make_ssa.py
 vyper/venom/passes/mem2var.py
 vyper/venom/passes/normalization.py
 vyper/venom/passes/remove_unused_variables.py
 vyper/venom/passes/simplify_cfg.py
 vyper/venom/passes/stack_reorder.py
+vyper/venom/passes/store_elimination.py
 vyper/venom/passes/sccp/__init__.py
 vyper/venom/passes/sccp/eval.py
 vyper/venom/passes/sccp/sccp.py
```

### Comparing `vyper-0.4.0rc3/vyper.egg-info/requires.txt` & `vyper-0.4.0rc4/vyper.egg-info/requires.txt`

 * *Files identical despite different names*

