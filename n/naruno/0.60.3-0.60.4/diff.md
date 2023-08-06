# Comparing `tmp/naruno-0.60.3.tar.gz` & `tmp/naruno-0.60.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno-0.60.3.tar", last modified: Wed Aug  2 15:08:28 2023, max compression
+gzip compressed data, was "naruno-0.60.4.tar", last modified: Sun Aug  6 19:45:52 2023, max compression
```

## Comparing `naruno-0.60.3.tar` & `naruno-0.60.4.tar`

### file list

```diff
@@ -1,304 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.646721 naruno-0.60.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENCE-naruno-gui_lib__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENCE-naruno-lib-kot__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENCE-naruno-lib-mix__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENCE-naruno-wallet-elipticcurve__.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-02 15:08:12.000000 naruno-0.60.3/LICENSE-others__.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 15:08:12.000000 naruno-0.60.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-02 15:08:28.646721 naruno-0.60.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-08-02 15:08:12.000000 naruno-0.60.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/accounts/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/commanders/delete_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/commanders/get_comnder.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/commanders/save_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/get_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/get_sequence_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/accounts/save_accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/api/buildozer/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/api/buildozer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/apps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    30414 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/apps/remote_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.586721 naruno-0.60.3/naruno/blockchain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/blockchain/block/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/block_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/change_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/create_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/get_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/get_block_from_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/get_minumum_transfer_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/blockchain/block/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/hash/accounts_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/hash/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/hash/calculate_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/hash/tx_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/just_one_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/max_data_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/max_tx_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/save_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/save_block_to_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/block/shares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/blockchain/candidate_block/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/blockchain/candidate_block/candidate_block_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    19173 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/consensus_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/finished/
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/finished/finished_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/finished/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/finished/transactions/transactions_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/finished/true_time/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/finished/true_time/true_time_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/ongoing/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/ongoing/ongoing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.594721 naruno-0.60.3/naruno/consensus/rounds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/rounds/round_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/candidate_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.590721 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.614721 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/checks/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_newly/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_validated/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_1/round_1_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.594721 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/process/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/process/rescue/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/rounds/round_2/process/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/process/validate/validate_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/rounds/round_2/round_2_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/consensus/sync/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/sync/send_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/sync/send_block_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/consensus/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/blocks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/commanders/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/connected_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/connected_nodes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/connected_nodes_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/connected_nodes_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/connected_nodes_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/connected_nodes_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/connected_nodes_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/connected_nodes_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/extracted_proofs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/extracted_proofs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.618721 naruno-0.60.3/naruno/db/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/my_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/pending_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/pending_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/pending_transactions_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/pending_transactions_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/pending_transactions_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/pending_transactions_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/pending_transactions_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/pending_transactions_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/proof/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/proof/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/qrs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/qrs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/remote_app_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/remote_app_cache/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/signs/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/signs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_consensus_trigger_finished/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_consensus_trigger_finished/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main_2/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main_3/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main_3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main_false_time/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main_false_time/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_finished_main_no_reset/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_finished_main_no_reset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/db/test_proof_extracted/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/db/test_proof_extracted/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.622721 naruno-0.60.3/naruno/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.606721 naruno-0.60.3/naruno/gui/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.630721 naruno-0.60.3/naruno/gui/lib/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/POPPINS_LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.634721 naruno-0.60.3/naruno/gui/lib/images/
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo_sm_orb_fw.png
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo_w_bc.png
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/images/logo_win.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.606721 naruno-0.60.3/naruno/gui/lib/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.634721 naruno-0.60.3/naruno/gui/lib/libs/baseclass/
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/node_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/operations_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/root_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/settings_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/tabnavigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/wallet_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/baseclass/welcome_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.634721 naruno-0.60.3/naruno/gui/lib/libs/kv/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/node_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/operations_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/root_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/settings_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/tabnavigation.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/wallet_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/lib/libs/kv/welcome_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/popup.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/gui/the_naruno_gui_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/lib/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/backup/naruno_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/backup/naruno_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    26004 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/kot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/lib/mix/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/mix/merkle_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/mix/mixlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/lib/performance_analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/blockshash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/blockshash_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/heartbeat_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/performance_analyzers/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/perpetualtimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/settings_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/lib/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/logs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/node/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/node/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/node/get_candidate_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.638721 naruno-0.60.3/naruno/node/server/
--rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/node/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/node/unl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/check_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/datas/
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/datas/check_datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/len/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/len/check_len.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/sign/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/sign/check_sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/check/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/check/type/check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/get_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/check_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/get_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/get_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/save_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/save_to_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/sended_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/my_transactions/validate_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.642721 naruno-0.60.3/naruno/transactions/pending/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/pending/delete_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/pending/get_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/pending/save_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/pending_to_validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/print_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/process_the_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/transactions/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.646721 naruno-0.60.3/naruno/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/delete_current_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.646721 naruno-0.60.3/naruno/wallet/ellipticcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/privateKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/publicKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.646721 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/der.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/ellipticcurve/utils/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/get_saved_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/print_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/save_wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/wallet_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/wallet_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/wallet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 15:08:12.000000 naruno-0.60.3/naruno/wallet/wallet_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:28.610721 naruno-0.60.3/naruno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 15:08:28.000000 naruno-0.60.3/naruno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:08:28.646721 naruno-0.60.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-02 15:08:12.000000 naruno-0.60.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.823934 naruno-0.60.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-06 19:45:41.000000 naruno-0.60.4/LICENCE-naruno-gui_lib__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-06 19:45:41.000000 naruno-0.60.4/LICENCE-naruno-lib-kot__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-06 19:45:41.000000 naruno-0.60.4/LICENCE-naruno-lib-mix__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 19:45:41.000000 naruno-0.60.4/LICENCE-naruno-wallet-elipticcurve__.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-06 19:45:41.000000 naruno-0.60.4/LICENSE-others__.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-06 19:45:41.000000 naruno-0.60.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-06 19:45:52.823934 naruno-0.60.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-08-06 19:45:41.000000 naruno-0.60.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.803934 naruno-0.60.4/naruno/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.803934 naruno-0.60.4/naruno/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/accounts/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.803934 naruno-0.60.4/naruno/accounts/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/accounts/commanders/delete_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/accounts/commanders/get_comnder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/accounts/commanders/save_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/accounts/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/accounts/get_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/accounts/get_sequence_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/accounts/save_accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.803934 naruno-0.60.4/naruno/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.803934 naruno-0.60.4/naruno/api/buildozer/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/api/buildozer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.803934 naruno-0.60.4/naruno/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/apps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32052 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/apps/remote_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.799934 naruno-0.60.4/naruno/blockchain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/blockchain/block/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/block_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/change_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/create_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/get_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/get_block_from_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/get_minumum_transfer_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/blockchain/block/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/hash/accounts_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/hash/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/hash/calculate_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/hash/tx_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/just_one_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/max_data_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/max_tx_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24418 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/save_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/save_block_to_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/block/shares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/blockchain/candidate_block/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/blockchain/candidate_block/candidate_block_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/consensus_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/finished/
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/finished/finished_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/finished/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/finished/transactions/transactions_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/finished/true_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/finished/true_time/true_time_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/ongoing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/ongoing/ongoing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.799934 naruno-0.60.4/naruno/consensus/rounds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/checks/candidate_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.799934 naruno-0.60.4/naruno/consensus/rounds/round_1/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/find_newly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/find_validated/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_1/round_1_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_2/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_2/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.799934 naruno-0.60.4/naruno/consensus/rounds/round_2/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_2/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_2/process/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_2/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_2/process/rescue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/rounds/round_2/process/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_2/process/validate/validate_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/rounds/round_2/round_2_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/consensus/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/sync/send_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/sync/send_block_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/consensus/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/blocks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/commanders/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/connected_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/connected_nodes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/connected_nodes_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/connected_nodes_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/connected_nodes_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/connected_nodes_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/connected_nodes_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/connected_nodes_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/extracted_proofs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/extracted_proofs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/my_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/pending_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/pending_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/pending_transactions_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/pending_transactions_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.807934 naruno-0.60.4/naruno/db/pending_transactions_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/pending_transactions_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/pending_transactions_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/pending_transactions_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/proof/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/proof/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/qrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/qrs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/remote_app_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/remote_app_cache/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/signs/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/signs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_consensus_trigger_finished/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_consensus_trigger_finished/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_finished_main/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_finished_main/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_finished_main_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_finished_main_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_finished_main_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_finished_main_3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_finished_main_false_time/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_finished_main_false_time/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_finished_main_no_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_finished_main_no_reset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/db/test_proof_extracted/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/db/test_proof_extracted/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.811934 naruno-0.60.4/naruno/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.799934 naruno-0.60.4/naruno/gui/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.815934 naruno-0.60.4/naruno/gui/lib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/POPPINS_LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.815934 naruno-0.60.4/naruno/gui/lib/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/images/logo_sm_orb_fw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/images/logo_w_bc.png
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/images/logo_win.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.799934 naruno-0.60.4/naruno/gui/lib/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.815934 naruno-0.60.4/naruno/gui/lib/libs/baseclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/baseclass/node_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/baseclass/operations_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/baseclass/root_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/baseclass/settings_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/baseclass/tabnavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/baseclass/wallet_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/baseclass/welcome_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/gui/lib/libs/kv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/kv/node_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/kv/operations_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/kv/root_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/kv/settings_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/kv/tabnavigation.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/kv/wallet_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/lib/libs/kv/welcome_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/gui/the_naruno_gui_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/lib/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/backup/naruno_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/backup/naruno_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26004 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/kot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/lib/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/mix/merkle_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/mix/mixlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/lib/performance_analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/performance_analyzers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/performance_analyzers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/performance_analyzers/blockshash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/performance_analyzers/blockshash_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/performance_analyzers/heartbeat_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/performance_analyzers/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/perpetualtimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/settings_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/lib/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/logs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/node/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/node/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/node/get_candidate_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/node/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/node/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/node/unl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/transactions/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/check/check_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/transactions/check/datas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/check/datas/check_datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/transactions/check/len/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/check/len/check_len.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/transactions/check/sign/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/check/sign/check_sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.819934 naruno-0.60.4/naruno/transactions/check/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/check/type/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/get_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.823934 naruno-0.60.4/naruno/transactions/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/my_transactions/check_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/my_transactions/get_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/my_transactions/get_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/my_transactions/save_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/my_transactions/save_to_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/my_transactions/sended_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/my_transactions/validate_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.823934 naruno-0.60.4/naruno/transactions/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/pending/delete_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/pending/get_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/pending/save_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/pending_to_validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/print_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/process_the_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/transactions/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.823934 naruno-0.60.4/naruno/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/delete_current_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.823934 naruno-0.60.4/naruno/wallet/ellipticcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/privateKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/publicKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.823934 naruno-0.60.4/naruno/wallet/ellipticcurve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/utils/der.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/utils/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/utils/oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/ellipticcurve/utils/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/get_saved_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/print_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/save_wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/wallet_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/wallet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/wallet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-06 19:45:41.000000 naruno-0.60.4/naruno/wallet/wallet_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:52.803934 naruno-0.60.4/naruno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-06 19:45:52.000000 naruno-0.60.4/naruno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-08-06 19:45:52.000000 naruno-0.60.4/naruno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:45:52.000000 naruno-0.60.4/naruno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-06 19:45:52.000000 naruno-0.60.4/naruno.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 19:45:52.000000 naruno-0.60.4/naruno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:45:52.823934 naruno-0.60.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-06 19:45:41.000000 naruno-0.60.4/setup.py
```

### Comparing `naruno-0.60.3/LICENCE-naruno-gui_lib__.md` & `naruno-0.60.4/LICENCE-naruno-gui_lib__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/LICENCE-naruno-lib-kot__.md` & `naruno-0.60.4/LICENCE-naruno-lib-kot__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/LICENCE-naruno-lib-mix__.md` & `naruno-0.60.4/LICENCE-naruno-lib-mix__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/LICENCE-naruno-wallet-elipticcurve__.md` & `naruno-0.60.4/LICENCE-naruno-wallet-elipticcurve__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/LICENSE-others__.md` & `naruno-0.60.4/LICENSE-others__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/PKG-INFO` & `naruno-0.60.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.60.3
+Version: 0.60.4
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.60.3 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.60.4 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.60.3/README.md` & `naruno-0.60.4/README.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/accounts/account.py` & `naruno-0.60.4/naruno/accounts/account.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/accounts/commanders/delete_commander.py` & `naruno-0.60.4/naruno/accounts/commanders/delete_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/accounts/commanders/get_comnder.py` & `naruno-0.60.4/naruno/accounts/commanders/get_comnder.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/accounts/commanders/save_commander.py` & `naruno-0.60.4/naruno/accounts/commanders/save_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/accounts/get_accounts.py` & `naruno-0.60.4/naruno/accounts/get_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/accounts/get_balance.py` & `naruno-0.60.4/naruno/accounts/get_balance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from urllib.request import urlopen
+from decimal import Decimal
+
 
 from naruno.accounts.get_accounts import GetAccounts
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.block.get_minumum_transfer_amount import \
     GetMinimumTransferAmount
 from naruno.lib.settings_system import the_settings
 from naruno.transactions.pending.get_pending import GetPending
