# Comparing `tmp/aiotx-0.6.0.tar.gz` & `tmp/aiotx-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.6.0.tar", last modified: Sat May  4 17:25:17 2024, max compression
+gzip compressed data, was "aiotx-1.0.0.tar", last modified: Sun May 19 09:59:19 2024, max compression
```

## Comparing `aiotx-0.6.0.tar` & `aiotx-1.0.0.tar`

### file list

```diff
@@ -1,125 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.947354 aiotx-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.927353 aiotx-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.931353 aiotx-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-04 17:25:12.000000 aiotx-0.6.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 17:25:12.000000 aiotx-0.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-04 17:25:12.000000 aiotx-0.6.0/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-04 17:25:12.000000 aiotx-0.6.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-04 17:25:12.000000 aiotx-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-04 17:25:12.000000 aiotx-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-04 17:25:12.000000 aiotx-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-04 17:25:12.000000 aiotx-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-04 17:25:12.000000 aiotx-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-04 17:25:17.947354 aiotx-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-04 17:25:12.000000 aiotx-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.931353 aiotx-0.6.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.931353 aiotx-0.6.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/clients/_utxo_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.931353 aiotx-0.6.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.931353 aiotx-0.6.0/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/utils/bep20_abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-04 17:25:12.000000 aiotx-0.6.0/aiotx/utils/erc20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.947354 aiotx-0.6.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-04 17:25:17.000000 aiotx-0.6.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-04 17:25:17.000000 aiotx-0.6.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:25:17.000000 aiotx-0.6.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-04 17:25:17.000000 aiotx-0.6.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 17:25:17.000000 aiotx-0.6.0/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.935354 aiotx-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.927353 aiotx-0.6.0/docs/clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.935354 aiotx-0.6.0/docs/clients/evm_client/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_contract_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_contract_decimals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_gas_price.rst
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_last_block.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_transaction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/get_transaction_count.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/send_token.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/evm_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.939354 aiotx-0.6.0/docs/clients/tron_client/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/tron_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/tron_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/tron_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/tron_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.939354 aiotx-0.6.0/docs/clients/utxo_client/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/utxo_client/from_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/utxo_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/utxo_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/clients/utxo_client/to_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/monitoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-04 17:25:12.000000 aiotx-0.6.0/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.939354 aiotx-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-04 17:25:12.000000 aiotx-0.6.0/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-04 17:25:12.000000 aiotx-0.6.0/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-04 17:25:12.000000 aiotx-0.6.0/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-04 17:25:12.000000 aiotx-0.6.0/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-04 17:25:12.000000 aiotx-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 17:25:12.000000 aiotx-0.6.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.939354 aiotx-0.6.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-04 17:25:12.000000 aiotx-0.6.0/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 17:25:17.947354 aiotx-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-04 17:25:12.000000 aiotx-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.939354 aiotx-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.927353 aiotx-0.6.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.927353 aiotx-0.6.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.943354 aiotx-0.6.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.943354 aiotx-0.6.0/tests/fixtures/cassettes/btc/
--rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.947354 aiotx-0.6.0/tests/fixtures/cassettes/eth/
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:25:17.947354 aiotx-0.6.0/tests/fixtures/cassettes/ltc/
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/ltc/get_last_block_with_auth.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28568 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_bsc_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_btc_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_eth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_eth_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_eth_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_ltc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-04 17:25:12.000000 aiotx-0.6.0/tests/test_ltc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.495382 aiotx-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.435382 aiotx-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-19 09:59:13.000000 aiotx-1.0.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 09:59:13.000000 aiotx-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-19 09:59:13.000000 aiotx-1.0.0/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 09:59:13.000000 aiotx-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-19 09:59:13.000000 aiotx-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-19 09:59:13.000000 aiotx-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-19 09:59:13.000000 aiotx-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-19 09:59:13.000000 aiotx-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-19 09:59:13.000000 aiotx-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-19 09:59:19.495382 aiotx-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-19 09:59:13.000000 aiotx-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.435382 aiotx-1.0.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.439382 aiotx-1.0.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18394 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/clients/_utxo_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.439382 aiotx-1.0.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.439382 aiotx-1.0.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/utils/bep20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/utils/erc20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.495382 aiotx-1.0.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.439382 aiotx-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/docs/clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/docs/clients/evm_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_contract_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_contract_decimals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_gas_price.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_last_block.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_transaction_count.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/send_token.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/docs/clients/tron_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/tron_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/tron_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/tron_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/tron_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/docs/clients/utxo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/estimate_smart_fee.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/from_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/get_last_block_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/import_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/send_bulk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/to_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/monitoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-19 09:59:13.000000 aiotx-1.0.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-19 09:59:13.000000 aiotx-1.0.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 09:59:13.000000 aiotx-1.0.0/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-19 09:59:13.000000 aiotx-1.0.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-19 09:59:13.000000 aiotx-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 09:59:13.000000 aiotx-1.0.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-19 09:59:13.000000 aiotx-1.0.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 09:59:19.495382 aiotx-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-19 09:59:13.000000 aiotx-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.447382 aiotx-1.0.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.459382 aiotx-1.0.0/tests/fixtures/cassettes/btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 10849634 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 21956267 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.487382 aiotx-1.0.0/tests/fixtures/cassettes/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.491382 aiotx-1.0.0/tests/fixtures/cassettes/ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    40578 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_bulk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    28458 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/networks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/tests/test_evm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.491382 aiotx-1.0.0/tests/test_evm/test_bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_bsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.491382 aiotx-1.0.0/tests/test_evm/test_eth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_eth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_eth/test_eth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_eth/test_eth_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_eth/test_eth_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/tests/test_utxo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.491382 aiotx-1.0.0/tests/test_utxo/test_btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_btc/test_btc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_btc/test_btc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.495382 aiotx-1.0.0/tests/test_utxo/test_ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_ltc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_ltc/test_ltc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_ltc/test_ltc_monitor.py
```

### Comparing `aiotx-0.6.0/.github/workflows/lint-check.yml` & `aiotx-1.0.0/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/.github/workflows/python-publish.yml` & `aiotx-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/.github/workflows/static.yml` & `aiotx-1.0.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/.github/workflows/test.yml` & `aiotx-1.0.0/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-# This workflow will install Python dependencies, run tests and lint with a variety of Python versions
-# For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
-
 name: Test
 
 env:
   TEST_BSC_WALLET_PRIVATE_KEY: ${{ secrets.TEST_BSC_WALLET_PRIVATE_KEY }}
   TEST_ETH_WALLET_PRIVATE_KEY: ${{ secrets.TEST_ETH_WALLET_PRIVATE_KEY }}
-  LTC_TEST_NODE_PASSWORD: ${{ secrets.LTC_TEST_NODE_PASSWORD }}
+  TEST_LTC_WALLET_PRIVATE_KEY: ${{ secrets.TEST_LTC_WALLET_PRIVATE_KEY }}
+  TEST_BTC_WALLET_PRIVATE_KEY: ${{ secrets.TEST_BTC_WALLET_PRIVATE_KEY }}
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
 jobs:
 
   build:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