@@ -38,25 +40,26 @@
     else:
         if block is None:
             try:
                 block = GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
             except TypeError:
                 return None
 
-        balance = -block.minumum_transfer_amount
+
+        balance = Decimal(str(-block.minumum_transfer_amount))
 
         the_account_list = GetAccounts(
         ) if account_list is None else account_list
-        balance += the_account_list[address][
-            1] if address in the_account_list else 0
+        balance = balance + Decimal(str(the_account_list[address][
+            1])) if address in the_account_list else balance + Decimal(str(0))
 
         if not block.just_one_tx:
             the_pending = custom_pending if custom_pending is not None else GetPending()
             for tx in block.validating_list + the_pending:
                 sub_control = True
                 if tx_signature is not None:
                     if tx.signature == tx_signature:
                         sub_control = False
                 if Address(tx.fromUser) == user and sub_control:
-                    balance -= float(tx.amount) + float(tx.transaction_fee)
+                    balance = balance - (Decimal(str(tx.amount)) + Decimal(str(tx.transaction_fee)))
 
-    return balance
+    return float(balance)
```

### Comparing `naruno-0.60.3/naruno/accounts/get_sequence_number.py` & `naruno-0.60.4/naruno/accounts/get_sequence_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/accounts/save_accounts.py` & `naruno-0.60.4/naruno/accounts/save_accounts.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,24 +41,22 @@
 
     os.chdir(get_config()["main_folder"])
 
     if type(new_account) != list:
         new_account = [new_account]
 
     if sequence is not None:
-        logger.info("Sequence is not node")
+        logger.debug("Sequence is not node")
         the_string=str(sequence)+str(custom_TEMP_ACCOUNTS_PATH)
-        logger.debug(f"String: {the_string}")
         the_hash = hashlib.sha256(the_string.encode()).hexdigest()
-        logger.debug(f"Hash: {the_hash}")
         if the_hash in operations_hashes:
             logger.warning("Two times try")
             return
         else:
-            logger.info("Passed")
+            logger.debug("Passed")
             operations_hashes.append(the_hash)
 
 
 
     the_TEMP_ACCOUNTS_PATH = (TEMP_ACCOUNTS_PATH if custom_TEMP_ACCOUNTS_PATH
                               is None else custom_TEMP_ACCOUNTS_PATH)
```

### Comparing `naruno-0.60.3/naruno/api/buildozer/main.py` & `naruno-0.60.4/naruno/api/buildozer/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/api/main.py` & `naruno-0.60.4/naruno/api/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/apps/checker.py` & `naruno-0.60.4/naruno/apps/checker.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/apps/remote_app.py` & `naruno-0.60.4/naruno/apps/remote_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,24 +41,26 @@
 from naruno.wallet.wallet_import import Address
 from naruno.wallet.wallet_import import wallet_import
 
 logger = get_logger("REMOTE_APP")
 
 
 class splitted_data:
+    """ """
 
     def __init__(self, split):
         self.split = split
         self.main_data = None
         self.validated = False
         self.data = []
         self.data_original = []
 
 
 class Integration:
+    """ """
 
     def __init__(
         self,
         app_name,
         host="localhost",
         port=8000,
         password="123",
@@ -170,110 +172,125 @@
 
         self.host = backup_host
         self.port = backup_port
 
         logger.info(f"Integration of {self.app_name} is started")
 
     def change_by_network(self):
+        """ """
         self.host = "test_net.1.naruno.org" if the_settings(
         )["baklava"] else self.host
         self.port = 8000 if the_settings()["baklava"] else self.port
 
     def init_api(self):
+        """ """
         try:
             self.prepare_request("/", "get")
         except Exception as e:
             self.start_api()
 
     def start_api(self):
+        """ """
         backup = sys.argv
         sys.argv = [sys.argv[0]]
 
         self.api = start(host=self.host, port=self.port, test=True)
 
         self.api_thread = threading.Thread(target=self.api.run)
         self.api_thread.start()
         sys.argv = backup
 
     def wait_until_complated(self, custom_list=None):
+        """
+
+        :param custom_list: Default value = None)
+
+        """
         while len(self.sended_txs) > 0:
             time.sleep(self.sending_wait_time)
             self.sended_txs = (custom_list
                                if custom_list is not None else self.sended_txs)
 
     def close(self):
+        """ """
         DeleteCommander(self.commander) if not self.commander is None else None
         self.wait_until_complated() if self.check_thread is not None else None
         self.check_thread.cancel() if self.check_thread is not None else None
         if self.api is not None:
             self.api.close()
 
     def disable_cache(self):
+        """ """
         self.cache_true = False
         self.cache = []
 
     def get_cache(self):
+        """ """
         if self.cache_true == False:
             self.cache = []
             return
 
         record = self.integrationcache_db.get("cache")
 
         if record is None:
             self.cache = []
             self.save_cache()
         else:
             self.cache = record
-            self.backward_support_cache()
             self.save_cache()
 
-    def backward_support_cache(self):
-        for each_cache in self.cache:
-            if len(self.cache[self.cache.index(each_cache)]) != 96:
-                # remoe the cache
-                self.cache.remove(each_cache)
-
     def save_cache(self):
+        """ """
         if self.cache_true == False:
             self.get_cache()
             return
 
-        self.backward_support_cache()
-
         self.integrationcache_db.set("cache", self.cache)
 
     def delete_cache(self):
+        """ """
         self.integrationcache_db.delete("cache")
 
     def prepare_request(self, end_point, type, data=None) -> requests.Response:
         """
+
         :param end_point: The end point of the request
         :param type: The type of the request (get, post)
-        :param data: The data of the request
-        :return: The response of the request
+        :param data: The data of the request (Default value = None)
+        :returns: The response of the request
+
         """
         api = f"http://{self.host}:{self.port}"
 
         response = None
         if type == "post":
             response = requests.post(api + end_point, data=data)
         elif type == "get":
             response = requests.get(api + end_point)
 
         return response
 
     def send_forcer(self, action, app_data, to_user, retrysecond):
+        """
+
+        :param action: param app_data:
+        :param to_user: param retrysecond:
+        :param app_data: param retrysecond:
+        :param retrysecond:
+
+        """
         stop = False
         while stop == False:
             stop = self.send(action, app_data, to_user, force=False)
             if stop == False:
                 time.sleep(retrysecond)
         return stop
 
     def generate_random_split_key(self):
+        """ """
         rando = ""
         for i in range(5):
             rando += random.choice(string.ascii_letters)
         return rando
 
     def send_splitter(
         self,
@@ -283,14 +300,27 @@
         system_length,
         true_length,
         force=True,
         retrysecond=10,
         custom_checker=None,
         custom_random=None,
     ) -> bool:
+        """
+
+        :param action: param app_data:
+        :param to_user: param system_length:
+        :param true_length: param force:  (Default value = True)
+        :param retrysecond: Default value = 10)
+        :param custom_checker: Default value = None)
+        :param custom_random: Default value = None)
+        :param app_data: param system_length:
+        :param force: Default value = True)
+        :param system_length:
+
+        """
         backup_checking = copy.copy(self.checking)
         self.checking = False
         # generate random charactere
         rando = (custom_random if custom_random is not None else
                  self.generate_random_split_key())
 
         split_random = rando + "-"
@@ -344,27 +374,33 @@
             to_user=to_user,
             force=force,
             retrysecond=retrysecond,
         )
         return True
 
     def wait_until_true_time(self):
+        """ """
         time.sleep(self.wait_amount - (time.time() - self.last_sended))
 
     def send(self,
              action,
              app_data,
              to_user,
              amount=None,
              force=True,
              retrysecond=10) -> bool:
         """
+
         :param action: The action of the app
         :param app_data: The data of the app
         :param to_user: The user to send the data to
+        :param amount: Default value = None)
+        :param force: Default value = True)
+        :param retrysecond: Default value = 10)
+
         """
 
         self.wait_until_true_time(
         ) if time.time() - self.last_sended < self.wait_amount else None
 
         self.host = copy.copy(self.first_host)
         self.port = copy.copy(self.first_port)
@@ -423,16 +459,17 @@
                 logger.error("Error on sending message")
                 if force:
                     logger.info("Trying to send again")
                     return self.send_forcer(action, app_data, to_user,
                                             retrysecond)
                 return False
             else:
+                response_json = json.loads(response.text)          
                 logger.info(
-                    f"Message sent: app_name:{self.app_name} action:{action} data: {data} to: {to_user}"
+                    f"Message sent: app_name:{self.app_name} action:{action} data: {app_data} to: {to_user} in TX: {response_json['signature']}"
                 )
                 time.sleep(1)
                 self.last_sended = time.time()
                 if self.checking and self.check_thread is None:
                     checker(self)
                 return True
 
@@ -441,14 +478,24 @@
         get_all,
         disable_caches,
         disable_sended_not_validated,
         force_sended,
         raw_data_return=False,
         raw_datas=None,
     ):
+        """
+
+        :param get_all: param disable_caches:
+        :param disable_sended_not_validated: param force_sended:
+        :param raw_data_return: Default value = False)
+        :param raw_datas: Default value = None)
+        :param disable_caches: param force_sended:
+        :param force_sended:
+
+        """
         self.get_cache() if not disable_caches else None
         response = self.prepare_request("/transactions/received", type="get")
         transactions = response.json()
 
         transactions_sended = {}
         transactions_sended_not_validated = {}
 
@@ -617,14 +664,15 @@
         last_list = []
 
         for transaction in new_dict:
             with contextlib.suppress(TypeError):
                 if not new_dict[transaction]["transaction"]["data"] == "NP":
                     if (self.app_name in new_dict[transaction]["transaction"]
                         ["data"]["action"]):
+                        new_dict[transaction]["transaction"]["data"]["action"] = new_dict[transaction]["transaction"]["data"]["action"].replace(self.app_name, "")
                         last_list.append(new_dict[transaction]["transaction"])
 
         splits = []
         # finding transactions that data start with split
         new_a_last_list = copy.copy(last_list)
         for transaction in last_list:
             # check new_dict[transaction]["transaction"]["data"] is start with split
@@ -732,27 +780,33 @@
                   or transaction["fromUser"] in commanders):
                 result.append(transaction)
 
         for transaction in result[:]:
             if transaction["data"]["app_data"].startswith("split-"):
                 result.remove(transaction) if not get_all else None
 
-        if not len(result) == 0:
-            logger.info("New datas received")
-
         return result
 
     def get(
         self,
         get_all=False,
         disable_caches=False,
         from_thread=False,
         disable_sended_not_validated=False,
         force_sended=False,
     ):