+        os: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ["3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
@@ -35,14 +34,14 @@
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest pytest-cov
         pip install .[test]
 
     - name: Run tests and generate coverage
       run: |
-        pytest --cov=./ --cov-report=xml
+        pytest -m "not mysql" --cov=./ --cov-report=xml
 
     - name: Upload coverage report
       uses: actions/upload-artifact@v3
       with:
         name: coverage-report
         path: coverage.xml
```

### Comparing `aiotx-0.6.0/.gitignore` & `aiotx-1.0.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -153,10 +153,11 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
 .vscode/
-test.py
+test.py
+*.sqlite
```

### Comparing `aiotx-0.6.0/CHANGELOG.md` & `aiotx-1.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [1.0.0]
+- LTC/BTC logic and tests added
+
 ## [0.6.0]
 - UTXO client block monitoring logic added and tested for LTC and BTC (both covered by tests)
 
 ## [0.5.1]
 - EVM client docs added
 
 ## [0.5.0]
```

### Comparing `aiotx-0.6.0/CODE_OF_CONDUCT.md` & `aiotx-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/CONTRIBUTING.md` & `aiotx-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/LICENSE` & `aiotx-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/aiotx/clients/_base_client.py` & `aiotx-1.0.0/aiotx/clients/_base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,30 +30,31 @@
 
     async def get_block_by_number(self, block_number: int):
         pass
 
     async def get_last_block_number(self) -> int:
         pass
 
-class BlockMonitor:   
+
+class BlockMonitor:
     def __init__(self, client: AioTxClient):
         self.client = client
         self.block_handlers = []
         self.transaction_handlers = []
         self.running = False
         self._latest_block = None
 
     def on_block(self, func):
         self.block_handlers.append(func)
         return func
 
     def on_transaction(self, func):
         self.transaction_handlers.append(func)
         return func
-    
+
     async def __aenter__(self):
         self.running = True
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         self.stop()
 
@@ -71,8 +72,8 @@
     def stop(self):
         self.running = False
 
     async def poll_blocks(self):
         pass
 
     async def process_block(self, block):
-        pass
+        pass
```

### Comparing `aiotx-0.6.0/aiotx/clients/_evm_base_client.py` & `aiotx-1.0.0/aiotx/clients/_evm_base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,99 +50,92 @@
         self._monitoring_task = None
 
     def generate_address(self):
         private_key_bytes = secrets.token_hex(32)
         private_key = "0x" + private_key_bytes
         acct = Account.from_key(private_key)
         return private_key, acct.address
-    
+
     def get_address_from_private_key(self, private_key: str):
         try:
             from_address = Account.from_key(private_key).address
         except binascii.Error as e:
             raise WrongPrivateKey(e)
         return to_checksum_address(from_address)
-    
+
     @staticmethod
     def from_wei(number: int, unit: str) -> Union[int, decimal.Decimal]:
         return currency.from_wei(number, unit)
-    
+
     @staticmethod
     def to_wei(number: Union[int, float, str, decimal.Decimal], unit: str) -> int:
         return currency.to_wei(number, unit)
-    
+
     def _get_abi_entries(self):
         # Redefine that in you client
         return []
 
     def decode_transaction_input(self, input_data: str) -> dict:
         if input_data == "0x":
-            return {
-            'function_name': None,
-            'parameters': None
-        }
+            return {"function_name": None, "parameters": None}
         for abi_entry in self._get_abi_entries():
             function_name = abi_entry.get("name")
             if function_name is None:
                 continue
-            input_types = [inp['type'] for inp in abi_entry['inputs']]
+            input_types = [inp["type"] for inp in abi_entry["inputs"]]
             function_signature = f"{function_name}({','.join(input_types)})"
             function_selector = function_signature_to_4byte_selector(function_signature)
 
-            if input_data.startswith('0x' + function_selector.hex()):
+            if input_data.startswith("0x" + function_selector.hex()):
                 decoded_data = decode(input_types, decode_hex(input_data[10:]))
                 decoded_params = {}
                 for i, param in enumerate(decoded_data):
                     param_name = abi_entry["inputs"][i]["name"]
                     param_value = param
                     decoded_params[param_name] = param_value
 
-                return {
-                    'function_name': function_name,
-                    'parameters': decoded_params
-                }
-
-        return {
-            'function_name': None,
-            'parameters': None
-        }
+                return {"function_name": function_name, "parameters": decoded_params}
+
+        return {"function_name": None, "parameters": None}
 
     async def get_last_block_number(self) -> int:
         payload = {"method": "eth_blockNumber", "params": []}
         result = await self._make_rpc_call(payload)
         last_block = result["result"]
         return int(last_block, 16)
-    
+
     async def get_block_by_number(self, block_number: int, transaction_detail_flag: bool = True):
         payload = {"method": "eth_getBlockByNumber", "params": [hex(block_number), transaction_detail_flag]}
         result = await self._make_rpc_call(payload)
         return result
 
     async def get_balance(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
         payload = {"method": "eth_getBalance", "params": [address, block_parameter.value]}
         result = await self._make_rpc_call(payload)
         balance = result["result"]
         return 0 if balance == "0x" else int(result["result"], 16)
-    
-    async def get_contract_balance(self, address, contract_address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
+
+    async def get_contract_balance(
+        self, address, contract_address, block_parameter: BlockParam = BlockParam.LATEST
+    ) -> int:
         function_signature = "balanceOf(address)".encode("UTF-8")
         hash_result = keccak(function_signature)
         method_id = hash_result.hex()[:8]
         padded_address = address.lower().replace("0x", "").zfill(64)
         data = f"0x{method_id}{padded_address}"
 
         payload = {
-                "method": "eth_call",
-                "params": [{"to": contract_address, "data": data}, block_parameter.value],
-            }
+            "method": "eth_call",
+            "params": [{"to": contract_address, "data": data}, block_parameter.value],
+        }
 
         result = await self._make_rpc_call(payload)
         balance = result["result"]
         return 0 if balance == "0x" else int(balance, 16)
-    
+
     async def get_contract_decimals(self, contract_address) -> int:
         function_signature = "decimals()".encode("UTF-8")
         hash_result = keccak(function_signature)
         method_id = hash_result.hex()[:8]
         payload = {
             "method": "eth_call",
             "params": [{"to": contract_address, "data": f"0x{method_id}"}, "latest"],
@@ -152,32 +145,38 @@
         return 0 if decimals == "0x" else int(decimals, 16)
 
     async def get_gas_price(self) -> int:
         payload = {"method": "eth_gasPrice", "params": []}
         result = await self._make_rpc_call(payload)
         price = result["result"]
         return 0 if price == "0x" else int(result["result"], 16)
-        
+
     async def get_transaction(self, hash) -> dict:
         payload = {"method": "eth_getTransactionByHash", "params": [hash]}
         result = await self._make_rpc_call(payload)
         if result["result"] is None:
             raise TransactionNotFound(f"Transaction {hash} not found!")
         tx_data = result["result"]
         tx_data["aiotx_decoded_input"] = self.decode_transaction_input(tx_data["input"])
         return tx_data
-    
+
     async def get_transactions_count(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
         payload = {"method": "eth_getTransactionCount", "params": [address, block_parameter.value]}
         result = await self._make_rpc_call(payload)
         tx_count = result["result"]
         return 0 if tx_count == "0x" else int(tx_count, 16)
 
     async def send(
-        self, private_key: str, to_address: str, amount: int, nonce: int = None, gas_price: int = None, gas_limit: int = 21000
+        self,
+        private_key: str,
+        to_address: str,
+        amount: int,
+        nonce: int = None,
+        gas_price: int = None,
+        gas_limit: int = 21000,
     ) -> str:
         if gas_price is None:
             gas_price = await self.get_gas_price()
 
         from_address = self.get_address_from_private_key(private_key)
         if nonce is None:
             nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
@@ -270,34 +269,40 @@
                     raise VMExecutionError(error_message)
                 elif error_code == -32601:
                     if "method not found" in error_message:
                         raise MethodNotFoundError(error_message)
                     elif "failed to parse request" in error_message:
                         raise InvalidRequestError(error_message)
                 elif error_code == -32602:
-                    if "invalid argument" in error_message and "cannot unmarshal hex string without 0x prefix" in error_message or "cannot unmarshal hex string of odd length into" in error_message or "hex string has length" in error_message:
+                    if (
+                        "invalid argument" in error_message
+                        and "cannot unmarshal hex string without 0x prefix" in error_message
+                        or "cannot unmarshal hex string of odd length into" in error_message
+                        or "hex string has length" in error_message
+                    ):
                         raise InvalidArgumentError(error_message)
                     elif "eth_getLogs and eth_newFilter are limited to a 10,000 blocks range" in error_message:
                         raise BlockRangeLimitExceededError(error_message)
                 elif error_code == -32603:
                     raise InternalJSONRPCError(error_message)
                 else:
                     raise AioTxError(f"Error {error_code}: {error_message}")
-                
 
-                
+
 class EvmMonitor(BlockMonitor):
     def __init__(self, client: AioTxEVMClient):
         self.client = client
         self.block_handlers = []
         self.transaction_handlers = []
         self.running = False
         self._latest_block = None
 
-    async def poll_blocks(self,):
+    async def poll_blocks(
+        self,
+    ):
         if self._latest_block is None:
             self._latest_block = await self.client.get_last_block_number()
         block = await self.client.get_block_by_number(self._latest_block)
         await self.process_block(block["result"])
         self._latest_block = self._latest_block + 1
 
     async def process_block(self, block):
```

### Comparing `aiotx-0.6.0/aiotx/exceptions.py` & `aiotx-1.0.0/aiotx/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,85 @@
 class AioTxError(Exception):
     """
     Base exception for all aiotx errors.
     """
+
+
 class BlockNotFoundError(AioTxError):
     pass
 
+
 class InternalJSONRPCError(AioTxError):
     pass
 
+
 class StackLimitReachedError(AioTxError):
     pass
 
+
 class MethodHandlerCrashedError(AioTxError):
     pass
 
+
 class ExecutionTimeoutError(AioTxError):
     pass
 
+
 class NonceTooLowError(AioTxError):
     pass
 
+
 class FilterNotFoundError(AioTxError):
     pass
 
+
 class TraceRequestLimitExceededError(AioTxError):
     pass
 
+
 class TransactionCostExceedsGasLimitError(AioTxError):
     pass
 
+
 class NetworkError(AioTxError):
     pass
 
+
 class VMExecutionError(AioTxError):
     pass
 
+
 class MethodNotFoundError(AioTxError):
     pass
 
+
 class InvalidRequestError(AioTxError):
     pass
 
+
 class InvalidArgumentError(AioTxError):
     pass
 
+
 class BlockRangeLimitExceededError(AioTxError):
     pass
 
+
 class InternalJSONAioTxError(AioTxError):
     pass
 
+
 class TransactionNotFound(AioTxError):
     pass
 
+
 class ReplacementTransactionUnderpriced(AioTxError):
     pass
 
+
 class WrongPrivateKey(AioTxError):
-    pass
+    pass
+
+
+class InsufficientFunds(AioTxError):
+    pass
+
```

### Comparing `aiotx-0.6.0/aiotx/utils/bep20_abi.json` & `aiotx-1.0.0/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/aiotx/utils/erc20_abi.json` & `aiotx-1.0.0/aiotx/utils/erc20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/aiotx.egg-info/SOURCES.txt` & `aiotx-1.0.0/aiotx.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 aiotx.egg-info/requires.txt
 aiotx.egg-info/top_level.txt
 aiotx/clients/__init__.py
 aiotx/clients/_base_client.py
 aiotx/clients/_evm_base_client.py
 aiotx/clients/_utxo_base_client.py
 aiotx/types/__init__.py
+aiotx/utils/__init__.py
 aiotx/utils/bep20_abi.json
 aiotx/utils/erc20_abi.json
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/monitoring.rst
@@ -47,56 +48,84 @@
 docs/clients/evm_client/send.rst
 docs/clients/evm_client/send_token.rst
 docs/clients/evm_client/to_wei.rst
 docs/clients/tron_client/from_wei.rst
 docs/clients/tron_client/generate_address.rst
 docs/clients/tron_client/index.rst
 docs/clients/tron_client/to_wei.rst
+docs/clients/utxo_client/estimate_smart_fee.rst
 docs/clients/utxo_client/from_satoshi.rst
 docs/clients/utxo_client/generate_address.rst
+docs/clients/utxo_client/get_address_from_private_key.rst
+docs/clients/utxo_client/get_balance.rst
+docs/clients/utxo_client/get_block_by_number.rst
+docs/clients/utxo_client/get_last_block_number.rst
+docs/clients/utxo_client/import_address.rst
 docs/clients/utxo_client/index.rst
+docs/clients/utxo_client/send.rst
+docs/clients/utxo_client/send_bulk.rst
 docs/clients/utxo_client/to_satoshi.rst
 examples/aiogram_notificator_bot.png
 examples/aiogram_notificator_bot.py
 examples/block_and_transactions_parser.py
 examples/two_block_parsers.py
 scripts/build_and_test.sh
 tests/conftest.py
-tests/test_bsc_client.py
-tests/test_bsc_input_decoding.py
-tests/test_bsc_monitoring.py
-tests/test_btc_monitor.py
-tests/test_eth_client.py
-tests/test_eth_input_decoding.py
-tests/test_eth_monitoring.py
-tests/test_ltc_client.py
-tests/test_ltc_monitor.py
+tests/fixtures/networks.json
 tests/fixtures/cassettes/bsc/get_balance.yaml
 tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
 tests/fixtures/cassettes/bsc/get_gas_price.yaml
 tests/fixtures/cassettes/bsc/get_last_block.yaml
 tests/fixtures/cassettes/bsc/get_token_balance.yaml
 tests/fixtures/cassettes/bsc/get_transaction.yaml
 tests/fixtures/cassettes/bsc/get_transaction_count.yaml
 tests/fixtures/cassettes/bsc/send_token_transaction.yaml
 tests/fixtures/cassettes/bsc/send_transaction.yaml
 tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
 tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
 tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
+tests/fixtures/cassettes/btc/send_transaction.yaml
+tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
 tests/fixtures/cassettes/btc/test_async_monitoring.yaml
+tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
 tests/fixtures/cassettes/eth/get_balance.yaml
 tests/fixtures/cassettes/eth/get_contract_decimals.yaml
 tests/fixtures/cassettes/eth/get_gas_price.yaml
 tests/fixtures/cassettes/eth/get_last_block.yaml
 tests/fixtures/cassettes/eth/get_token_balance.yaml
 tests/fixtures/cassettes/eth/get_transaction.yaml
 tests/fixtures/cassettes/eth/get_transaction_count.yaml
 tests/fixtures/cassettes/eth/send_token_transaction.yaml
 tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
 tests/fixtures/cassettes/eth/send_transaction.yaml
 tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
 tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
 tests/fixtures/cassettes/eth/test_async_monitoring.yaml
+tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
 tests/fixtures/cassettes/ltc/get_block_by_number.yaml
 tests/fixtures/cassettes/ltc/get_last_block.yaml
-tests/fixtures/cassettes/ltc/get_last_block_with_auth.yaml
-tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
+tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
+tests/fixtures/cassettes/ltc/send_bulk.yaml
+tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
+tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
+tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
+tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
+tests/fixtures/cassettes/ltc/send_transaction.yaml
+tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
+tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
+tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
+tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
+tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
+tests/test_evm/test_bsc/__init__.py
+tests/test_evm/test_bsc/test_bsc_client.py
+tests/test_evm/test_bsc/test_bsc_input_decoding.py
+tests/test_evm/test_bsc/test_bsc_monitoring.py
+tests/test_evm/test_eth/__init__.py
+tests/test_evm/test_eth/test_eth_client.py
+tests/test_evm/test_eth/test_eth_input_decoding.py
+tests/test_evm/test_eth/test_eth_monitoring.py
+tests/test_utxo/test_btc/test_btc_client.py
+tests/test_utxo/test_btc/test_btc_monitor.py
+tests/test_utxo/test_ltc/__init__.py
+tests/test_utxo/test_ltc/test_ltc_client.py
+tests/test_utxo/test_ltc/test_ltc_monitor.py
```

### Comparing `aiotx-0.6.0/docs/Makefile` & `aiotx-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/get_balance.rst` & `aiotx-1.0.0/docs/clients/evm_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/get_block_by_number.rst` & `aiotx-1.0.0/docs/clients/evm_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/get_contract_balance.rst` & `aiotx-1.0.0/docs/clients/evm_client/get_contract_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/get_contract_decimals.rst` & `aiotx-1.0.0/docs/clients/evm_client/get_contract_decimals.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/get_transaction.rst` & `aiotx-1.0.0/docs/clients/evm_client/get_transaction.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/get_transaction_count.rst` & `aiotx-1.0.0/docs/clients/evm_client/get_transaction_count.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/index.rst` & `aiotx-1.0.0/docs/clients/evm_client/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/send.rst` & `aiotx-1.0.0/docs/clients/evm_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/clients/evm_client/send_token.rst` & `aiotx-1.0.0/docs/clients/evm_client/send_token.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/conf.py` & `aiotx-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/make.bat` & `aiotx-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/docs/monitoring.rst` & `aiotx-1.0.0/docs/monitoring.rst`

 * *Files 12% similar despite different names*

```diff
@@ -57,27 +57,27 @@
     from aiotx.clients import AioTxBSCClient, AioTxETHClient
     import asyncio
 
     bsc_client = AioTxBSCClient("NODE_URL", 97)
     eth_client = AioTxETHClient("NODE_URL", 1151511)
 
     @bsc_client.monitor.on_block
-    def handle_block(block):
+    async def handle_block(block):
         print("bsc_client: block", block)
 
     @bsc_client.monitor.on_transaction
-    def handle_transaction(transaction):
+    async def handle_transaction(transaction):
         print("bsc_client: transaction", transaction)
 
     @eth_client.monitor.on_block
-    def handle_block(block):
+    async def handle_block(block):
         print("eth_client: block", block)
 
     @eth_client.monitor.on_transaction
-    def handle_transaction(transaction):
+    async def handle_transaction(transaction):
         print("eth_client: transaction", transaction)
 
     async def main():
         bsc_task = asyncio.create_task(bsc_client.start_monitoring())
         eth_task = asyncio.create_task(eth_client.start_monitoring())
         await asyncio.gather(bsc_task, eth_task)
```

### Comparing `aiotx-0.6.0/docs/testing.rst` & `aiotx-1.0.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/examples/aiogram_notificator_bot.png` & `aiotx-1.0.0/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/examples/aiogram_notificator_bot.py` & `aiotx-1.0.0/examples/aiogram_notificator_bot.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/examples/block_and_transactions_parser.py` & `aiotx-1.0.0/examples/block_and_transactions_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from aiotx.clients import AioTxBSCClient
 import asyncio
 
 client = AioTxBSCClient("NODE_URL", 97)
 
 @client.monitor.on_block
-def handle_block(block):
+async def handle_block(block):
     print("block", block)
 
 @client.monitor.on_transaction
-def handle_transaction(transaction):
+async def handle_transaction(transaction):
     print("transaction", transaction)
 
 
 async def main():
     await client.start_monitoring()
 
     try:
```

### Comparing `aiotx-0.6.0/examples/two_block_parsers.py` & `aiotx-1.0.0/examples/two_block_parsers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from aiotx.clients import AioTxBSCClient, AioTxETHClient
 import asyncio
 
 bsc_client = AioTxBSCClient("NODE_URL", 97)
 eth_client = AioTxETHClient("NODE_URL", 1151511)
 
 @bsc_client.monitor.on_block
-def handle_block(block):
+async def handle_block(block):
     print("bsc_client: block", block)
 
 @bsc_client.monitor.on_transaction
-def handle_transaction(transaction):
+async def handle_transaction(transaction):
     print("bsc_client: transaction", transaction)
 
 @eth_client.monitor.on_block
-def handle_block(block):
+async def handle_block(block):
     print("eth_client: block", block)
 
 @eth_client.monitor.on_transaction
-def handle_transaction(transaction):
+async def handle_transaction(transaction):
     print("eth_client: transaction", transaction)
 
 async def main():
     monitoring_task1 = asyncio.create_task(bsc_client.start_monitoring(584))
     monitoring_task2 = asyncio.create_task(eth_client.start_monitoring(900))
     await asyncio.gather(monitoring_task1, monitoring_task2)
```

### Comparing `aiotx-0.6.0/setup.py` & `aiotx-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,22 @@
     setup_requires=[
         "setuptools_scm",
     ],
     install_requires=[
         "aiohttp",
         "eth_keys",
         "eth_utils",
-        "eth_account"
+        "eth_account",
+        "sqlalchemy",
+        "aiosqlite",
+        "aiomysql",
+        "cryptography",
+        "ecdsa",
+        "bitcoinlib",
+        "greenlet"
     ],
     extras_require={
         "test": extras_test,
     },
     url="https://github.com/Grommash9/aiotx",
     project_urls={
         'Documentation': 'https://grommash9.github.io/aiotx/',
```

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/get_balance.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/get_gas_price.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/get_last_block.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/get_token_balance.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/get_transaction.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/send_transaction.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/ltc/get_last_block.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/ltc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml` & `aiotx-1.0.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 interactions:
 - request:
-    body: '{"method": "getblockhash", "params": [3247853], "jsonrpc": "2.0", "id":
-      "curltest"}'
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","error":null,"id":"curltest"}'
+      string: '{"result":3248792,"error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87e9510a4d30940b-LHR
+      - 87f6ea286fb49584-LHR
       Connection:
       - keep-alive
-      Content-Encoding:
-      - gzip
+      Content-Length:
+      - '47'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Sat, 04 May 2024 14:52:47 GMT
+      - Mon, 06 May 2024 06:29:13 GMT
       Etag:
-      - W/"6a-LkLLyOVV1TG/alYlITH3LlU0UyM"
+      - W/"2f-VGszqwZqefFJmjtjv2jYlBzuGQ4"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=g08LR0FG9%2BsNlTNwRpNSmZ8AHLjCC9GCXpVEyzeeCSxA%2Fl4MmA%2B0hX98KJbntHlTd0yxMuPy3Ytt79481ri8lnyf31fa2paQo%2FNRbtoKXuy0NmuKQYn5smcTh6iwCdQ%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=3mKegiq2qgcHOYTxb5KA7FTjeROz6mf2XnvIERoT1BqRNgZJdtldiO6KooG5PSkAT1DJ9ELgooU8OMM51KrtEO7%2BBkDMBO3i9E%2FDVVQ9XtuolbGnPV1Rs19hqjosHD4%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
-      Transfer-Encoding:
-      - chunked
       Via:
       - 1.1 google
       alt-svc:
       - h3=":443"; ma=86400
       content-security-policy:
       - 'default-src ''self'';base-uri ''self'';block-all-mixed-content;font-src ''self''
         https: data:;frame-ancestors ''self'';img-src ''self'' data:;object-src ''none'';script-src
@@ -63,54 +60,47 @@
       - '3'
       x-xss-protection:
       - '0'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "getblock", "params": ["b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b",
-      2], "jsonrpc": "2.0", "id": "curltest"}'
+    body: '{"method": "getblockhash", "params": [3247853], "jsonrpc": "2.0", "id":
+      "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":{"hash":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","confirmations":7,"strippedsize":464,"size":890,"weight":2108,"height":3247853,"version":536870912,"versionHex":"20000000","merkleroot":"983577cb9a5f6d9e0cf17c04a5c330e2a9cd5e54e365b4ecb567e33dee075604","tx":[{"txid":"7604930759225ab74868969da6b19b399d8b189bd9506f39e15019f8e08a1d44","hash":"80a7072798f45aa72450e348c719e169ce72a49995105b927971eae7b4c58732","version":2,"size":171,"vsize":144,"weight":576,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ed8e310101","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"ismweb":false,"value":6.25002728,"n":0,"scriptPubKey":{"asm":"0
-        7bd19b7434e4d9c93c534621c23c5eba8a35c187","hex":"00147bd19b7434e4d9c93c534621c23c5eba8a35c187","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q00gekap5unvuj0zngcsuy0z7h29rtsv8d6xwsj"]}},{"ismweb":false,"value":0,"n":1,"scriptPubKey":{"asm":"OP_RETURN
-        aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d","hex":"6a24aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d","type":"nulldata"}}],"hex":"020000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff0603ed8e310101ffffffff02e8c84025000000001600147bd19b7434e4d9c93c534621c23c5eba8a35c1870000000000000000266a24aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d0120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"51d57f58f3ede964f0105e6a01795cc0df6f275ba4e5d408bc3ba7b57448f74b","hash":"a62d6fb8666b94654acbcf5a541c1848e712af9f96fed8197c0a7b482b3c9802","version":1,"size":370,"vsize":208,"weight":832,"locktime":0,"vin":[{"ismweb":false,"txid":"6b0f1847a67c6d4d40bd557324db7f0258a1d555d3176e666d2420730078c635","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["304402206debc508ebab4d24441cb85fd818c442eb3b803fd5af5fc2c4f5d8ddfae84b64022061b01a7345e8ae0e7558c446e5b9e80afd2f22250aa02f8f70f7c0af29f4ff0d01","035bc96345ad6257836f8c0267a067ac6bd3c9f7dd413f23330cc4f64248977e34"],"sequence":4294967295},{"ismweb":false,"txid":"6b0f1847a67c6d4d40bd557324db7f0258a1d555d3176e666d2420730078c635","vout":1,"scriptSig":{"asm":"","hex":""},"txinwitness":["3044022044c1e352b24403724f97b1d129bbc926a9b5b80fb743b3eeac6f119ee3ca4e5102204abcbc25491be3c6724720dd54cf6ec1e40831fb45fb554f809b92c57fc44fb701","02a1559f3b65652e92b529a5acc64cd9000a6eaa24531f61a7f928028fa3a87ac6"],"sequence":4294967295}],"vout":[{"ismweb":false,"value":6.69379664,"n":0,"scriptPubKey":{"asm":"0
-        3efcd669a05d842fb1b05ec45b3b946b8f55774d","hex":"00143efcd669a05d842fb1b05ec45b3b946b8f55774d","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q8m7dv6dqtkzzlvdstmz9kwu5dw842a6d7hd5fr"]}},{"ismweb":false,"value":0.00407272,"n":1,"scriptPubKey":{"asm":"0
-        abd50c308b9563c615aeb0eb00752925ab2ff279","hex":"0014abd50c308b9563c615aeb0eb00752925ab2ff279","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q402scvytj43uv9dwkr4sqaffyk4jlunet2cwyg"]}}],"hex":"0100000000010235c678007320246d666e17d355d5a158027fdb247355bd404d6d7ca647180f6b0000000000ffffffff35c678007320246d666e17d355d5a158027fdb247355bd404d6d7ca647180f6b0100000000ffffffff0250ece527000000001600143efcd669a05d842fb1b05ec45b3b946b8f55774de836060000000000160014abd50c308b9563c615aeb0eb00752925ab2ff2790247304402206debc508ebab4d24441cb85fd818c442eb3b803fd5af5fc2c4f5d8ddfae84b64022061b01a7345e8ae0e7558c446e5b9e80afd2f22250aa02f8f70f7c0af29f4ff0d0121035bc96345ad6257836f8c0267a067ac6bd3c9f7dd413f23330cc4f64248977e3402473044022044c1e352b24403724f97b1d129bbc926a9b5b80fb743b3eeac6f119ee3ca4e5102204abcbc25491be3c6724720dd54cf6ec1e40831fb45fb554f809b92c57fc44fb7012102a1559f3b65652e92b529a5acc64cd9000a6eaa24531f61a7f928028fa3a87ac600000000"},{"txid":"155b9bd93528a805975d549b8891c1de468cdcbf3c41b7cb22042cb6c58417fe","hash":"155b9bd93528a805975d549b8891c1de468cdcbf3c41b7cb22042cb6c58417fe","version":2,"size":97,"vsize":94,"weight":376,"locktime":0,"vin":[{"ismweb":false,"txid":"acee20a3c85c660599447e1f6c298f5009b47622303db4bc6cd3b79e4fea96d3","vout":0,"scriptSig":{"asm":"","hex":""},"sequence":4294967295}],"vout":[{"ismweb":false,"value":1791337.37993343,"n":0,"scriptPubKey":{"asm":"8
-        a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","hex":"5820a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","type":"witness_mweb_hogaddr"}}],"hex":"02000000000801d396ea4f9eb7d36cbcb43d302276b409508f296c1f7e449905665cc8a320eeac0000000000ffffffff017f04d2d2eba20000225820a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d570000000000"}],"time":1714833888,"mediantime":1714833364,"nonce":44487,"bits":"1e044362","difficulty":0.000916254800568373,"chainwork":"00000000000000000000000000000000000000000000000000c3adb1cb5e171c","nTx":3,"mweb":{"hash":"a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","height":3247853,"kernel_offset":"9a966bcbe6fcf6b94d7428142a0027b004b1af6a28f2f1999e3d21a565ddb187","stealth_offset":"0000000000000000000000000000000000000000000000000000000000000000","num_kernels":0,"num_txos":4722,"kernel_root":"0000000000000000000000000000000000000000000000000000000000000000","output_root":"69f9f4774c9afd3dab444bbad6df6ae0dcb2c5d6051b5054d7b306a0d348f3c4","leaf_root":"2551128703060a6d3002845179551621ff1d77ce9055933276092f9e7ba97382","inputs":[],"outputs":[],"kernels":[]},"previousblockhash":"c6f01ca05384915909b49a16cfd4a5ea6ec986b1b376c0d31a2fbdc0967d5cb8","nextblockhash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06"},"error":null,"id":"curltest"}'
+      string: '{"result":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87e9510c5b016431-LHR
+      - 87f6ea2a9c4c48b6-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Sat, 04 May 2024 14:52:47 GMT
+      - Mon, 06 May 2024 06:29:14 GMT
       Etag:
-      - W/"15e6-9Qyr98buo+rsutuIkzu6dj62Ybo"
+      - W/"6a-LkLLyOVV1TG/alYlITH3LlU0UyM"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=YDcuIS7kQwNKPeyQLxkXd1fPleTkLfX%2BvWms7vpwvinf5QyPzgEffDJbiSjQ3QzDvHHFkenbYtTf4kgyg3BWBPw%2FNGI%2BXcIEgo4%2BqrOHssI5oInLalwo%2Fl574PiAs6k%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=FlILk8NoWcZgWdQHshepcJ7TNqS1znvPL%2BilXeDW9AGiQWMZmtn5DbgSHHMR0VkA%2BD58oSgHOyz%2FV88lbjCl7%2FfK3%2FDGIDNe3Cx%2BnBdaI6wSh3bwmvJlmwBPtGVV6ck%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
-      Vary:
-      - Accept-Encoding
       Via:
       - 1.1 google
       alt-svc:
       - h3=":443"; ma=86400
       content-security-policy:
       - 'default-src ''self'';base-uri ''self'';block-all-mixed-content;font-src ''self''
         https: data:;frame-ancestors ''self'';img-src ''self'' data:;object-src ''none'';script-src
@@ -137,47 +127,54 @@
       - '3'
       x-xss-protection:
       - '0'
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "getblockhash", "params": [3247853], "jsonrpc": "2.0", "id":
-      "curltest"}'
+    body: '{"method": "getblock", "params": ["b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b",
+      2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","error":null,"id":"curltest"}'
+      string: '{"result":{"hash":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","confirmations":940,"strippedsize":464,"size":890,"weight":2108,"height":3247853,"version":536870912,"versionHex":"20000000","merkleroot":"983577cb9a5f6d9e0cf17c04a5c330e2a9cd5e54e365b4ecb567e33dee075604","tx":[{"txid":"7604930759225ab74868969da6b19b399d8b189bd9506f39e15019f8e08a1d44","hash":"80a7072798f45aa72450e348c719e169ce72a49995105b927971eae7b4c58732","version":2,"size":171,"vsize":144,"weight":576,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ed8e310101","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"ismweb":false,"value":6.25002728,"n":0,"scriptPubKey":{"asm":"0
+        7bd19b7434e4d9c93c534621c23c5eba8a35c187","hex":"00147bd19b7434e4d9c93c534621c23c5eba8a35c187","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q00gekap5unvuj0zngcsuy0z7h29rtsv8d6xwsj"]}},{"ismweb":false,"value":0,"n":1,"scriptPubKey":{"asm":"OP_RETURN
+        aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d","hex":"6a24aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d","type":"nulldata"}}],"hex":"020000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff0603ed8e310101ffffffff02e8c84025000000001600147bd19b7434e4d9c93c534621c23c5eba8a35c1870000000000000000266a24aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d0120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"51d57f58f3ede964f0105e6a01795cc0df6f275ba4e5d408bc3ba7b57448f74b","hash":"a62d6fb8666b94654acbcf5a541c1848e712af9f96fed8197c0a7b482b3c9802","version":1,"size":370,"vsize":208,"weight":832,"locktime":0,"vin":[{"ismweb":false,"txid":"6b0f1847a67c6d4d40bd557324db7f0258a1d555d3176e666d2420730078c635","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["304402206debc508ebab4d24441cb85fd818c442eb3b803fd5af5fc2c4f5d8ddfae84b64022061b01a7345e8ae0e7558c446e5b9e80afd2f22250aa02f8f70f7c0af29f4ff0d01","035bc96345ad6257836f8c0267a067ac6bd3c9f7dd413f23330cc4f64248977e34"],"sequence":4294967295},{"ismweb":false,"txid":"6b0f1847a67c6d4d40bd557324db7f0258a1d555d3176e666d2420730078c635","vout":1,"scriptSig":{"asm":"","hex":""},"txinwitness":["3044022044c1e352b24403724f97b1d129bbc926a9b5b80fb743b3eeac6f119ee3ca4e5102204abcbc25491be3c6724720dd54cf6ec1e40831fb45fb554f809b92c57fc44fb701","02a1559f3b65652e92b529a5acc64cd9000a6eaa24531f61a7f928028fa3a87ac6"],"sequence":4294967295}],"vout":[{"ismweb":false,"value":6.69379664,"n":0,"scriptPubKey":{"asm":"0
+        3efcd669a05d842fb1b05ec45b3b946b8f55774d","hex":"00143efcd669a05d842fb1b05ec45b3b946b8f55774d","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q8m7dv6dqtkzzlvdstmz9kwu5dw842a6d7hd5fr"]}},{"ismweb":false,"value":0.00407272,"n":1,"scriptPubKey":{"asm":"0
+        abd50c308b9563c615aeb0eb00752925ab2ff279","hex":"0014abd50c308b9563c615aeb0eb00752925ab2ff279","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q402scvytj43uv9dwkr4sqaffyk4jlunet2cwyg"]}}],"hex":"0100000000010235c678007320246d666e17d355d5a158027fdb247355bd404d6d7ca647180f6b0000000000ffffffff35c678007320246d666e17d355d5a158027fdb247355bd404d6d7ca647180f6b0100000000ffffffff0250ece527000000001600143efcd669a05d842fb1b05ec45b3b946b8f55774de836060000000000160014abd50c308b9563c615aeb0eb00752925ab2ff2790247304402206debc508ebab4d24441cb85fd818c442eb3b803fd5af5fc2c4f5d8ddfae84b64022061b01a7345e8ae0e7558c446e5b9e80afd2f22250aa02f8f70f7c0af29f4ff0d0121035bc96345ad6257836f8c0267a067ac6bd3c9f7dd413f23330cc4f64248977e3402473044022044c1e352b24403724f97b1d129bbc926a9b5b80fb743b3eeac6f119ee3ca4e5102204abcbc25491be3c6724720dd54cf6ec1e40831fb45fb554f809b92c57fc44fb7012102a1559f3b65652e92b529a5acc64cd9000a6eaa24531f61a7f928028fa3a87ac600000000"},{"txid":"155b9bd93528a805975d549b8891c1de468cdcbf3c41b7cb22042cb6c58417fe","hash":"155b9bd93528a805975d549b8891c1de468cdcbf3c41b7cb22042cb6c58417fe","version":2,"size":97,"vsize":94,"weight":376,"locktime":0,"vin":[{"ismweb":false,"txid":"acee20a3c85c660599447e1f6c298f5009b47622303db4bc6cd3b79e4fea96d3","vout":0,"scriptSig":{"asm":"","hex":""},"sequence":4294967295}],"vout":[{"ismweb":false,"value":1791337.37993343,"n":0,"scriptPubKey":{"asm":"8
+        a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","hex":"5820a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","type":"witness_mweb_hogaddr"}}],"hex":"02000000000801d396ea4f9eb7d36cbcb43d302276b409508f296c1f7e449905665cc8a320eeac0000000000ffffffff017f04d2d2eba20000225820a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d570000000000"}],"time":1714833888,"mediantime":1714833364,"nonce":44487,"bits":"1e044362","difficulty":0.000916254800568373,"chainwork":"00000000000000000000000000000000000000000000000000c3adb1cb5e171c","nTx":3,"mweb":{"hash":"a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","height":3247853,"kernel_offset":"9a966bcbe6fcf6b94d7428142a0027b004b1af6a28f2f1999e3d21a565ddb187","stealth_offset":"0000000000000000000000000000000000000000000000000000000000000000","num_kernels":0,"num_txos":4722,"kernel_root":"0000000000000000000000000000000000000000000000000000000000000000","output_root":"69f9f4774c9afd3dab444bbad6df6ae0dcb2c5d6051b5054d7b306a0d348f3c4","leaf_root":"2551128703060a6d3002845179551621ff1d77ce9055933276092f9e7ba97382","inputs":[],"outputs":[],"kernels":[]},"previousblockhash":"c6f01ca05384915909b49a16cfd4a5ea6ec986b1b376c0d31a2fbdc0967d5cb8","nextblockhash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06"},"error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87e951199cc777a8-LHR
+      - 87f6ea2b5db9547b-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Sat, 04 May 2024 14:52:49 GMT
+      - Mon, 06 May 2024 06:29:14 GMT
       Etag:
-      - W/"6a-LkLLyOVV1TG/alYlITH3LlU0UyM"
+      - W/"15e8-Y8Jmn48qDfT1hdy5kmmKkqtbpw0"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=MH0l4qR%2BFKMJIKQqhDcTYqGqkUD4q6jz5IePrsJtPnMof3EoHHYvEO%2BxqOOTBQgnupYdsOBzkxw8UU4IIBpW53f3Wl85c3n1XAgsIDzapwFaLJ5h8Tx%2FxBrsv5LQo0M%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=w97rJhafQV1sjGEuzKiHBJwLDqoYDNlsYQCUrqlj1r32L9Wr3HBSn3NGR6Ii98y6xJDrWGi2APMOEix9Wyme%2F%2FQOZL%2BzWqbt2PPJAAa3xI86Rycf6QHYddhvBM9nP6U%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      Vary:
+      - Accept-Encoding
       Via:
       - 1.1 google
       alt-svc:
       - h3=":443"; ma=86400
       content-security-policy:
       - 'default-src ''self'';base-uri ''self'';block-all-mixed-content;font-src ''self''
         https: data:;frame-ancestors ''self'';img-src ''self'' data:;object-src ''none'';script-src
@@ -218,29 +215,29 @@
       string: '{"result":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06","error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87e951cacf76dd79-LHR
+      - 87f6ea326ac160f6-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Sat, 04 May 2024 14:53:17 GMT
+      - Mon, 06 May 2024 06:29:15 GMT
       Etag:
       - W/"6a-AlT1INyeQ1FXH50qhJDUOe3VEos"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=oi9cCqJ%2FUvI5XRLJ9nSenAr0IcrnWnDwh5qH3rAGrbwRqrPKIzagY56pdpFtts1mpOCxyn7GhK5mjCws0UQr%2FOXp0%2FRr6PpwQUeOk9eqoM%2FUQjKVQMdK8umYZaOo3qc%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=F2K6fwjENosOf%2F0nAJ4EZY3Hd7IOhsFLzZi2K8oEXaFtR%2FI1hUDbBf0CpPVO6CuAh6SVzcJpTZ%2B9aqyxWrbE7d8rgnicLXf9TLjE%2FvojR4x5o88objfa9gEr0PKauxk%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Via:
       - 1.1 google
       alt-svc:
@@ -278,40 +275,40 @@
     body: '{"method": "getblock", "params": ["6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":{"hash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06","confirmations":6,"strippedsize":435,"size":645,"weight":1776,"height":3247854,"version":536870912,"versionHex":"20000000","merkleroot":"9e036e586c8202e96cfbd92437e113ed23359a1e071cfc040dd3432e6fdce386","tx":[{"txid":"40d43cdee20338c0002597d00d52daadc66fb4e8a6af9a002c1da84ca7cfb170","hash":"ec1d51a86c4111648da61cb2a7755c46e999ce012d381eae0000fe393255ab8d","version":1,"size":296,"vsize":269,"weight":1076,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ee8e3104e94936660861803ced00000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":0}],"vout":[{"ismweb":false,"value":6.249375,"n":0,"scriptPubKey":{"asm":"0
+      string: '{"result":{"hash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06","confirmations":939,"strippedsize":435,"size":645,"weight":1776,"height":3247854,"version":536870912,"versionHex":"20000000","merkleroot":"9e036e586c8202e96cfbd92437e113ed23359a1e071cfc040dd3432e6fdce386","tx":[{"txid":"40d43cdee20338c0002597d00d52daadc66fb4e8a6af9a002c1da84ca7cfb170","hash":"ec1d51a86c4111648da61cb2a7755c46e999ce012d381eae0000fe393255ab8d","version":1,"size":296,"vsize":269,"weight":1076,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ee8e3104e94936660861803ced00000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":0}],"vout":[{"ismweb":false,"value":6.249375,"n":0,"scriptPubKey":{"asm":"0
         94a1914d5e14ba06b02bb9d2b0b672f2fd125415","hex":"001494a1914d5e14ba06b02bb9d2b0b672f2fd125415","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1qjjsezn27zjaqdvpth8ftpdnj7t73y4q4vja4dq"]}},{"ismweb":false,"value":0.000625,"n":1,"scriptPubKey":{"asm":"OP_DUP
         OP_HASH160 684a4a9d1c027eddb12029e40ccd86215360790a OP_EQUALVERIFY OP_CHECKSIG","hex":"76a914684a4a9d1c027eddb12029e40ccd86215360790a88ac","reqSigs":1,"type":"pubkeyhash","addresses":["mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX"]}},{"ismweb":false,"value":0,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9ede746e1e45c418a43d974963c15c7d4ecd9e02232cf06849f9d091b841f001746","hex":"6a24aa21a9ede746e1e45c418a43d974963c15c7d4ecd9e02232cf06849f9d091b841f001746","type":"nulldata"}}],"hex":"010000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff6103ee8e3104e94936660861803ced00000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f00000000031cca3f250000000016001494a1914d5e14ba06b02bb9d2b0b672f2fd12541524f40000000000001976a914684a4a9d1c027eddb12029e40ccd86215360790a88ac0000000000000000266a24aa21a9ede746e1e45c418a43d974963c15c7d4ecd9e02232cf06849f9d091b841f0017460120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"992b887a10aa924430e905174535fd92733136b76d39e835c109e3ff2719bd69","hash":"992b887a10aa924430e905174535fd92733136b76d39e835c109e3ff2719bd69","version":2,"size":97,"vsize":94,"weight":376,"locktime":0,"vin":[{"ismweb":false,"txid":"155b9bd93528a805975d549b8891c1de468cdcbf3c41b7cb22042cb6c58417fe","vout":0,"scriptSig":{"asm":"","hex":""},"sequence":4294967295}],"vout":[{"ismweb":false,"value":1791337.37993343,"n":0,"scriptPubKey":{"asm":"8
         086024bcc947aadc5053e0a51bcaabf1f7b4c264904fb72fa3f05c47dfb7575e","hex":"5820086024bcc947aadc5053e0a51bcaabf1f7b4c264904fb72fa3f05c47dfb7575e","type":"witness_mweb_hogaddr"}}],"hex":"02000000000801fe1784c5b62c0422cbb7413cbfdc8c46dec191889b545d9705a82835d99b5b150000000000ffffffff017f04d2d2eba20000225820086024bcc947aadc5053e0a51bcaabf1f7b4c264904fb72fa3f05c47dfb7575e0000000000"}],"time":1714833897,"mediantime":1714833369,"nonce":945226240,"bits":"1e044362","difficulty":0.000916254800568373,"chainwork":"00000000000000000000000000000000000000000000000000c3adb1cb9a238c","nTx":2,"mweb":{"hash":"086024bcc947aadc5053e0a51bcaabf1f7b4c264904fb72fa3f05c47dfb7575e","height":3247854,"kernel_offset":"9a966bcbe6fcf6b94d7428142a0027b004b1af6a28f2f1999e3d21a565ddb187","stealth_offset":"0000000000000000000000000000000000000000000000000000000000000000","num_kernels":0,"num_txos":4722,"kernel_root":"0000000000000000000000000000000000000000000000000000000000000000","output_root":"69f9f4774c9afd3dab444bbad6df6ae0dcb2c5d6051b5054d7b306a0d348f3c4","leaf_root":"2551128703060a6d3002845179551621ff1d77ce9055933276092f9e7ba97382","inputs":[],"outputs":[],"kernels":[]},"previousblockhash":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","nextblockhash":"2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9"},"error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87e951cb8975654c-LHR
+      - 87f6ea33a90c48cd-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Sat, 04 May 2024 14:53:18 GMT
+      - Mon, 06 May 2024 06:29:15 GMT
       Etag:
-      - W/"fd4-OoJLAHKHhjQAK7I5AQHtX2CHwjc"
+      - W/"fd6-Vp1fkFZYOYkVcldYilDUrhCFXAk"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=fmTljGzbPbQAGI6j5r2anhgl8dSP5Ef2P4jDKJdIerxMs5twuZ2anDIP8roFuOrkUr68iKlN2IF0TbiQveq17Ex3sCQQm2GSM3LDx96p4ZfP5edVHwnRUn79B2dz3Ks%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=BeP6quUsHMcNjjfd3xE1Ea1dB6CQVsmxrHGY5yo1c8y%2BJf2os4XRxxMmj0ssv2vprnjmATTvuznbwqSsIwUajFQpEqOAK0EqmVbXc1Rkcokuund3TRcKHmTB9lYzSEo%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       Via:
@@ -358,29 +355,29 @@
       string: '{"result":"2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9","error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87e951d2f851418e-LHR
+      - 87f6ea3b0ac56557-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Sat, 04 May 2024 14:53:19 GMT
+      - Mon, 06 May 2024 06:29:16 GMT
       Etag:
       - W/"6a-NIsU6VTx+O5+ZiMXacgz3yRGZ4w"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=WWP6nnpl%2FTz1OvQC4RREGlZ0Sz%2Bd2MzRcBuAeOgM%2BzRSxB4luR5qgI38XY33THatTYFtie51jvrvGMJZGtP6GEMfbtsnSLxW9eFtzkAdBmVKJYpSpSR1wTcd2koGY1I%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=511x3CeuFllDPCSQ56A1hNKAQah3HSi7C2xtvpv6oHkJZ5Cu9FStumH2Cu6So2uBU5rKDY1vCkhemogLSX2DtRiP9oHLEn2jHXnXjZcjZ1s%2FyGduC2nwa6LVImPW%2BcM%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Via:
       - 1.1 google
       alt-svc:
@@ -418,40 +415,40 @@
     body: '{"method": "getblock", "params": ["2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":{"hash":"2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9","confirmations":5,"strippedsize":435,"size":645,"weight":1776,"height":3247855,"version":536870912,"versionHex":"20000000","merkleroot":"ea7d884bbc471d6c6ca1373c718fa8e24c0a57d280e5a4c2b633b1743d1712cd","tx":[{"txid":"cc2f6dcf37ee8cf019145c2a3eaabf70f14a42dd9aa5f31ed1baa549716fe7b9","hash":"26cd1fbff30b0fadb066f00de9f86ff29f3a54360dbfc528d9b02f489f1704b4","version":1,"size":296,"vsize":269,"weight":1076,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ef8e3104ff49366608bf4bc2d500000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":0}],"vout":[{"ismweb":false,"value":6.249375,"n":0,"scriptPubKey":{"asm":"0
+      string: '{"result":{"hash":"2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9","confirmations":938,"strippedsize":435,"size":645,"weight":1776,"height":3247855,"version":536870912,"versionHex":"20000000","merkleroot":"ea7d884bbc471d6c6ca1373c718fa8e24c0a57d280e5a4c2b633b1743d1712cd","tx":[{"txid":"cc2f6dcf37ee8cf019145c2a3eaabf70f14a42dd9aa5f31ed1baa549716fe7b9","hash":"26cd1fbff30b0fadb066f00de9f86ff29f3a54360dbfc528d9b02f489f1704b4","version":1,"size":296,"vsize":269,"weight":1076,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ef8e3104ff49366608bf4bc2d500000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":0}],"vout":[{"ismweb":false,"value":6.249375,"n":0,"scriptPubKey":{"asm":"0
         94a1914d5e14ba06b02bb9d2b0b672f2fd125415","hex":"001494a1914d5e14ba06b02bb9d2b0b672f2fd125415","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1qjjsezn27zjaqdvpth8ftpdnj7t73y4q4vja4dq"]}},{"ismweb":false,"value":0.000625,"n":1,"scriptPubKey":{"asm":"OP_DUP
         OP_HASH160 684a4a9d1c027eddb12029e40ccd86215360790a OP_EQUALVERIFY OP_CHECKSIG","hex":"76a914684a4a9d1c027eddb12029e40ccd86215360790a88ac","reqSigs":1,"type":"pubkeyhash","addresses":["mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX"]}},{"ismweb":false,"value":0,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9edb2b3b4be9f62e0f20409d7bddecca7547ef5254dc0c6978a3985ffb60215ad8e","hex":"6a24aa21a9edb2b3b4be9f62e0f20409d7bddecca7547ef5254dc0c6978a3985ffb60215ad8e","type":"nulldata"}}],"hex":"010000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff6103ef8e3104ff49366608bf4bc2d500000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f00000000031cca3f250000000016001494a1914d5e14ba06b02bb9d2b0b672f2fd12541524f40000000000001976a914684a4a9d1c027eddb12029e40ccd86215360790a88ac0000000000000000266a24aa21a9edb2b3b4be9f62e0f20409d7bddecca7547ef5254dc0c6978a3985ffb60215ad8e0120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"39aea883ba364db920f2f8e36e326491749b2a576306ed253223860efcda1e0c","hash":"39aea883ba364db920f2f8e36e326491749b2a576306ed253223860efcda1e0c","version":2,"size":97,"vsize":94,"weight":376,"locktime":0,"vin":[{"ismweb":false,"txid":"992b887a10aa924430e905174535fd92733136b76d39e835c109e3ff2719bd69","vout":0,"scriptSig":{"asm":"","hex":""},"sequence":4294967295}],"vout":[{"ismweb":false,"value":1791337.37993343,"n":0,"scriptPubKey":{"asm":"8
         fc6a93f9d465d93d5f82974181c905e1ddf4c4705439109f7f38403ee8f771bb","hex":"5820fc6a93f9d465d93d5f82974181c905e1ddf4c4705439109f7f38403ee8f771bb","type":"witness_mweb_hogaddr"}}],"hex":"0200000000080169bd1927ffe309c135e8396db736317392fd35451705e9304492aa107a882b990000000000ffffffff017f04d2d2eba20000225820fc6a93f9d465d93d5f82974181c905e1ddf4c4705439109f7f38403ee8f771bb0000000000"}],"time":1714833919,"mediantime":1714833495,"nonce":4096197120,"bits":"1e044362","difficulty":0.000916254800568373,"chainwork":"00000000000000000000000000000000000000000000000000c3adb1cbd62ffc","nTx":2,"mweb":{"hash":"fc6a93f9d465d93d5f82974181c905e1ddf4c4705439109f7f38403ee8f771bb","height":3247855,"kernel_offset":"9a966bcbe6fcf6b94d7428142a0027b004b1af6a28f2f1999e3d21a565ddb187","stealth_offset":"0000000000000000000000000000000000000000000000000000000000000000","num_kernels":0,"num_txos":4722,"kernel_root":"0000000000000000000000000000000000000000000000000000000000000000","output_root":"69f9f4774c9afd3dab444bbad6df6ae0dcb2c5d6051b5054d7b306a0d348f3c4","leaf_root":"2551128703060a6d3002845179551621ff1d77ce9055933276092f9e7ba97382","inputs":[],"outputs":[],"kernels":[]},"previousblockhash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06","nextblockhash":"5105e7d547d990af00aeb27bf86187c2ff0a0274899e14723745e1403a931bc1"},"error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87e951d399574177-LHR
+      - 87f6ea3bace563d7-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Sat, 04 May 2024 14:53:19 GMT
+      - Mon, 06 May 2024 06:29:16 GMT
       Etag:
-      - W/"fd5-GPoEP3mNPV8+vP9vQm2EjzlMsrs"
+      - W/"fd7-946Hn+hqC84SMNRjTSfXcVVNXto"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=8fF%2FaMm0kzsqfXjuqzc7rAt4HmdEjwrfveyJqDNDH8lUe%2BoY7DxVQp%2FPPm0fruUKkzNVMZyA1ySQz66GHPcz6cgop%2Bne9ZTvNkL4z25KwmotEUUqhq59ejpPt9Fq1Dc%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=xugW16nHfuqbkym1kU3aa6ykNnvv7RUbjbItscCj5%2BPoopPPD4FjMzg9AjV%2FwPz7UPGwIDpW9xr4QsFxVxrSReQaDbPNfm%2BmogLgdGF0Ac9SR0XW%2FAI1GBpqbAiqN6Q%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       Via:
```

### Comparing `aiotx-0.6.0/tests/test_bsc_client.py` & `aiotx-1.0.0/tests/test_evm/test_eth/test_eth_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,253 +1,355 @@
 import os
 
 import pytest
-from conftest import vcr_c  # noqa
+from conftest import vcr_c
 
-from aiotx.clients import AioTxBSCClient
+from aiotx.clients import AioTxETHClient
 from aiotx.exceptions import (
     AioTxError,
     InvalidArgumentError,
     ReplacementTransactionUnderpriced,
     TransactionNotFound,
     WrongPrivateKey,
 )
 
-PRIVATE_KEY_TO_SEND_FROM = os.environ.get("TEST_BSC_WALLET_PRIVATE_KEY")
-assert PRIVATE_KEY_TO_SEND_FROM is not None, "Please provide TEST_BSC_WALLET_PRIVATE_KEY"
-CONTRACT = "0x337610d27c682E347C9cD60BD4b3b107C9d34dDd"
-DESTINATION_ADDRESS = "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a"
+PRIVATE_KEY_TO_SEND_FROM = os.environ.get("TEST_ETH_WALLET_PRIVATE_KEY")
+assert PRIVATE_KEY_TO_SEND_FROM is not None, "Please provide TEST_ETH_WALLET_PRIVATE_KEY"
+CONTRACT = "0x419Fe9f14Ff3aA22e46ff1d03a73EdF3b70A62ED"
+DESTINATION_ADDRESS = "0xD515F5737044238B0f0d6c100109DA44066bE749"
 
 
-@vcr_c.use_cassette("bsc/get_last_block.yaml")
-async def test_get_last_block(bsc_client: AioTxBSCClient):
-    block_id = await bsc_client.get_last_block_number()
+@vcr_c.use_cassette("eth/get_last_block.yaml")
+async def test_get_last_block(eth_client: AioTxETHClient):
+    block_id = await eth_client.get_last_block_number()
     assert isinstance(block_id, int)
 
+
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_balance",
     [
-        ("0x1284214b9b9c85549aB3D2b972df0dEEf66aC2c9", None, 10561622435613231665),
-        ("0x3a82a5a2b77d33a12621e860d1d19cdfb8bf63b4", None, 99724094999968300),
-        ("0x0e28BD8B2D4efb8A3128f7fB310f4e227E25DB6F", None, 691239109999999988),
-        ("0xfb2bdebad0cb9486e714b053a2dbfaf7c05151c9", None, 271930000000000),
-        ("0x040bA056435A7675847F4D577d3Cb8Fc2646A946", None, 421930000000000),
-        ("0x040bA056435A7675847F4D577d3Cb8Fc2646A948", None, 0),
-        ("040bA056435A7675847F4D577d3Cb8Fc2646A946", InvalidArgumentError, 0),
+        ("0x56ebc43d764761bc09d5918787672e2c8d46da5f", None, 22243749149992258),
+        ("0xf663792Be0EdD00AFFB8BBe4Ac6d8185efD5671d", None, 72596311066831845012),
+        ("0xA869aF2883DD6C881bC59594aDfB3e8b136321b4", None, 2360954490480603880),
+        ("0xE27017DD9EF7e3D0A8321C2041Fc4402e89945b6", None, 9148320984250803464),
+        ("0x39832298befa06a6db0c920ada31cfebAD2e33aB", None, 36026722467628523),
+        ("0xC4BfcCb1668d6e464f33a76bAdD8c8d7d341E04B", None, 0),
+        ("0x68EfbC84d1Eabc193979beab2E2DDc20B219A14", InvalidArgumentError, 0),
     ],
 )
-@vcr_c.use_cassette("bsc/get_balance.yaml")
-async def test_get_balance(bsc_client: AioTxBSCClient, wallet_address, expected_exception, expected_balance):
+@vcr_c.use_cassette("eth/get_balance.yaml")
+async def test_get_balance(eth_client: AioTxETHClient, wallet_address, expected_exception, expected_balance):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await bsc_client.get_balance(wallet_address)
+            await eth_client.get_balance(wallet_address)
     else:
-        balance = await bsc_client.get_balance(wallet_address)
+        balance = await eth_client.get_balance(wallet_address)
         assert isinstance(balance, int)
         assert balance == expected_balance
 
 
 @pytest.mark.parametrize(
     "tx_id, expected_exception",
     [
-        ("0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b9451909118", None),
-        ("0xdeac5f03c42970ec4c89ec540c886a2738b8b8fc8c415d0bd231ea94dad81727", None),
-        ("0x26611f5796882c8f45a52c4443c2cda4580ef0bb06d57686d34672207312dfd3", None),
-        ("0xf82c96662db872899f16ea9dfed73fb7c29f3942fdbfc97500ca071793f5a397", None),
-        ("0x8a0dc46462919c8a1c15c90e79782ba4e56b9053fad8975c9b6bec094f001895", None),
-        ("0x41c8e2e03195c29cea37d67ad234d91c52258a514c78f9fcfd196aa5992209ae", None),
-        ("0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b9451909111", TransactionNotFound),
-        ("0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b945190911", InvalidArgumentError),
-        ("41c8e2e03195c29cea37d67ad234d91c52258a514c78f9fcfd196aa5992209ae", InvalidArgumentError),
-
+        ("0x293fbb7d14e6a11a152fad9d621abdf810acfccb7c8c95977622223638fad96a", None),
+        ("0x0d03e84a4d1673b590885ec270553fbd310620debd12d1779796e9ff181f66fe", None),
+        ("0x82e8a1058cdadcd0cd728388c48456db7e79051a198d654de85a7f51bf326fb8", None),
+        ("0x2f88aa536f9ef65087ce0e81918febf65396cf4a8ff5d535d58a45de4a13d076", None),
+        ("0xcb5ad4fd610b6e9e687b5154f4832c0233a527719dcfad6d47500c9f3a50f7cc", None),
+        ("0x93ff17f18511c4fa74166a2dbd53ffa7ce5cc2ee431cbb4fd5e02bbdf2701b72", None),
+        ("0x93ff17f18511c4fa74166a2dbd53ffa7ce5cc2ee431cbb4fd5e02bbdf2701b73", TransactionNotFound),
+        ("0x93ff17f18511c4fa74166a2dbd53ffa7ce5cc2ee431cbb4fd5e02bbdf2701b2", InvalidArgumentError),
+        ("0x93ff17f18511c4fa74166a2dbd53ffa7ce5cc2ee431cbb4fd5e02bbdf701b72", InvalidArgumentError),
     ],
 )
-@vcr_c.use_cassette("bsc/get_transaction.yaml")
-async def test_get_transaction(bsc_client: AioTxBSCClient, tx_id, expected_exception):
+@vcr_c.use_cassette("eth/get_transaction.yaml")
+async def test_get_transaction(eth_client: AioTxETHClient, tx_id, expected_exception):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await bsc_client.get_transaction(tx_id)
+            await eth_client.get_transaction(tx_id)
     else:
-        tx = await bsc_client.get_transaction(tx_id)
+        tx = await eth_client.get_transaction(tx_id)
         assert "aiotx_decoded_input" in tx.keys()
 
 
-
 @pytest.mark.parametrize(
     "wallet_address, contract, expected_exception, expected_balance",
     [
-        ("0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", CONTRACT, None, 1000000001000000000),
-        ("0x896c54023265f2c821f241BC694d8A0E1FA7DF2E", CONTRACT, None, 3570000000000000000),
-        ("0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", CONTRACT, None, 15469999999000000000),
-        ("0x98265f1Dd3224aBA2148C6cF2Ef873b05A3476C1", CONTRACT, None, 629546202581319287241),
-        ("0xf6626A900e4Cc958D2cD0Eb2186Fd6B29EDB63ce", CONTRACT, None, 950000000000000000),
-        ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", CONTRACT, None, 32963423288412440122),
+        ("0x159bD467fafcfA348D2b5f357b23aA1d70E814A0", CONTRACT, None, 10109029605),
+        ("0x265253254239F1ce54B2580d6Bfa39Afe41D545A", CONTRACT, None, 1665000000),
+        ("0xAf0Eca5c36b0380f27412155f6e59618a38e778F", CONTRACT, None, 14000000000),
+        ("0x85213732c4F14EaB4B00eB1960a29077302CF131", CONTRACT, None, 12500000000),
+        ("0x9cd384d1Dc5Ba08234aE8D57b0d43724caE8C4d6", CONTRACT, None, 11200000000),
+        ("0x42827369CD85aD4E88d93D482C144803Aca448C1", CONTRACT, None, 11000000000),
         ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", CONTRACT, None, 0),
         ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", "Eeaa7E347ee4557f9a6F71C", InvalidArgumentError, 0),
     ],
 )
-@vcr_c.use_cassette("bsc/get_token_balance.yaml")
-async def test_get_token_balance(bsc_client: AioTxBSCClient, wallet_address, contract, expected_exception, expected_balance):
-    
+@vcr_c.use_cassette("eth/get_token_balance.yaml")
+async def test_get_token_balance(
+    eth_client: AioTxETHClient, wallet_address, contract, expected_exception, expected_balance
+):
+
     if expected_exception:
         with pytest.raises(expected_exception):
-            await bsc_client.get_contract_balance(wallet_address, contract)
+            await eth_client.get_contract_balance(wallet_address, contract)
     else:
-        balance = await bsc_client.get_contract_balance(wallet_address, contract)
+        balance = await eth_client.get_contract_balance(wallet_address, contract)
         assert isinstance(balance, int)
         assert expected_balance == balance
 
 
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_count",
     [
-        ("0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", None, 0),
-        ("0x896c54023265f2c821f241BC694d8A0E1FA7DF2E", None, 0),
-        ("0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", None, 102),
-        ("0x98265f1Dd3224aBA2148C6cF2Ef873b05A3476C1", None, 1751),
-        ("0xf6626A900e4Cc958D2cD0Eb2186Fd6B29EDB63ce", None, 17),
-        ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", None, 1),
-        ("2dbB5a4c235164B9f772179A43faca2c71a8abDB", InvalidArgumentError, 0),
-        ("0x2dbB5a4c235164B9f772179A43faca2c71a8ab", InvalidArgumentError, 0),
+        ("0x159bD467fafcfA348D2b5f357b23aA1d70E814A0", None, 1),
+        ("0x265253254239F1ce54B2580d6Bfa39Afe41D545A", None, 2317),
+        ("0xAf0Eca5c36b0380f27412155f6e59618a38e778F", None, 358),
+        ("0x85213732c4F14EaB4B00eB1960a29077302CF131", None, 809),
+        ("0x9cd384d1Dc5Ba08234aE8D57b0d43724caE8C4d6", None, 902),
+        ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", None, 0),
+        ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71", InvalidArgumentError, 0),
+        ("DA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", InvalidArgumentError, 0),
     ],
 )
-@vcr_c.use_cassette("bsc/get_transaction_count.yaml")
-async def test_get_transaction_count(bsc_client: AioTxBSCClient, wallet_address, expected_exception, expected_count):
+@vcr_c.use_cassette("eth/get_transaction_count.yaml")
+async def test_get_transaction_count(eth_client: AioTxETHClient, wallet_address, expected_exception, expected_count):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await bsc_client.get_transactions_count(wallet_address)
+            await eth_client.get_transactions_count(wallet_address)
     else:
-        count = await bsc_client.get_transactions_count(wallet_address)
+        count = await eth_client.get_transactions_count(wallet_address)
         assert isinstance(count, int)
         assert expected_count == count
 
 
-
-@vcr_c.use_cassette("bsc/get_gas_price.yaml")
-async def test_send_get_gas_price(bsc_client: AioTxBSCClient):
-    result = await bsc_client.get_gas_price()
+@vcr_c.use_cassette("eth/get_gas_price.yaml")
+async def test_get_gas_price(eth_client: AioTxETHClient):
+    result = await eth_client.get_gas_price()
     assert isinstance(result, int)
-    assert result == 5000000000
 
 
 @pytest.mark.parametrize(
     "private_key, to_address, amount, gas_price, gas_limit, expected_exception",
     [
-        ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS, 0.00001, 5, 21000, WrongPrivateKey),
-        ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch", DESTINATION_ADDRESS, 0.00001, 5, 21000, WrongPrivateKey),
-        ("e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS, 0.00001, 5, 21000, WrongPrivateKey),
+        (
+            "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
+            DESTINATION_ADDRESS,
+            0.00001,
+            5,
+            21000,
+            WrongPrivateKey,
+        ),
+        (
+            "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch",
+            DESTINATION_ADDRESS,
+            0.00001,
+            5,
+            21000,
+            WrongPrivateKey,
+        ),
+        (
+            "e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
+            DESTINATION_ADDRESS,
+            0.00001,
+            5,
+            21000,
+            WrongPrivateKey,
+        ),
         (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5", 0.00001, 5, 21000, ValueError),
         (PRIVATE_KEY_TO_SEND_FROM, "f9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", 0.00001, 5, 21000, None),
         (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E84d3f6FF662Ba4c306b5a", 0.00001, 5, 21000, ValueError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 21000, None),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 21000, ReplacementTransactionUnderpriced),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 5, 5, 21000, AioTxError),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 0, 21000, AioTxError),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0, 5, 21000, ReplacementTransactionUnderpriced),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 0, AioTxError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 61000, ReplacementTransactionUnderpriced)
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 61000, ReplacementTransactionUnderpriced),
     ],
 )
-@vcr_c.use_cassette("bsc/send_transaction.yaml")
-async def test_send_transaction(bsc_client: AioTxBSCClient, private_key, to_address, amount, gas_price, gas_limit, expected_exception):
+@vcr_c.use_cassette("eth/send_transaction.yaml")
+async def test_send_transaction(
+    eth_client: AioTxETHClient, private_key, to_address, amount, gas_price, gas_limit, expected_exception
+):
     """
     Here it's raising ReplacementTransactionUnderpriced and NonceTooLowError because we have reusing
     the same VCR data for every get nonce request, we should investigate how we can change that maybe?
     """
-    gas_price = bsc_client.to_wei(gas_price, "gwei")
-    wei_amount = bsc_client.to_wei(amount, "ether")
+    gas_price = eth_client.to_wei(gas_price, "gwei")
+    wei_amount = eth_client.to_wei(amount, "ether")
     if expected_exception:
         with pytest.raises(expected_exception):
-            await bsc_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
+            await eth_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
     else:
-        result = await bsc_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
+        result = await eth_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
         assert isinstance(result, str)
 
 
 @pytest.mark.parametrize(
     "private_key, to_address, amount, expected_exception",
     [
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, None),
-        (PRIVATE_KEY_TO_SEND_FROM, "0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", 0.00001, ReplacementTransactionUnderpriced),
+        (
+            PRIVATE_KEY_TO_SEND_FROM,
+            "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a",
+            0.00001,
+            ReplacementTransactionUnderpriced,
+        ),
     ],
 )
-@vcr_c.use_cassette("bsc/send_transaction_with_auto_gas.yaml")
-async def test_send_transaction_with_auto_gas(bsc_client: AioTxBSCClient, private_key, to_address, amount, expected_exception):
+@vcr_c.use_cassette("eth/send_transaction_with_auto_gas.yaml")
+async def test_send_transaction_with_auto_gas(
+    eth_client: AioTxETHClient, private_key, to_address, amount, expected_exception
+):
     """
     Here it's raising ReplacementTransactionUnderpriced and NonceTooLowError because we have reusing
     the same VCR data for every get nonce request, we should investigate how we can change that maybe?
     """
-    wei_amount = bsc_client.to_wei(amount, "ether")
+    wei_amount = eth_client.to_wei(amount, "ether")
     if expected_exception:
         with pytest.raises(expected_exception):
-            await bsc_client.send(private_key, to_address, wei_amount)
+            await eth_client.send(private_key, to_address, wei_amount)
     else:
-        result = await bsc_client.send(private_key, to_address, wei_amount)
+        result = await eth_client.send(private_key, to_address, wei_amount)
         assert isinstance(result, str)
 
 
-@vcr_c.use_cassette("bsc/send_transaction_with_custom_nonce.yaml")
-async def test_send_transaction_with_custom_nonce(bsc_client: AioTxBSCClient):
-    wei_amount = bsc_client.to_wei(0.00001, "ether")
-    sender_address = bsc_client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
-    nonce = await bsc_client.get_transactions_count(sender_address)
-    first_tx = await bsc_client.send(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, wei_amount, nonce=nonce)
+@vcr_c.use_cassette("eth/send_transaction_with_custom_nonce.yaml")
+async def test_send_transaction_with_custom_nonce(eth_client: AioTxETHClient):
+    wei_amount = eth_client.to_wei(0.00001, "ether")
+    sender_address = eth_client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
+    nonce = await eth_client.get_transactions_count(sender_address)
+    first_tx = await eth_client.send(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, wei_amount, nonce=nonce)
     assert isinstance(first_tx, str)
-    second_tx = await bsc_client.send(PRIVATE_KEY_TO_SEND_FROM, sender_address, wei_amount, nonce=nonce + 1)
+    second_tx = await eth_client.send(PRIVATE_KEY_TO_SEND_FROM, sender_address, wei_amount, nonce=nonce + 1)
     assert isinstance(second_tx, str)
 
+
+@pytest.mark.parametrize(
+    "contract, expected_decimals, expected_exception",
+    [
+        (CONTRACT, 6, None),
+        ("0x337610d27c682E347C9cD60BD4b3b107C9d34dD", 18, InvalidArgumentError),
+        ("0x1a0cdabee2c57c965b8bbc037671e458805dfdd5", 18, None),
+    ],
+)
+@vcr_c.use_cassette("eth/get_contract_decimals.yaml")
+async def test_get_contract_decimals(eth_client: AioTxETHClient, contract, expected_decimals, expected_exception):
+    if expected_exception:
+        with pytest.raises(expected_exception):
+            await eth_client.get_contract_decimals(contract)
+    else:
+        decimals = await eth_client.get_contract_decimals(contract)
+        assert decimals == expected_decimals
+
+
 @pytest.mark.parametrize(
     "private_key, to_address, contract, amount, gas_price, gas_limit, expected_exception",
     [
-        ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, WrongPrivateKey),
-        ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch", DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, WrongPrivateKey),
-        ("e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, WrongPrivateKey),
-        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a",CONTRACT, 1, 5, 61000, ValueError),
+        (
+            "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
+            DESTINATION_ADDRESS,
+            CONTRACT,
+            1,
+            5,
+            61000,
+            WrongPrivateKey,
+        ),
+        (
+            "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch",
+            DESTINATION_ADDRESS,
+            CONTRACT,
+            1,
+            5,
+            61000,
+            WrongPrivateKey,
+        ),
+        (
+            "e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
+            DESTINATION_ADDRESS,
+            CONTRACT,
+            1,
+            5,
+            61000,
+            WrongPrivateKey,
+        ),
+        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a", CONTRACT, 1, 5, 61000, ValueError),
         (PRIVATE_KEY_TO_SEND_FROM, "f9E5E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", CONTRACT, 1, 5, 61000, ValueError),
-        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b",CONTRACT, 1, 5, 61000, ValueError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a", 0.00001, 5, 61000, TypeError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, "f9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", 1, 5, 61000, TypeError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b", 1, 5, 61000, TypeError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, None),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1000, 5, 61000, ReplacementTransactionUnderpriced),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1, 0, 61000, AioTxError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 0, 5, 61000, ReplacementTransactionUnderpriced),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1, 5, 0, AioTxError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, None)
+        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b", CONTRACT, 1, 5, 61000, ValueError),
+        (
+            PRIVATE_KEY_TO_SEND_FROM,
+            DESTINATION_ADDRESS,
+            "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a",
+            0.00001,
+            5,
+            61000,
+            TypeError,
+        ),
+        (
+            PRIVATE_KEY_TO_SEND_FROM,
+            DESTINATION_ADDRESS,
+            "f9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a",
+            1,
+            5,
+            61000,
+            TypeError,
+        ),
+        (
+            PRIVATE_KEY_TO_SEND_FROM,
+            DESTINATION_ADDRESS,
+            "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b",
+            1,
+            5,
+            61000,
+            TypeError,
+        ),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, None),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1000, 5, 61000, ReplacementTransactionUnderpriced),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 0, 61000, AioTxError),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 0, 5, 61000, ReplacementTransactionUnderpriced),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 0, AioTxError),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, None),
     ],
 )