+        """
+
+        :param get_all: Default value = False)
+        :param disable_caches: Default value = False)
+        :param from_thread: Default value = False)
+        :param disable_sended_not_validated: Default value = False)
+        :param force_sended: Default value = False)
+
+        """
         self.host = copy.copy(self.first_host)
         self.port = copy.copy(self.first_port)
 
         backup_host = copy.copy(self.host)
         backup_port = copy.copy(self.port)
 
         self.wait_until_complated() if ((self.sended or force_sended)
@@ -782,14 +836,17 @@
             disable_sended_not_validated=disable_sended_not_validated,
             force_sended=force_sended,
             raw_datas=baklava_datas,
         )
 
         the_list = second
 
+        if not len(the_list) == 0:
+            logger.info("New datas received")
+
         with contextlib.suppress(TypeError):
             if "print" in inspect.stack()[1].code_context[0]:
                 total = ""
                 for data in the_list:
                     fromUser = data["fromUser"]
                     toUser = data["toUser"]
                     action = data["data"]["action"].replace(self.app_name, "")
```

### Comparing `naruno-0.60.3/naruno/blockchain/block/block_main.py` & `naruno-0.60.4/naruno/blockchain/block/block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/blocks_hash.py` & `naruno-0.60.4/naruno/blockchain/block/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/change_transaction_fee.py` & `naruno-0.60.4/naruno/blockchain/block/change_transaction_fee.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     custom_pending_transaction_len=None,
     custom_PENDING_TRANSACTIONS_PATH=None,
 ):
     """
     Increase transaction fee by 0.01 naruno coin for each block.default_optimum_transaction_number argument
     """
     logger.info("Calculating the transaction fee")
-    logger.info(f"Start fee is: {block.transaction_fee}")
+    logger.debug(f"Start fee is: {block.transaction_fee}")
     pending_transactions = (GetPendingLen(
         custom_PENDING_TRANSACTIONS_PATH=custom_PENDING_TRANSACTIONS_PATH)
                             if custom_pending_transaction_len is None else
                             custom_pending_transaction_len)
     validating_list_len = 0
     for tx in block.validating_list:
         if tx.signature != "NARUNO":
@@ -38,13 +38,13 @@
     logger.debug(
         f"block.default_increase_of_fee {block.default_increase_of_fee}")
     if (total_len // block.default_optimum_transaction_number) != 0:
         increase = (total_len // block.default_optimum_transaction_number
                     ) * block.default_increase_of_fee
         decimal_amount = Decimal(str(block.transaction_fee)) + Decimal(str(increase))
         block.transaction_fee = float(decimal_amount)
-        logger.info("Transaction fee will be increased")
+        logger.debug("Transaction fee will be increased")
 
     else:
-        logger.info("Transaction fee is not changed")
+        logger.debug("Transaction fee is not changed")
         block.transaction_fee = block.default_transaction_fee
-    logger.info(f"New transaction fee is : {block.transaction_fee} ")
+    logger.debug(f"New transaction fee is : {block.transaction_fee} ")
```

### Comparing `naruno-0.60.3/naruno/blockchain/block/create_block.py` & `naruno-0.60.4/naruno/blockchain/block/create_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/get_block.py` & `naruno-0.60.4/naruno/blockchain/block/get_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/get_block_from_blockchain_db.py` & `naruno-0.60.4/naruno/blockchain/block/get_block_from_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/get_minumum_transfer_amount.py` & `naruno-0.60.4/naruno/blockchain/block/get_minumum_transfer_amount.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/hash/accounts_hash.py` & `naruno-0.60.4/naruno/blockchain/block/hash/accounts_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/hash/blocks_hash.py` & `naruno-0.60.4/naruno/blockchain/block/hash/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/hash/calculate_hash.py` & `naruno-0.60.4/naruno/blockchain/block/hash/calculate_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/hash/tx_hash.py` & `naruno-0.60.4/naruno/blockchain/block/hash/tx_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/just_one_tx.py` & `naruno-0.60.4/naruno/blockchain/block/just_one_tx.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/max_data_size.py` & `naruno-0.60.4/naruno/blockchain/block/max_data_size.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/max_tx_number.py` & `naruno-0.60.4/naruno/blockchain/block/max_tx_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/block/save_block_to_blockchain_db.py` & `naruno-0.60.4/naruno/blockchain/block/save_block_to_blockchain_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ):
     """
     Adds the block to the blockchain database
     at BLOCKS_PATH.
     """
 
     logger.info("Saving block to blockchain database...")