-@vcr_c.use_cassette("bsc/send_token_transaction.yaml")
-async def test_send_token_transaction(bsc_client: AioTxBSCClient, private_key, to_address, contract, amount, gas_price, gas_limit, expected_exception):
+@vcr_c.use_cassette("eth/send_token_transaction.yaml")
+async def test_send_token_transaction(
+    eth_client: AioTxETHClient, private_key, to_address, contract, amount, gas_price, gas_limit, expected_exception
+):
     """
     Here it's raising ReplacementTransactionUnderpriced and NonceTooLowError because we have reusing
     the same VCR data for every get nonce request, we should investigate how we can change that maybe?
     """
-    gas_price = bsc_client.to_wei(gas_price, "gwei")
-    wei_amount = bsc_client.to_wei(amount, "ether")
+    gas_price = eth_client.to_wei(gas_price, "gwei")
+    wei_amount = eth_client.to_wei(amount, "mwei")
 
     if expected_exception:
         with pytest.raises(expected_exception):
-            await bsc_client.send_token(
-        private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
-    )
+            await eth_client.send_token(
+                private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
+            )
     else:
-        result = await bsc_client.send_token(
-        private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
-    )
+        result = await eth_client.send_token(
+            private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
+        )
         assert isinstance(result, str)
 
 
-@pytest.mark.parametrize(
-    "contract, expected_decimals, expected_exception",
-    [
-        (CONTRACT, 18, None),
-        ("0x337610d27c682E347C9cD60BD4b3b107C9d34dD", 18, InvalidArgumentError),
-        ("0x757fc78bb4df4ce6605ae669bf0b71074176aac3", 9, None),
-    ],
-)
-@vcr_c.use_cassette("bsc/get_contract_decimals.yaml")
-async def test_get_contract_decimals(bsc_client: AioTxBSCClient, contract, expected_decimals, expected_exception):
-    if expected_exception:
-        with pytest.raises(expected_exception):
-            await bsc_client.get_contract_decimals(contract)
-    else:
-        decimals = await bsc_client.get_contract_decimals(contract)
-        assert decimals == expected_decimals
+@vcr_c.use_cassette("eth/send_token_transaction_with_custom_nonce.yaml")
+async def send_token_transaction_with_custom_nonce(eth_client: AioTxETHClient):
+    wei_amount = eth_client.to_wei(0.00001, "mwei")
+    sender_address = eth_client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
+    nonce = await eth_client.get_transactions_count(sender_address)
+    first_tx = await eth_client.send_token(
+        PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, wei_amount, nonce=nonce
+    )
+    assert isinstance(first_tx, str)
+    second_tx = await eth_client.send_token(
+        PRIVATE_KEY_TO_SEND_FROM, sender_address, CONTRACT, wei_amount, nonce=nonce + 1
+    )
+    assert isinstance(second_tx, str)
+
+
+@vcr_c.use_cassette("eth/send_token_transaction_with_auto_params.yaml")
+async def test_send_transaction_with_auto_params(eth_client: AioTxETHClient):
+    wei_amount = eth_client.to_wei(0.00001, "mwei")
+    tx_id = await eth_client.send_token(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, wei_amount)
+    assert isinstance(tx_id, str)
```

### Comparing `aiotx-0.6.0/tests/test_bsc_monitoring.py` & `aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.6.0/tests/test_btc_monitor.py` & `aiotx-1.0.0/tests/test_evm/test_eth/test_eth_monitoring.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import asyncio
 
 from conftest import vcr_c
 