-    logger.info(f"Block: {block.__dict__}")
+    logger.debug(f"Block: {block.__dict__}")
 
     if the_settings()["dont_save_blocks"]:
         logger.debug("Not saving blocks because of settings.")
         return True
 
     my_public_key = "".join([
         l.strip() for l in wallet_import(-1, 0).splitlines()
```

### Comparing `naruno-0.60.3/naruno/blockchain/block/shares.py` & `naruno-0.60.4/naruno/blockchain/block/shares.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/blockchain/candidate_block/candidate_block_main.py` & `naruno-0.60.4/naruno/blockchain/candidate_block/candidate_block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/cli/main.py` & `naruno-0.60.4/naruno/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import threading
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", ".."))
 import time
 from getpass import getpass
 
 from naruno.accounts.get_balance import GetBalance
-from naruno.blockchain.block.create_block import CreateBlock
 from naruno.blockchain.block.block_main import Block
+from naruno.blockchain.block.create_block import CreateBlock
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.block.save_block import SaveBlock
 from naruno.config import MY_TRANSACTION_EXPORT_PATH
 from naruno.consensus.consensus_main import consensus_trigger
 from naruno.lib.backup.naruno_export import naruno_export
 from naruno.lib.backup.naruno_import import naruno_import
 from naruno.lib.export import export_the_transactions
@@ -48,17 +48,15 @@
 from naruno.wallet.wallet_import import wallet_import
 from naruno.wallet.wallet_selector import wallet_selector
 
 logger = get_logger("CLI")
 
 
 def show_menu():
-    """
-    Prints some information and the menu.
-    """
+    """Prints some information and the menu."""
 
     print(
         banner_maker(
             sc_name="Naruno",
             description=
             "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.",
             author="Naruno Developers",
@@ -105,26 +103,31 @@
         menu_space() + menu_maker(menu_number="publishermodeon",
                                   menu_text="Publisher Mode On") +
         menu_maker(menu_number="publishermodeoff",
                    menu_text="Publisher Mode Off") + menu_space())
 
     print(quit_menu_maker(mode="main"))
 
+
 def get_block_process():
-                the_block = CreateBlock()
-                SaveBlock(the_block)
-                server.Server.send_block_to_other_nodes()
-                logger.info("Consensus timer is started")
-                perpetualTimer(the_block.consensus_timer, consensus_trigger, the_consensus=True)    
+    """ """
+    the_block = CreateBlock()
+    SaveBlock(the_block)
+    server.Server.send_block_to_other_nodes()
+    logger.info("Consensus timer is started")
+    perpetualTimer(the_block.consensus_timer,
+                   consensus_trigger,
+                   the_consensus=True)
 
 
 def menu():
-    """
-    The main structure of the cli mode, this function prints the menu,
+    """The main structure of the cli mode, this function prints the menu,
     listens to the entries, makes the directions.
+
+
     """
 
     animation = [
         "[■□□□□□□□□□]",
         "[■■□□□□□□□□]",
         "[■■■□□□□□□□]",
         "[■■■■□□□□□□]",
@@ -165,44 +168,46 @@
                 getpass("Password: "),
                 input("Please write receiver adress: "),
                 amount=input("Coin Amount (ex. 1.0): "),
                 block=block,
             )
 
             if send_tx != False:
-                    SavetoMyTransaction(send_tx, sended=True)
-                    if not the_settings()["baklava"]:
-                        from naruno.node.server.server import server
-                        if server.Server is None:
-                            print("Please start the node server")
-                            return False
-                        server.send_transaction(send_tx)
-                        SaveBlock(block)
+                SavetoMyTransaction(send_tx, sended=True)
+                if not the_settings()["baklava"]:
+                    from naruno.node.server.server import server
+
+                    if server.Server is None:
+                        print("Please start the node server")
+                        return False
+                    server.send_transaction(send_tx)
+                    SaveBlock(block)
 
         if choices_input == "scd":
             if not the_settings()["baklava"]:
                 block = GetBlock()
             else:
                 block = Block("baklava")
             send_tx = send(
                 getpass("Password: "),
                 input("Please write receiver adress: "),
                 amount=input("Coin Amount (ex. 1.0): "),
                 data=input("Data: "),
                 block=block,
             )
             if send_tx != False:
-                    SavetoMyTransaction(send_tx, sended=True)
-                    if not the_settings()["baklava"]:
-                        from naruno.node.server.server import server
-                        if server.Server is None:
-                            print("Please start the node server")
-                            return False
-                        server.send_transaction(send_tx)
-                        SaveBlock(block)
+                SavetoMyTransaction(send_tx, sended=True)
+                if not the_settings()["baklava"]:
+                    from naruno.node.server.server import server
+
+                    if server.Server is None:
+                        print("Please start the node server")
+                        return False
+                    server.send_transaction(send_tx)
+                    SaveBlock(block)
 
         if choices_input == "gb":
             print(GetBalance(wallet_import(-1, 0)))
         if choices_input == "help":
             show_menu()
         if choices_input == "ndstart":
             server(str(input("ip: ")), int(input("port: ")))
@@ -275,17 +280,15 @@
         os.system("cls" if os.name == "nt" else "clear")
 
         if choices_input == "0":
             exit()
 
 
 def arguments():
-    """
-    This function parses the arguments and makes the directions.
-    """
+    """This function parses the arguments and makes the directions."""
 
     parser = argparse.ArgumentParser(
         description=
         "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system. Use the menu (-m) or GUI to gain full control and use the node, operation, etc."
     )
 
     parser.add_argument("-pw",
@@ -422,14 +425,16 @@
         "--timeout",
         type=int,
         help="Timeout",
     )
 
     args = parser.parse_args()
 
+    safety_check(args.interface, args.timeout)
+
     if len(sys.argv) < 2:
         parser.print_help()
 
     if args.printwallet:
         print_wallets()
 
     if args.getbalance:
@@ -466,16 +471,14 @@
 
     if args.returntransactions:
         PrintTransactions()
 
     if args.status:
         print(Status())
 
-    safety_check(args.interface, args.timeout)
-
     if args.ndnewunl is not None:
         Unl.save_new_unl_node(args.ndnewunl)
 
     if args.createwallet is not None:
         wallet_create(args.createwallet)
 
     if args.deletewallet:
@@ -522,17 +525,15 @@
             return
 
     if args.menu:
         menu()
 
 
 def start():
-    """
-    Start the CLI mode with arguments.
-    """
+    """Start the CLI mode with arguments."""
 
     logger.info("Starting CLI mode")
 
     arguments()
 
 
 if __name__ == "__main__":
```

### Comparing `naruno-0.60.3/naruno/config.py` & `naruno-0.60.4/naruno/config.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/consensus_main.py` & `naruno-0.60.4/naruno/consensus/consensus_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,39 +52,39 @@
                 if custom_block is None else custom_block)
         pending_list_txs = GetPending()
 
         logger.info(
             f"BLOCK#{block.sequence_number}:{block.empty_block_number} Consensus process started"
         )
 
-        logger.info("Consensus Sync process started")
+        logger.debug("Consensus Sync process started")
         threading.Thread(
             target=sync,
             args=(
                 block,
                 pending_list_txs,
                 custom_server,
             ),
         ).start()
 
         if block.validated:
-            logger.info(
+            logger.debug(
                 "BLOCK is an validated block, consensus process is finished")
             finished_main(
                 block,
                 custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
                 custom_BLOCKS_PATH=custom_BLOCKS_PATH,
                 custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
                 custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
                 custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
                 pass_sync=pass_sync,
                 dont_clean=dont_clean,
             )
         else:
-            logger.info(
+            logger.debug(
                 "BLOCK is an unvalidated block, consensus process is ongoing")
             ongoing_main(
                 block,
                 custom_candidate_class=custom_candidate_class,
                 custom_unl_nodes=custom_unl_nodes,
                 custom_UNL_NODES_PATH=custom_UNL_NODES_PATH,
                 custom_server=custom_server,
@@ -94,12 +94,12 @@
                 custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
                 custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
                 pass_sync=pass_sync,
             )
     except:
         traceback.print_exc()
 
-    logger.info("Consensus process is done")
+    logger.debug("Consensus process is done")
     with contextlib.suppress(Exception):
         naruno.lib.perpetualtimer.the_consensus_thread = False    
 
     return block
```

### Comparing `naruno-0.60.3/naruno/consensus/finished/finished_main.py` & `naruno-0.60.4/naruno/consensus/finished/finished_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from naruno.transactions.pending_to_validating import PendingtoValidating
 from naruno.transactions.cleaner import Cleaner
 from naruno.transactions.pending.get_pending import GetPending
 import naruno
 
 logger = get_logger("CONSENSUS")
 def make_sync(the_server):
-    logger.info("Syncing the block to other nodes is triggered")
+    logger.debug("Syncing the block to other nodes is triggered")
     with contextlib.suppress(Exception):
         [
             the_server.send_block_to_other_nodes(sync_client, sync=True)
             for sync_client in the_server.sync_clients
         ]
 def finished_main(
     block: Block,
```

### Comparing `naruno-0.60.3/naruno/consensus/finished/transactions/transactions_main.py` & `naruno-0.60.4/naruno/consensus/finished/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/finished/true_time/true_time_main.py` & `naruno-0.60.4/naruno/consensus/finished/true_time/true_time_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 logger = get_logger("CONSENSUS")
 
 
 def true_time(block: Block, return_result=False) -> bool:
     the_time = (block.genesis_time + block.block_time + (
         (block.sequence_number + block.empty_block_number) * block.block_time))
     current_time = int(time.time())
-    logger.info("Consensus time control started")
+    logger.debug("Consensus time control started")
     logger.debug(f"current_time: {current_time}")
     logger.debug(f"the_time: {the_time}")        
     if current_time >= the_time:
         return True
     else:
         return False if return_result is False else the_time
```

### Comparing `naruno-0.60.3/naruno/consensus/ongoing/ongoing_main.py` & `naruno-0.60.4/naruno/consensus/ongoing/ongoing_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
     )
 
     the_block = Block(creator="Naruno") if block is None else block
 
     logger.debug(f"len(unl_nodes): {len(unl_nodes)}")
     if len(candidate_class.candidate_blocks) > ((
         (len(unl_nodes) + 1) * the_block.candidate_blocks_check) / 100):
-        logger.info("Candidate block number is True")
+        logger.debug("Candidate block number is True")
         return True
     else:
-        logger.info("Candidate block number is not True")
+        logger.debug("Candidate block number is not True")
         return False
```

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/checks/checks_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
     the_time = block.start_time + block.round_1_time
     current_time = int(time.time())
     logger.info("Round 1 time control started")
     logger.debug(f"current_time: {current_time}")
     logger.debug(f"the_time: {the_time}")
     if current_time >= the_time:
-        logger.info("Time is true")
+        logger.debug("Time is true")
         return True
     else:
         if not current_time >= the_time - (block.round_1_time / 2):
             #PendingtoValidating(block)
             SaveBlock(
                 block,
                 custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
                 custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
                 custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
                 custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
             )     
-        logger.info("Time is not true")
+        logger.debug("Time is not true")
         return False if return_result is False else the_time
```

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/process/process_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/process/process_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,21 +54,19 @@
     block = resukt_of_proccesstransaction[0]
     account_list = resukt_of_proccesstransaction[1]
 
     part_of_blocks_hash = GetBlockshash_part(
         custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH)
     the_blocks_hash = GetBlockshash(
         custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH)
-    logger.debug(f"part_of_blocks_hash: {part_of_blocks_hash}")
-    logger.debug(f"the_blocks_hash: {the_blocks_hash}")
-    logger.debug(f"account_list: {account_list}")
+
     block.hash = CalculateHash(block, part_of_blocks_hash, the_blocks_hash,
                                account_list)
 
-    logger.debug(f"Block hash {block.hash}")
+
 
     SaveBlock(
         block,
         custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
         custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
         custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
         custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
```

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 
     new_validating_list = []
     for tx in block.validating_list:
         if tx.signature == "NARUNO" or not any(tx.signature == tx2.signature
                    for tx2 in new_validating_list):
             new_validating_list.append(tx)
         else:
-            logger.info(
+            logger.debug(
                 f"tx: {tx} will be removed because its added more than one")
     block.validating_list = new_validating_list
     logger.debug(f"End block.validatin_list: {block.validating_list}")
     return block
```

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
     for my_validating_list in block.validating_list[:]:
         ok = any(
             (my_validating_list.signature == my_temp_validating_list.signature)
             for my_temp_validating_list in temp_validating_list[:])
 
         block.validating_list.remove(my_validating_list)
-        logger.info(
+        logger.debug(
             f"tx: {my_validating_list} will removed fron block.validating_list"
         )
         if not ok:
-            logger.info(
+            logger.debug(
                 f"tx: {temp_validating_list} will added to temp validating list"
             )
             newly_added_list.append(my_validating_list)
     logger.debug(f"End newly_added_list: {newly_added_list}")
     return newly_added_list
```

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_1/round_1_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_1/round_1_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,12 +19,12 @@
         f"len(candidate_class.candidate_block_hashes): {len(candidate_class.candidate_block_hashes)}"
     )
     logger.debug(f"len(unl_nodes): {len(unl_nodes)}")
 
     the_block = Block(creator="Naruno") if block is None else block
     if len(candidate_class.candidate_block_hashes) > ((
         (len(unl_nodes) + 1) * the_block.candidate_blocks_hashes_check) / 100):
-        logger.info("Candidate block hash number is True")
+        logger.debug("Candidate block hash number is True")
         return True
     else:
-        logger.info("Candidate block hash number is not True")
+        logger.debug("Candidate block hash number is not True")
         return False
```

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_2/checks/checks_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_2/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 
     true_time = block.round_2_starting_time + block.round_2_time
     current_time = int(time.time())
     logger.info("Round 2 time control started")
     logger.debug(f"current_time: {current_time}")
     logger.debug(f"true_time: {true_time}")
     if current_time >= true_time:
-        logger.info("Time is true")
+        logger.debug("Time is true")
         return True
     else:
-        logger.info("Time is not true")
+        logger.debug("Time is not true")
         return False
```

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,30 +35,30 @@
             if (candidate_block_hash != other_block
                     and candidate_block_hash["hash"] == other_block["hash"]):
                 tx_valid += 1
 
         logger.debug(f"Hash valid of  {candidate_block_hash} : {tx_valid}")
 
         if tx_valid > (((len(unl_nodes)+1) * block.process_candidate_blocks_hashes) / 100):
-            logger.info(
+            logger.debug(
                 f"candidate_block_hash: {candidate_block_hash} is validated.")
             current_hash = candidate_block_hash
 
     for candidate_block_hash in candidate_class.candidate_block_hashes[:]:
         logger.debug(f"Candidate block hash previous_hash {candidate_block_hash}")
 
         tx_valid = 1
 
         for other_block in candidate_class.candidate_block_hashes[:]:
             if (candidate_block_hash != other_block
                     and candidate_block_hash["previous_hash"] == other_block["previous_hash"]):
                 tx_valid += 1
         logger.debug(f"Hash valid of previous_hash  {candidate_block_hash} : {tx_valid}")
         if tx_valid > (((len(unl_nodes)+1) * block.process_candidate_blocks_hashes) / 100):
-            logger.info(
+            logger.debug(
                 f"candidate_block_hash previous_hash: {candidate_block_hash} is validated.")
             previous_hash = candidate_block_hash
 
 
 
     if current_hash != {"signature": "A", "hash": False, "previous_hash": False} or previous_hash != {"signature": "A", "hash": False, "previous_hash": False}:
         if current_hash["signature"] == "self":
```

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_2/process/process_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_2/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_2/process/validate/validate_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_2/process/validate/validate_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/rounds/round_2/round_2_main.py` & `naruno-0.60.4/naruno/consensus/rounds/round_2/round_2_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/sync/send_block.py` & `naruno-0.60.4/naruno/consensus/sync/send_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/sync/send_block_hash.py` & `naruno-0.60.4/naruno/consensus/sync/send_block_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/consensus/sync/sync.py` & `naruno-0.60.4/naruno/consensus/sync/sync.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/POPPINS_LICENCE` & `naruno-0.60.4/naruno/gui/lib/fonts/POPPINS_LICENCE`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Black.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Bold.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Italic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Light.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-LightItalic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Medium.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Regular.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-SemiBold.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-Thin.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf` & `naruno-0.60.4/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/images/logo.ico` & `naruno-0.60.4/naruno/gui/lib/images/logo.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/images/logo.png` & `naruno-0.60.4/naruno/gui/lib/images/logo.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/images/logo_sm_orb_fw.png` & `naruno-0.60.4/naruno/gui/lib/images/logo_sm_orb_fw.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/images/logo_w_bc.png` & `naruno-0.60.4/naruno/gui/lib/images/logo_w_bc.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/images/logo_win.ico` & `naruno-0.60.4/naruno/gui/lib/images/logo_win.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/baseclass/node_screen.py` & `naruno-0.60.4/naruno/gui/lib/libs/baseclass/node_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/baseclass/operations_screen.py` & `naruno-0.60.4/naruno/gui/lib/libs/baseclass/operations_screen.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,21 +28,26 @@
 from naruno.transactions.my_transactions.save_to_my_transaction import \
     SavetoMyTransaction
 from naruno.transactions.send import send
 from naruno.wallet.wallet_import import wallet_import
 
 
 class OperationScreen(MDScreen):
+    """ """
+
     pass
 
 
 class OperationBox(MDGridLayout):
+    """ """
+
     cols = 2
 
     def sent_the_coins(self):
+        """ """
         if not the_settings()["baklava"]:
             the_block = GetBlock()
         else:
             the_block = Block("baklava")
 
         the_balance = GetBalance(
             self.send_coin_dialog.input_results["Receiver"],
@@ -78,26 +83,28 @@
 
             else:
                 popup(title="Password is not correct", type="failure")
         else:
             popup(title="Amount is not enough", type="failure")
 
     def show_send_coin_dialog(self):
+        """ """
         self.send_coin_dialog = popup(
             title="Send Coin&Data",
             target=self.sent_the_coins,
             inputs=[
                 ["Receiver", False],
                 ["Amount", False],
                 ["Data", False],
                 ["Password", True],
             ],
         )
 
     def sign_the_data(self):
+        """ """
         path = sign(
             self.sign_dialog.input_results["Data"],
             self.sign_dialog.input_results["Password"],
         )
         if path == "Password is not True":
             popup(title="Password is not correct", type="failure")
         else:
@@ -115,21 +122,23 @@
                 )
             popup(
                 title="Signed data file copied to your clipboard.",
                 type="success",
             )
 
     def show_sign_dialog(self):
+        """ """
         self.sign_dialog = popup(
             title="Sign Data",
             target=self.sign_the_data,
             inputs=[["Data", False], ["Password", True]],
         )
 
     def verify_the_data(self):
+        """ """
         result = verify(self.verify_dialog.input_results["Path"])
 
         if result[0] == True:
             data_text = f"{result[1][:20]}..." if len(
                 result[1]) > 20 else result[1]
             popup(
                 title="Data is verified",
@@ -137,58 +146,82 @@
                 thirdly_title=f"The sender is : {result[2]}",
                 type="success",
             )
         else:
             popup(title="Data is not verified", type="failure")
 
     def show_verify_dialog(self):
+        """ """
         self.verify_dialog = popup(
             title="Verify Signed Data",
             target=self.verify_the_data,
             inputs=[["Path", False]],
         )
 
     def send_coin(self):
+        """ """
         try:
             GetBlock()
         except TypeError:
             if not the_settings()["baklava"]:
                 popup(title="Please connect to an network.", type="failure")
                 return False
         self.show_send_coin_dialog()
 
     def sign(self):
+        """ """
         self.show_sign_dialog()
 
     def verify(self):
+        """ """
         self.show_verify_dialog()
 
     def export_transaction_csv(self):
+        """ """
         if export_the_transactions():
+            export_location = MY_TRANSACTION_EXPORT_PATH
             Clipboard.copy(MY_TRANSACTION_EXPORT_PATH)
+            if platform == "android":
+                from android.storage import primary_external_storage_path
+
+                dir = primary_external_storage_path()
+                download_dir_path = os.path.join(dir, "Download")
+                new_path = os.path.join(download_dir_path,
+                                        export_location.split("/")[-1])
+                Clipboard.copy(new_path)
+                shutil.move(
+                    export_location,
+                    new_path,
+                )
             popup(
                 title=
-                f"CSV file created in {MY_TRANSACTION_EXPORT_PATH} directory, The directory has been copied to your clipboard.",
+                f"CSV file created and location has been copied to your clipboard.",
                 type="success",
             )
 
         else:
             popup(title="You have not a transaction", type="warning")
 
     def callback_for_transaction_history_items(self, *args):
+        """
+
+        :param *args:
+
+        """
         the_signature_of_tx = args[0].signature
         Clipboard.copy(the_signature_of_tx)
         popup(
             title=
             "The signature of transaction has been copied to your clipboard.",
             text=f"The signature is : {the_signature_of_tx}",
             type="success",
         )
 
     def transaction_history(self):
+        """ """
         transactions = GetMyTransaction()
         if len(transactions) != 0:
             bottom_sheet_menu = MDListBottomSheet(radius=25, radius_from="top")
             data = {
                 tx[0]:
                 f"{tx[0].toUser} | {str(tx[0].amount)} | {str(tx[0].transaction_fee)} | {str(tx[1])}"
                 for tx in transactions
```

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/baseclass/root_screen.py` & `naruno-0.60.4/naruno/gui/lib/libs/baseclass/root_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/baseclass/settings_screen.py` & `naruno-0.60.4/naruno/gui/lib/libs/baseclass/settings_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/baseclass/tabnavigation.py` & `naruno-0.60.4/naruno/gui/lib/libs/baseclass/tabnavigation.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/baseclass/wallet_screen.py` & `naruno-0.60.4/naruno/gui/lib/libs/baseclass/wallet_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/baseclass/welcome_screen.py` & `naruno-0.60.4/naruno/gui/lib/libs/baseclass/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/kv/node_screen.kv` & `naruno-0.60.4/naruno/gui/lib/libs/kv/node_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/kv/operations_screen.kv` & `naruno-0.60.4/naruno/gui/lib/libs/kv/operations_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/kv/root_screen.kv` & `naruno-0.60.4/naruno/gui/lib/libs/kv/root_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/kv/settings_screen.kv` & `naruno-0.60.4/naruno/gui/lib/libs/kv/settings_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/kv/tabnavigation.kv` & `naruno-0.60.4/naruno/gui/lib/libs/kv/tabnavigation.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/kv/wallet_screen.kv` & `naruno-0.60.4/naruno/gui/lib/libs/kv/wallet_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/lib/libs/kv/welcome_screen.kv` & `naruno-0.60.4/naruno/gui/lib/libs/kv/welcome_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/main.py` & `naruno-0.60.4/naruno/gui/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/gui/popup.py` & `naruno-0.60.4/naruno/gui/popup.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/backup/naruno_export.py` & `naruno-0.60.4/naruno/lib/backup/naruno_export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/backup/naruno_import.py` & `naruno-0.60.4/naruno/lib/backup/naruno_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/clean_up.py` & `naruno-0.60.4/naruno/lib/clean_up.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/config_system.py` & `naruno-0.60.4/naruno/lib/config_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/encryption.py` & `naruno-0.60.4/naruno/lib/encryption.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/export.py` & `naruno-0.60.4/naruno/lib/export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/kot.py` & `naruno-0.60.4/naruno/lib/kot.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/log.py` & `naruno-0.60.4/naruno/lib/log.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/mix/merkle_root.py` & `naruno-0.60.4/naruno/lib/mix/merkle_root.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/mix/mixlib.py` & `naruno-0.60.4/naruno/lib/mix/mixlib.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/notification.py` & `naruno-0.60.4/naruno/lib/notification.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/performance_analyzers/accounts.py` & `naruno-0.60.4/naruno/lib/performance_analyzers/accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/performance_analyzers/block.py` & `naruno-0.60.4/naruno/lib/performance_analyzers/block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/performance_analyzers/blockshash.py` & `naruno-0.60.4/naruno/lib/performance_analyzers/blockshash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/performance_analyzers/blockshash_part.py` & `naruno-0.60.4/naruno/lib/performance_analyzers/blockshash_part.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/performance_analyzers/heartbeat_db.py` & `naruno-0.60.4/naruno/lib/performance_analyzers/heartbeat_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/performance_analyzers/transactions.py` & `naruno-0.60.4/naruno/lib/performance_analyzers/transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/perpetualtimer.py` & `naruno-0.60.4/naruno/lib/perpetualtimer.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/qr.py` & `naruno-0.60.4/naruno/lib/qr.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/safety.py` & `naruno-0.60.4/naruno/lib/safety.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,24 @@
 def safety_check(
     interface=None,
     timeout=None,
     exit_on_error=True,
     custom_pywall=None,
     custom_debug_mode=None,
 ):
-    logger.info("Checking safety")
+    """
+
+    :param interface: Default value = None)
+    :param timeout: Default value = None)
+    :param exit_on_error: Default value = True)
+    :param custom_pywall: Default value = None)
+    :param custom_debug_mode: Default value = None)
+
+    """
+    logger.debug("Checking safety")
     try:
         the_import_string = "from pywall import pywall"
         pywall_class = (exec(the_import_string)
                         if custom_pywall is None else custom_pywall)
         the_pywall = pywall() if custom_pywall is None else custom_pywall()
         the_pywall.iface = the_pywall.iface if interface is None else interface
         the_pywall.timeout = the_pywall.timeout if timeout is None else timeout
@@ -33,15 +42,15 @@
 
         if control is not None:
             if control:
                 logger.error("NOT Safe")
                 exit() if exit_on_error else None
                 return False
             else:
-                logger.info("Safe")
+                logger.debug("Safe")
                 return True
         elif debug_mode:
             logger.debug(
                 "Control check is none but passing because of debug mode")
             return None
         else:
             logger.debug("NOT Safe (Control check is None)")
```

### Comparing `naruno-0.60.3/naruno/lib/settings_system.py` & `naruno-0.60.4/naruno/lib/settings_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,26 +35,22 @@
 def save_settings(new_settings):
     """
     Saves the settings.
     """
     settings_db.set("settings", new_settings)
 
 
-def create_and_save_the_settings(test_mode_settings=False,
-                                 debug_mode_settings=True):
+def create_and_save_the_settings():
     """
     Creates and saves settings.
     """
     global temp_json
 
     save_settings(temp_json)
 
-    t_mode_settings(test_mode_settings)
-    d_mode_settings(debug_mode_settings)
-
     return temp_json
 
 
 def t_mode_settings(new_value):
     """
     Changes the test_mode setting.
```

### Comparing `naruno-0.60.3/naruno/lib/sign.py` & `naruno-0.60.4/naruno/lib/sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/status.py` & `naruno-0.60.4/naruno/lib/status.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/lib/verify.py` & `naruno-0.60.4/naruno/lib/verify.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/node/client/client.py` & `naruno-0.60.4/naruno/node/client/client.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/node/get_candidate_blocks.py` & `naruno-0.60.4/naruno/node/get_candidate_blocks.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/node/server/server.py` & `naruno-0.60.4/naruno/node/server/server.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/node/unl.py` & `naruno-0.60.4/naruno/node/unl.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/check/check_transaction.py` & `naruno-0.60.4/naruno/transactions/check/check_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/check/datas/check_datas.py` & `naruno-0.60.4/naruno/transactions/check/datas/check_datas.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/check/len/check_len.py` & `naruno-0.60.4/naruno/transactions/check/len/check_len.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/check/sign/check_sign.py` & `naruno-0.60.4/naruno/transactions/check/sign/check_sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/check/type/check_type.py` & `naruno-0.60.4/naruno/transactions/check/type/check_type.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/cleaner.py` & `naruno-0.60.4/naruno/transactions/cleaner.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/get_transaction.py` & `naruno-0.60.4/naruno/transactions/get_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/my_transactions/check_proof.py` & `naruno-0.60.4/naruno/transactions/my_transactions/check_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/my_transactions/get_my_transaction.py` & `naruno-0.60.4/naruno/transactions/my_transactions/get_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/my_transactions/get_proof.py` & `naruno-0.60.4/naruno/transactions/my_transactions/get_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/my_transactions/save_my_transaction.py` & `naruno-0.60.4/naruno/transactions/my_transactions/save_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/my_transactions/save_to_my_transaction.py` & `naruno-0.60.4/naruno/transactions/my_transactions/save_to_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/my_transactions/sended_transaction.py` & `naruno-0.60.4/naruno/transactions/my_transactions/sended_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/my_transactions/validate_transaction.py` & `naruno-0.60.4/naruno/transactions/my_transactions/validate_transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,14 @@
     for i in custom_currently_list:
         first_signature = None
         if isinstance(i,str):
             first_signature = i
         else:
             first_signature = i[0].signature
 