-from aiotx.clients import AioTxBTCClient
+from aiotx.clients import AioTxBSCClient
 
 
-@vcr_c.use_cassette("btc/test_async_monitoring.yaml")
-async def test_async_monitoring(btc_client: AioTxBTCClient):
+@vcr_c.use_cassette("tests/fixtures/cassettes/eth/test_async_monitoring.yaml")
+async def test_async_monitoring(eth_client: AioTxBSCClient):
     blocks = []
     transactions = []
 
-    @btc_client.monitor.on_block
+    @eth_client.monitor.on_block
     async def handle_block(block):
         blocks.append(block)
 
-    @btc_client.monitor.on_transaction
+    @eth_client.monitor.on_transaction
     async def handle_transaction(transaction):
         transactions.append(transaction)
 
-    await btc_client.start_monitoring(555)
+    await eth_client.start_monitoring(2834064)
     try:
         await asyncio.sleep(3)
     except KeyboardInterrupt:
-        btc_client.stop_monitoring()
+        eth_client.stop_monitoring()
 
     assert len(blocks) > 0
     assert len(transactions) > 0
 
-    assert 555 in blocks
-    assert 556 in blocks
-    assert "070a808197d97c8982587f75fef6d531282863a110ad5e8b42cdec8ddb6dc4e0" in [tx["txid"] for tx in transactions]
-    assert "c852040a873a8f3c1ee69fda40dcf32a118978a923f62176272e840fc042de54" in [tx["txid"] for tx in transactions]
-
+    assert 2834064 in blocks
+    assert 2834065 in blocks
+    assert "0x5b6fd8fda590e887531df12dec5faf2ce8c94a3eeb56bcc1fde760fabd64e56e" in [tx["hash"] for tx in transactions]
+    assert "0x10f4376f7efe2637be4d012eebad143dce58626146befa48204f1275476064d6" in [tx["hash"] for tx in transactions]
 
+    for tx in transactions:
+        assert "aiotx_decoded_input" in tx.keys()
```

### Comparing `aiotx-0.6.0/tests/test_eth_client.py` & `aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,274 +1,334 @@
 import os
 
 import pytest
-from conftest import vcr_c
+from conftest import vcr_c  # noqa
 
-from aiotx.clients import AioTxETHClient
+from aiotx.clients import AioTxBSCClient
 from aiotx.exceptions import (
     AioTxError,
     InvalidArgumentError,
     ReplacementTransactionUnderpriced,
     TransactionNotFound,
     WrongPrivateKey,
 )
 
-PRIVATE_KEY_TO_SEND_FROM = os.environ.get("TEST_ETH_WALLET_PRIVATE_KEY")
-assert PRIVATE_KEY_TO_SEND_FROM is not None, "Please provide TEST_ETH_WALLET_PRIVATE_KEY"
-CONTRACT = "0x419Fe9f14Ff3aA22e46ff1d03a73EdF3b70A62ED"
-DESTINATION_ADDRESS = "0xD515F5737044238B0f0d6c100109DA44066bE749"
+PRIVATE_KEY_TO_SEND_FROM = os.environ.get("TEST_BSC_WALLET_PRIVATE_KEY")
+assert PRIVATE_KEY_TO_SEND_FROM is not None, "Please provide TEST_BSC_WALLET_PRIVATE_KEY"
+CONTRACT = "0x337610d27c682E347C9cD60BD4b3b107C9d34dDd"
+DESTINATION_ADDRESS = "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a"
 
 
-@vcr_c.use_cassette("eth/get_last_block.yaml")
-async def test_get_last_block(eth_client: AioTxETHClient):
-    block_id = await eth_client.get_last_block_number()
+@vcr_c.use_cassette("bsc/get_last_block.yaml")
+async def test_get_last_block(bsc_client: AioTxBSCClient):
+    block_id = await bsc_client.get_last_block_number()
     assert isinstance(block_id, int)
 