-        
-        logger.debug(f"First one: {i}")
-        logger.debug(f"Second one: {tx}")
         if first_signature == tx.signature:
            
             if not i[1] or force_notify:
                 notification("Validated TX",
                              f"{tx.data}:{tx.amount} to {tx.toUser}")
             i[1] = True
             save_list.append(i)
```

### Comparing `naruno-0.60.3/naruno/transactions/pending/delete_pending.py` & `naruno-0.60.4/naruno/transactions/pending/delete_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/pending/get_pending.py` & `naruno-0.60.4/naruno/transactions/pending/get_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/pending/save_pending.py` & `naruno-0.60.4/naruno/transactions/pending/save_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/pending_to_validating.py` & `naruno-0.60.4/naruno/transactions/pending_to_validating.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,26 +45,26 @@
 
     logger.debug(f"Pending list is sent to server")
     if len(block.validating_list) < block.max_tx_number:
         logger.debug("List is not full")
         for tx in OrderbyFee(the_list_of_tx):
             logger.debug(f"TX {tx.signature} is checking")
             if len(block.validating_list) < block.max_tx_number:
-                logger.info(f"tx {tx.signature} is moved to validating list")
+                logger.debug(f"tx {tx.signature} is moved to validating list")
 
                 block.validating_list.append(tx)
                 the_list_of_tx.remove(tx)
                 if not tx in first_situation:
                     DeletePending(tx)
 
             else:
-                logger.info(
+                logger.debug(
                     f"TX {tx.signature} is can not moved to validating list")
     else:
-        logger.info("List is full")
+        logger.debug("List is full")
     
     for i in the_list_of_tx:
         if i in first_situation:
             SavePending(i)
```

### Comparing `naruno-0.60.3/naruno/transactions/print_transactions.py` & `naruno-0.60.4/naruno/transactions/print_transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/process_the_transaction.py` & `naruno-0.60.4/naruno/transactions/process_the_transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                                    key=lambda x: x.fromUser)
 
     temp_validating_list = block.validating_list
 
     actions = []
 
     for trans in block.validating_list:
-        logger.info(f"Transaction: {trans.__dict__}")
+        logger.debug(f"Transaction: {trans.__dict__}")
 
         touser_inlist = True
         to_user_in_new_list = False
 
         address_of_fromUser = Address(trans.fromUser)
         logger.debug(f"FromUser address: {address_of_fromUser}")
         the_record_account_list = []
@@ -117,30 +117,30 @@
                 i.balance += float(trans.amount)
                 to_user_in_new_list = True
 
         # If not included in the account_list, add.
         if not touser_inlist and not to_user_in_new_list:
             new_added_accounts_list.append(
                 Account(trans.toUser, float(trans.amount)))
-    logger.info(f"Actions: {actions}")
+    logger.debug(f"Actions: {actions}")
     for action in actions:
         for account in account_list:
             if action[0] == account.Address:
                 alread_in = True if account in edited_accounts else False
                 the_account = edited_accounts[edited_accounts.index(account)] if account in edited_accounts else account                
                 if the_account.Address == block.fee_address:
-                    logger.info(f"Fee Address Input: {the_account.dump_json()}")
+                    logger.debug(f"Fee Address Input: {the_account.dump_json()}")
                 if action[1] == "balance":
                     balance_decimal = Decimal(str(the_account.balance)) + Decimal(str(action[2]))
                     the_account.balance = float(balance_decimal)
                 elif action[1] == "sequence_number":
                     the_account.sequence_number += action[2]
 
                 if the_account.Address == block.fee_address:
-                    logger.info(f"Fee Address Output: {the_account.dump_json()}")
+                    logger.debug(f"Fee Address Output: {the_account.dump_json()}")
                 if not alread_in:
                     edited_accounts.append(the_account)
 
     # Syncs new sorted list to block.validating_list
 
     block.validating_list = sorted(temp_validating_list,
                                    key=lambda x: x.signature)
```

### Comparing `naruno-0.60.3/naruno/transactions/send.py` & `naruno-0.60.4/naruno/transactions/send.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/transactions/transaction.py` & `naruno-0.60.4/naruno/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/delete_current_wallet.py` & `naruno-0.60.4/naruno/wallet/delete_current_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/curve.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/curve.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/ecdsa.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/ecdsa.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/math.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/math.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/privateKey.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/privateKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/publicKey.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/publicKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/signature.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/signature.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/utils/binary.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/utils/binary.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/utils/compatibility.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/utils/der.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/utils/der.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/ellipticcurve/utils/oid.py` & `naruno-0.60.4/naruno/wallet/ellipticcurve/utils/oid.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/get_saved_wallet.py` & `naruno-0.60.4/naruno/wallet/get_saved_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/print_wallets.py` & `naruno-0.60.4/naruno/wallet/print_wallets.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/save_wallet_list.py` & `naruno-0.60.4/naruno/wallet/save_wallet_list.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/wallet_create.py` & `naruno-0.60.4/naruno/wallet/wallet_create.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/wallet_delete.py` & `naruno-0.60.4/naruno/wallet/wallet_delete.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/wallet_import.py` & `naruno-0.60.4/naruno/wallet/wallet_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno/wallet/wallet_selector.py` & `naruno-0.60.4/naruno/wallet/wallet_selector.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/naruno.egg-info/PKG-INFO` & `naruno-0.60.4/naruno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.60.3
+Version: 0.60.4
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.60.3 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.60.4 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.60.3/naruno.egg-info/SOURCES.txt` & `naruno-0.60.4/naruno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naruno-0.60.3/setup.py` & `naruno-0.60.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 setup(
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     packages=["naruno"],
     name="naruno",
-    version="0.60.3",
+    version="0.60.4",
     url="https://github.com/Naruno/Naruno",
     description=
     "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.",
     keywords=[
         "python",
         "cryptography",
         "blockchain",
```