+
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_balance",
     [
-        ("0x56ebc43d764761bc09d5918787672e2c8d46da5f", None, 22243749149992258),
-        ("0xf663792Be0EdD00AFFB8BBe4Ac6d8185efD5671d", None, 72596311066831845012),
-        ("0xA869aF2883DD6C881bC59594aDfB3e8b136321b4", None, 2360954490480603880),
-        ("0xE27017DD9EF7e3D0A8321C2041Fc4402e89945b6", None, 9148320984250803464),
-        ("0x39832298befa06a6db0c920ada31cfebAD2e33aB", None, 36026722467628523),
-        ("0xC4BfcCb1668d6e464f33a76bAdD8c8d7d341E04B", None, 0),
-        ("0x68EfbC84d1Eabc193979beab2E2DDc20B219A14", InvalidArgumentError, 0),
+        ("0x1284214b9b9c85549aB3D2b972df0dEEf66aC2c9", None, 10561622435613231665),
+        ("0x3a82a5a2b77d33a12621e860d1d19cdfb8bf63b4", None, 99724094999968300),
+        ("0x0e28BD8B2D4efb8A3128f7fB310f4e227E25DB6F", None, 691239109999999988),
+        ("0xfb2bdebad0cb9486e714b053a2dbfaf7c05151c9", None, 271930000000000),
+        ("0x040bA056435A7675847F4D577d3Cb8Fc2646A946", None, 421930000000000),
+        ("0x040bA056435A7675847F4D577d3Cb8Fc2646A948", None, 0),
+        ("040bA056435A7675847F4D577d3Cb8Fc2646A946", InvalidArgumentError, 0),
     ],
 )
-@vcr_c.use_cassette("eth/get_balance.yaml")
-async def test_get_balance(eth_client: AioTxETHClient, wallet_address, expected_exception, expected_balance):
+@vcr_c.use_cassette("bsc/get_balance.yaml")
+async def test_get_balance(bsc_client: AioTxBSCClient, wallet_address, expected_exception, expected_balance):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await eth_client.get_balance(wallet_address)
+            await bsc_client.get_balance(wallet_address)
     else:
-        balance = await eth_client.get_balance(wallet_address)
+        balance = await bsc_client.get_balance(wallet_address)
         assert isinstance(balance, int)
         assert balance == expected_balance
 
 
 @pytest.mark.parametrize(
     "tx_id, expected_exception",
     [
-        ("0x293fbb7d14e6a11a152fad9d621abdf810acfccb7c8c95977622223638fad96a", None),
-        ("0x0d03e84a4d1673b590885ec270553fbd310620debd12d1779796e9ff181f66fe", None),
-        ("0x82e8a1058cdadcd0cd728388c48456db7e79051a198d654de85a7f51bf326fb8", None),
-        ("0x2f88aa536f9ef65087ce0e81918febf65396cf4a8ff5d535d58a45de4a13d076", None),
-        ("0xcb5ad4fd610b6e9e687b5154f4832c0233a527719dcfad6d47500c9f3a50f7cc", None),
-        ("0x93ff17f18511c4fa74166a2dbd53ffa7ce5cc2ee431cbb4fd5e02bbdf2701b72", None),
-        ("0x93ff17f18511c4fa74166a2dbd53ffa7ce5cc2ee431cbb4fd5e02bbdf2701b73", TransactionNotFound),
-        ("0x93ff17f18511c4fa74166a2dbd53ffa7ce5cc2ee431cbb4fd5e02bbdf2701b2", InvalidArgumentError),
-        ("0x93ff17f18511c4fa74166a2dbd53ffa7ce5cc2ee431cbb4fd5e02bbdf701b72", InvalidArgumentError),
-
+        ("0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b9451909118", None),
+        ("0xdeac5f03c42970ec4c89ec540c886a2738b8b8fc8c415d0bd231ea94dad81727", None),
+        ("0x26611f5796882c8f45a52c4443c2cda4580ef0bb06d57686d34672207312dfd3", None),
+        ("0xf82c96662db872899f16ea9dfed73fb7c29f3942fdbfc97500ca071793f5a397", None),
+        ("0x8a0dc46462919c8a1c15c90e79782ba4e56b9053fad8975c9b6bec094f001895", None),
+        ("0x41c8e2e03195c29cea37d67ad234d91c52258a514c78f9fcfd196aa5992209ae", None),
+        ("0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b9451909111", TransactionNotFound),
+        ("0x6007710c9bc82da8a9cb6104e39fef7b259df0d257a0efcf46908b945190911", InvalidArgumentError),
+        ("41c8e2e03195c29cea37d67ad234d91c52258a514c78f9fcfd196aa5992209ae", InvalidArgumentError),
     ],
 )
-@vcr_c.use_cassette("eth/get_transaction.yaml")
-async def test_get_transaction(eth_client: AioTxETHClient, tx_id, expected_exception):
+@vcr_c.use_cassette("bsc/get_transaction.yaml")
+async def test_get_transaction(bsc_client: AioTxBSCClient, tx_id, expected_exception):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await eth_client.get_transaction(tx_id)
+            await bsc_client.get_transaction(tx_id)
     else:
-        tx = await eth_client.get_transaction(tx_id)
+        tx = await bsc_client.get_transaction(tx_id)
         assert "aiotx_decoded_input" in tx.keys()
 
 
-
 @pytest.mark.parametrize(
     "wallet_address, contract, expected_exception, expected_balance",
     [
-        ("0x159bD467fafcfA348D2b5f357b23aA1d70E814A0", CONTRACT, None, 10109029605),
-        ("0x265253254239F1ce54B2580d6Bfa39Afe41D545A", CONTRACT, None, 1665000000),
-        ("0xAf0Eca5c36b0380f27412155f6e59618a38e778F", CONTRACT, None, 14000000000),
-        ("0x85213732c4F14EaB4B00eB1960a29077302CF131", CONTRACT, None, 12500000000),
-        ("0x9cd384d1Dc5Ba08234aE8D57b0d43724caE8C4d6", CONTRACT, None, 11200000000),
-        ("0x42827369CD85aD4E88d93D482C144803Aca448C1", CONTRACT, None, 11000000000),
+        ("0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", CONTRACT, None, 1000000001000000000),
+        ("0x896c54023265f2c821f241BC694d8A0E1FA7DF2E", CONTRACT, None, 3570000000000000000),
+        ("0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", CONTRACT, None, 15469999999000000000),
+        ("0x98265f1Dd3224aBA2148C6cF2Ef873b05A3476C1", CONTRACT, None, 629546202581319287241),
+        ("0xf6626A900e4Cc958D2cD0Eb2186Fd6B29EDB63ce", CONTRACT, None, 950000000000000000),
+        ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", CONTRACT, None, 32963423288412440122),
         ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", CONTRACT, None, 0),
         ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", "Eeaa7E347ee4557f9a6F71C", InvalidArgumentError, 0),
     ],
 )
-@vcr_c.use_cassette("eth/get_token_balance.yaml")
-async def test_get_token_balance(eth_client: AioTxETHClient, wallet_address, contract, expected_exception, expected_balance):
-    
+@vcr_c.use_cassette("bsc/get_token_balance.yaml")
+async def test_get_token_balance(
+    bsc_client: AioTxBSCClient, wallet_address, contract, expected_exception, expected_balance
+):
+
     if expected_exception:
         with pytest.raises(expected_exception):
-            await eth_client.get_contract_balance(wallet_address, contract)
+            await bsc_client.get_contract_balance(wallet_address, contract)
     else:
-        balance = await eth_client.get_contract_balance(wallet_address, contract)
+        balance = await bsc_client.get_contract_balance(wallet_address, contract)
         assert isinstance(balance, int)
         assert expected_balance == balance
 
 
 @pytest.mark.parametrize(
     "wallet_address, expected_exception, expected_count",
     [
-        ("0x159bD467fafcfA348D2b5f357b23aA1d70E814A0", None, 1),
-        ("0x265253254239F1ce54B2580d6Bfa39Afe41D545A", None, 2317),
-        ("0xAf0Eca5c36b0380f27412155f6e59618a38e778F", None, 358),
-        ("0x85213732c4F14EaB4B00eB1960a29077302CF131", None, 809),
-        ("0x9cd384d1Dc5Ba08234aE8D57b0d43724caE8C4d6", None, 902),
-        ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", None, 0),
-        ("0xDA31b5ac94C559478Eeaa7E347ee4557f9a6F71", InvalidArgumentError, 0),
-        ("DA31b5ac94C559478Eeaa7E347ee4557f9a6F71C", InvalidArgumentError, 0),
+        ("0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", None, 0),
+        ("0x896c54023265f2c821f241BC694d8A0E1FA7DF2E", None, 0),
+        ("0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", None, 102),
+        ("0x98265f1Dd3224aBA2148C6cF2Ef873b05A3476C1", None, 1751),
+        ("0xf6626A900e4Cc958D2cD0Eb2186Fd6B29EDB63ce", None, 17),
+        ("0x2dbB5a4c235164B9f772179A43faca2c71a8abDB", None, 1),
+        ("2dbB5a4c235164B9f772179A43faca2c71a8abDB", InvalidArgumentError, 0),
+        ("0x2dbB5a4c235164B9f772179A43faca2c71a8ab", InvalidArgumentError, 0),
     ],
 )
-@vcr_c.use_cassette("eth/get_transaction_count.yaml")
-async def test_get_transaction_count(eth_client: AioTxETHClient, wallet_address, expected_exception, expected_count):
+@vcr_c.use_cassette("bsc/get_transaction_count.yaml")
+async def test_get_transaction_count(bsc_client: AioTxBSCClient, wallet_address, expected_exception, expected_count):
     if expected_exception:
         with pytest.raises(expected_exception):
-            await eth_client.get_transactions_count(wallet_address)
+            await bsc_client.get_transactions_count(wallet_address)
     else:
-        count = await eth_client.get_transactions_count(wallet_address)
+        count = await bsc_client.get_transactions_count(wallet_address)
         assert isinstance(count, int)
         assert expected_count == count
 
 
-
-@vcr_c.use_cassette("eth/get_gas_price.yaml")
-async def test_get_gas_price(eth_client: AioTxETHClient):
-    result = await eth_client.get_gas_price()
+@vcr_c.use_cassette("bsc/get_gas_price.yaml")
+async def test_send_get_gas_price(bsc_client: AioTxBSCClient):
+    result = await bsc_client.get_gas_price()
     assert isinstance(result, int)
-
+    assert result == 5000000000
 
 
 @pytest.mark.parametrize(
     "private_key, to_address, amount, gas_price, gas_limit, expected_exception",
     [
-        ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS, 0.00001, 5, 21000, WrongPrivateKey),
-        ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch", DESTINATION_ADDRESS, 0.00001, 5, 21000, WrongPrivateKey),
-        ("e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS, 0.00001, 5, 21000, WrongPrivateKey),
+        (
+            "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
+            DESTINATION_ADDRESS,
+            0.00001,
+            5,
+            21000,
+            WrongPrivateKey,
+        ),
+        (
+            "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch",
+            DESTINATION_ADDRESS,
+            0.00001,
+            5,
+            21000,
+            WrongPrivateKey,
+        ),
+        (
+            "e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
+            DESTINATION_ADDRESS,
+            0.00001,
+            5,
+            21000,
+            WrongPrivateKey,
+        ),
         (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5", 0.00001, 5, 21000, ValueError),
         (PRIVATE_KEY_TO_SEND_FROM, "f9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", 0.00001, 5, 21000, None),
         (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E84d3f6FF662Ba4c306b5a", 0.00001, 5, 21000, ValueError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 21000, ReplacementTransactionUnderpriced),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 21000, None),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 5, 5, 21000, AioTxError),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 0, 21000, AioTxError),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0, 5, 21000, ReplacementTransactionUnderpriced),
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 0, AioTxError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 61000, ReplacementTransactionUnderpriced)
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, 5, 61000, ReplacementTransactionUnderpriced),
     ],
 )
-@vcr_c.use_cassette("eth/send_transaction.yaml")
-async def test_send_transaction(eth_client: AioTxETHClient, private_key, to_address, amount, gas_price, gas_limit, expected_exception):
+@vcr_c.use_cassette("bsc/send_transaction.yaml")
+async def test_send_transaction(
+    bsc_client: AioTxBSCClient, private_key, to_address, amount, gas_price, gas_limit, expected_exception
+):
     """
     Here it's raising ReplacementTransactionUnderpriced and NonceTooLowError because we have reusing
     the same VCR data for every get nonce request, we should investigate how we can change that maybe?
     """
-    gas_price = eth_client.to_wei(gas_price, "gwei")
-    wei_amount = eth_client.to_wei(amount, "ether")
+    gas_price = bsc_client.to_wei(gas_price, "gwei")
+    wei_amount = bsc_client.to_wei(amount, "ether")
     if expected_exception:
         with pytest.raises(expected_exception):
-            await eth_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
+            await bsc_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
     else:
-        result = await eth_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
+        result = await bsc_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
         assert isinstance(result, str)
 
 
 @pytest.mark.parametrize(
     "private_key, to_address, amount, expected_exception",
     [
         (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, None),
-        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", 0.00001, ReplacementTransactionUnderpriced),
+        (
+            PRIVATE_KEY_TO_SEND_FROM,
+            "0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e",
+            0.00001,
+            ReplacementTransactionUnderpriced,
+        ),
     ],
 )
-@vcr_c.use_cassette("eth/send_transaction_with_auto_gas.yaml")
-async def test_send_transaction_with_auto_gas(eth_client: AioTxETHClient, private_key, to_address, amount, expected_exception):
+@vcr_c.use_cassette("bsc/send_transaction_with_auto_gas.yaml")
+async def test_send_transaction_with_auto_gas(
+    bsc_client: AioTxBSCClient, private_key, to_address, amount, expected_exception
+):
     """
     Here it's raising ReplacementTransactionUnderpriced and NonceTooLowError because we have reusing
     the same VCR data for every get nonce request, we should investigate how we can change that maybe?
     """
-    wei_amount = eth_client.to_wei(amount, "ether")
+    wei_amount = bsc_client.to_wei(amount, "ether")
     if expected_exception:
         with pytest.raises(expected_exception):
-            await eth_client.send(private_key, to_address, wei_amount)
+            await bsc_client.send(private_key, to_address, wei_amount)
     else:
-        result = await eth_client.send(private_key, to_address, wei_amount)
+        result = await bsc_client.send(private_key, to_address, wei_amount)
         assert isinstance(result, str)
 
 
-
-@vcr_c.use_cassette("eth/send_transaction_with_custom_nonce.yaml")
-async def test_send_transaction_with_custom_nonce(eth_client: AioTxETHClient):
-    wei_amount = eth_client.to_wei(0.00001, "ether")
-    sender_address = eth_client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
-    nonce = await eth_client.get_transactions_count(sender_address)
-    first_tx = await eth_client.send(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, wei_amount, nonce=nonce)
+@vcr_c.use_cassette("bsc/send_transaction_with_custom_nonce.yaml")
+async def test_send_transaction_with_custom_nonce(bsc_client: AioTxBSCClient):
+    wei_amount = bsc_client.to_wei(0.00001, "ether")
+    sender_address = bsc_client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
+    nonce = await bsc_client.get_transactions_count(sender_address)
+    first_tx = await bsc_client.send(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, wei_amount, nonce=nonce)
     assert isinstance(first_tx, str)
-    second_tx = await eth_client.send(PRIVATE_KEY_TO_SEND_FROM, sender_address, wei_amount, nonce=nonce + 1)
+    second_tx = await bsc_client.send(PRIVATE_KEY_TO_SEND_FROM, sender_address, wei_amount, nonce=nonce + 1)
     assert isinstance(second_tx, str)
-    
-
-@pytest.mark.parametrize(
-    "contract, expected_decimals, expected_exception",
-    [
-        (CONTRACT, 6, None),
-        ("0x337610d27c682E347C9cD60BD4b3b107C9d34dD", 18, InvalidArgumentError),
-        ("0x1a0cdabee2c57c965b8bbc037671e458805dfdd5", 18, None),
-    ],
-)
-@vcr_c.use_cassette("eth/get_contract_decimals.yaml")
-async def test_get_contract_decimals(eth_client: AioTxETHClient, contract, expected_decimals, expected_exception):
-    if expected_exception:
-        with pytest.raises(expected_exception):
-            await eth_client.get_contract_decimals(contract)
-    else:
-        decimals = await eth_client.get_contract_decimals(contract)
-        assert decimals == expected_decimals
 
 
 @pytest.mark.parametrize(
     "private_key, to_address, contract, amount, gas_price, gas_limit, expected_exception",
     [
-        ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, WrongPrivateKey),
-        ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch", DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, WrongPrivateKey),
-        ("e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, WrongPrivateKey),
-        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a",CONTRACT, 1, 5, 61000, ValueError),
+        (
+            "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
+            DESTINATION_ADDRESS,
+            CONTRACT,
+            1,
+            5,
+            61000,
+            WrongPrivateKey,
+        ),
+        (
+            "87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch",
+            DESTINATION_ADDRESS,
+            CONTRACT,
+            1,
+            5,
+            61000,
+            WrongPrivateKey,
+        ),
+        (
+            "e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd",
+            DESTINATION_ADDRESS,
+            CONTRACT,
+            1,
+            5,
+            61000,
+            WrongPrivateKey,
+        ),
+        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a", CONTRACT, 1, 5, 61000, ValueError),
         (PRIVATE_KEY_TO_SEND_FROM, "f9E5E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", CONTRACT, 1, 5, 61000, ValueError),
-        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b",CONTRACT, 1, 5, 61000, ValueError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a", 0.00001, 5, 61000, TypeError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, "f9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a", 1, 5, 61000, TypeError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b", 1, 5, 61000, TypeError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, None),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1000, 5, 61000, ReplacementTransactionUnderpriced),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1, 0, 61000, AioTxError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 0, 5, 61000, ReplacementTransactionUnderpriced),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1, 5, 0, AioTxError),
-        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, None)
+        (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b", CONTRACT, 1, 5, 61000, ValueError),
+        (
+            PRIVATE_KEY_TO_SEND_FROM,
+            DESTINATION_ADDRESS,
+            "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a",
+            0.00001,
+            5,
+            61000,
+            TypeError,
+        ),
+        (
+            PRIVATE_KEY_TO_SEND_FROM,
+            DESTINATION_ADDRESS,
+            "f9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b5a",
+            1,
+            5,
+            61000,
+            TypeError,
+        ),
+        (
+            PRIVATE_KEY_TO_SEND_FROM,
+            DESTINATION_ADDRESS,
+            "0xf9E35E4e1CbcF08E99B84d3f6FF662Ba4c306b",
+            1,
+            5,
+            61000,
+            TypeError,
+        ),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, None),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1000, 5, 61000, ReplacementTransactionUnderpriced),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 0, 61000, AioTxError),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 0, 5, 61000, ReplacementTransactionUnderpriced),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 0, AioTxError),
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, None),
     ],
 )
-@vcr_c.use_cassette("eth/send_token_transaction.yaml")
-async def test_send_token_transaction(eth_client: AioTxETHClient, private_key, to_address, contract, amount, gas_price, gas_limit, expected_exception):
+@vcr_c.use_cassette("bsc/send_token_transaction.yaml")
+async def test_send_token_transaction(
+    bsc_client: AioTxBSCClient, private_key, to_address, contract, amount, gas_price, gas_limit, expected_exception
+):
     """
     Here it's raising ReplacementTransactionUnderpriced and NonceTooLowError because we have reusing
     the same VCR data for every get nonce request, we should investigate how we can change that maybe?
     """
-    gas_price = eth_client.to_wei(gas_price, "gwei")
-    wei_amount = eth_client.to_wei(amount, "mwei")
+    gas_price = bsc_client.to_wei(gas_price, "gwei")
+    wei_amount = bsc_client.to_wei(amount, "ether")
 
     if expected_exception:
         with pytest.raises(expected_exception):
-            await eth_client.send_token(
-        private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
-    )
+            await bsc_client.send_token(
+                private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
+            )
     else:
-        result = await eth_client.send_token(
-        private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
-    )
+        result = await bsc_client.send_token(
+            private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
+        )
         assert isinstance(result, str)
 
 
-
-@vcr_c.use_cassette("eth/send_token_transaction_with_custom_nonce.yaml")
-async def send_token_transaction_with_custom_nonce(eth_client: AioTxETHClient):
-    wei_amount = eth_client.to_wei(0.00001, "mwei")
-    sender_address = eth_client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
-    nonce = await eth_client.get_transactions_count(sender_address)
-    first_tx = await eth_client.send_token(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, wei_amount, nonce=nonce)
-    assert isinstance(first_tx, str)
-    second_tx = await eth_client.send_token(PRIVATE_KEY_TO_SEND_FROM, sender_address, CONTRACT, wei_amount, nonce=nonce + 1)
-    assert isinstance(second_tx, str)
-
-
-@vcr_c.use_cassette("eth/send_token_transaction_with_auto_params.yaml")
-async def test_send_transaction_with_auto_params(eth_client: AioTxETHClient):
-    wei_amount = eth_client.to_wei(0.00001, "mwei")
-    tx_id = await eth_client.send_token(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, CONTRACT, wei_amount)
-    assert isinstance(tx_id, str)
+@pytest.mark.parametrize(
+    "contract, expected_decimals, expected_exception",
+    [
+        (CONTRACT, 18, None),
+        ("0x337610d27c682E347C9cD60BD4b3b107C9d34dD", 18, InvalidArgumentError),
+        ("0x757fc78bb4df4ce6605ae669bf0b71074176aac3", 9, None),
+    ],
+)
+@vcr_c.use_cassette("bsc/get_contract_decimals.yaml")
+async def test_get_contract_decimals(bsc_client: AioTxBSCClient, contract, expected_decimals, expected_exception):
+    if expected_exception:
+        with pytest.raises(expected_exception):
+            await bsc_client.get_contract_decimals(contract)
+    else:
+        decimals = await bsc_client.get_contract_decimals(contract)
+        assert decimals == expected_decimals
```

### Comparing `aiotx-0.6.0/tests/test_eth_input_decoding.py` & `aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 import pytest
 
 
-@pytest.mark.parametrize("input_data, expected_output", [
-    ("0x", {'function_name': None, 'parameters': None}),
-
-    ("0xa9059cbb00000000000000000000000012345678901234567890123456789012345678900000000000000000000000000000000000000000000000000000000000000064",
-     {'function_name': 'transfer',
-      'parameters': {'_to': '0x1234567890123456789012345678901234567890', '_value': 100}}),
-
-    ("0x095ea7b3000000000000000000000000098765432109876543210987654321098765432100000000000000000000000000000000000000000000000000000000000003e8",
-     {'function_name': 'approve',
-      'parameters': {'_spender': '0x0987654321098765432109876543210987654321', '_value': 1000}}),
-
-    ("0x23b872dd000000000000000000000000111111111111111111111111111111111111111100000000000000000000000022222222222222222222222222222222222222220000000000000000000000000000000000000000000000000000000000001388",
-     {'function_name': 'transferFrom',
-      'parameters': {'_from': '0x1111111111111111111111111111111111111111',
-                     '_to': '0x2222222222222222222222222222222222222222',
-                     '_value': 5000}}),
-
-    ("0x12345678", {'function_name': None, 'parameters': None}),
-])
-def test_decode_transaction_input(eth_client, input_data, expected_output):
-    result = eth_client.decode_transaction_input(input_data)
-    assert result == expected_output
+@pytest.mark.parametrize(
+    "input_data, expected_output",
+    [
+        ("0x", {"function_name": None, "parameters": None}),
+        (
+            "0xa9059cbb00000000000000000000000012345678901234567890123456789012345678900000000000000000000000000000000000000000000000000000000000000064",
+            {
+                "function_name": "transfer",
+                "parameters": {"recipient": "0x1234567890123456789012345678901234567890", "amount": 100},
+            },
+        ),
+        (
+            "0x095ea7b3000000000000000000000000098765432109876543210987654321098765432100000000000000000000000000000000000000000000000000000000000003e8",
+            {
+                "function_name": "approve",
+                "parameters": {"spender": "0x0987654321098765432109876543210987654321", "amount": 1000},
+            },
+        ),
+        (
+            "0x23b872dd000000000000000000000000111111111111111111111111111111111111111100000000000000000000000022222222222222222222222222222222222222220000000000000000000000000000000000000000000000000000000000001388",
+            {
+                "function_name": "transferFrom",
+                "parameters": {
+                    "sender": "0x1111111111111111111111111111111111111111",
+                    "recipient": "0x2222222222222222222222222222222222222222",
+                    "amount": 5000,
+                },
+            },
+        ),
+        ("0x12345678", {"function_name": None, "parameters": None}),
+    ],
+)
+def test_decode_transaction_input(bsc_client, input_data, expected_output):
+    result = bsc_client.decode_transaction_input(input_data)
+    assert result == expected_output
```

### Comparing `aiotx-0.6.0/tests/test_eth_monitoring.py` & `aiotx-1.0.0/tests/test_utxo/test_ltc/test_ltc_monitor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import asyncio
 
 from conftest import vcr_c
 
-from aiotx.clients import AioTxBSCClient
+from aiotx.clients import AioTxLTCClient
 
 
-@vcr_c.use_cassette("tests/fixtures/cassettes/eth/test_async_monitoring.yaml")
-async def test_async_monitoring(eth_client: AioTxBSCClient):
+@vcr_c.use_cassette("tests/fixtures/cassettes/ltc/test_async_monitoring.yaml")
+async def test_async_monitoring(ltc_public_client: AioTxLTCClient):
     blocks = []
     transactions = []
 
-    @eth_client.monitor.on_block
+    @ltc_public_client.monitor.on_block
     async def handle_block(block):
         blocks.append(block)
 
-    @eth_client.monitor.on_transaction
+    @ltc_public_client.monitor.on_transaction
     async def handle_transaction(transaction):
         transactions.append(transaction)
 
-    await eth_client.start_monitoring(2834064)
+    await ltc_public_client.import_address("tltc1qsawz44ppfnxmnat7635f83exgf9mynrzs5tsgl", 3247853)
+    await ltc_public_client.start_monitoring()
+
     try:
         await asyncio.sleep(3)
     except KeyboardInterrupt:
-        eth_client.stop_monitoring()
+        ltc_public_client.stop_monitoring()
 
     assert len(blocks) > 0
     assert len(transactions) > 0
 
-    assert 2834064 in blocks
-    assert 2834065 in blocks
-    assert "0x5b6fd8fda590e887531df12dec5faf2ce8c94a3eeb56bcc1fde760fabd64e56e" in [tx["hash"] for tx in transactions]
-    assert "0x10f4376f7efe2637be4d012eebad143dce58626146befa48204f1275476064d6" in [tx["hash"] for tx in transactions]
-
-    for tx in transactions:
-        assert "aiotx_decoded_input" in tx.keys()
+    assert 3247853 in blocks
+    assert 3247854 in blocks
+    assert "7604930759225ab74868969da6b19b399d8b189bd9506f39e15019f8e08a1d44" in [tx["txid"] for tx in transactions]
+    assert "992b887a10aa924430e905174535fd92733136b76d39e835c109e3ff2719bd69" in [tx["txid"] for tx in transactions]
```

