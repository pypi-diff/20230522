# Comparing `tmp/nibiru_proto-0.20.0b5.tar.gz` & `tmp/nibiru_proto-0.20.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nibiru_proto-0.20.0b5.tar", max compression
+gzip compressed data, was "nibiru_proto-0.20.0rc1.tar", max compression
```

## Comparing `nibiru_proto-0.20.0b5.tar` & `nibiru_proto-0.20.0rc1.tar`

### file list

```diff
@@ -1,494 +1,490 @@
--rw-r--r--   0        0        0     1069 2023-05-21 22:44:58.061484 nibiru_proto-0.20.0b5/LICENSE
--rw-r--r--   0        0        0        1 2023-05-21 22:44:58.061484 nibiru_proto-0.20.0b5/nibiru_proto/__init__.py
--rw-r--r--   0        0        0       84 2023-05-21 22:44:58.061484 nibiru_proto-0.20.0b5/nibiru_proto/proto/__init__.py
--rw-r--r--   0        0        0     5420 2023-05-21 22:44:58.061484 nibiru_proto-0.20.0b5/nibiru_proto/proto/confio/proofs_pb2.py
--rw-r--r--   0        0        0    22610 2023-05-21 22:44:58.061484 nibiru_proto-0.20.0b5/nibiru_proto/proto/confio/proofs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/confio/proofs_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/confio/proofs_pb2_grpc.pyi
--rw-r--r--   0        0        0     4844 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2.py
--rw-r--r--   0        0        0     4086 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0     1747 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1555 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     5852 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6495 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     7921 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2640 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3105 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     3451 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2_grpc.pyi
--rw-r--r--   0        0        0     1427 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     2114 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2_grpc.pyi
--rw-r--r--   0        0        0     1595 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1194 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     4380 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     7628 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6335 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2372 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3423 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     4774 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6246 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2801 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1955 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     1223 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2_grpc.pyi
--rw-r--r--   0        0        0     4846 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2.py
--rw-r--r--   0        0        0     7345 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2_grpc.pyi
--rw-r--r--   0        0        0     3219 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     3446 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    10733 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    15102 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    15085 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     5016 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3554 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3040 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4237 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1505 2023-05-21 22:44:58.065484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     7219 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.py
--rw-r--r--   0        0        0    12319 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.pyi
--rw-r--r--   0        0        0     1544 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.py
--rw-r--r--   0        0        0     1558 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.pyi
--rw-r--r--   0        0        0     1851 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1213 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2762 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1022 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     1514 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.py
--rw-r--r--   0        0        0     3388 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.pyi
--rw-r--r--   0        0        0     3010 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
--rw-r--r--   0        0        0     3055 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
--rw-r--r--   0        0        0     5144 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     1988 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.pyi
--rw-r--r--   0        0        0    10387 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
--rw-r--r--   0        0        0    23085 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
--rw-r--r--   0        0        0    13573 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     5145 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.pyi
--rw-r--r--   0        0        0     3229 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
--rw-r--r--   0        0        0     6441 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.pyi
--rw-r--r--   0        0        0     2141 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.py
--rw-r--r--   0        0        0     2713 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.pyi
--rw-r--r--   0        0        0     2320 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2.py
--rw-r--r--   0        0        0     5092 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.pyi
--rw-r--r--   0        0        0     8334 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    13862 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    12460 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4039 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2694 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2.py
--rw-r--r--   0        0        0     2703 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2_grpc.pyi
--rw-r--r--   0        0        0     2548 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2.py
--rw-r--r--   0        0        0     2304 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0     2152 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     1671 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1192 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     2353 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1574 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2685 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1004 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1842 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2.py
--rw-r--r--   0        0        0     1690 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0     2055 2023-05-21 22:44:58.069484 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2.py
--rw-r--r--   0        0        0     1351 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0     1730 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
--rw-r--r--   0        0        0     2062 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.pyi
--rw-r--r--   0        0        0     1475 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2.py
--rw-r--r--   0        0        0     1519 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0     1813 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2.py
--rw-r--r--   0        0        0     1523 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0    12364 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.py
--rw-r--r--   0        0        0    12622 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.pyi
--rw-r--r--   0        0        0    13234 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0    13972 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    13651 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    16160 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    18352 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     6277 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     5830 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     5086 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     8774 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3369 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     2200 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.py
--rw-r--r--   0        0        0     1509 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.pyi
--rw-r--r--   0        0        0     1317 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1155 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3519 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     4011 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4459 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1516 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2295 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1890 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2754 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1122 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     5368 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
--rw-r--r--   0        0        0     6920 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.pyi
--rw-r--r--   0        0        0     1616 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1188 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     4316 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6811 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6408 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2265 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2563 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3204 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4601 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1823 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1579 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1086 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3478 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     3284 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    15234 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0    15147 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2_grpc.pyi
--rw-r--r--   0        0        0    10678 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    15840 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14598 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4657 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     6446 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     6020 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     7675 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2610 2023-05-21 22:44:58.073485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1805 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1405 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3917 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2.py
--rw-r--r--   0        0        0     2590 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2_grpc.pyi
--rw-r--r--   0        0        0     4275 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3563 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6210 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2105 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2129 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2.py
--rw-r--r--   0        0        0     2127 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2_grpc.pyi
--rw-r--r--   0        0        0     2371 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1922 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2674 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1051 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3519 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4858 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     4610 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     5194 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6284 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2133 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     5094 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.py
--rw-r--r--   0        0        0     4327 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.pyi
--rw-r--r--   0        0        0     1962 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1152 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2717 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1204 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     2766 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     5176 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2_grpc.pyi
--rw-r--r--   0        0        0     3931 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4598 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    19200 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    29051 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    26968 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     9115 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0    24776 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2.py
--rw-r--r--   0        0        0    27750 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2_grpc.pyi
--rw-r--r--   0        0        0    11071 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0    10196 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     9842 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3547 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     3092 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.py
--rw-r--r--   0        0        0     9075 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.pyi
--rw-r--r--   0        0        0     6963 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2.py
--rw-r--r--   0        0        0    14464 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2.pyi
--rw-r--r--   0        0        0     9577 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.py
--rw-r--r--   0        0        0     3087 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4482 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0    16485 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     4980 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6147 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     8732 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3705 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3641 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
--rw-r--r--   0        0        0     5332 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.pyi
--rw-r--r--   0        0        0     3117 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2095 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2780 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1087 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     7460 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.py
--rw-r--r--   0        0        0     7575 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.pyi
--rw-r--r--   0        0        0     1671 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos_proto/cosmos_pb2.py
--rw-r--r--   0        0        0      838 2023-05-21 22:44:58.077485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos_proto/cosmos_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos_proto/cosmos_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos_proto/cosmos_pb2_grpc.pyi
--rw-r--r--   0        0        0     1805 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/event_pb2.py
--rw-r--r--   0        0        0     1813 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/event_pb2_grpc.pyi
--rw-r--r--   0        0        0     1769 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1087 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3168 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/query_pb2.py
--rw-r--r--   0        0        0     2298 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/query_pb2.pyi
--rw-r--r--   0        0        0     4253 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1434 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2763 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/state_pb2.py
--rw-r--r--   0        0        0     2806 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/state_pb2_grpc.pyi
--rw-r--r--   0        0        0    14512 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/gogoproto/gogo_pb2.py
--rw-r--r--   0        0        0    15688 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/gogoproto/gogo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/gogoproto/gogo_pb2_grpc.py
--rw-r--r--   0        0        0     1446 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/gogoproto/gogo_pb2_grpc.pyi
--rw-r--r--   0        0        0     1580 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1053 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      633 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2125 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/http_pb2.py
--rw-r--r--   0        0        0    15201 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     1507 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/httpbody_pb2.py
--rw-r--r--   0        0        0     3509 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/httpbody_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/httpbody_pb2_grpc.py
--rw-r--r--   0        0        0      628 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/httpbody_pb2_grpc.pyi
--rw-r--r--   0        0        0     1588 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/protobuf/any_pb2.py
--rw-r--r--   0        0        0     6380 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/protobuf/any_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/protobuf/any_pb2_grpc.py
--rw-r--r--   0        0        0     1651 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/google/protobuf/any_pb2_grpc.pyi
--rw-r--r--   0        0        0     2386 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/genesis_pb2.py
--rw-r--r--   0        0        0     3451 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3313 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/inflation_pb2.py
--rw-r--r--   0        0        0     2746 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/inflation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/inflation_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/inflation_pb2_grpc.pyi
--rw-r--r--   0        0        0     6990 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/query_pb2.py
--rw-r--r--   0        0        0     7288 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/query_pb2.pyi
--rw-r--r--   0        0        0    11268 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3785 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     1683 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/event_pb2.py
--rw-r--r--   0        0        0     1072 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/event_pb2_grpc.pyi
--rw-r--r--   0        0        0     4116 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/genesis_pb2.py
--rw-r--r--   0        0        0     5114 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     8728 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/oracle_pb2.py
--rw-r--r--   0        0        0     8160 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/oracle_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/oracle_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/oracle_pb2_grpc.pyi
--rw-r--r--   0        0        0    13728 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/query_pb2.py
--rw-r--r--   0        0        0    15145 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/query_pb2.pyi
--rw-r--r--   0        0        0    21135 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     6550 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2230 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/state_pb2.py
--rw-r--r--   0        0        0     1119 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/state_pb2_grpc.pyi
--rw-r--r--   0        0        0     6341 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/tx_pb2.py
--rw-r--r--   0        0        0     4671 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     6438 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2532 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0    13724 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/event_pb2.py
--rw-r--r--   0        0        0    15963 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/event_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.081485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/event_pb2_grpc.pyi
--rw-r--r--   0        0        0     2468 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/genesis_pb2.py
--rw-r--r--   0        0        0     1985 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     7495 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/query_pb2.py
--rw-r--r--   0        0        0     7235 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/query_pb2.pyi
--rw-r--r--   0        0        0     7536 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/query_pb2_grpc.py
--rw-r--r--   0        0        0     2082 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     9812 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/state_pb2.py
--rw-r--r--   0        0        0    11455 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/state_pb2_grpc.pyi
--rw-r--r--   0        0        0    15485 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/tx_pb2.py
--rw-r--r--   0        0        0    15137 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/tx_pb2.pyi
--rw-r--r--   0        0        0    10618 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2533 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     4476 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/event_pb2.py
--rw-r--r--   0        0        0     5718 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/event_pb2_grpc.pyi
--rw-r--r--   0        0        0     1486 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1020 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     2031 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/params_pb2.py
--rw-r--r--   0        0        0     1850 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/params_pb2_grpc.pyi
--rw-r--r--   0        0        0     5309 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/pool_pb2.py
--rw-r--r--   0        0        0     5345 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/pool_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/pool_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/pool_pb2_grpc.pyi
--rw-r--r--   0        0        0    19291 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/query_pb2.py
--rw-r--r--   0        0        0    20949 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/query_pb2.pyi
--rw-r--r--   0        0        0    27996 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     8706 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     8496 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/tx_pb2.py
--rw-r--r--   0        0        0     7824 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     7046 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2039 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     5160 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/events_pb2.py
--rw-r--r--   0        0        0     5131 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/events_pb2_grpc.pyi
--rw-r--r--   0        0        0     2055 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1413 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     1874 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/params_pb2.py
--rw-r--r--   0        0        0     3069 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/params_pb2_grpc.pyi
--rw-r--r--   0        0        0     7872 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/query_pb2.py
--rw-r--r--   0        0        0     7570 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/query_pb2.pyi
--rw-r--r--   0        0        0     7946 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2416 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     7098 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/tx_pb2.py
--rw-r--r--   0        0        0     8375 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     8010 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3497 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1664 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/event_pb2.py
--rw-r--r--   0        0        0     1169 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/event_pb2_grpc.pyi
--rw-r--r--   0        0        0     2169 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/query_pb2.py
--rw-r--r--   0        0        0     1315 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2524 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0      797 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     1756 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/state_pb2.py
--rw-r--r--   0        0        0     1817 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/state_pb2_grpc.pyi
--rw-r--r--   0        0        0     1921 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/tx_pb2.py
--rw-r--r--   0        0        0     1977 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     2966 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1212 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0    21318 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/abci/types_pb2.py
--rw-r--r--   0        0        0    49906 2023-05-21 22:44:58.085485 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/abci/types_pb2.pyi
--rw-r--r--   0        0        0    25991 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/abci/types_pb2_grpc.py
--rw-r--r--   0        0        0     6123 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/abci/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     1471 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/keys_pb2.py
--rw-r--r--   0        0        0     1291 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/keys_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0     2208 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/proof_pb2.py
--rw-r--r--   0        0        0     4101 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/proof_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/proof_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/proof_pb2_grpc.pyi
--rw-r--r--   0        0        0     1222 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/libs/bits/types_pb2.py
--rw-r--r--   0        0        0     1049 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/libs/bits/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/libs/bits/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/libs/bits/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     3488 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/p2p/types_pb2.py
--rw-r--r--   0        0        0     3901 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/p2p/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/p2p/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/p2p/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2173 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/block_pb2.py
--rw-r--r--   0        0        0     1707 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/block_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/block_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/block_pb2_grpc.pyi
--rw-r--r--   0        0        0     3521 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/evidence_pb2.py
--rw-r--r--   0        0        0     5767 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/evidence_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/evidence_pb2_grpc.pyi
--rw-r--r--   0        0        0     3858 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/params_pb2.py
--rw-r--r--   0        0        0     6657 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/params_pb2_grpc.pyi
--rw-r--r--   0        0        0    10988 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/types_pb2.py
--rw-r--r--   0        0        0    18419 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2231 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/validator_pb2.py
--rw-r--r--   0        0        0     3356 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/validator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/validator_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/validator_pb2_grpc.pyi
--rw-r--r--   0        0        0     1550 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/version/types_pb2.py
--rw-r--r--   0        0        0     1793 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/version/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/version/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/version/types_pb2_grpc.pyi
--rw-r--r--   0        0        0      733 2023-05-21 22:44:58.089486 nibiru_proto-0.20.0b5/pyproject.toml
--rw-r--r--   0        0        0     3033 1970-01-01 00:00:00.000000 nibiru_proto-0.20.0b5/setup.py
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 nibiru_proto-0.20.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/LICENSE
+-rw-r--r--   0        0        0        1 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/__init__.py
+-rw-r--r--   0        0        0       84 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/__init__.py
+-rw-r--r--   0        0        0     5420 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/confio/proofs_pb2.py
+-rw-r--r--   0        0        0    22610 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/confio/proofs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/confio/proofs_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/confio/proofs_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4844 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2.py
+-rw-r--r--   0        0        0     4086 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1747 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1555 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5852 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6495 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     7921 2023-03-30 19:51:13.964504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2640 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3105 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     3451 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1427 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     2114 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1595 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1194 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4380 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     7628 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6335 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2372 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3423 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     4774 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6246 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2801 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1955 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     1223 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4846 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2.py
+-rw-r--r--   0        0        0     7345 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3219 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     3446 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10733 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    15102 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    15085 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     5016 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3554 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3040 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4237 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1505 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7219 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.py
+-rw-r--r--   0        0        0    12319 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1544 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.py
+-rw-r--r--   0        0        0     1558 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1851 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1213 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2762 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1022 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1514 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.py
+-rw-r--r--   0        0        0     3388 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3010 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
+-rw-r--r--   0        0        0     3055 2023-03-30 19:51:13.968504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     5144 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     1988 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10387 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
+-rw-r--r--   0        0        0    23085 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
+-rw-r--r--   0        0        0    13573 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     5145 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3229 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
+-rw-r--r--   0        0        0     6441 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2141 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.py
+-rw-r--r--   0        0        0     2713 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2320 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2.py
+-rw-r--r--   0        0        0     5092 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8334 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    13862 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    12460 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4039 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2694 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2.py
+-rw-r--r--   0        0        0     2703 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2548 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2.py
+-rw-r--r--   0        0        0     2304 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2152 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2428 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1671 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1192 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2353 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1574 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2685 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1004 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1842 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2.py
+-rw-r--r--   0        0        0     1690 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2055 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2.py
+-rw-r--r--   0        0        0     1351 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1730 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
+-rw-r--r--   0        0        0     2062 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1475 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2.py
+-rw-r--r--   0        0        0     1519 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1813 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2.py
+-rw-r--r--   0        0        0     1523 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12364 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.py
+-rw-r--r--   0        0        0    12622 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13234 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0    13972 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13651 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    16160 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    18352 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     6277 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5830 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     5086 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     8774 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3369 2023-03-30 19:51:13.972504 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2200 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.py
+-rw-r--r--   0        0        0     1509 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1317 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1155 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3519 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     4011 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4459 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1516 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2295 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1890 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2754 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1122 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5368 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
+-rw-r--r--   0        0        0     6920 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1616 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1188 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4316 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6811 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6408 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2265 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2563 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3204 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4601 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1823 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1579 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1086 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3478 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     3284 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15234 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0    15147 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10678 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    15840 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14598 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4657 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6446 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6020 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     7675 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2610 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1805 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1405 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3917 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2.py
+-rw-r--r--   0        0        0     2590 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4275 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3563 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6210 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2105 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2129 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2.py
+-rw-r--r--   0        0        0     2127 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2371 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1922 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2674 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1051 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3519 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4858 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4610 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     5194 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6284 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2133 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5094 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.py
+-rw-r--r--   0        0        0     4327 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1962 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1152 2023-03-30 19:51:13.976505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2717 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1204 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2766 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     5176 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3931 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4598 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    19200 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    29051 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    26968 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     9115 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24776 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2.py
+-rw-r--r--   0        0        0    27750 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11071 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    10196 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     9842 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3547 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3092 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.py
+-rw-r--r--   0        0        0     9075 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6963 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2.py
+-rw-r--r--   0        0        0    14464 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2.pyi
+-rw-r--r--   0        0        0     9577 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.py
+-rw-r--r--   0        0        0     3087 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4482 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    16485 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4980 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6147 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     8732 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3705 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3641 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
+-rw-r--r--   0        0        0     5332 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3117 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2095 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2780 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1087 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7460 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.py
+-rw-r--r--   0        0        0     7575 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1671 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos_proto/cosmos_pb2.py
+-rw-r--r--   0        0        0      838 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos_proto/cosmos_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos_proto/cosmos_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos_proto/cosmos_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1796 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/event_pb2.py
+-rw-r--r--   0        0        0     1813 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/event_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/event_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1747 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/genesis_pb2.py
+-rw-r--r--   0        0        0     1078 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3146 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/query_pb2.py
+-rw-r--r--   0        0        0     2289 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/query_pb2.pyi
+-rw-r--r--   0        0        0     4159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1407 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2754 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/state_pb2.py
+-rw-r--r--   0        0        0     2797 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/state_pb2_grpc.pyi
+-rw-r--r--   0        0        0    14512 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/gogoproto/gogo_pb2.py
+-rw-r--r--   0        0        0    15688 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/gogoproto/gogo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/gogoproto/gogo_pb2_grpc.py
+-rw-r--r--   0        0        0     1446 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/gogoproto/gogo_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1580 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1053 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      633 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2125 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/http_pb2.py
+-rw-r--r--   0        0        0    15201 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1507 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/httpbody_pb2.py
+-rw-r--r--   0        0        0     3509 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/httpbody_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.980505 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/httpbody_pb2_grpc.py
+-rw-r--r--   0        0        0      628 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/httpbody_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1588 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/protobuf/any_pb2.py
+-rw-r--r--   0        0        0     6380 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/protobuf/any_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/protobuf/any_pb2_grpc.py
+-rw-r--r--   0        0        0     1651 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/protobuf/any_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1704 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     1072 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/event_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4206 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     5200 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8680 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/oracle_pb2.py
+-rw-r--r--   0        0        0     8106 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/oracle_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/oracle_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/oracle_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13976 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    15044 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    21630 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     6795 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2265 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/state_pb2.py
+-rw-r--r--   0        0        0     1119 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6389 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     4651 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6575 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2601 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15339 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/event_pb2.py
+-rw-r--r--   0        0        0    17609 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/event_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2491 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     2051 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8465 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/query_pb2.py
+-rw-r--r--   0        0        0     8365 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     9262 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2665 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12609 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/state_pb2.py
+-rw-r--r--   0        0        0    15662 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/state_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15450 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/tx_pb2.py
+-rw-r--r--   0        0        0    15073 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0    10618 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2533 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4476 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/event_pb2.py
+-rw-r--r--   0        0        0     5718 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/event_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1486 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1020 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2031 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/params_pb2.py
+-rw-r--r--   0        0        0     1850 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5309 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/pool_pb2.py
+-rw-r--r--   0        0        0     5335 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/pool_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/pool_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/pool_pb2_grpc.pyi
+-rw-r--r--   0        0        0    19291 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/query_pb2.py
+-rw-r--r--   0        0        0    20949 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    27996 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     8706 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8496 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/tx_pb2.py
+-rw-r--r--   0        0        0     7824 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     7046 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2039 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5151 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/events_pb2.py
+-rw-r--r--   0        0        0     5131 2023-03-30 19:51:13.984506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2033 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/genesis_pb2.py
+-rw-r--r--   0        0        0     1404 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1865 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/params_pb2.py
+-rw-r--r--   0        0        0     3069 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7844 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/query_pb2.py
+-rw-r--r--   0        0        0     7541 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/query_pb2.pyi
+-rw-r--r--   0        0        0     7768 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2365 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7089 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/tx_pb2.py
+-rw-r--r--   0        0        0     8375 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/tx_pb2.pyi
+-rw-r--r--   0        0        0     7832 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3446 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0    21318 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/abci/types_pb2.py
+-rw-r--r--   0        0        0    49906 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/abci/types_pb2.pyi
+-rw-r--r--   0        0        0    25991 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/abci/types_pb2_grpc.py
+-rw-r--r--   0        0        0     6123 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/abci/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1471 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/keys_pb2.py
+-rw-r--r--   0        0        0     1291 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2208 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/proof_pb2.py
+-rw-r--r--   0        0        0     4101 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/proof_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/proof_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/proof_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1222 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/libs/bits/types_pb2.py
+-rw-r--r--   0        0        0     1049 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/libs/bits/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/libs/bits/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/libs/bits/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3488 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/p2p/types_pb2.py
+-rw-r--r--   0        0        0     3901 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/p2p/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/p2p/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/p2p/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2173 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/block_pb2.py
+-rw-r--r--   0        0        0     1707 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/block_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/block_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/block_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3521 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/evidence_pb2.py
+-rw-r--r--   0        0        0     5767 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/evidence_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3858 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/params_pb2.py
+-rw-r--r--   0        0        0     6657 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10988 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/types_pb2.py
+-rw-r--r--   0        0        0    18419 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2231 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/validator_pb2.py
+-rw-r--r--   0        0        0     3356 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/validator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/validator_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/validator_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1550 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/version/types_pb2.py
+-rw-r--r--   0        0        0     1793 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/version/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/version/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/version/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2980 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/util/v1/query_pb2.py
+-rw-r--r--   0        0        0     2261 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/util/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2604 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/util/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0      993 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/util/v1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5453 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/event_pb2.py
+-rw-r--r--   0        0        0     3904 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/event_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1492 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1075 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5166 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/gov_pb2.py
+-rw-r--r--   0        0        0     5514 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/gov_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5952 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/query_pb2.py
+-rw-r--r--   0        0        0     4551 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     5860 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1866 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8241 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/state_pb2.py
+-rw-r--r--   0        0        0     9138 2023-03-30 19:51:13.988506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-30 19:51:13.992506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-03-30 19:51:13.992506 nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/state_pb2_grpc.pyi
+-rw-r--r--   0        0        0      735 2023-03-30 19:51:13.992506 nibiru_proto-0.20.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 nibiru_proto-0.20.0rc1/setup.py
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 nibiru_proto-0.20.0rc1/PKG-INFO
```

### Comparing `nibiru_proto-0.20.0b5/LICENSE` & `nibiru_proto-0.20.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/confio/proofs_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/confio/proofs_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/confio/proofs_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/confio/proofs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/bank_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/node/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/store/v1beta1/listening_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/base/v1beta1/coin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/capability/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/ed25519/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256k1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/crypto/secp256r1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/gov_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/mint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/staking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/tx/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos_proto/cosmos_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos_proto/cosmos_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/cosmos_proto/cosmos_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/cosmos_proto/cosmos_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/event_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/event_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: epochs/v1/event.proto
+# source: epochs/event.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x65pochs/v1/event.proto\x12\x10nibiru.epochs.v1\x1a\x14gogoproto/gogo.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"g\n\x0f\x45ventEpochStart\x12\x14\n\x0c\x65poch_number\x18\x01 \x01(\x04\x12>\n\x10\x65poch_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\x90\xdf\x1f\x01\xc8\xde\x1f\x00\"%\n\rEventEpochEnd\x12\x14\n\x0c\x65poch_number\x18\x01 \x01(\x04\x42.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x65pochs/event.proto\x12\x10nibiru.epochs.v1\x1a\x14gogoproto/gogo.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"g\n\x0f\x45ventEpochStart\x12\x14\n\x0c\x65poch_number\x18\x01 \x01(\x04\x12>\n\x10\x65poch_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\x90\xdf\x1f\x01\xc8\xde\x1f\x00\"%\n\rEventEpochEnd\x12\x14\n\x0c\x65poch_number\x18\x01 \x01(\x04\x42.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'epochs.v1.event_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'epochs.event_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/epochs/types'
   _EVENTEPOCHSTART.fields_by_name['epoch_start_time']._options = None
   _EVENTEPOCHSTART.fields_by_name['epoch_start_time']._serialized_options = b'\220\337\037\001\310\336\037\000'
-  _EVENTEPOCHSTART._serialized_start=98
-  _EVENTEPOCHSTART._serialized_end=201
-  _EVENTEPOCHEND._serialized_start=203
-  _EVENTEPOCHEND._serialized_end=240
+  _EVENTEPOCHSTART._serialized_start=95
+  _EVENTEPOCHSTART._serialized_end=198
+  _EVENTEPOCHEND._serialized_start=200
+  _EVENTEPOCHEND._serialized_end=237
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/event_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/genesis_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: epochs/v1/genesis.proto
+# source: epochs/genesis.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from epochs.v1 import state_pb2 as epochs_dot_v1_dot_state__pb2
+from epochs import state_pb2 as epochs_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x65pochs/v1/genesis.proto\x12\x15nibiru.epochs.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x15\x65pochs/v1/state.proto\"F\n\x0cGenesisState\x12\x36\n\x06\x65pochs\x18\x01 \x03(\x0b\x32 .nibiru.epochs.v1beta1.EpochInfoB\x04\xc8\xde\x1f\x00\x42.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x65pochs/genesis.proto\x12\x15nibiru.epochs.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x12\x65pochs/state.proto\"F\n\x0cGenesisState\x12\x36\n\x06\x65pochs\x18\x01 \x03(\x0b\x32 .nibiru.epochs.v1beta1.EpochInfoB\x04\xc8\xde\x1f\x00\x42.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'epochs.v1.genesis_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'epochs.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/epochs/types'
   _GENESISSTATE.fields_by_name['epochs']._options = None
   _GENESISSTATE.fields_by_name['epochs']._serialized_options = b'\310\336\037\000'
-  _GENESISSTATE._serialized_start=160
-  _GENESISSTATE._serialized_end=230
+  _GENESISSTATE._serialized_start=154
+  _GENESISSTATE._serialized_end=224
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/genesis_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import collections.abc
-import epochs.v1.state_pb2
+import epochs.state_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
@@ -21,16 +21,16 @@
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the epochs module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EPOCHS_FIELD_NUMBER: builtins.int
     @property
-    def epochs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[epochs.v1.state_pb2.EpochInfo]: ...
+    def epochs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[epochs.state_pb2.EpochInfo]: ...
     def __init__(
         self,
         *,
-        epochs: collections.abc.Iterable[epochs.v1.state_pb2.EpochInfo] | None = ...,
+        epochs: collections.abc.Iterable[epochs.state_pb2.EpochInfo] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["epochs", b"epochs"]) -> None: ...
 
 global___GenesisState = GenesisState
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/query_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: epochs/v1/query.proto
+# source: epochs/query.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.query.v1beta1 import pagination_pb2 as cosmos_dot_base_dot_query_dot_v1beta1_dot_pagination__pb2
-from epochs.v1 import state_pb2 as epochs_dot_v1_dot_state__pb2
+from epochs import state_pb2 as epochs_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x65pochs/v1/query.proto\x12\x15nibiru.epochs.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a*cosmos/base/query/v1beta1/pagination.proto\x1a\x15\x65pochs/v1/state.proto\"\x18\n\x16QueryEpochsInfoRequest\"Q\n\x17QueryEpochsInfoResponse\x12\x36\n\x06\x65pochs\x18\x01 \x03(\x0b\x32 .nibiru.epochs.v1beta1.EpochInfoB\x04\xc8\xde\x1f\x00\".\n\x18QueryCurrentEpochRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\"2\n\x19QueryCurrentEpochResponse\x12\x15\n\rcurrent_epoch\x18\x01 \x01(\x04\x32\xbe\x02\n\x05Query\x12\x92\x01\n\nEpochInfos\x12-.nibiru.epochs.v1beta1.QueryEpochsInfoRequest\x1a..nibiru.epochs.v1beta1.QueryEpochsInfoResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/nibiru/epochs/v1beta1/epochs\x12\x9f\x01\n\x0c\x43urrentEpoch\x12/.nibiru.epochs.v1beta1.QueryCurrentEpochRequest\x1a\x30.nibiru.epochs.v1beta1.QueryCurrentEpochResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/epochs/v1beta1/current_epochB.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x65pochs/query.proto\x12\x15nibiru.epochs.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a*cosmos/base/query/v1beta1/pagination.proto\x1a\x12\x65pochs/state.proto\"\x18\n\x16QueryEpochsInfoRequest\"Q\n\x17QueryEpochsInfoResponse\x12\x36\n\x06\x65pochs\x18\x01 \x03(\x0b\x32 .nibiru.epochs.v1beta1.EpochInfoB\x04\xc8\xde\x1f\x00\".\n\x18QueryCurrentEpochRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\"2\n\x19QueryCurrentEpochResponse\x12\x15\n\rcurrent_epoch\x18\x01 \x01(\x04\x32\xbe\x02\n\x05Query\x12\x92\x01\n\nEpochInfos\x12-.nibiru.epochs.v1beta1.QueryEpochsInfoRequest\x1a..nibiru.epochs.v1beta1.QueryEpochsInfoResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/nibiru/epochs/v1beta1/epochs\x12\x9f\x01\n\x0c\x43urrentEpoch\x12/.nibiru.epochs.v1beta1.QueryCurrentEpochRequest\x1a\x30.nibiru.epochs.v1beta1.QueryCurrentEpochResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/epochs/v1beta1/current_epochB.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'epochs.v1.query_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'epochs.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/epochs/types'
   _QUERYEPOCHSINFORESPONSE.fields_by_name['epochs']._options = None
   _QUERYEPOCHSINFORESPONSE.fields_by_name['epochs']._serialized_options = b'\310\336\037\000'
   _QUERY.methods_by_name['EpochInfos']._options = None
   _QUERY.methods_by_name['EpochInfos']._serialized_options = b'\202\323\344\223\002\037\022\035/nibiru/epochs/v1beta1/epochs'
   _QUERY.methods_by_name['CurrentEpoch']._options = None
   _QUERY.methods_by_name['CurrentEpoch']._serialized_options = b'\202\323\344\223\002&\022$/nibiru/epochs/v1beta1/current_epoch'
-  _QUERYEPOCHSINFOREQUEST._serialized_start=167
-  _QUERYEPOCHSINFOREQUEST._serialized_end=191
-  _QUERYEPOCHSINFORESPONSE._serialized_start=193
-  _QUERYEPOCHSINFORESPONSE._serialized_end=274
-  _QUERYCURRENTEPOCHREQUEST._serialized_start=276
-  _QUERYCURRENTEPOCHREQUEST._serialized_end=322
-  _QUERYCURRENTEPOCHRESPONSE._serialized_start=324
-  _QUERYCURRENTEPOCHRESPONSE._serialized_end=374
-  _QUERY._serialized_start=377
-  _QUERY._serialized_end=695
+  _QUERYEPOCHSINFOREQUEST._serialized_start=161
+  _QUERYEPOCHSINFOREQUEST._serialized_end=185
+  _QUERYEPOCHSINFORESPONSE._serialized_start=187
+  _QUERYEPOCHSINFORESPONSE._serialized_end=268
+  _QUERYCURRENTEPOCHREQUEST._serialized_start=270
+  _QUERYCURRENTEPOCHREQUEST._serialized_end=316
+  _QUERYCURRENTEPOCHRESPONSE._serialized_start=318
+  _QUERYCURRENTEPOCHRESPONSE._serialized_end=368
+  _QUERY._serialized_start=371
+  _QUERY._serialized_end=689
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/query_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import collections.abc
-import epochs.v1.state_pb2
+import epochs.state_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
@@ -29,19 +29,19 @@
 
 @typing_extensions.final
 class QueryEpochsInfoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EPOCHS_FIELD_NUMBER: builtins.int
     @property
-    def epochs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[epochs.v1.state_pb2.EpochInfo]: ...
+    def epochs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[epochs.state_pb2.EpochInfo]: ...
     def __init__(
         self,
         *,
-        epochs: collections.abc.Iterable[epochs.v1.state_pb2.EpochInfo] | None = ...,
+        epochs: collections.abc.Iterable[epochs.state_pb2.EpochInfo] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["epochs", b"epochs"]) -> None: ...
 
 global___QueryEpochsInfoResponse = QueryEpochsInfoResponse
 
 @typing_extensions.final
 class QueryCurrentEpochRequest(google.protobuf.message.Message):
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/query_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from epochs.v1 import query_pb2 as epochs_dot_v1_dot_query__pb2
+from epochs import query_pb2 as epochs_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.EpochInfos = channel.unary_unary(
                 '/nibiru.epochs.v1beta1.Query/EpochInfos',
-                request_serializer=epochs_dot_v1_dot_query__pb2.QueryEpochsInfoRequest.SerializeToString,
-                response_deserializer=epochs_dot_v1_dot_query__pb2.QueryEpochsInfoResponse.FromString,
+                request_serializer=epochs_dot_query__pb2.QueryEpochsInfoRequest.SerializeToString,
+                response_deserializer=epochs_dot_query__pb2.QueryEpochsInfoResponse.FromString,
                 )
         self.CurrentEpoch = channel.unary_unary(
                 '/nibiru.epochs.v1beta1.Query/CurrentEpoch',
-                request_serializer=epochs_dot_v1_dot_query__pb2.QueryCurrentEpochRequest.SerializeToString,
-                response_deserializer=epochs_dot_v1_dot_query__pb2.QueryCurrentEpochResponse.FromString,
+                request_serializer=epochs_dot_query__pb2.QueryCurrentEpochRequest.SerializeToString,
+                response_deserializer=epochs_dot_query__pb2.QueryCurrentEpochResponse.FromString,
                 )
 
 
 class QueryServicer(object):
     """Query defines the gRPC querier service.
     """
 
@@ -46,21 +46,21 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_QueryServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'EpochInfos': grpc.unary_unary_rpc_method_handler(
                     servicer.EpochInfos,
-                    request_deserializer=epochs_dot_v1_dot_query__pb2.QueryEpochsInfoRequest.FromString,
-                    response_serializer=epochs_dot_v1_dot_query__pb2.QueryEpochsInfoResponse.SerializeToString,
+                    request_deserializer=epochs_dot_query__pb2.QueryEpochsInfoRequest.FromString,
+                    response_serializer=epochs_dot_query__pb2.QueryEpochsInfoResponse.SerializeToString,
             ),
             'CurrentEpoch': grpc.unary_unary_rpc_method_handler(
                     servicer.CurrentEpoch,
-                    request_deserializer=epochs_dot_v1_dot_query__pb2.QueryCurrentEpochRequest.FromString,
-                    response_serializer=epochs_dot_v1_dot_query__pb2.QueryCurrentEpochResponse.SerializeToString,
+                    request_deserializer=epochs_dot_query__pb2.QueryCurrentEpochRequest.FromString,
+                    response_serializer=epochs_dot_query__pb2.QueryCurrentEpochResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'nibiru.epochs.v1beta1.Query', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -77,16 +77,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.epochs.v1beta1.Query/EpochInfos',
-            epochs_dot_v1_dot_query__pb2.QueryEpochsInfoRequest.SerializeToString,
-            epochs_dot_v1_dot_query__pb2.QueryEpochsInfoResponse.FromString,
+            epochs_dot_query__pb2.QueryEpochsInfoRequest.SerializeToString,
+            epochs_dot_query__pb2.QueryEpochsInfoResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def CurrentEpoch(request,
             target,
             options=(),
@@ -94,11 +94,11 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.epochs.v1beta1.Query/CurrentEpoch',
-            epochs_dot_v1_dot_query__pb2.QueryCurrentEpochRequest.SerializeToString,
-            epochs_dot_v1_dot_query__pb2.QueryCurrentEpochResponse.FromString,
+            epochs_dot_query__pb2.QueryCurrentEpochRequest.SerializeToString,
+            epochs_dot_query__pb2.QueryCurrentEpochResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/query_pb2_grpc.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
-import epochs.v1.query_pb2
+import epochs.query_pb2
 import grpc
 
 class QueryStub:
     """Query defines the gRPC querier service."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
     EpochInfos: grpc.UnaryUnaryMultiCallable[
-        epochs.v1.query_pb2.QueryEpochsInfoRequest,
-        epochs.v1.query_pb2.QueryEpochsInfoResponse,
+        epochs.query_pb2.QueryEpochsInfoRequest,
+        epochs.query_pb2.QueryEpochsInfoResponse,
     ]
     """EpochInfos provide running epochInfos"""
     CurrentEpoch: grpc.UnaryUnaryMultiCallable[
-        epochs.v1.query_pb2.QueryCurrentEpochRequest,
-        epochs.v1.query_pb2.QueryCurrentEpochResponse,
+        epochs.query_pb2.QueryCurrentEpochRequest,
+        epochs.query_pb2.QueryCurrentEpochResponse,
     ]
     """CurrentEpoch provide current epoch of specified identifier"""
 
 class QueryServicer(metaclass=abc.ABCMeta):
     """Query defines the gRPC querier service."""
 
     @abc.abstractmethod
     def EpochInfos(
         self,
-        request: epochs.v1.query_pb2.QueryEpochsInfoRequest,
+        request: epochs.query_pb2.QueryEpochsInfoRequest,
         context: grpc.ServicerContext,
-    ) -> epochs.v1.query_pb2.QueryEpochsInfoResponse:
+    ) -> epochs.query_pb2.QueryEpochsInfoResponse:
         """EpochInfos provide running epochInfos"""
     @abc.abstractmethod
     def CurrentEpoch(
         self,
-        request: epochs.v1.query_pb2.QueryCurrentEpochRequest,
+        request: epochs.query_pb2.QueryCurrentEpochRequest,
         context: grpc.ServicerContext,
-    ) -> epochs.v1.query_pb2.QueryCurrentEpochResponse:
+    ) -> epochs.query_pb2.QueryCurrentEpochResponse:
         """CurrentEpoch provide current epoch of specified identifier"""
 
 def add_QueryServicer_to_server(servicer: QueryServicer, server: grpc.Server) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/state_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/state_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: epochs/v1/state.proto
+# source: epochs/state.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
@@ -12,24 +12,24 @@
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x65pochs/v1/state.proto\x12\x15nibiru.epochs.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x94\x03\n\tEpochInfo\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12M\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x1d\x90\xdf\x1f\x01\xc8\xde\x1f\x00\xf2\xde\x1f\x11yaml:\"start_time\"\x12^\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationB1\xc8\xde\x1f\x00\x98\xdf\x1f\x01\xea\xde\x1f\x12\x64uration,omitempty\xf2\xde\x1f\x0fyaml:\"duration\"\x12\x15\n\rcurrent_epoch\x18\x04 \x01(\x04\x12i\n\x18\x63urrent_epoch_start_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB+\x90\xdf\x1f\x01\xc8\xde\x1f\x00\xf2\xde\x1f\x1fyaml:\"current_epoch_start_time\"\x12\x1e\n\x16\x65poch_counting_started\x18\x06 \x01(\x08\x12\"\n\x1a\x63urrent_epoch_start_height\x18\x07 \x01(\x03\x42.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x65pochs/state.proto\x12\x15nibiru.epochs.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x94\x03\n\tEpochInfo\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12M\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x1d\x90\xdf\x1f\x01\xc8\xde\x1f\x00\xf2\xde\x1f\x11yaml:\"start_time\"\x12^\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationB1\xc8\xde\x1f\x00\x98\xdf\x1f\x01\xea\xde\x1f\x12\x64uration,omitempty\xf2\xde\x1f\x0fyaml:\"duration\"\x12\x15\n\rcurrent_epoch\x18\x04 \x01(\x04\x12i\n\x18\x63urrent_epoch_start_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB+\x90\xdf\x1f\x01\xc8\xde\x1f\x00\xf2\xde\x1f\x1fyaml:\"current_epoch_start_time\"\x12\x1e\n\x16\x65poch_counting_started\x18\x06 \x01(\x08\x12\"\n\x1a\x63urrent_epoch_start_height\x18\x07 \x01(\x03\x42.Z,github.com/NibiruChain/nibiru/x/epochs/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'epochs.v1.state_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'epochs.state_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/epochs/types'
   _EPOCHINFO.fields_by_name['start_time']._options = None
   _EPOCHINFO.fields_by_name['start_time']._serialized_options = b'\220\337\037\001\310\336\037\000\362\336\037\021yaml:\"start_time\"'
   _EPOCHINFO.fields_by_name['duration']._options = None
   _EPOCHINFO.fields_by_name['duration']._serialized_options = b'\310\336\037\000\230\337\037\001\352\336\037\022duration,omitempty\362\336\037\017yaml:\"duration\"'
   _EPOCHINFO.fields_by_name['current_epoch_start_time']._options = None
   _EPOCHINFO.fields_by_name['current_epoch_start_time']._serialized_options = b'\220\337\037\001\310\336\037\000\362\336\037\037yaml:\"current_epoch_start_time\"'
-  _EPOCHINFO._serialized_start=136
-  _EPOCHINFO._serialized_end=540
+  _EPOCHINFO._serialized_start=133
+  _EPOCHINFO._serialized_end=537
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/epochs/v1/state_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/epochs/state_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -37,17 +37,15 @@
         """How long each epoch lasts for."""
     current_epoch: builtins.int
     """The current epoch number, starting from 1."""
     @property
     def current_epoch_start_time(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """The start timestamp of the current epoch."""
     epoch_counting_started: builtins.bool
-    """Whether or not this epoch has started. Set to true if current blocktime >=
-    start_time.
-    """
+    """Whether or not this epoch has started. Set to true if current blocktime >= start_time."""
     current_epoch_start_height: builtins.int
     """The block height at which the current epoch started at."""
     def __init__(
         self,
         *,
         identifier: builtins.str = ...,
         start_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/gogoproto/gogo_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/gogoproto/gogo_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/gogoproto/gogo_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/gogoproto/gogo_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/annotations_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/annotations_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/annotations_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/http_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/http_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/http_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/httpbody_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/httpbody_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/httpbody_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/api/httpbody_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/api/httpbody_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/protobuf/any_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/protobuf/any_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/protobuf/any_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/protobuf/any_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/google/protobuf/any_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/google/protobuf/any_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/params_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: inflation/v1/genesis.proto
+# source: stablecoin/params.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from inflation.v1 import inflation_pb2 as inflation_dot_v1_dot_inflation__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ainflation/v1/genesis.proto\x12\x13nibiru.inflation.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cinflation/v1/inflation.proto\"i\n\x0cGenesisState\x12\x31\n\x06params\x18\x01 \x01(\x0b\x32\x1b.nibiru.inflation.v1.ParamsB\x04\xc8\xde\x1f\x00\x12\x0e\n\x06period\x18\x02 \x01(\x04\x12\x16\n\x0eskipped_epochs\x18\x03 \x01(\x04\"\xe4\x01\n\x06Params\x12\x19\n\x11inflation_enabled\x18\x01 \x01(\x08\x12R\n\x17\x65xponential_calculation\x18\x02 \x01(\x0b\x32+.nibiru.inflation.v1.ExponentialCalculationB\x04\xc8\xde\x1f\x00\x12P\n\x16inflation_distribution\x18\x03 \x01(\x0b\x32*.nibiru.inflation.v1.InflationDistributionB\x04\xc8\xde\x1f\x00\x12\x19\n\x11\x65pochs_per_period\x18\x04 \x01(\x04\x42\x31Z/github.com/NibiruChain/nibiru/x/inflation/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17stablecoin/params.proto\x12\x14nibiru.stablecoin.v1\x1a\x14gogoproto/gogo.proto\"\x95\x02\n\x06Params\x12\x12\n\ncoll_ratio\x18\x01 \x01(\x03\x12\x11\n\tfee_ratio\x18\x02 \x01(\x03\x12\x14\n\x0c\x65\x66_fee_ratio\x18\x03 \x01(\x03\x12\x19\n\x11\x62onus_rate_recoll\x18\x04 \x01(\x03\x12\x41\n\x16\x64istr_epoch_identifier\x18\x05 \x01(\tB!\xf2\xde\x1f\x1dyaml:\"distr_epoch_identifier\"\x12\x17\n\x0f\x61\x64justment_step\x18\x06 \x01(\x03\x12\x19\n\x11price_lower_bound\x18\x07 \x01(\x03\x12\x19\n\x11price_upper_bound\x18\x08 \x01(\x03\x12!\n\x19is_collateral_ratio_valid\x18\t \x01(\x08\x42\x32Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'inflation.v1.genesis_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.params_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z/github.com/NibiruChain/nibiru/x/inflation/types'
-  _GENESISSTATE.fields_by_name['params']._options = None
-  _GENESISSTATE.fields_by_name['params']._serialized_options = b'\310\336\037\000'
-  _PARAMS.fields_by_name['exponential_calculation']._options = None
-  _PARAMS.fields_by_name['exponential_calculation']._serialized_options = b'\310\336\037\000'
-  _PARAMS.fields_by_name['inflation_distribution']._options = None
-  _PARAMS.fields_by_name['inflation_distribution']._serialized_options = b'\310\336\037\000'
-  _GENESISSTATE._serialized_start=103
-  _GENESISSTATE._serialized_end=208
-  _PARAMS._serialized_start=211
-  _PARAMS._serialized_end=439
+  DESCRIPTOR._serialized_options = b'Z0github.com/NibiruChain/nibiru/x/stablecoin/types'
+  _PARAMS.fields_by_name['distr_epoch_identifier']._options = None
+  _PARAMS.fields_by_name['distr_epoch_identifier']._serialized_options = b'\362\336\037\035yaml:\"distr_epoch_identifier\"'
+  _PARAMS._serialized_start=72
+  _PARAMS._serialized_end=349
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/inflation_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/util/v1/query_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: inflation/v1/inflation.proto
+# source: util/v1/query.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
+from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
+from vpool.v1 import state_pb2 as vpool_dot_v1_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cinflation/v1/inflation.proto\x12\x13nibiru.inflation.v1\x1a\x14gogoproto/gogo.proto\"\xf4\x01\n\x15InflationDistribution\x12G\n\x0fstaking_rewards\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x46\n\x0e\x63ommunity_pool\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12J\n\x12strategic_reserves\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\xc9\x01\n\x16\x45xponentialCalculation\x12\x39\n\x01\x61\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x39\n\x01r\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x39\n\x01\x63\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x42\x31Z/github.com/NibiruChain/nibiru/x/inflation/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13util/v1/query.proto\x12\x0enibiru.util.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14vpool/v1/state.proto\"\x1c\n\x1aQueryModuleAccountsRequest\"Y\n\x1bQueryModuleAccountsResponse\x12:\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\".nibiru.util.v1.AccountWithBalanceB\x04\xc8\xde\x1f\x00\"\x91\x01\n\x12\x41\x63\x63ountWithBalance\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\\\n\x07\x62\x61lance\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins2\x99\x01\n\x05Query\x12\x8f\x01\n\x0eModuleAccounts\x12*.nibiru.util.v1.QueryModuleAccountsRequest\x1a+.nibiru.util.v1.QueryModuleAccountsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/nibiru/util/module_accountsB,Z*github.com/NibiruChain/nibiru/x/util/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'inflation.v1.inflation_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'util.v1.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z/github.com/NibiruChain/nibiru/x/inflation/types'
-  _INFLATIONDISTRIBUTION.fields_by_name['staking_rewards']._options = None
-  _INFLATIONDISTRIBUTION.fields_by_name['staking_rewards']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _INFLATIONDISTRIBUTION.fields_by_name['community_pool']._options = None
-  _INFLATIONDISTRIBUTION.fields_by_name['community_pool']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _INFLATIONDISTRIBUTION.fields_by_name['strategic_reserves']._options = None
-  _INFLATIONDISTRIBUTION.fields_by_name['strategic_reserves']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _EXPONENTIALCALCULATION.fields_by_name['a']._options = None
-  _EXPONENTIALCALCULATION.fields_by_name['a']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _EXPONENTIALCALCULATION.fields_by_name['r']._options = None
-  _EXPONENTIALCALCULATION.fields_by_name['r']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _EXPONENTIALCALCULATION.fields_by_name['c']._options = None
-  _EXPONENTIALCALCULATION.fields_by_name['c']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _INFLATIONDISTRIBUTION._serialized_start=76
-  _INFLATIONDISTRIBUTION._serialized_end=320
-  _EXPONENTIALCALCULATION._serialized_start=323
-  _EXPONENTIALCALCULATION._serialized_end=524
+  DESCRIPTOR._serialized_options = b'Z*github.com/NibiruChain/nibiru/x/util/types'
+  _QUERYMODULEACCOUNTSRESPONSE.fields_by_name['accounts']._options = None
+  _QUERYMODULEACCOUNTSRESPONSE.fields_by_name['accounts']._serialized_options = b'\310\336\037\000'
+  _ACCOUNTWITHBALANCE.fields_by_name['balance']._options = None
+  _ACCOUNTWITHBALANCE.fields_by_name['balance']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
+  _QUERY.methods_by_name['ModuleAccounts']._options = None
+  _QUERY.methods_by_name['ModuleAccounts']._serialized_options = b'\202\323\344\223\002\036\022\034/nibiru/util/module_accounts'
+  _QUERYMODULEACCOUNTSREQUEST._serialized_start=145
+  _QUERYMODULEACCOUNTSREQUEST._serialized_end=173
+  _QUERYMODULEACCOUNTSRESPONSE._serialized_start=175
+  _QUERYMODULEACCOUNTSRESPONSE._serialized_end=264
+  _ACCOUNTWITHBALANCE._serialized_start=267
+  _ACCOUNTWITHBALANCE._serialized_end=412
+  _QUERY._serialized_start=415
+  _QUERY._serialized_end=568
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/query_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,81 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: inflation/v1/query.proto
+# source: stablecoin/query.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
-from inflation.v1 import genesis_pb2 as inflation_dot_v1_dot_genesis__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from cosmos.base.query.v1beta1 import pagination_pb2 as cosmos_dot_base_dot_query_dot_v1beta1_dot_pagination__pb2
+from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
+from stablecoin import params_pb2 as stablecoin_dot_params__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18inflation/v1/query.proto\x12\x13nibiru.inflation.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x1ainflation/v1/genesis.proto\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"\x14\n\x12QueryPeriodRequest\"%\n\x13QueryPeriodResponse\x12\x0e\n\x06period\x18\x01 \x01(\x04\" \n\x1eQueryEpochMintProvisionRequest\"\x92\x01\n\x1fQueryEpochMintProvisionResponse\x12o\n\x14\x65poch_mint_provision\x18\x01 \x01(\x0b\x32\x1c.cosmos.base.v1beta1.DecCoinB3\xc8\xde\x1f\x00\xaa\xdf\x1f+github.com/cosmos/cosmos-sdk/types.DecCoins\"\x1b\n\x19QuerySkippedEpochsRequest\"4\n\x1aQuerySkippedEpochsResponse\x12\x16\n\x0eskipped_epochs\x18\x01 \x01(\x04\"\x1f\n\x1dQueryCirculatingSupplyRequest\"\x8f\x01\n\x1eQueryCirculatingSupplyResponse\x12m\n\x12\x63irculating_supply\x18\x01 \x01(\x0b\x32\x1c.cosmos.base.v1beta1.DecCoinB3\xc8\xde\x1f\x00\xaa\xdf\x1f+github.com/cosmos/cosmos-sdk/types.DecCoins\"\x1b\n\x19QueryInflationRateRequest\"d\n\x1aQueryInflationRateResponse\x12\x46\n\x0einflation_rate\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\x14\n\x12QueryParamsRequest\"H\n\x13QueryParamsResponse\x12\x31\n\x06params\x18\x01 \x01(\x0b\x32\x1b.nibiru.inflation.v1.ParamsB\x04\xc8\xde\x1f\x00\x32\xb2\x07\n\x05Query\x12\x80\x01\n\x06Period\x12\'.nibiru.inflation.v1.QueryPeriodRequest\x1a(.nibiru.inflation.v1.QueryPeriodResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/nibiru/inflation/v1/period\x12\xb2\x01\n\x12\x45pochMintProvision\x12\x33.nibiru.inflation.v1.QueryEpochMintProvisionRequest\x1a\x34.nibiru.inflation.v1.QueryEpochMintProvisionResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/inflation/v1/epoch_mint_provision\x12\x9d\x01\n\rSkippedEpochs\x12..nibiru.inflation.v1.QuerySkippedEpochsRequest\x1a/.nibiru.inflation.v1.QuerySkippedEpochsResponse\"+\x82\xd3\xe4\x93\x02%\x12#/nibiru/inflation/v1/skipped_epochs\x12\xad\x01\n\x11\x43irculatingSupply\x12\x32.nibiru.inflation.v1.QueryCirculatingSupplyRequest\x1a\x33.nibiru.inflation.v1.QueryCirculatingSupplyResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/nibiru/inflation/v1/circulating_supply\x12\x9d\x01\n\rInflationRate\x12..nibiru.inflation.v1.QueryInflationRateRequest\x1a/.nibiru.inflation.v1.QueryInflationRateResponse\"+\x82\xd3\xe4\x93\x02%\x12#/nibiru/inflation/v1/inflation_rate\x12\x80\x01\n\x06Params\x12\'.nibiru.inflation.v1.QueryParamsRequest\x1a(.nibiru.inflation.v1.QueryParamsResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/nibiru/inflation/v1/paramsB1Z/github.com/NibiruChain/nibiru/x/inflation/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16stablecoin/query.proto\x12\x14nibiru.stablecoin.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a*cosmos/base/query/v1beta1/pagination.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x17stablecoin/params.proto\"\x14\n\x12QueryParamsRequest\"I\n\x13QueryParamsResponse\x12\x32\n\x06params\x18\x01 \x01(\x0b\x32\x1c.nibiru.stablecoin.v1.ParamsB\x04\xc8\xde\x1f\x00\"\x1c\n\x1aQueryModuleAccountBalances\"\xa2\x01\n\"QueryModuleAccountBalancesResponse\x12|\n\x17module_account_balances\x18\x01 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB@\xf2\xde\x1f\x0cyaml:\"coins\"\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\"\x1a\n\x18QueryCirculatingSupplies\"\x80\x01\n QueryCirculatingSuppliesResponse\x12-\n\x04nibi\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12-\n\x04nusd\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"K\n\x14QueryGovToMintStable\x12\x33\n\ncollateral\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"L\n\x1cQueryGovToMintStableResponse\x12,\n\x03gov\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\xe5\x01\n\x12LiquidityRatioInfo\x12G\n\x0fliquidity_ratio\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x42\n\nupper_band\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x42\n\nlower_band\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\" \n\x1eQueryLiquidityRatioInfoRequest\"_\n\x1fQueryLiquidityRatioInfoResponse\x12<\n\x04info\x18\x01 \x01(\x0b\x32(.nibiru.stablecoin.v1.LiquidityRatioInfoB\x04\xc8\xde\x1f\x00\x32\xa9\x05\n\x05Query\x12\x80\x01\n\x06Params\x12(.nibiru.stablecoin.v1.QueryParamsRequest\x1a).nibiru.stablecoin.v1.QueryParamsResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/nibiru/stablecoin/params\x12\xb6\x01\n\x15ModuleAccountBalances\x12\x30.nibiru.stablecoin.v1.QueryModuleAccountBalances\x1a\x38.nibiru.stablecoin.v1.QueryModuleAccountBalancesResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/stablecoin/module_account_balance\x12\xae\x01\n\x13\x43irculatingSupplies\x12..nibiru.stablecoin.v1.QueryCirculatingSupplies\x1a\x36.nibiru.stablecoin.v1.QueryCirculatingSuppliesResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/nibiru/stablecoin/circulating_supplies\x12\xb2\x01\n\x12LiquidityRatioInfo\x12\x34.nibiru.stablecoin.v1.QueryLiquidityRatioInfoRequest\x1a\x35.nibiru.stablecoin.v1.QueryLiquidityRatioInfoResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/nibiru/stablecoin/liquidity_ratio_infoB2Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'inflation.v1.query_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z/github.com/NibiruChain/nibiru/x/inflation/types'
-  _QUERYEPOCHMINTPROVISIONRESPONSE.fields_by_name['epoch_mint_provision']._options = None
-  _QUERYEPOCHMINTPROVISIONRESPONSE.fields_by_name['epoch_mint_provision']._serialized_options = b'\310\336\037\000\252\337\037+github.com/cosmos/cosmos-sdk/types.DecCoins'
-  _QUERYCIRCULATINGSUPPLYRESPONSE.fields_by_name['circulating_supply']._options = None
-  _QUERYCIRCULATINGSUPPLYRESPONSE.fields_by_name['circulating_supply']._serialized_options = b'\310\336\037\000\252\337\037+github.com/cosmos/cosmos-sdk/types.DecCoins'
-  _QUERYINFLATIONRATERESPONSE.fields_by_name['inflation_rate']._options = None
-  _QUERYINFLATIONRATERESPONSE.fields_by_name['inflation_rate']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  DESCRIPTOR._serialized_options = b'Z0github.com/NibiruChain/nibiru/x/stablecoin/types'
   _QUERYPARAMSRESPONSE.fields_by_name['params']._options = None
   _QUERYPARAMSRESPONSE.fields_by_name['params']._serialized_options = b'\310\336\037\000'
-  _QUERY.methods_by_name['Period']._options = None
-  _QUERY.methods_by_name['Period']._serialized_options = b'\202\323\344\223\002\035\022\033/nibiru/inflation/v1/period'
-  _QUERY.methods_by_name['EpochMintProvision']._options = None
-  _QUERY.methods_by_name['EpochMintProvision']._serialized_options = b'\202\323\344\223\002+\022)/nibiru/inflation/v1/epoch_mint_provision'
-  _QUERY.methods_by_name['SkippedEpochs']._options = None
-  _QUERY.methods_by_name['SkippedEpochs']._serialized_options = b'\202\323\344\223\002%\022#/nibiru/inflation/v1/skipped_epochs'
-  _QUERY.methods_by_name['CirculatingSupply']._options = None
-  _QUERY.methods_by_name['CirculatingSupply']._serialized_options = b'\202\323\344\223\002)\022\'/nibiru/inflation/v1/circulating_supply'
-  _QUERY.methods_by_name['InflationRate']._options = None
-  _QUERY.methods_by_name['InflationRate']._serialized_options = b'\202\323\344\223\002%\022#/nibiru/inflation/v1/inflation_rate'
+  _QUERYMODULEACCOUNTBALANCESRESPONSE.fields_by_name['module_account_balances']._options = None
+  _QUERYMODULEACCOUNTBALANCESRESPONSE.fields_by_name['module_account_balances']._serialized_options = b'\362\336\037\014yaml:\"coins\"\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
+  _QUERYCIRCULATINGSUPPLIESRESPONSE.fields_by_name['nibi']._options = None
+  _QUERYCIRCULATINGSUPPLIESRESPONSE.fields_by_name['nibi']._serialized_options = b'\310\336\037\000'
+  _QUERYCIRCULATINGSUPPLIESRESPONSE.fields_by_name['nusd']._options = None
+  _QUERYCIRCULATINGSUPPLIESRESPONSE.fields_by_name['nusd']._serialized_options = b'\310\336\037\000'
+  _QUERYGOVTOMINTSTABLE.fields_by_name['collateral']._options = None
+  _QUERYGOVTOMINTSTABLE.fields_by_name['collateral']._serialized_options = b'\310\336\037\000'
+  _QUERYGOVTOMINTSTABLERESPONSE.fields_by_name['gov']._options = None
+  _QUERYGOVTOMINTSTABLERESPONSE.fields_by_name['gov']._serialized_options = b'\310\336\037\000'
+  _LIQUIDITYRATIOINFO.fields_by_name['liquidity_ratio']._options = None
+  _LIQUIDITYRATIOINFO.fields_by_name['liquidity_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _LIQUIDITYRATIOINFO.fields_by_name['upper_band']._options = None
+  _LIQUIDITYRATIOINFO.fields_by_name['upper_band']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _LIQUIDITYRATIOINFO.fields_by_name['lower_band']._options = None
+  _LIQUIDITYRATIOINFO.fields_by_name['lower_band']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _QUERYLIQUIDITYRATIOINFORESPONSE.fields_by_name['info']._options = None
+  _QUERYLIQUIDITYRATIOINFORESPONSE.fields_by_name['info']._serialized_options = b'\310\336\037\000'
   _QUERY.methods_by_name['Params']._options = None
-  _QUERY.methods_by_name['Params']._serialized_options = b'\202\323\344\223\002\035\022\033/nibiru/inflation/v1/params'
-  _QUERYPERIODREQUEST._serialized_start=161
-  _QUERYPERIODREQUEST._serialized_end=181
-  _QUERYPERIODRESPONSE._serialized_start=183
-  _QUERYPERIODRESPONSE._serialized_end=220
-  _QUERYEPOCHMINTPROVISIONREQUEST._serialized_start=222
-  _QUERYEPOCHMINTPROVISIONREQUEST._serialized_end=254
-  _QUERYEPOCHMINTPROVISIONRESPONSE._serialized_start=257
-  _QUERYEPOCHMINTPROVISIONRESPONSE._serialized_end=403
-  _QUERYSKIPPEDEPOCHSREQUEST._serialized_start=405
-  _QUERYSKIPPEDEPOCHSREQUEST._serialized_end=432
-  _QUERYSKIPPEDEPOCHSRESPONSE._serialized_start=434
-  _QUERYSKIPPEDEPOCHSRESPONSE._serialized_end=486
-  _QUERYCIRCULATINGSUPPLYREQUEST._serialized_start=488
-  _QUERYCIRCULATINGSUPPLYREQUEST._serialized_end=519
-  _QUERYCIRCULATINGSUPPLYRESPONSE._serialized_start=522
-  _QUERYCIRCULATINGSUPPLYRESPONSE._serialized_end=665
-  _QUERYINFLATIONRATEREQUEST._serialized_start=667
-  _QUERYINFLATIONRATEREQUEST._serialized_end=694
-  _QUERYINFLATIONRATERESPONSE._serialized_start=696
-  _QUERYINFLATIONRATERESPONSE._serialized_end=796
-  _QUERYPARAMSREQUEST._serialized_start=798
-  _QUERYPARAMSREQUEST._serialized_end=818
-  _QUERYPARAMSRESPONSE._serialized_start=820
-  _QUERYPARAMSRESPONSE._serialized_end=892
-  _QUERY._serialized_start=895
-  _QUERY._serialized_end=1841
+  _QUERY.methods_by_name['Params']._serialized_options = b'\202\323\344\223\002\033\022\031/nibiru/stablecoin/params'
+  _QUERY.methods_by_name['ModuleAccountBalances']._options = None
+  _QUERY.methods_by_name['ModuleAccountBalances']._serialized_options = b'\202\323\344\223\002+\022)/nibiru/stablecoin/module_account_balance'
+  _QUERY.methods_by_name['CirculatingSupplies']._options = None
+  _QUERY.methods_by_name['CirculatingSupplies']._serialized_options = b'\202\323\344\223\002)\022\'/nibiru/stablecoin/circulating_supplies'
+  _QUERY.methods_by_name['LiquidityRatioInfo']._options = None
+  _QUERY.methods_by_name['LiquidityRatioInfo']._serialized_options = b'\202\323\344\223\002)\022\'/nibiru/stablecoin/liquidity_ratio_info'
+  _QUERYPARAMSREQUEST._serialized_start=201
+  _QUERYPARAMSREQUEST._serialized_end=221
+  _QUERYPARAMSRESPONSE._serialized_start=223
+  _QUERYPARAMSRESPONSE._serialized_end=296
+  _QUERYMODULEACCOUNTBALANCES._serialized_start=298
+  _QUERYMODULEACCOUNTBALANCES._serialized_end=326
+  _QUERYMODULEACCOUNTBALANCESRESPONSE._serialized_start=329
+  _QUERYMODULEACCOUNTBALANCESRESPONSE._serialized_end=491
+  _QUERYCIRCULATINGSUPPLIES._serialized_start=493
+  _QUERYCIRCULATINGSUPPLIES._serialized_end=519
+  _QUERYCIRCULATINGSUPPLIESRESPONSE._serialized_start=522
+  _QUERYCIRCULATINGSUPPLIESRESPONSE._serialized_end=650
+  _QUERYGOVTOMINTSTABLE._serialized_start=652
+  _QUERYGOVTOMINTSTABLE._serialized_end=727
+  _QUERYGOVTOMINTSTABLERESPONSE._serialized_start=729
+  _QUERYGOVTOMINTSTABLERESPONSE._serialized_end=805
+  _LIQUIDITYRATIOINFO._serialized_start=808
+  _LIQUIDITYRATIOINFO._serialized_end=1037
+  _QUERYLIQUIDITYRATIOINFOREQUEST._serialized_start=1039
+  _QUERYLIQUIDITYRATIOINFOREQUEST._serialized_end=1071
+  _QUERYLIQUIDITYRATIOINFORESPONSE._serialized_start=1073
+  _QUERYLIQUIDITYRATIOINFORESPONSE._serialized_end=1168
+  _QUERY._serialized_start=1171
+  _QUERY._serialized_end=1852
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/inflation/v1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/query_pb2_grpc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,241 +1,203 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from inflation.v1 import query_pb2 as inflation_dot_v1_dot_query__pb2
+from perp.v1 import query_pb2 as perp_dot_v1_dot_query__pb2
 
 
 class QueryStub(object):
-    """Query provides defines the gRPC querier service.
+    """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.Period = channel.unary_unary(
-                '/nibiru.inflation.v1.Query/Period',
-                request_serializer=inflation_dot_v1_dot_query__pb2.QueryPeriodRequest.SerializeToString,
-                response_deserializer=inflation_dot_v1_dot_query__pb2.QueryPeriodResponse.FromString,
-                )
-        self.EpochMintProvision = channel.unary_unary(
-                '/nibiru.inflation.v1.Query/EpochMintProvision',
-                request_serializer=inflation_dot_v1_dot_query__pb2.QueryEpochMintProvisionRequest.SerializeToString,
-                response_deserializer=inflation_dot_v1_dot_query__pb2.QueryEpochMintProvisionResponse.FromString,
-                )
-        self.SkippedEpochs = channel.unary_unary(
-                '/nibiru.inflation.v1.Query/SkippedEpochs',
-                request_serializer=inflation_dot_v1_dot_query__pb2.QuerySkippedEpochsRequest.SerializeToString,
-                response_deserializer=inflation_dot_v1_dot_query__pb2.QuerySkippedEpochsResponse.FromString,
-                )
-        self.CirculatingSupply = channel.unary_unary(
-                '/nibiru.inflation.v1.Query/CirculatingSupply',
-                request_serializer=inflation_dot_v1_dot_query__pb2.QueryCirculatingSupplyRequest.SerializeToString,
-                response_deserializer=inflation_dot_v1_dot_query__pb2.QueryCirculatingSupplyResponse.FromString,
-                )
-        self.InflationRate = channel.unary_unary(
-                '/nibiru.inflation.v1.Query/InflationRate',
-                request_serializer=inflation_dot_v1_dot_query__pb2.QueryInflationRateRequest.SerializeToString,
-                response_deserializer=inflation_dot_v1_dot_query__pb2.QueryInflationRateResponse.FromString,
-                )
         self.Params = channel.unary_unary(
-                '/nibiru.inflation.v1.Query/Params',
-                request_serializer=inflation_dot_v1_dot_query__pb2.QueryParamsRequest.SerializeToString,
-                response_deserializer=inflation_dot_v1_dot_query__pb2.QueryParamsResponse.FromString,
+                '/nibiru.perp.v1.Query/Params',
+                request_serializer=perp_dot_v1_dot_query__pb2.QueryParamsRequest.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_query__pb2.QueryParamsResponse.FromString,
+                )
+        self.QueryPosition = channel.unary_unary(
+                '/nibiru.perp.v1.Query/QueryPosition',
+                request_serializer=perp_dot_v1_dot_query__pb2.QueryPositionRequest.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_query__pb2.QueryPositionResponse.FromString,
+                )
+        self.QueryPositions = channel.unary_unary(
+                '/nibiru.perp.v1.Query/QueryPositions',
+                request_serializer=perp_dot_v1_dot_query__pb2.QueryPositionsRequest.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_query__pb2.QueryPositionsResponse.FromString,
+                )
+        self.CumulativePremiumFraction = channel.unary_unary(
+                '/nibiru.perp.v1.Query/CumulativePremiumFraction',
+                request_serializer=perp_dot_v1_dot_query__pb2.QueryCumulativePremiumFractionRequest.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_query__pb2.QueryCumulativePremiumFractionResponse.FromString,
+                )
+        self.Metrics = channel.unary_unary(
+                '/nibiru.perp.v1.Query/Metrics',
+                request_serializer=perp_dot_v1_dot_query__pb2.QueryMetricsRequest.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_query__pb2.QueryMetricsResponse.FromString,
                 )
 
 
 class QueryServicer(object):
-    """Query provides defines the gRPC querier service.
+    """Query defines the gRPC querier service.
     """
 
-    def Period(self, request, context):
-        """Period retrieves current period.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def EpochMintProvision(self, request, context):
-        """EpochMintProvision retrieves current minting epoch provision value.
+    def Params(self, request, context):
+        """Parameters queries the parameters of the x/perp module.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SkippedEpochs(self, request, context):
-        """SkippedEpochs retrieves the total number of skipped epochs.
-        """
+    def QueryPosition(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CirculatingSupply(self, request, context):
-        """CirculatingSupply retrieves the total number of tokens that are in
-        circulation (i.e. excluding unvested tokens).
-        """
+    def QueryPositions(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def InflationRate(self, request, context):
-        """InflationRate retrieves the inflation rate of the current period.
+    def CumulativePremiumFraction(self, request, context):
+        """Queries the latest cumulative premium fraction and the estimated next cumulative premium fraction.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Params(self, request, context):
-        """Params retrieves the total set of minting parameters.
-        """
+    def Metrics(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_QueryServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'Period': grpc.unary_unary_rpc_method_handler(
-                    servicer.Period,
-                    request_deserializer=inflation_dot_v1_dot_query__pb2.QueryPeriodRequest.FromString,
-                    response_serializer=inflation_dot_v1_dot_query__pb2.QueryPeriodResponse.SerializeToString,
-            ),
-            'EpochMintProvision': grpc.unary_unary_rpc_method_handler(
-                    servicer.EpochMintProvision,
-                    request_deserializer=inflation_dot_v1_dot_query__pb2.QueryEpochMintProvisionRequest.FromString,
-                    response_serializer=inflation_dot_v1_dot_query__pb2.QueryEpochMintProvisionResponse.SerializeToString,
-            ),
-            'SkippedEpochs': grpc.unary_unary_rpc_method_handler(
-                    servicer.SkippedEpochs,
-                    request_deserializer=inflation_dot_v1_dot_query__pb2.QuerySkippedEpochsRequest.FromString,
-                    response_serializer=inflation_dot_v1_dot_query__pb2.QuerySkippedEpochsResponse.SerializeToString,
-            ),
-            'CirculatingSupply': grpc.unary_unary_rpc_method_handler(
-                    servicer.CirculatingSupply,
-                    request_deserializer=inflation_dot_v1_dot_query__pb2.QueryCirculatingSupplyRequest.FromString,
-                    response_serializer=inflation_dot_v1_dot_query__pb2.QueryCirculatingSupplyResponse.SerializeToString,
-            ),
-            'InflationRate': grpc.unary_unary_rpc_method_handler(
-                    servicer.InflationRate,
-                    request_deserializer=inflation_dot_v1_dot_query__pb2.QueryInflationRateRequest.FromString,
-                    response_serializer=inflation_dot_v1_dot_query__pb2.QueryInflationRateResponse.SerializeToString,
-            ),
             'Params': grpc.unary_unary_rpc_method_handler(
                     servicer.Params,
-                    request_deserializer=inflation_dot_v1_dot_query__pb2.QueryParamsRequest.FromString,
-                    response_serializer=inflation_dot_v1_dot_query__pb2.QueryParamsResponse.SerializeToString,
+                    request_deserializer=perp_dot_v1_dot_query__pb2.QueryParamsRequest.FromString,
+                    response_serializer=perp_dot_v1_dot_query__pb2.QueryParamsResponse.SerializeToString,
+            ),
+            'QueryPosition': grpc.unary_unary_rpc_method_handler(
+                    servicer.QueryPosition,
+                    request_deserializer=perp_dot_v1_dot_query__pb2.QueryPositionRequest.FromString,
+                    response_serializer=perp_dot_v1_dot_query__pb2.QueryPositionResponse.SerializeToString,
+            ),
+            'QueryPositions': grpc.unary_unary_rpc_method_handler(
+                    servicer.QueryPositions,
+                    request_deserializer=perp_dot_v1_dot_query__pb2.QueryPositionsRequest.FromString,
+                    response_serializer=perp_dot_v1_dot_query__pb2.QueryPositionsResponse.SerializeToString,
+            ),
+            'CumulativePremiumFraction': grpc.unary_unary_rpc_method_handler(
+                    servicer.CumulativePremiumFraction,
+                    request_deserializer=perp_dot_v1_dot_query__pb2.QueryCumulativePremiumFractionRequest.FromString,
+                    response_serializer=perp_dot_v1_dot_query__pb2.QueryCumulativePremiumFractionResponse.SerializeToString,
+            ),
+            'Metrics': grpc.unary_unary_rpc_method_handler(
+                    servicer.Metrics,
+                    request_deserializer=perp_dot_v1_dot_query__pb2.QueryMetricsRequest.FromString,
+                    response_serializer=perp_dot_v1_dot_query__pb2.QueryMetricsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'nibiru.inflation.v1.Query', rpc_method_handlers)
+            'nibiru.perp.v1.Query', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Query(object):
-    """Query provides defines the gRPC querier service.
+    """Query defines the gRPC querier service.
     """
 
     @staticmethod
-    def Period(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.inflation.v1.Query/Period',
-            inflation_dot_v1_dot_query__pb2.QueryPeriodRequest.SerializeToString,
-            inflation_dot_v1_dot_query__pb2.QueryPeriodResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def EpochMintProvision(request,
+    def Params(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.inflation.v1.Query/EpochMintProvision',
-            inflation_dot_v1_dot_query__pb2.QueryEpochMintProvisionRequest.SerializeToString,
-            inflation_dot_v1_dot_query__pb2.QueryEpochMintProvisionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Query/Params',
+            perp_dot_v1_dot_query__pb2.QueryParamsRequest.SerializeToString,
+            perp_dot_v1_dot_query__pb2.QueryParamsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SkippedEpochs(request,
+    def QueryPosition(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.inflation.v1.Query/SkippedEpochs',
-            inflation_dot_v1_dot_query__pb2.QuerySkippedEpochsRequest.SerializeToString,
-            inflation_dot_v1_dot_query__pb2.QuerySkippedEpochsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Query/QueryPosition',
+            perp_dot_v1_dot_query__pb2.QueryPositionRequest.SerializeToString,
+            perp_dot_v1_dot_query__pb2.QueryPositionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CirculatingSupply(request,
+    def QueryPositions(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.inflation.v1.Query/CirculatingSupply',
-            inflation_dot_v1_dot_query__pb2.QueryCirculatingSupplyRequest.SerializeToString,
-            inflation_dot_v1_dot_query__pb2.QueryCirculatingSupplyResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Query/QueryPositions',
+            perp_dot_v1_dot_query__pb2.QueryPositionsRequest.SerializeToString,
+            perp_dot_v1_dot_query__pb2.QueryPositionsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def InflationRate(request,
+    def CumulativePremiumFraction(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.inflation.v1.Query/InflationRate',
-            inflation_dot_v1_dot_query__pb2.QueryInflationRateRequest.SerializeToString,
-            inflation_dot_v1_dot_query__pb2.QueryInflationRateResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Query/CumulativePremiumFraction',
+            perp_dot_v1_dot_query__pb2.QueryCumulativePremiumFractionRequest.SerializeToString,
+            perp_dot_v1_dot_query__pb2.QueryCumulativePremiumFractionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Params(request,
+    def Metrics(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.inflation.v1.Query/Params',
-            inflation_dot_v1_dot_query__pb2.QueryParamsRequest.SerializeToString,
-            inflation_dot_v1_dot_query__pb2.QueryParamsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Query/Metrics',
+            perp_dot_v1_dot_query__pb2.QueryMetricsRequest.SerializeToString,
+            perp_dot_v1_dot_query__pb2.QueryMetricsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/event_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/event_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: oracle/v1/event.proto
+# source: oracle/v1beta1/event.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15oracle/v1/event.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"v\n\x11OraclePriceUpdate\x12\x0c\n\x04pair\x18\x01 \x01(\t\x12=\n\x05price\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0ctimestamp_ms\x18\x03 \x01(\x03\x42.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aoracle/v1beta1/event.proto\x12\x15nibiru.oracle.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"v\n\x11OraclePriceUpdate\x12\x0c\n\x04pair\x18\x01 \x01(\t\x12=\n\x05price\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0ctimestamp_ms\x18\x03 \x01(\x03\x42.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1.event_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1beta1.event_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/oracle/types'
   _ORACLEPRICEUPDATE.fields_by_name['price']._options = None
   _ORACLEPRICEUPDATE.fields_by_name['price']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _ORACLEPRICEUPDATE._serialized_start=95
-  _ORACLEPRICEUPDATE._serialized_end=213
+  _ORACLEPRICEUPDATE._serialized_start=105
+  _ORACLEPRICEUPDATE._serialized_end=223
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/event_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/genesis_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: oracle/v1/genesis.proto
+# source: oracle/v1beta1/genesis.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from oracle.v1 import oracle_pb2 as oracle_dot_v1_dot_oracle__pb2
+from oracle.v1beta1 import oracle_pb2 as oracle_dot_v1beta1_dot_oracle__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17oracle/v1/genesis.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x16oracle/v1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\xcf\x04\n\x0cGenesisState\x12.\n\x06params\x18\x01 \x01(\x0b\x32\x18.nibiru.oracle.v1.ParamsB\x04\xc8\xde\x1f\x00\x12\x44\n\x12\x66\x65\x65\x64\x65r_delegations\x18\x02 \x03(\x0b\x32\".nibiru.oracle.v1.FeederDelegationB\x04\xc8\xde\x1f\x00\x12W\n\x0e\x65xchange_rates\x18\x03 \x03(\x0b\x32#.nibiru.oracle.v1.ExchangeRateTupleB\x1a\xaa\xdf\x1f\x12\x45xchangeRateTuples\xc8\xde\x1f\x00\x12:\n\rmiss_counters\x18\x04 \x03(\x0b\x32\x1d.nibiru.oracle.v1.MissCounterB\x04\xc8\xde\x1f\x00\x12^\n aggregate_exchange_rate_prevotes\x18\x05 \x03(\x0b\x32..nibiru.oracle.v1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00\x12X\n\x1d\x61ggregate_exchange_rate_votes\x18\x06 \x03(\x0b\x32+.nibiru.oracle.v1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00\x12H\n\x05pairs\x18\x07 \x03(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x30\n\x07rewards\x18\x08 \x03(\x0b\x32\x19.nibiru.oracle.v1.RewardsB\x04\xc8\xde\x1f\x00\"E\n\x10\x46\x65\x65\x64\x65rDelegation\x12\x16\n\x0e\x66\x65\x65\x64\x65r_address\x18\x01 \x01(\t\x12\x19\n\x11validator_address\x18\x02 \x01(\t\">\n\x0bMissCounter\x12\x19\n\x11validator_address\x18\x01 \x01(\t\x12\x14\n\x0cmiss_counter\x18\x02 \x01(\x04\x42.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1coracle/v1beta1/genesis.proto\x12\x15nibiru.oracle.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1boracle/v1beta1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\xfa\x04\n\x0cGenesisState\x12\x33\n\x06params\x18\x01 \x01(\x0b\x32\x1d.nibiru.oracle.v1beta1.ParamsB\x04\xc8\xde\x1f\x00\x12I\n\x12\x66\x65\x65\x64\x65r_delegations\x18\x02 \x03(\x0b\x32\'.nibiru.oracle.v1beta1.FeederDelegationB\x04\xc8\xde\x1f\x00\x12\\\n\x0e\x65xchange_rates\x18\x03 \x03(\x0b\x32(.nibiru.oracle.v1beta1.ExchangeRateTupleB\x1a\xaa\xdf\x1f\x12\x45xchangeRateTuples\xc8\xde\x1f\x00\x12?\n\rmiss_counters\x18\x04 \x03(\x0b\x32\".nibiru.oracle.v1beta1.MissCounterB\x04\xc8\xde\x1f\x00\x12\x63\n aggregate_exchange_rate_prevotes\x18\x05 \x03(\x0b\x32\x33.nibiru.oracle.v1beta1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00\x12]\n\x1d\x61ggregate_exchange_rate_votes\x18\x06 \x03(\x0b\x32\x30.nibiru.oracle.v1beta1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00\x12H\n\x05pairs\x18\x07 \x03(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12=\n\x0cpair_rewards\x18\x08 \x03(\x0b\x32!.nibiru.oracle.v1beta1.PairRewardB\x04\xc8\xde\x1f\x00\"E\n\x10\x46\x65\x65\x64\x65rDelegation\x12\x16\n\x0e\x66\x65\x65\x64\x65r_address\x18\x01 \x01(\t\x12\x19\n\x11validator_address\x18\x02 \x01(\t\">\n\x0bMissCounter\x12\x19\n\x11validator_address\x18\x01 \x01(\t\x12\x14\n\x0cmiss_counter\x18\x02 \x01(\x04\x42.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1.genesis_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1beta1.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/oracle/types'
   _GENESISSTATE.fields_by_name['params']._options = None
   _GENESISSTATE.fields_by_name['params']._serialized_options = b'\310\336\037\000'
   _GENESISSTATE.fields_by_name['feeder_delegations']._options = None
@@ -34,16 +34,16 @@
   _GENESISSTATE.fields_by_name['miss_counters']._serialized_options = b'\310\336\037\000'
   _GENESISSTATE.fields_by_name['aggregate_exchange_rate_prevotes']._options = None
   _GENESISSTATE.fields_by_name['aggregate_exchange_rate_prevotes']._serialized_options = b'\310\336\037\000'
   _GENESISSTATE.fields_by_name['aggregate_exchange_rate_votes']._options = None
   _GENESISSTATE.fields_by_name['aggregate_exchange_rate_votes']._serialized_options = b'\310\336\037\000'
   _GENESISSTATE.fields_by_name['pairs']._options = None
   _GENESISSTATE.fields_by_name['pairs']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
-  _GENESISSTATE.fields_by_name['rewards']._options = None
-  _GENESISSTATE.fields_by_name['rewards']._serialized_options = b'\310\336\037\000'
-  _GENESISSTATE._serialized_start=124
-  _GENESISSTATE._serialized_end=715
-  _FEEDERDELEGATION._serialized_start=717
-  _FEEDERDELEGATION._serialized_end=786
-  _MISSCOUNTER._serialized_start=788
-  _MISSCOUNTER._serialized_end=850
+  _GENESISSTATE.fields_by_name['pair_rewards']._options = None
+  _GENESISSTATE.fields_by_name['pair_rewards']._serialized_options = b'\310\336\037\000'
+  _GENESISSTATE._serialized_start=139
+  _GENESISSTATE._serialized_end=773
+  _FEEDERDELEGATION._serialized_start=775
+  _FEEDERDELEGATION._serialized_end=844
+  _MISSCOUNTER._serialized_start=846
+  _MISSCOUNTER._serialized_end=908
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/genesis_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import oracle.v1.oracle_pb2
+import oracle.v1beta1.oracle_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -26,45 +26,45 @@
     PARAMS_FIELD_NUMBER: builtins.int
     FEEDER_DELEGATIONS_FIELD_NUMBER: builtins.int
     EXCHANGE_RATES_FIELD_NUMBER: builtins.int
     MISS_COUNTERS_FIELD_NUMBER: builtins.int
     AGGREGATE_EXCHANGE_RATE_PREVOTES_FIELD_NUMBER: builtins.int
     AGGREGATE_EXCHANGE_RATE_VOTES_FIELD_NUMBER: builtins.int
     PAIRS_FIELD_NUMBER: builtins.int
-    REWARDS_FIELD_NUMBER: builtins.int
+    PAIR_REWARDS_FIELD_NUMBER: builtins.int
     @property
-    def params(self) -> oracle.v1.oracle_pb2.Params: ...
+    def params(self) -> oracle.v1beta1.oracle_pb2.Params: ...
     @property
     def feeder_delegations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FeederDelegation]: ...
     @property
-    def exchange_rates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1.oracle_pb2.ExchangeRateTuple]: ...
+    def exchange_rates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1beta1.oracle_pb2.ExchangeRateTuple]: ...
     @property
     def miss_counters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MissCounter]: ...
     @property
-    def aggregate_exchange_rate_prevotes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1.oracle_pb2.AggregateExchangeRatePrevote]: ...
+    def aggregate_exchange_rate_prevotes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1beta1.oracle_pb2.AggregateExchangeRatePrevote]: ...
     @property
-    def aggregate_exchange_rate_votes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1.oracle_pb2.AggregateExchangeRateVote]: ...
+    def aggregate_exchange_rate_votes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1beta1.oracle_pb2.AggregateExchangeRateVote]: ...
     @property
     def pairs(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
-    def rewards(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1.oracle_pb2.Rewards]: ...
+    def pair_rewards(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1beta1.oracle_pb2.PairReward]: ...
     def __init__(
         self,
         *,
-        params: oracle.v1.oracle_pb2.Params | None = ...,
+        params: oracle.v1beta1.oracle_pb2.Params | None = ...,
         feeder_delegations: collections.abc.Iterable[global___FeederDelegation] | None = ...,
-        exchange_rates: collections.abc.Iterable[oracle.v1.oracle_pb2.ExchangeRateTuple] | None = ...,
+        exchange_rates: collections.abc.Iterable[oracle.v1beta1.oracle_pb2.ExchangeRateTuple] | None = ...,
         miss_counters: collections.abc.Iterable[global___MissCounter] | None = ...,
-        aggregate_exchange_rate_prevotes: collections.abc.Iterable[oracle.v1.oracle_pb2.AggregateExchangeRatePrevote] | None = ...,
-        aggregate_exchange_rate_votes: collections.abc.Iterable[oracle.v1.oracle_pb2.AggregateExchangeRateVote] | None = ...,
+        aggregate_exchange_rate_prevotes: collections.abc.Iterable[oracle.v1beta1.oracle_pb2.AggregateExchangeRatePrevote] | None = ...,
+        aggregate_exchange_rate_votes: collections.abc.Iterable[oracle.v1beta1.oracle_pb2.AggregateExchangeRateVote] | None = ...,
         pairs: collections.abc.Iterable[builtins.str] | None = ...,
-        rewards: collections.abc.Iterable[oracle.v1.oracle_pb2.Rewards] | None = ...,
+        pair_rewards: collections.abc.Iterable[oracle.v1beta1.oracle_pb2.PairReward] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["aggregate_exchange_rate_prevotes", b"aggregate_exchange_rate_prevotes", "aggregate_exchange_rate_votes", b"aggregate_exchange_rate_votes", "exchange_rates", b"exchange_rates", "feeder_delegations", b"feeder_delegations", "miss_counters", b"miss_counters", "pairs", b"pairs", "params", b"params", "rewards", b"rewards"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["aggregate_exchange_rate_prevotes", b"aggregate_exchange_rate_prevotes", "aggregate_exchange_rate_votes", b"aggregate_exchange_rate_votes", "exchange_rates", b"exchange_rates", "feeder_delegations", b"feeder_delegations", "miss_counters", b"miss_counters", "pair_rewards", b"pair_rewards", "pairs", b"pairs", "params", b"params"]) -> None: ...
 
 global___GenesisState = GenesisState
 
 @typing_extensions.final
 class FeederDelegation(google.protobuf.message.Message):
     """FeederDelegation is the address for where oracle feeder authority are
     delegated to. By default this struct is only used at genesis to feed in
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/oracle_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/oracle_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: oracle/v1/oracle.proto
+# source: oracle/v1beta1/oracle.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
@@ -12,18 +12,18 @@
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16oracle/v1/oracle.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\xf1\x06\n\x06Params\x12+\n\x0bvote_period\x18\x01 \x01(\x04\x42\x16\xf2\xde\x1f\x12yaml:\"vote_period\"\x12_\n\x0evote_threshold\x18\x02 \x01(\tBG\xf2\xde\x1f\x15yaml:\"vote_threshold\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12Y\n\x0breward_band\x18\x03 \x01(\tBD\xf2\xde\x1f\x12yaml:\"reward_band\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\\\n\twhitelist\x18\x04 \x03(\tBI\xf2\xde\x1f\x10yaml:\"whitelist\"\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\x12_\n\x0eslash_fraction\x18\x05 \x01(\tBG\xf2\xde\x1f\x15yaml:\"slash_fraction\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12-\n\x0cslash_window\x18\x06 \x01(\x04\x42\x17\xf2\xde\x1f\x13yaml:\"slash_window\"\x12k\n\x14min_valid_per_window\x18\x07 \x01(\tBM\xf2\xde\x1f\x1byaml:\"min_valid_per_window\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x82\x01\n\x14twap_lookback_window\x18\x08 \x01(\x0b\x32\x19.google.protobuf.DurationBI\xc8\xde\x1f\x00\x98\xdf\x1f\x01\xea\xde\x1f\x1etwap_lookback_window,omitempty\xf2\xde\x1f\x1byaml:\"twap_lookback_window\"\x12)\n\nmin_voters\x18\t \x01(\x04\x42\x15\xf2\xde\x1f\x11yaml:\"min_voters\"\x12i\n\x13validator_fee_ratio\x18\n \x01(\tBL\xf2\xde\x1f\x1ayaml:\"validator_fee_ratio\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00:\x08\xe8\xa0\x1f\x01\x98\xa0\x1f\x00\"\x9b\x01\n\x1c\x41ggregateExchangeRatePrevote\x12\x1d\n\x04hash\x18\x01 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"hash\"\x12\x1f\n\x05voter\x18\x02 \x01(\tB\x10\xf2\xde\x1f\x0cyaml:\"voter\"\x12-\n\x0csubmit_block\x18\x03 \x01(\x04\x42\x17\xf2\xde\x1f\x13yaml:\"submit_block\":\x0c\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\x98\xa0\x1f\x00\"\xc8\x01\n\x19\x41ggregateExchangeRateVote\x12|\n\x14\x65xchange_rate_tuples\x18\x01 \x03(\x0b\x32#.nibiru.oracle.v1.ExchangeRateTupleB9\xf2\xde\x1f\x1byaml:\"exchange_rate_tuples\"\xaa\xdf\x1f\x12\x45xchangeRateTuples\xc8\xde\x1f\x00\x12\x1f\n\x05voter\x18\x02 \x01(\tB\x10\xf2\xde\x1f\x0cyaml:\"voter\":\x0c\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\x98\xa0\x1f\x00\"\xd8\x01\n\x11\x45xchangeRateTuple\x12V\n\x04pair\x18\x01 \x01(\tBH\xf2\xde\x1f\x0byaml:\"pair\"\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12]\n\rexchange_rate\x18\x02 \x01(\tBF\xf2\xde\x1f\x14yaml:\"exchange_rate\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00:\x0c\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\x98\xa0\x1f\x00\"[\n\x07Rewards\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x14\n\x0cvote_periods\x18\x02 \x01(\x04\x12.\n\x05\x63oins\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x42.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1boracle/v1beta1/oracle.proto\x12\x15nibiru.oracle.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\x86\x06\n\x06Params\x12+\n\x0bvote_period\x18\x01 \x01(\x04\x42\x16\xf2\xde\x1f\x12yaml:\"vote_period\"\x12_\n\x0evote_threshold\x18\x02 \x01(\tBG\xf2\xde\x1f\x15yaml:\"vote_threshold\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12Y\n\x0breward_band\x18\x03 \x01(\tBD\xf2\xde\x1f\x12yaml:\"reward_band\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\\\n\twhitelist\x18\x04 \x03(\tBI\xf2\xde\x1f\x10yaml:\"whitelist\"\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\x12_\n\x0eslash_fraction\x18\x05 \x01(\tBG\xf2\xde\x1f\x15yaml:\"slash_fraction\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12-\n\x0cslash_window\x18\x06 \x01(\x04\x42\x17\xf2\xde\x1f\x13yaml:\"slash_window\"\x12k\n\x14min_valid_per_window\x18\x07 \x01(\tBM\xf2\xde\x1f\x1byaml:\"min_valid_per_window\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x82\x01\n\x14twap_lookback_window\x18\x08 \x01(\x0b\x32\x19.google.protobuf.DurationBI\xc8\xde\x1f\x00\x98\xdf\x1f\x01\xea\xde\x1f\x1etwap_lookback_window,omitempty\xf2\xde\x1f\x1byaml:\"twap_lookback_window\"\x12)\n\nmin_voters\x18\t \x01(\x04\x42\x15\xf2\xde\x1f\x11yaml:\"min_voters\":\x08\xe8\xa0\x1f\x01\x98\xa0\x1f\x00\"\x9b\x01\n\x1c\x41ggregateExchangeRatePrevote\x12\x1d\n\x04hash\x18\x01 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"hash\"\x12\x1f\n\x05voter\x18\x02 \x01(\tB\x10\xf2\xde\x1f\x0cyaml:\"voter\"\x12-\n\x0csubmit_block\x18\x03 \x01(\x04\x42\x17\xf2\xde\x1f\x13yaml:\"submit_block\":\x0c\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\x98\xa0\x1f\x00\"\xce\x01\n\x19\x41ggregateExchangeRateVote\x12\x81\x01\n\x14\x65xchange_rate_tuples\x18\x01 \x03(\x0b\x32(.nibiru.oracle.v1beta1.ExchangeRateTupleB9\xf2\xde\x1f\x1byaml:\"exchange_rate_tuples\"\xaa\xdf\x1f\x12\x45xchangeRateTuples\xc8\xde\x1f\x00\x12\x1f\n\x05voter\x18\x02 \x01(\tB\x10\xf2\xde\x1f\x0cyaml:\"voter\":\x0c\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\x98\xa0\x1f\x00\"\xd8\x01\n\x11\x45xchangeRateTuple\x12V\n\x04pair\x18\x01 \x01(\tBH\xf2\xde\x1f\x0byaml:\"pair\"\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12]\n\rexchange_rate\x18\x02 \x01(\tBF\xf2\xde\x1f\x14yaml:\"exchange_rate\"\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00:\x0c\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\x98\xa0\x1f\x00\"\xa7\x01\n\nPairReward\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x14\n\x0cvote_periods\x18\x03 \x01(\x04\x12.\n\x05\x63oins\x18\x04 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x42.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1.oracle_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1beta1.oracle_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/oracle/types'
   _PARAMS.fields_by_name['vote_period']._options = None
   _PARAMS.fields_by_name['vote_period']._serialized_options = b'\362\336\037\022yaml:\"vote_period\"'
   _PARAMS.fields_by_name['vote_threshold']._options = None
@@ -38,16 +38,14 @@
   _PARAMS.fields_by_name['slash_window']._serialized_options = b'\362\336\037\023yaml:\"slash_window\"'
   _PARAMS.fields_by_name['min_valid_per_window']._options = None
   _PARAMS.fields_by_name['min_valid_per_window']._serialized_options = b'\362\336\037\033yaml:\"min_valid_per_window\"\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _PARAMS.fields_by_name['twap_lookback_window']._options = None
   _PARAMS.fields_by_name['twap_lookback_window']._serialized_options = b'\310\336\037\000\230\337\037\001\352\336\037\036twap_lookback_window,omitempty\362\336\037\033yaml:\"twap_lookback_window\"'
   _PARAMS.fields_by_name['min_voters']._options = None
   _PARAMS.fields_by_name['min_voters']._serialized_options = b'\362\336\037\021yaml:\"min_voters\"'
-  _PARAMS.fields_by_name['validator_fee_ratio']._options = None
-  _PARAMS.fields_by_name['validator_fee_ratio']._serialized_options = b'\362\336\037\032yaml:\"validator_fee_ratio\"\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _PARAMS._options = None
   _PARAMS._serialized_options = b'\350\240\037\001\230\240\037\000'
   _AGGREGATEEXCHANGERATEPREVOTE.fields_by_name['hash']._options = None
   _AGGREGATEEXCHANGERATEPREVOTE.fields_by_name['hash']._serialized_options = b'\362\336\037\013yaml:\"hash\"'
   _AGGREGATEEXCHANGERATEPREVOTE.fields_by_name['voter']._options = None
   _AGGREGATEEXCHANGERATEPREVOTE.fields_by_name['voter']._serialized_options = b'\362\336\037\014yaml:\"voter\"'
   _AGGREGATEEXCHANGERATEPREVOTE.fields_by_name['submit_block']._options = None
@@ -62,20 +60,22 @@
   _AGGREGATEEXCHANGERATEVOTE._serialized_options = b'\350\240\037\000\210\240\037\000\230\240\037\000'
   _EXCHANGERATETUPLE.fields_by_name['pair']._options = None
   _EXCHANGERATETUPLE.fields_by_name['pair']._serialized_options = b'\362\336\037\013yaml:\"pair\"\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
   _EXCHANGERATETUPLE.fields_by_name['exchange_rate']._options = None
   _EXCHANGERATETUPLE.fields_by_name['exchange_rate']._serialized_options = b'\362\336\037\024yaml:\"exchange_rate\"\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _EXCHANGERATETUPLE._options = None
   _EXCHANGERATETUPLE._serialized_options = b'\350\240\037\000\210\240\037\000\230\240\037\000'
-  _REWARDS.fields_by_name['coins']._options = None
-  _REWARDS.fields_by_name['coins']._serialized_options = b'\310\336\037\000'
-  _PARAMS._serialized_start=131
-  _PARAMS._serialized_end=1012
-  _AGGREGATEEXCHANGERATEPREVOTE._serialized_start=1015
-  _AGGREGATEEXCHANGERATEPREVOTE._serialized_end=1170
-  _AGGREGATEEXCHANGERATEVOTE._serialized_start=1173
-  _AGGREGATEEXCHANGERATEVOTE._serialized_end=1373
-  _EXCHANGERATETUPLE._serialized_start=1376
-  _EXCHANGERATETUPLE._serialized_end=1592
-  _REWARDS._serialized_start=1594
-  _REWARDS._serialized_end=1685
+  _PAIRREWARD.fields_by_name['pair']._options = None
+  _PAIRREWARD.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
+  _PAIRREWARD.fields_by_name['coins']._options = None
+  _PAIRREWARD.fields_by_name['coins']._serialized_options = b'\310\336\037\000'
+  _PARAMS._serialized_start=141
+  _PARAMS._serialized_end=915
+  _AGGREGATEEXCHANGERATEPREVOTE._serialized_start=918
+  _AGGREGATEEXCHANGERATEPREVOTE._serialized_end=1073
+  _AGGREGATEEXCHANGERATEVOTE._serialized_start=1076
+  _AGGREGATEEXCHANGERATEVOTE._serialized_end=1282
+  _EXCHANGERATETUPLE._serialized_start=1285
+  _EXCHANGERATETUPLE._serialized_end=1501
+  _PAIRREWARD._serialized_start=1504
+  _PAIRREWARD._serialized_end=1671
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/oracle_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/oracle_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,82 +29,77 @@
     REWARD_BAND_FIELD_NUMBER: builtins.int
     WHITELIST_FIELD_NUMBER: builtins.int
     SLASH_FRACTION_FIELD_NUMBER: builtins.int
     SLASH_WINDOW_FIELD_NUMBER: builtins.int
     MIN_VALID_PER_WINDOW_FIELD_NUMBER: builtins.int
     TWAP_LOOKBACK_WINDOW_FIELD_NUMBER: builtins.int
     MIN_VOTERS_FIELD_NUMBER: builtins.int
-    VALIDATOR_FEE_RATIO_FIELD_NUMBER: builtins.int
     vote_period: builtins.int
     """VotePeriod defines the number of blocks during which voting takes place."""
     vote_threshold: builtins.str
-    """VoteThreshold specifies the minimum proportion of votes that must be
+    """VoteThreshold specifies the minimum proportion of votes that must be 
     received for a ballot to pass.
     """
     reward_band: builtins.str
     """RewardBand defines a maxium divergence that a price vote can have from the
     weighted median in the ballot. If a vote lies within the valid range
     defined by:
     	μ := weightedMedian,
     	validRange := μ ± (μ * rewardBand / 2),
     then rewards are added to the validator performance.
     Note that if the reward band is smaller than 1 standard
     deviation, the band is taken to be 1 standard deviation.a price
     """
     @property
     def whitelist(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """The set of whitelisted markets, or asset pairs, for the module.
+        """The set of whitelisted markets, or asset pairs, for the module. 
         Ex. '["unibi:uusd","ubtc:uusd"]'
         """
     slash_fraction: builtins.str
-    """SlashFraction returns the proportion of an oracle's stake that gets
-    slashed in the event of slashing. `SlashFraction` specifies the exact
+    """SlashFraction returns the proportion of an oracle's stake that gets 
+    slashed in the event of slashing. `SlashFraction` specifies the exact 
     penalty for failing a voting period.
     """
     slash_window: builtins.int
-    """SlashWindow returns the number of voting periods that specify a
-    "slash window". After each slash window, all oracles that have missed more
-    than the penalty threshold are slashed. Missing the penalty threshold is
+    """SlashWindow returns the number of voting periods that specify a 
+    "slash window". After each slash window, all oracles that have missed more 
+    than the penalty threshold are slashed. Missing the penalty threshold is 
     synonymous with submitting fewer valid votes than `MinValidPerWindow`.
     """
     min_valid_per_window: builtins.str
     @property
     def twap_lookback_window(self) -> google.protobuf.duration_pb2.Duration:
         """Amount of time to look back for TWAP calculations"""
     min_voters: builtins.int
-    """The minimum number of voters (i.e. oracle validators) per pair for it to be
-    considered a passing ballot. Recommended at least 4.
+    """The minimum number of voters (i.e. oracle validators) per pair for it to be considered a passing ballot.
+    Recommended at least 4.
     """
-    validator_fee_ratio: builtins.str
-    """The validator fee ratio that is given to validators every epoch."""
     def __init__(
         self,
         *,
         vote_period: builtins.int = ...,
         vote_threshold: builtins.str = ...,
         reward_band: builtins.str = ...,
         whitelist: collections.abc.Iterable[builtins.str] | None = ...,
         slash_fraction: builtins.str = ...,
         slash_window: builtins.int = ...,
         min_valid_per_window: builtins.str = ...,
         twap_lookback_window: google.protobuf.duration_pb2.Duration | None = ...,
         min_voters: builtins.int = ...,
-        validator_fee_ratio: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["twap_lookback_window", b"twap_lookback_window"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["min_valid_per_window", b"min_valid_per_window", "min_voters", b"min_voters", "reward_band", b"reward_band", "slash_fraction", b"slash_fraction", "slash_window", b"slash_window", "twap_lookback_window", b"twap_lookback_window", "validator_fee_ratio", b"validator_fee_ratio", "vote_period", b"vote_period", "vote_threshold", b"vote_threshold", "whitelist", b"whitelist"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["min_valid_per_window", b"min_valid_per_window", "min_voters", b"min_voters", "reward_band", b"reward_band", "slash_fraction", b"slash_fraction", "slash_window", b"slash_window", "twap_lookback_window", b"twap_lookback_window", "vote_period", b"vote_period", "vote_threshold", b"vote_threshold", "whitelist", b"whitelist"]) -> None: ...
 
 global___Params = Params
 
 @typing_extensions.final
 class AggregateExchangeRatePrevote(google.protobuf.message.Message):
     """Struct for aggregate prevoting on the ExchangeRateVote.
     The purpose of aggregate prevote is to hide vote exchange rates with hash
-    which is formatted as hex string in
-    SHA256("{salt}:({pair},{exchange_rate})|...|({pair},{exchange_rate}):{voter}")
+    which is formatted as hex string in SHA256("{salt}:({pair},{exchange_rate})|...|({pair},{exchange_rate}):{voter}")
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HASH_FIELD_NUMBER: builtins.int
     VOTER_FIELD_NUMBER: builtins.int
     SUBMIT_BLOCK_FIELD_NUMBER: builtins.int
@@ -162,36 +157,38 @@
         exchange_rate: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["exchange_rate", b"exchange_rate", "pair", b"pair"]) -> None: ...
 
 global___ExchangeRateTuple = ExchangeRateTuple
 
 @typing_extensions.final
-class Rewards(google.protobuf.message.Message):
-    """Rewards defines a credit object towards validators
+class PairReward(google.protobuf.message.Message):
+    """PairReward defines a credit object towards validators
     which provide prices faithfully for different pairs.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    PAIR_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     VOTE_PERIODS_FIELD_NUMBER: builtins.int
     COINS_FIELD_NUMBER: builtins.int
+    pair: builtins.str
+    """pair defines the pair for which we incentivize validator to provide prices for."""
     id: builtins.int
     """id uniquely identifies the rewards instance of the pair"""
     vote_periods: builtins.int
-    """vote_periods defines the vote periods left in which rewards will be
-    distributed.
-    """
+    """vote_periods defines the vote periods left in which rewards will be distributed."""
     @property
     def coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]:
         """Coins defines the amount of coins to distribute in a single vote period."""
     def __init__(
         self,
         *,
+        pair: builtins.str = ...,
         id: builtins.int = ...,
         vote_periods: builtins.int = ...,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins", "id", b"id", "vote_periods", b"vote_periods"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins", "id", b"id", "pair", b"pair", "vote_periods", b"vote_periods"]) -> None: ...
 
-global___Rewards = Rewards
+global___PairReward = PairReward
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/query_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: oracle/v1/query.proto
+# source: oracle/v1beta1/query.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from oracle.v1 import oracle_pb2 as oracle_dot_v1_dot_oracle__pb2
+from oracle.v1beta1 import oracle_pb2 as oracle_dot_v1beta1_dot_oracle__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15oracle/v1/query.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x16oracle/v1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"m\n\x18QueryExchangeRateRequest\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"b\n\x19QueryExchangeRateResponse\x12\x45\n\rexchange_rate\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\x1b\n\x19QueryExchangeRatesRequest\"u\n\x1aQueryExchangeRatesResponse\x12W\n\x0e\x65xchange_rates\x18\x01 \x03(\x0b\x32#.nibiru.oracle.v1.ExchangeRateTupleB\x1a\xaa\xdf\x1f\x12\x45xchangeRateTuples\xc8\xde\x1f\x00\"\x15\n\x13QueryActivesRequest\"b\n\x14QueryActivesResponse\x12J\n\x07\x61\x63tives\x18\x01 \x03(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\"\x19\n\x17QueryVoteTargetsRequest\"k\n\x18QueryVoteTargetsResponse\x12O\n\x0cvote_targets\x18\x01 \x03(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\"@\n\x1cQueryFeederDelegationRequest\x12\x16\n\x0evalidator_addr\x18\x01 \x01(\t:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"4\n\x1dQueryFeederDelegationResponse\x12\x13\n\x0b\x66\x65\x65\x64\x65r_addr\x18\x01 \x01(\t\";\n\x17QueryMissCounterRequest\x12\x16\n\x0evalidator_addr\x18\x01 \x01(\t:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"0\n\x18QueryMissCounterResponse\x12\x14\n\x0cmiss_counter\x18\x01 \x01(\x04\"@\n\x1cQueryAggregatePrevoteRequest\x12\x16\n\x0evalidator_addr\x18\x01 \x01(\t:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"p\n\x1dQueryAggregatePrevoteResponse\x12O\n\x11\x61ggregate_prevote\x18\x01 \x01(\x0b\x32..nibiru.oracle.v1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00\"\x1f\n\x1dQueryAggregatePrevotesRequest\"r\n\x1eQueryAggregatePrevotesResponse\x12P\n\x12\x61ggregate_prevotes\x18\x01 \x03(\x0b\x32..nibiru.oracle.v1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00\"=\n\x19QueryAggregateVoteRequest\x12\x16\n\x0evalidator_addr\x18\x01 \x01(\t:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"g\n\x1aQueryAggregateVoteResponse\x12I\n\x0e\x61ggregate_vote\x18\x01 \x01(\x0b\x32+.nibiru.oracle.v1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00\"\x1c\n\x1aQueryAggregateVotesRequest\"i\n\x1bQueryAggregateVotesResponse\x12J\n\x0f\x61ggregate_votes\x18\x01 \x03(\x0b\x32+.nibiru.oracle.v1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00\"\x14\n\x12QueryParamsRequest\"E\n\x13QueryParamsResponse\x12.\n\x06params\x18\x01 \x01(\x0b\x32\x18.nibiru.oracle.v1.ParamsB\x04\xc8\xde\x1f\x00\x32\xc2\x0f\n\x05Query\x12\x95\x01\n\x0c\x45xchangeRate\x12*.nibiru.oracle.v1.QueryExchangeRateRequest\x1a+.nibiru.oracle.v1.QueryExchangeRateResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/oracle/v1beta1/exchange_rate\x12\x9e\x01\n\x10\x45xchangeRateTwap\x12*.nibiru.oracle.v1.QueryExchangeRateRequest\x1a+.nibiru.oracle.v1.QueryExchangeRateResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/oracle/v1beta1/exchange_rate_twap\x12\x9f\x01\n\rExchangeRates\x12+.nibiru.oracle.v1.QueryExchangeRatesRequest\x1a,.nibiru.oracle.v1.QueryExchangeRatesResponse\"3\x82\xd3\xe4\x93\x02-\x12+/nibiru/oracle/v1beta1/pairs/exchange_rates\x12\x86\x01\n\x07\x41\x63tives\x12%.nibiru.oracle.v1.QueryActivesRequest\x1a&.nibiru.oracle.v1.QueryActivesResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/oracle/v1beta1/pairs/actives\x12\x97\x01\n\x0bVoteTargets\x12).nibiru.oracle.v1.QueryVoteTargetsRequest\x1a*.nibiru.oracle.v1.QueryVoteTargetsResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/oracle/v1beta1/pairs/vote_targets\x12\xb6\x01\n\x10\x46\x65\x65\x64\x65rDelegation\x12..nibiru.oracle.v1.QueryFeederDelegationRequest\x1a/.nibiru.oracle.v1.QueryFeederDelegationResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/nibiru/oracle/v1beta1/validators/{validator_addr}/feeder\x12\xa5\x01\n\x0bMissCounter\x12).nibiru.oracle.v1.QueryMissCounterRequest\x1a*.nibiru.oracle.v1.QueryMissCounterResponse\"?\x82\xd3\xe4\x93\x02\x39\x12\x37/nibiru/oracle/v1beta1/validators/{validator_addr}/miss\x12\xc1\x01\n\x10\x41ggregatePrevote\x12..nibiru.oracle.v1.QueryAggregatePrevoteRequest\x1a/.nibiru.oracle.v1.QueryAggregatePrevoteResponse\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/nibiru/oracle/v1beta1/validators/{validator_addr}/aggregate_prevote\x12\xb4\x01\n\x11\x41ggregatePrevotes\x12/.nibiru.oracle.v1.QueryAggregatePrevotesRequest\x1a\x30.nibiru.oracle.v1.QueryAggregatePrevotesResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/nibiru/oracle/v1beta1/validators/aggregate_prevotes\x12\xb5\x01\n\rAggregateVote\x12+.nibiru.oracle.v1.QueryAggregateVoteRequest\x1a,.nibiru.oracle.v1.QueryAggregateVoteResponse\"I\x82\xd3\xe4\x93\x02\x43\x12\x41/nibiru/oracle/v1beta1/valdiators/{validator_addr}/aggregate_vote\x12\xa8\x01\n\x0e\x41ggregateVotes\x12,.nibiru.oracle.v1.QueryAggregateVotesRequest\x1a-.nibiru.oracle.v1.QueryAggregateVotesResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/nibiru/oracle/v1beta1/validators/aggregate_votes\x12|\n\x06Params\x12$.nibiru.oracle.v1.QueryParamsRequest\x1a%.nibiru.oracle.v1.QueryParamsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/nibiru/oracle/v1beta1/paramsB.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aoracle/v1beta1/query.proto\x12\x15nibiru.oracle.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1boracle/v1beta1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"m\n\x18QueryExchangeRateRequest\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"b\n\x19QueryExchangeRateResponse\x12\x45\n\rexchange_rate\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\x1b\n\x19QueryExchangeRatesRequest\"z\n\x1aQueryExchangeRatesResponse\x12\\\n\x0e\x65xchange_rates\x18\x01 \x03(\x0b\x32(.nibiru.oracle.v1beta1.ExchangeRateTupleB\x1a\xaa\xdf\x1f\x12\x45xchangeRateTuples\xc8\xde\x1f\x00\"\x15\n\x13QueryActivesRequest\"b\n\x14QueryActivesResponse\x12J\n\x07\x61\x63tives\x18\x01 \x03(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\"\x19\n\x17QueryVoteTargetsRequest\"k\n\x18QueryVoteTargetsResponse\x12O\n\x0cvote_targets\x18\x01 \x03(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\"@\n\x1cQueryFeederDelegationRequest\x12\x16\n\x0evalidator_addr\x18\x01 \x01(\t:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"4\n\x1dQueryFeederDelegationResponse\x12\x13\n\x0b\x66\x65\x65\x64\x65r_addr\x18\x01 \x01(\t\";\n\x17QueryMissCounterRequest\x12\x16\n\x0evalidator_addr\x18\x01 \x01(\t:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"0\n\x18QueryMissCounterResponse\x12\x14\n\x0cmiss_counter\x18\x01 \x01(\x04\"@\n\x1cQueryAggregatePrevoteRequest\x12\x16\n\x0evalidator_addr\x18\x01 \x01(\t:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"u\n\x1dQueryAggregatePrevoteResponse\x12T\n\x11\x61ggregate_prevote\x18\x01 \x01(\x0b\x32\x33.nibiru.oracle.v1beta1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00\"\x1f\n\x1dQueryAggregatePrevotesRequest\"w\n\x1eQueryAggregatePrevotesResponse\x12U\n\x12\x61ggregate_prevotes\x18\x01 \x03(\x0b\x32\x33.nibiru.oracle.v1beta1.AggregateExchangeRatePrevoteB\x04\xc8\xde\x1f\x00\"=\n\x19QueryAggregateVoteRequest\x12\x16\n\x0evalidator_addr\x18\x01 \x01(\t:\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"l\n\x1aQueryAggregateVoteResponse\x12N\n\x0e\x61ggregate_vote\x18\x01 \x01(\x0b\x32\x30.nibiru.oracle.v1beta1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00\"\x1c\n\x1aQueryAggregateVotesRequest\"n\n\x1bQueryAggregateVotesResponse\x12O\n\x0f\x61ggregate_votes\x18\x01 \x03(\x0b\x32\x30.nibiru.oracle.v1beta1.AggregateExchangeRateVoteB\x04\xc8\xde\x1f\x00\"\x14\n\x12QueryParamsRequest\"J\n\x13QueryParamsResponse\x12\x33\n\x06params\x18\x01 \x01(\x0b\x32\x1d.nibiru.oracle.v1beta1.ParamsB\x04\xc8\xde\x1f\x00\x32\xbb\x10\n\x05Query\x12\x9f\x01\n\x0c\x45xchangeRate\x12/.nibiru.oracle.v1beta1.QueryExchangeRateRequest\x1a\x30.nibiru.oracle.v1beta1.QueryExchangeRateResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/oracle/v1beta1/exchange_rate\x12\xa8\x01\n\x10\x45xchangeRateTwap\x12/.nibiru.oracle.v1beta1.QueryExchangeRateRequest\x1a\x30.nibiru.oracle.v1beta1.QueryExchangeRateResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/oracle/v1beta1/exchange_rate_twap\x12\xa9\x01\n\rExchangeRates\x12\x30.nibiru.oracle.v1beta1.QueryExchangeRatesRequest\x1a\x31.nibiru.oracle.v1beta1.QueryExchangeRatesResponse\"3\x82\xd3\xe4\x93\x02-\x12+/nibiru/oracle/v1beta1/pairs/exchange_rates\x12\x90\x01\n\x07\x41\x63tives\x12*.nibiru.oracle.v1beta1.QueryActivesRequest\x1a+.nibiru.oracle.v1beta1.QueryActivesResponse\",\x82\xd3\xe4\x93\x02&\x12$/nibiru/oracle/v1beta1/pairs/actives\x12\xa1\x01\n\x0bVoteTargets\x12..nibiru.oracle.v1beta1.QueryVoteTargetsRequest\x1a/.nibiru.oracle.v1beta1.QueryVoteTargetsResponse\"1\x82\xd3\xe4\x93\x02+\x12)/nibiru/oracle/v1beta1/pairs/vote_targets\x12\xc0\x01\n\x10\x46\x65\x65\x64\x65rDelegation\x12\x33.nibiru.oracle.v1beta1.QueryFeederDelegationRequest\x1a\x34.nibiru.oracle.v1beta1.QueryFeederDelegationResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/nibiru/oracle/v1beta1/validators/{validator_addr}/feeder\x12\xaf\x01\n\x0bMissCounter\x12..nibiru.oracle.v1beta1.QueryMissCounterRequest\x1a/.nibiru.oracle.v1beta1.QueryMissCounterResponse\"?\x82\xd3\xe4\x93\x02\x39\x12\x37/nibiru/oracle/v1beta1/validators/{validator_addr}/miss\x12\xcb\x01\n\x10\x41ggregatePrevote\x12\x33.nibiru.oracle.v1beta1.QueryAggregatePrevoteRequest\x1a\x34.nibiru.oracle.v1beta1.QueryAggregatePrevoteResponse\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/nibiru/oracle/v1beta1/validators/{validator_addr}/aggregate_prevote\x12\xbe\x01\n\x11\x41ggregatePrevotes\x12\x34.nibiru.oracle.v1beta1.QueryAggregatePrevotesRequest\x1a\x35.nibiru.oracle.v1beta1.QueryAggregatePrevotesResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/nibiru/oracle/v1beta1/validators/aggregate_prevotes\x12\xbf\x01\n\rAggregateVote\x12\x30.nibiru.oracle.v1beta1.QueryAggregateVoteRequest\x1a\x31.nibiru.oracle.v1beta1.QueryAggregateVoteResponse\"I\x82\xd3\xe4\x93\x02\x43\x12\x41/nibiru/oracle/v1beta1/valdiators/{validator_addr}/aggregate_vote\x12\xb2\x01\n\x0e\x41ggregateVotes\x12\x31.nibiru.oracle.v1beta1.QueryAggregateVotesRequest\x1a\x32.nibiru.oracle.v1beta1.QueryAggregateVotesResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/nibiru/oracle/v1beta1/validators/aggregate_votes\x12\x86\x01\n\x06Params\x12).nibiru.oracle.v1beta1.QueryParamsRequest\x1a*.nibiru.oracle.v1beta1.QueryParamsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/nibiru/oracle/v1beta1/paramsB.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1.query_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1beta1.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/oracle/types'
   _QUERYEXCHANGERATEREQUEST.fields_by_name['pair']._options = None
   _QUERYEXCHANGERATEREQUEST.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
   _QUERYEXCHANGERATEREQUEST._options = None
@@ -75,54 +75,54 @@
   _QUERY.methods_by_name['AggregatePrevotes']._serialized_options = b'\202\323\344\223\0026\0224/nibiru/oracle/v1beta1/validators/aggregate_prevotes'
   _QUERY.methods_by_name['AggregateVote']._options = None
   _QUERY.methods_by_name['AggregateVote']._serialized_options = b'\202\323\344\223\002C\022A/nibiru/oracle/v1beta1/valdiators/{validator_addr}/aggregate_vote'
   _QUERY.methods_by_name['AggregateVotes']._options = None
   _QUERY.methods_by_name['AggregateVotes']._serialized_options = b'\202\323\344\223\0023\0221/nibiru/oracle/v1beta1/validators/aggregate_votes'
   _QUERY.methods_by_name['Params']._options = None
   _QUERY.methods_by_name['Params']._serialized_options = b'\202\323\344\223\002\037\022\035/nibiru/oracle/v1beta1/params'
-  _QUERYEXCHANGERATEREQUEST._serialized_start=151
-  _QUERYEXCHANGERATEREQUEST._serialized_end=260
-  _QUERYEXCHANGERATERESPONSE._serialized_start=262
-  _QUERYEXCHANGERATERESPONSE._serialized_end=360
-  _QUERYEXCHANGERATESREQUEST._serialized_start=362
-  _QUERYEXCHANGERATESREQUEST._serialized_end=389
-  _QUERYEXCHANGERATESRESPONSE._serialized_start=391
-  _QUERYEXCHANGERATESRESPONSE._serialized_end=508
-  _QUERYACTIVESREQUEST._serialized_start=510
-  _QUERYACTIVESREQUEST._serialized_end=531
-  _QUERYACTIVESRESPONSE._serialized_start=533
-  _QUERYACTIVESRESPONSE._serialized_end=631
-  _QUERYVOTETARGETSREQUEST._serialized_start=633
-  _QUERYVOTETARGETSREQUEST._serialized_end=658
-  _QUERYVOTETARGETSRESPONSE._serialized_start=660
-  _QUERYVOTETARGETSRESPONSE._serialized_end=767
-  _QUERYFEEDERDELEGATIONREQUEST._serialized_start=769
-  _QUERYFEEDERDELEGATIONREQUEST._serialized_end=833
-  _QUERYFEEDERDELEGATIONRESPONSE._serialized_start=835
-  _QUERYFEEDERDELEGATIONRESPONSE._serialized_end=887
-  _QUERYMISSCOUNTERREQUEST._serialized_start=889
-  _QUERYMISSCOUNTERREQUEST._serialized_end=948
-  _QUERYMISSCOUNTERRESPONSE._serialized_start=950
-  _QUERYMISSCOUNTERRESPONSE._serialized_end=998
-  _QUERYAGGREGATEPREVOTEREQUEST._serialized_start=1000
-  _QUERYAGGREGATEPREVOTEREQUEST._serialized_end=1064
-  _QUERYAGGREGATEPREVOTERESPONSE._serialized_start=1066
-  _QUERYAGGREGATEPREVOTERESPONSE._serialized_end=1178
-  _QUERYAGGREGATEPREVOTESREQUEST._serialized_start=1180
-  _QUERYAGGREGATEPREVOTESREQUEST._serialized_end=1211
-  _QUERYAGGREGATEPREVOTESRESPONSE._serialized_start=1213
-  _QUERYAGGREGATEPREVOTESRESPONSE._serialized_end=1327
-  _QUERYAGGREGATEVOTEREQUEST._serialized_start=1329
-  _QUERYAGGREGATEVOTEREQUEST._serialized_end=1390
-  _QUERYAGGREGATEVOTERESPONSE._serialized_start=1392
-  _QUERYAGGREGATEVOTERESPONSE._serialized_end=1495
-  _QUERYAGGREGATEVOTESREQUEST._serialized_start=1497
-  _QUERYAGGREGATEVOTESREQUEST._serialized_end=1525
-  _QUERYAGGREGATEVOTESRESPONSE._serialized_start=1527
-  _QUERYAGGREGATEVOTESRESPONSE._serialized_end=1632
-  _QUERYPARAMSREQUEST._serialized_start=1634
-  _QUERYPARAMSREQUEST._serialized_end=1654
-  _QUERYPARAMSRESPONSE._serialized_start=1656
-  _QUERYPARAMSRESPONSE._serialized_end=1725
-  _QUERY._serialized_start=1728
-  _QUERY._serialized_end=3714
+  _QUERYEXCHANGERATEREQUEST._serialized_start=166
+  _QUERYEXCHANGERATEREQUEST._serialized_end=275
+  _QUERYEXCHANGERATERESPONSE._serialized_start=277
+  _QUERYEXCHANGERATERESPONSE._serialized_end=375
+  _QUERYEXCHANGERATESREQUEST._serialized_start=377
+  _QUERYEXCHANGERATESREQUEST._serialized_end=404
+  _QUERYEXCHANGERATESRESPONSE._serialized_start=406
+  _QUERYEXCHANGERATESRESPONSE._serialized_end=528
+  _QUERYACTIVESREQUEST._serialized_start=530
+  _QUERYACTIVESREQUEST._serialized_end=551
+  _QUERYACTIVESRESPONSE._serialized_start=553
+  _QUERYACTIVESRESPONSE._serialized_end=651
+  _QUERYVOTETARGETSREQUEST._serialized_start=653
+  _QUERYVOTETARGETSREQUEST._serialized_end=678
+  _QUERYVOTETARGETSRESPONSE._serialized_start=680
+  _QUERYVOTETARGETSRESPONSE._serialized_end=787
+  _QUERYFEEDERDELEGATIONREQUEST._serialized_start=789
+  _QUERYFEEDERDELEGATIONREQUEST._serialized_end=853
+  _QUERYFEEDERDELEGATIONRESPONSE._serialized_start=855
+  _QUERYFEEDERDELEGATIONRESPONSE._serialized_end=907
+  _QUERYMISSCOUNTERREQUEST._serialized_start=909
+  _QUERYMISSCOUNTERREQUEST._serialized_end=968
+  _QUERYMISSCOUNTERRESPONSE._serialized_start=970
+  _QUERYMISSCOUNTERRESPONSE._serialized_end=1018
+  _QUERYAGGREGATEPREVOTEREQUEST._serialized_start=1020
+  _QUERYAGGREGATEPREVOTEREQUEST._serialized_end=1084
+  _QUERYAGGREGATEPREVOTERESPONSE._serialized_start=1086
+  _QUERYAGGREGATEPREVOTERESPONSE._serialized_end=1203
+  _QUERYAGGREGATEPREVOTESREQUEST._serialized_start=1205
+  _QUERYAGGREGATEPREVOTESREQUEST._serialized_end=1236
+  _QUERYAGGREGATEPREVOTESRESPONSE._serialized_start=1238
+  _QUERYAGGREGATEPREVOTESRESPONSE._serialized_end=1357
+  _QUERYAGGREGATEVOTEREQUEST._serialized_start=1359
+  _QUERYAGGREGATEVOTEREQUEST._serialized_end=1420
+  _QUERYAGGREGATEVOTERESPONSE._serialized_start=1422
+  _QUERYAGGREGATEVOTERESPONSE._serialized_end=1530
+  _QUERYAGGREGATEVOTESREQUEST._serialized_start=1532
+  _QUERYAGGREGATEVOTESREQUEST._serialized_end=1560
+  _QUERYAGGREGATEVOTESRESPONSE._serialized_start=1562
+  _QUERYAGGREGATEVOTESRESPONSE._serialized_end=1672
+  _QUERYPARAMSREQUEST._serialized_start=1674
+  _QUERYPARAMSREQUEST._serialized_end=1694
+  _QUERYPARAMSRESPONSE._serialized_start=1696
+  _QUERYPARAMSRESPONSE._serialized_end=1770
+  _QUERY._serialized_start=1773
+  _QUERY._serialized_end=3880
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/query_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import oracle.v1.oracle_pb2
+import oracle.v1beta1.oracle_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
 class QueryExchangeRateRequest(google.protobuf.message.Message):
-    """QueryExchangeRateRequest is the request type for the Query/ExchangeRate RPC
-    method.
-    """
+    """QueryExchangeRateRequest is the request type for the Query/ExchangeRate RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAIR_FIELD_NUMBER: builtins.int
     pair: builtins.str
     """pair defines the pair to query for."""
     def __init__(
@@ -55,17 +53,15 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["exchange_rate", b"exchange_rate"]) -> None: ...
 
 global___QueryExchangeRateResponse = QueryExchangeRateResponse
 
 @typing_extensions.final
 class QueryExchangeRatesRequest(google.protobuf.message.Message):
-    """QueryExchangeRatesRequest is the request type for the Query/ExchangeRates RPC
-    method.
-    """
+    """QueryExchangeRatesRequest is the request type for the Query/ExchangeRates RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
@@ -77,22 +73,20 @@
     Query/ExchangeRates RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXCHANGE_RATES_FIELD_NUMBER: builtins.int
     @property
-    def exchange_rates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1.oracle_pb2.ExchangeRateTuple]:
-        """exchange_rates defines a list of the exchange rate for all whitelisted
-        pairs.
-        """
+    def exchange_rates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1beta1.oracle_pb2.ExchangeRateTuple]:
+        """exchange_rates defines a list of the exchange rate for all whitelisted pairs."""
     def __init__(
         self,
         *,
-        exchange_rates: collections.abc.Iterable[oracle.v1.oracle_pb2.ExchangeRateTuple] | None = ...,
+        exchange_rates: collections.abc.Iterable[oracle.v1beta1.oracle_pb2.ExchangeRateTuple] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["exchange_rates", b"exchange_rates"]) -> None: ...
 
 global___QueryExchangeRatesResponse = QueryExchangeRatesResponse
 
 @typing_extensions.final
 class QueryActivesRequest(google.protobuf.message.Message):
@@ -125,17 +119,15 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["actives", b"actives"]) -> None: ...
 
 global___QueryActivesResponse = QueryActivesResponse
 
 @typing_extensions.final
 class QueryVoteTargetsRequest(google.protobuf.message.Message):
-    """QueryVoteTargetsRequest is the request type for the Query/VoteTargets RPC
-    method.
-    """
+    """QueryVoteTargetsRequest is the request type for the Query/VoteTargets RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
@@ -162,17 +154,15 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["vote_targets", b"vote_targets"]) -> None: ...
 
 global___QueryVoteTargetsResponse = QueryVoteTargetsResponse
 
 @typing_extensions.final
 class QueryFeederDelegationRequest(google.protobuf.message.Message):
-    """QueryFeederDelegationRequest is the request type for the
-    Query/FeederDelegation RPC method.
-    """
+    """QueryFeederDelegationRequest is the request type for the Query/FeederDelegation RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDR_FIELD_NUMBER: builtins.int
     validator_addr: builtins.str
     """validator defines the validator address to query for."""
     def __init__(
@@ -202,17 +192,15 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["feeder_addr", b"feeder_addr"]) -> None: ...
 
 global___QueryFeederDelegationResponse = QueryFeederDelegationResponse
 
 @typing_extensions.final
 class QueryMissCounterRequest(google.protobuf.message.Message):
-    """QueryMissCounterRequest is the request type for the Query/MissCounter RPC
-    method.
-    """
+    """QueryMissCounterRequest is the request type for the Query/MissCounter RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDR_FIELD_NUMBER: builtins.int
     validator_addr: builtins.str
     """validator defines the validator address to query for."""
     def __init__(
@@ -242,17 +230,15 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["miss_counter", b"miss_counter"]) -> None: ...
 
 global___QueryMissCounterResponse = QueryMissCounterResponse
 
 @typing_extensions.final
 class QueryAggregatePrevoteRequest(google.protobuf.message.Message):
-    """QueryAggregatePrevoteRequest is the request type for the
-    Query/AggregatePrevote RPC method.
-    """
+    """QueryAggregatePrevoteRequest is the request type for the Query/AggregatePrevote RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDR_FIELD_NUMBER: builtins.int
     validator_addr: builtins.str
     """validator defines the validator address to query for."""
     def __init__(
@@ -270,33 +256,29 @@
     Query/AggregatePrevote RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AGGREGATE_PREVOTE_FIELD_NUMBER: builtins.int
     @property
-    def aggregate_prevote(self) -> oracle.v1.oracle_pb2.AggregateExchangeRatePrevote:
-        """aggregate_prevote defines oracle aggregate prevote submitted by a validator
-        in the current vote period
-        """
+    def aggregate_prevote(self) -> oracle.v1beta1.oracle_pb2.AggregateExchangeRatePrevote:
+        """aggregate_prevote defines oracle aggregate prevote submitted by a validator in the current vote period"""
     def __init__(
         self,
         *,
-        aggregate_prevote: oracle.v1.oracle_pb2.AggregateExchangeRatePrevote | None = ...,
+        aggregate_prevote: oracle.v1beta1.oracle_pb2.AggregateExchangeRatePrevote | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["aggregate_prevote", b"aggregate_prevote"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["aggregate_prevote", b"aggregate_prevote"]) -> None: ...
 
 global___QueryAggregatePrevoteResponse = QueryAggregatePrevoteResponse
 
 @typing_extensions.final
 class QueryAggregatePrevotesRequest(google.protobuf.message.Message):
-    """QueryAggregatePrevotesRequest is the request type for the
-    Query/AggregatePrevotes RPC method.
-    """
+    """QueryAggregatePrevotesRequest is the request type for the Query/AggregatePrevotes RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
@@ -308,32 +290,28 @@
     Query/AggregatePrevotes RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AGGREGATE_PREVOTES_FIELD_NUMBER: builtins.int
     @property
-    def aggregate_prevotes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1.oracle_pb2.AggregateExchangeRatePrevote]:
-        """aggregate_prevotes defines all oracle aggregate prevotes submitted in the
-        current vote period
-        """
+    def aggregate_prevotes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1beta1.oracle_pb2.AggregateExchangeRatePrevote]:
+        """aggregate_prevotes defines all oracle aggregate prevotes submitted in the current vote period"""
     def __init__(
         self,
         *,
-        aggregate_prevotes: collections.abc.Iterable[oracle.v1.oracle_pb2.AggregateExchangeRatePrevote] | None = ...,
+        aggregate_prevotes: collections.abc.Iterable[oracle.v1beta1.oracle_pb2.AggregateExchangeRatePrevote] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["aggregate_prevotes", b"aggregate_prevotes"]) -> None: ...
 
 global___QueryAggregatePrevotesResponse = QueryAggregatePrevotesResponse
 
 @typing_extensions.final
 class QueryAggregateVoteRequest(google.protobuf.message.Message):
-    """QueryAggregateVoteRequest is the request type for the Query/AggregateVote RPC
-    method.
-    """
+    """QueryAggregateVoteRequest is the request type for the Query/AggregateVote RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDR_FIELD_NUMBER: builtins.int
     validator_addr: builtins.str
     """validator defines the validator address to query for."""
     def __init__(
@@ -351,33 +329,29 @@
     Query/AggregateVote RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AGGREGATE_VOTE_FIELD_NUMBER: builtins.int
     @property
-    def aggregate_vote(self) -> oracle.v1.oracle_pb2.AggregateExchangeRateVote:
-        """aggregate_vote defines oracle aggregate vote submitted by a validator in
-        the current vote period
-        """
+    def aggregate_vote(self) -> oracle.v1beta1.oracle_pb2.AggregateExchangeRateVote:
+        """aggregate_vote defines oracle aggregate vote submitted by a validator in the current vote period"""
     def __init__(
         self,
         *,
-        aggregate_vote: oracle.v1.oracle_pb2.AggregateExchangeRateVote | None = ...,
+        aggregate_vote: oracle.v1beta1.oracle_pb2.AggregateExchangeRateVote | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["aggregate_vote", b"aggregate_vote"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["aggregate_vote", b"aggregate_vote"]) -> None: ...
 
 global___QueryAggregateVoteResponse = QueryAggregateVoteResponse
 
 @typing_extensions.final
 class QueryAggregateVotesRequest(google.protobuf.message.Message):
-    """QueryAggregateVotesRequest is the request type for the Query/AggregateVotes
-    RPC method.
-    """
+    """QueryAggregateVotesRequest is the request type for the Query/AggregateVotes RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
@@ -389,22 +363,20 @@
     Query/AggregateVotes RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AGGREGATE_VOTES_FIELD_NUMBER: builtins.int
     @property
-    def aggregate_votes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1.oracle_pb2.AggregateExchangeRateVote]:
-        """aggregate_votes defines all oracle aggregate votes submitted in the current
-        vote period
-        """
+    def aggregate_votes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[oracle.v1beta1.oracle_pb2.AggregateExchangeRateVote]:
+        """aggregate_votes defines all oracle aggregate votes submitted in the current vote period"""
     def __init__(
         self,
         *,
-        aggregate_votes: collections.abc.Iterable[oracle.v1.oracle_pb2.AggregateExchangeRateVote] | None = ...,
+        aggregate_votes: collections.abc.Iterable[oracle.v1beta1.oracle_pb2.AggregateExchangeRateVote] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["aggregate_votes", b"aggregate_votes"]) -> None: ...
 
 global___QueryAggregateVotesResponse = QueryAggregateVotesResponse
 
 @typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
@@ -422,18 +394,18 @@
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is the response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
-    def params(self) -> oracle.v1.oracle_pb2.Params:
+    def params(self) -> oracle.v1beta1.oracle_pb2.Params:
         """params defines the parameters of the module."""
     def __init__(
         self,
         *,
-        params: oracle.v1.oracle_pb2.Params | None = ...,
+        params: oracle.v1beta1.oracle_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/query_pb2_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from oracle.v1 import query_pb2 as oracle_dot_v1_dot_query__pb2
+from oracle.v1beta1 import query_pb2 as oracle_dot_v1beta1_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.ExchangeRate = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/ExchangeRate',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRateRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRateResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/ExchangeRate',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateResponse.FromString,
                 )
         self.ExchangeRateTwap = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/ExchangeRateTwap',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRateRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRateResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/ExchangeRateTwap',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateResponse.FromString,
                 )
         self.ExchangeRates = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/ExchangeRates',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRatesRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRatesResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/ExchangeRates',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRatesRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRatesResponse.FromString,
                 )
         self.Actives = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/Actives',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryActivesRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryActivesResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/Actives',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryActivesRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryActivesResponse.FromString,
                 )
         self.VoteTargets = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/VoteTargets',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryVoteTargetsRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryVoteTargetsResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/VoteTargets',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryVoteTargetsRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryVoteTargetsResponse.FromString,
                 )
         self.FeederDelegation = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/FeederDelegation',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryFeederDelegationRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryFeederDelegationResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/FeederDelegation',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryFeederDelegationRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryFeederDelegationResponse.FromString,
                 )
         self.MissCounter = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/MissCounter',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryMissCounterRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryMissCounterResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/MissCounter',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryMissCounterRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryMissCounterResponse.FromString,
                 )
         self.AggregatePrevote = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/AggregatePrevote',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryAggregatePrevoteRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryAggregatePrevoteResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/AggregatePrevote',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevoteRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevoteResponse.FromString,
                 )
         self.AggregatePrevotes = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/AggregatePrevotes',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryAggregatePrevotesRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryAggregatePrevotesResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/AggregatePrevotes',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevotesRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevotesResponse.FromString,
                 )
         self.AggregateVote = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/AggregateVote',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryAggregateVoteRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryAggregateVoteResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/AggregateVote',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVoteRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVoteResponse.FromString,
                 )
         self.AggregateVotes = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/AggregateVotes',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryAggregateVotesRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryAggregateVotesResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/AggregateVotes',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVotesRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVotesResponse.FromString,
                 )
         self.Params = channel.unary_unary(
-                '/nibiru.oracle.v1.Query/Params',
-                request_serializer=oracle_dot_v1_dot_query__pb2.QueryParamsRequest.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_query__pb2.QueryParamsResponse.FromString,
+                '/nibiru.oracle.v1beta1.Query/Params',
+                request_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryParamsRequest.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryParamsResponse.FromString,
                 )
 
 
 class QueryServicer(object):
     """Query defines the gRPC querier service.
     """
 
@@ -166,75 +166,75 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_QueryServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ExchangeRate': grpc.unary_unary_rpc_method_handler(
                     servicer.ExchangeRate,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRateRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRateResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateResponse.SerializeToString,
             ),
             'ExchangeRateTwap': grpc.unary_unary_rpc_method_handler(
                     servicer.ExchangeRateTwap,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRateRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRateResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateResponse.SerializeToString,
             ),
             'ExchangeRates': grpc.unary_unary_rpc_method_handler(
                     servicer.ExchangeRates,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRatesRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryExchangeRatesResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRatesRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRatesResponse.SerializeToString,
             ),
             'Actives': grpc.unary_unary_rpc_method_handler(
                     servicer.Actives,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryActivesRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryActivesResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryActivesRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryActivesResponse.SerializeToString,
             ),
             'VoteTargets': grpc.unary_unary_rpc_method_handler(
                     servicer.VoteTargets,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryVoteTargetsRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryVoteTargetsResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryVoteTargetsRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryVoteTargetsResponse.SerializeToString,
             ),
             'FeederDelegation': grpc.unary_unary_rpc_method_handler(
                     servicer.FeederDelegation,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryFeederDelegationRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryFeederDelegationResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryFeederDelegationRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryFeederDelegationResponse.SerializeToString,
             ),
             'MissCounter': grpc.unary_unary_rpc_method_handler(
                     servicer.MissCounter,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryMissCounterRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryMissCounterResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryMissCounterRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryMissCounterResponse.SerializeToString,
             ),
             'AggregatePrevote': grpc.unary_unary_rpc_method_handler(
                     servicer.AggregatePrevote,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryAggregatePrevoteRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryAggregatePrevoteResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevoteRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevoteResponse.SerializeToString,
             ),
             'AggregatePrevotes': grpc.unary_unary_rpc_method_handler(
                     servicer.AggregatePrevotes,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryAggregatePrevotesRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryAggregatePrevotesResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevotesRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevotesResponse.SerializeToString,
             ),
             'AggregateVote': grpc.unary_unary_rpc_method_handler(
                     servicer.AggregateVote,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryAggregateVoteRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryAggregateVoteResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVoteRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVoteResponse.SerializeToString,
             ),
             'AggregateVotes': grpc.unary_unary_rpc_method_handler(
                     servicer.AggregateVotes,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryAggregateVotesRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryAggregateVotesResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVotesRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVotesResponse.SerializeToString,
             ),
             'Params': grpc.unary_unary_rpc_method_handler(
                     servicer.Params,
-                    request_deserializer=oracle_dot_v1_dot_query__pb2.QueryParamsRequest.FromString,
-                    response_serializer=oracle_dot_v1_dot_query__pb2.QueryParamsResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_query__pb2.QueryParamsRequest.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_query__pb2.QueryParamsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'nibiru.oracle.v1.Query', rpc_method_handlers)
+            'nibiru.oracle.v1beta1.Query', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Query(object):
     """Query defines the gRPC querier service.
     """
@@ -246,199 +246,199 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/ExchangeRate',
-            oracle_dot_v1_dot_query__pb2.QueryExchangeRateRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryExchangeRateResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/ExchangeRate',
+            oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ExchangeRateTwap(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/ExchangeRateTwap',
-            oracle_dot_v1_dot_query__pb2.QueryExchangeRateRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryExchangeRateResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/ExchangeRateTwap',
+            oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ExchangeRates(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/ExchangeRates',
-            oracle_dot_v1_dot_query__pb2.QueryExchangeRatesRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryExchangeRatesResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/ExchangeRates',
+            oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRatesRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryExchangeRatesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Actives(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/Actives',
-            oracle_dot_v1_dot_query__pb2.QueryActivesRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryActivesResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/Actives',
+            oracle_dot_v1beta1_dot_query__pb2.QueryActivesRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryActivesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def VoteTargets(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/VoteTargets',
-            oracle_dot_v1_dot_query__pb2.QueryVoteTargetsRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryVoteTargetsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/VoteTargets',
+            oracle_dot_v1beta1_dot_query__pb2.QueryVoteTargetsRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryVoteTargetsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def FeederDelegation(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/FeederDelegation',
-            oracle_dot_v1_dot_query__pb2.QueryFeederDelegationRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryFeederDelegationResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/FeederDelegation',
+            oracle_dot_v1beta1_dot_query__pb2.QueryFeederDelegationRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryFeederDelegationResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def MissCounter(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/MissCounter',
-            oracle_dot_v1_dot_query__pb2.QueryMissCounterRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryMissCounterResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/MissCounter',
+            oracle_dot_v1beta1_dot_query__pb2.QueryMissCounterRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryMissCounterResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def AggregatePrevote(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/AggregatePrevote',
-            oracle_dot_v1_dot_query__pb2.QueryAggregatePrevoteRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryAggregatePrevoteResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/AggregatePrevote',
+            oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevoteRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevoteResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def AggregatePrevotes(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/AggregatePrevotes',
-            oracle_dot_v1_dot_query__pb2.QueryAggregatePrevotesRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryAggregatePrevotesResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/AggregatePrevotes',
+            oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevotesRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryAggregatePrevotesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def AggregateVote(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/AggregateVote',
-            oracle_dot_v1_dot_query__pb2.QueryAggregateVoteRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryAggregateVoteResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/AggregateVote',
+            oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVoteRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVoteResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def AggregateVotes(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/AggregateVotes',
-            oracle_dot_v1_dot_query__pb2.QueryAggregateVotesRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryAggregateVotesResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/AggregateVotes',
+            oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVotesRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryAggregateVotesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Params(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Query/Params',
-            oracle_dot_v1_dot_query__pb2.QueryParamsRequest.SerializeToString,
-            oracle_dot_v1_dot_query__pb2.QueryParamsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Query/Params',
+            oracle_dot_v1beta1_dot_query__pb2.QueryParamsRequest.SerializeToString,
+            oracle_dot_v1beta1_dot_query__pb2.QueryParamsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/query_pb2_grpc.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,162 +1,162 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import grpc
-import oracle.v1.query_pb2
+import oracle.v1beta1.query_pb2
 
 class QueryStub:
     """Query defines the gRPC querier service."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
     ExchangeRate: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryExchangeRateRequest,
-        oracle.v1.query_pb2.QueryExchangeRateResponse,
+        oracle.v1beta1.query_pb2.QueryExchangeRateRequest,
+        oracle.v1beta1.query_pb2.QueryExchangeRateResponse,
     ]
     """ExchangeRate returns exchange rate of a pair"""
     ExchangeRateTwap: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryExchangeRateRequest,
-        oracle.v1.query_pb2.QueryExchangeRateResponse,
+        oracle.v1beta1.query_pb2.QueryExchangeRateRequest,
+        oracle.v1beta1.query_pb2.QueryExchangeRateResponse,
     ]
     """ExchangeRateTwap returns twap exchange rate of a pair"""
     ExchangeRates: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryExchangeRatesRequest,
-        oracle.v1.query_pb2.QueryExchangeRatesResponse,
+        oracle.v1beta1.query_pb2.QueryExchangeRatesRequest,
+        oracle.v1beta1.query_pb2.QueryExchangeRatesResponse,
     ]
     """ExchangeRates returns exchange rates of all pairs"""
     Actives: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryActivesRequest,
-        oracle.v1.query_pb2.QueryActivesResponse,
+        oracle.v1beta1.query_pb2.QueryActivesRequest,
+        oracle.v1beta1.query_pb2.QueryActivesResponse,
     ]
     """Actives returns all active pairs"""
     VoteTargets: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryVoteTargetsRequest,
-        oracle.v1.query_pb2.QueryVoteTargetsResponse,
+        oracle.v1beta1.query_pb2.QueryVoteTargetsRequest,
+        oracle.v1beta1.query_pb2.QueryVoteTargetsResponse,
     ]
     """VoteTargets returns all vote target for pairs"""
     FeederDelegation: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryFeederDelegationRequest,
-        oracle.v1.query_pb2.QueryFeederDelegationResponse,
+        oracle.v1beta1.query_pb2.QueryFeederDelegationRequest,
+        oracle.v1beta1.query_pb2.QueryFeederDelegationResponse,
     ]
     """FeederDelegation returns feeder delegation of a validator"""
     MissCounter: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryMissCounterRequest,
-        oracle.v1.query_pb2.QueryMissCounterResponse,
+        oracle.v1beta1.query_pb2.QueryMissCounterRequest,
+        oracle.v1beta1.query_pb2.QueryMissCounterResponse,
     ]
     """MissCounter returns oracle miss counter of a validator"""
     AggregatePrevote: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryAggregatePrevoteRequest,
-        oracle.v1.query_pb2.QueryAggregatePrevoteResponse,
+        oracle.v1beta1.query_pb2.QueryAggregatePrevoteRequest,
+        oracle.v1beta1.query_pb2.QueryAggregatePrevoteResponse,
     ]
     """AggregatePrevote returns an aggregate prevote of a validator"""
     AggregatePrevotes: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryAggregatePrevotesRequest,
-        oracle.v1.query_pb2.QueryAggregatePrevotesResponse,
+        oracle.v1beta1.query_pb2.QueryAggregatePrevotesRequest,
+        oracle.v1beta1.query_pb2.QueryAggregatePrevotesResponse,
     ]
     """AggregatePrevotes returns aggregate prevotes of all validators"""
     AggregateVote: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryAggregateVoteRequest,
-        oracle.v1.query_pb2.QueryAggregateVoteResponse,
+        oracle.v1beta1.query_pb2.QueryAggregateVoteRequest,
+        oracle.v1beta1.query_pb2.QueryAggregateVoteResponse,
     ]
     """AggregateVote returns an aggregate vote of a validator"""
     AggregateVotes: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryAggregateVotesRequest,
-        oracle.v1.query_pb2.QueryAggregateVotesResponse,
+        oracle.v1beta1.query_pb2.QueryAggregateVotesRequest,
+        oracle.v1beta1.query_pb2.QueryAggregateVotesResponse,
     ]
     """AggregateVotes returns aggregate votes of all validators"""
     Params: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.query_pb2.QueryParamsRequest,
-        oracle.v1.query_pb2.QueryParamsResponse,
+        oracle.v1beta1.query_pb2.QueryParamsRequest,
+        oracle.v1beta1.query_pb2.QueryParamsResponse,
     ]
     """Params queries all parameters."""
 
 class QueryServicer(metaclass=abc.ABCMeta):
     """Query defines the gRPC querier service."""
 
     @abc.abstractmethod
     def ExchangeRate(
         self,
-        request: oracle.v1.query_pb2.QueryExchangeRateRequest,
+        request: oracle.v1beta1.query_pb2.QueryExchangeRateRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryExchangeRateResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryExchangeRateResponse:
         """ExchangeRate returns exchange rate of a pair"""
     @abc.abstractmethod
     def ExchangeRateTwap(
         self,
-        request: oracle.v1.query_pb2.QueryExchangeRateRequest,
+        request: oracle.v1beta1.query_pb2.QueryExchangeRateRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryExchangeRateResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryExchangeRateResponse:
         """ExchangeRateTwap returns twap exchange rate of a pair"""
     @abc.abstractmethod
     def ExchangeRates(
         self,
-        request: oracle.v1.query_pb2.QueryExchangeRatesRequest,
+        request: oracle.v1beta1.query_pb2.QueryExchangeRatesRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryExchangeRatesResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryExchangeRatesResponse:
         """ExchangeRates returns exchange rates of all pairs"""
     @abc.abstractmethod
     def Actives(
         self,
-        request: oracle.v1.query_pb2.QueryActivesRequest,
+        request: oracle.v1beta1.query_pb2.QueryActivesRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryActivesResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryActivesResponse:
         """Actives returns all active pairs"""
     @abc.abstractmethod
     def VoteTargets(
         self,
-        request: oracle.v1.query_pb2.QueryVoteTargetsRequest,
+        request: oracle.v1beta1.query_pb2.QueryVoteTargetsRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryVoteTargetsResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryVoteTargetsResponse:
         """VoteTargets returns all vote target for pairs"""
     @abc.abstractmethod
     def FeederDelegation(
         self,
-        request: oracle.v1.query_pb2.QueryFeederDelegationRequest,
+        request: oracle.v1beta1.query_pb2.QueryFeederDelegationRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryFeederDelegationResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryFeederDelegationResponse:
         """FeederDelegation returns feeder delegation of a validator"""
     @abc.abstractmethod
     def MissCounter(
         self,
-        request: oracle.v1.query_pb2.QueryMissCounterRequest,
+        request: oracle.v1beta1.query_pb2.QueryMissCounterRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryMissCounterResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryMissCounterResponse:
         """MissCounter returns oracle miss counter of a validator"""
     @abc.abstractmethod
     def AggregatePrevote(
         self,
-        request: oracle.v1.query_pb2.QueryAggregatePrevoteRequest,
+        request: oracle.v1beta1.query_pb2.QueryAggregatePrevoteRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryAggregatePrevoteResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryAggregatePrevoteResponse:
         """AggregatePrevote returns an aggregate prevote of a validator"""
     @abc.abstractmethod
     def AggregatePrevotes(
         self,
-        request: oracle.v1.query_pb2.QueryAggregatePrevotesRequest,
+        request: oracle.v1beta1.query_pb2.QueryAggregatePrevotesRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryAggregatePrevotesResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryAggregatePrevotesResponse:
         """AggregatePrevotes returns aggregate prevotes of all validators"""
     @abc.abstractmethod
     def AggregateVote(
         self,
-        request: oracle.v1.query_pb2.QueryAggregateVoteRequest,
+        request: oracle.v1beta1.query_pb2.QueryAggregateVoteRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryAggregateVoteResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryAggregateVoteResponse:
         """AggregateVote returns an aggregate vote of a validator"""
     @abc.abstractmethod
     def AggregateVotes(
         self,
-        request: oracle.v1.query_pb2.QueryAggregateVotesRequest,
+        request: oracle.v1beta1.query_pb2.QueryAggregateVotesRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryAggregateVotesResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryAggregateVotesResponse:
         """AggregateVotes returns aggregate votes of all validators"""
     @abc.abstractmethod
     def Params(
         self,
-        request: oracle.v1.query_pb2.QueryParamsRequest,
+        request: oracle.v1beta1.query_pb2.QueryParamsRequest,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.query_pb2.QueryParamsResponse:
+    ) -> oracle.v1beta1.query_pb2.QueryParamsResponse:
         """Params queries all parameters."""
 
 def add_QueryServicer_to_server(servicer: QueryServicer, server: grpc.Server) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/state_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/state_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: oracle/v1/state.proto
+# source: oracle/v1beta1/state.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from oracle.v1 import oracle_pb2 as oracle_dot_v1_dot_oracle__pb2
+from oracle.v1beta1 import oracle_pb2 as oracle_dot_v1beta1_dot_oracle__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15oracle/v1/state.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x16oracle/v1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\xbc\x01\n\rPriceSnapshot\x12V\n\x04pair\x18\x01 \x01(\tBH\xf2\xde\x1f\x0byaml:\"pair\"\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12=\n\x05price\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0ctimestamp_ms\x18\x03 \x01(\x03\x42.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aoracle/v1beta1/state.proto\x12\x15nibiru.oracle.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1boracle/v1beta1/oracle.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\xbc\x01\n\rPriceSnapshot\x12V\n\x04pair\x18\x01 \x01(\tBH\xf2\xde\x1f\x0byaml:\"pair\"\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12=\n\x05price\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0ctimestamp_ms\x18\x03 \x01(\x03\x42.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1.state_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1beta1.state_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/oracle/types'
   _PRICESNAPSHOT.fields_by_name['pair']._options = None
   _PRICESNAPSHOT.fields_by_name['pair']._serialized_options = b'\362\336\037\013yaml:\"pair\"\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
   _PRICESNAPSHOT.fields_by_name['price']._options = None
   _PRICESNAPSHOT.fields_by_name['price']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _PRICESNAPSHOT._serialized_start=152
-  _PRICESNAPSHOT._serialized_end=340
+  _PRICESNAPSHOT._serialized_start=167
+  _PRICESNAPSHOT._serialized_end=355
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/state_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/tx_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: oracle/v1/tx.proto
+# source: oracle/v1beta1/tx.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12oracle/v1/tx.proto\x12\x10nibiru.oracle.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"\x96\x01\n\x1fMsgAggregateExchangeRatePrevote\x12\x1d\n\x04hash\x18\x01 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"hash\"\x12!\n\x06\x66\x65\x65\x64\x65r\x18\x02 \x01(\tB\x11\xf2\xde\x1f\ryaml:\"feeder\"\x12\'\n\tvalidator\x18\x03 \x01(\tB\x14\xf2\xde\x1f\x10yaml:\"validator\":\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\")\n\'MsgAggregateExchangeRatePrevoteResponse\"\xc6\x01\n\x1cMsgAggregateExchangeRateVote\x12\x1d\n\x04salt\x18\x01 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"salt\"\x12\x31\n\x0e\x65xchange_rates\x18\x02 \x01(\tB\x19\xf2\xde\x1f\x15yaml:\"exchange_rates\"\x12!\n\x06\x66\x65\x65\x64\x65r\x18\x03 \x01(\tB\x11\xf2\xde\x1f\ryaml:\"feeder\"\x12\'\n\tvalidator\x18\x04 \x01(\tB\x14\xf2\xde\x1f\x10yaml:\"validator\":\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"&\n$MsgAggregateExchangeRateVoteResponse\"p\n\x16MsgDelegateFeedConsent\x12%\n\x08operator\x18\x01 \x01(\tB\x13\xf2\xde\x1f\x0fyaml:\"operator\"\x12%\n\x08\x64\x65legate\x18\x02 \x01(\tB\x13\xf2\xde\x1f\x0fyaml:\"delegate\":\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\" \n\x1eMsgDelegateFeedConsentResponse2\xf3\x03\n\x03Msg\x12\xac\x01\n\x1c\x41ggregateExchangeRatePrevote\x12\x31.nibiru.oracle.v1.MsgAggregateExchangeRatePrevote\x1a\x39.nibiru.oracle.v1.MsgAggregateExchangeRatePrevoteResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x16/nibiru/oracle/prevote\x12\xa0\x01\n\x19\x41ggregateExchangeRateVote\x12..nibiru.oracle.v1.MsgAggregateExchangeRateVote\x1a\x36.nibiru.oracle.v1.MsgAggregateExchangeRateVoteResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\"\x13/nibiru/oracle/vote\x12\x99\x01\n\x13\x44\x65legateFeedConsent\x12(.nibiru.oracle.v1.MsgDelegateFeedConsent\x1a\x30.nibiru.oracle.v1.MsgDelegateFeedConsentResponse\"&\x82\xd3\xe4\x93\x02 \"\x1e/nibiru/oracle/feeder-delegateB.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17oracle/v1beta1/tx.proto\x12\x15nibiru.oracle.v1beta1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"\x96\x01\n\x1fMsgAggregateExchangeRatePrevote\x12\x1d\n\x04hash\x18\x01 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"hash\"\x12!\n\x06\x66\x65\x65\x64\x65r\x18\x02 \x01(\tB\x11\xf2\xde\x1f\ryaml:\"feeder\"\x12\'\n\tvalidator\x18\x03 \x01(\tB\x14\xf2\xde\x1f\x10yaml:\"validator\":\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\")\n\'MsgAggregateExchangeRatePrevoteResponse\"\xc6\x01\n\x1cMsgAggregateExchangeRateVote\x12\x1d\n\x04salt\x18\x01 \x01(\tB\x0f\xf2\xde\x1f\x0byaml:\"salt\"\x12\x31\n\x0e\x65xchange_rates\x18\x02 \x01(\tB\x19\xf2\xde\x1f\x15yaml:\"exchange_rates\"\x12!\n\x06\x66\x65\x65\x64\x65r\x18\x03 \x01(\tB\x11\xf2\xde\x1f\ryaml:\"feeder\"\x12\'\n\tvalidator\x18\x04 \x01(\tB\x14\xf2\xde\x1f\x10yaml:\"validator\":\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\"&\n$MsgAggregateExchangeRateVoteResponse\"p\n\x16MsgDelegateFeedConsent\x12%\n\x08operator\x18\x01 \x01(\tB\x13\xf2\xde\x1f\x0fyaml:\"operator\"\x12%\n\x08\x64\x65legate\x18\x02 \x01(\tB\x13\xf2\xde\x1f\x0fyaml:\"delegate\":\x08\xe8\xa0\x1f\x00\x88\xa0\x1f\x00\" \n\x1eMsgDelegateFeedConsentResponse2\x91\x04\n\x03Msg\x12\xb6\x01\n\x1c\x41ggregateExchangeRatePrevote\x12\x36.nibiru.oracle.v1beta1.MsgAggregateExchangeRatePrevote\x1a>.nibiru.oracle.v1beta1.MsgAggregateExchangeRatePrevoteResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x16/nibiru/oracle/prevote\x12\xaa\x01\n\x19\x41ggregateExchangeRateVote\x12\x33.nibiru.oracle.v1beta1.MsgAggregateExchangeRateVote\x1a;.nibiru.oracle.v1beta1.MsgAggregateExchangeRateVoteResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\"\x13/nibiru/oracle/vote\x12\xa3\x01\n\x13\x44\x65legateFeedConsent\x12-.nibiru.oracle.v1beta1.MsgDelegateFeedConsent\x1a\x35.nibiru.oracle.v1beta1.MsgDelegateFeedConsentResponse\"&\x82\xd3\xe4\x93\x02 \"\x1e/nibiru/oracle/feeder-delegateB.Z,github.com/NibiruChain/nibiru/x/oracle/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1.tx_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'oracle.v1beta1.tx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/NibiruChain/nibiru/x/oracle/types'
   _MSGAGGREGATEEXCHANGERATEPREVOTE.fields_by_name['hash']._options = None
   _MSGAGGREGATEEXCHANGERATEPREVOTE.fields_by_name['hash']._serialized_options = b'\362\336\037\013yaml:\"hash\"'
   _MSGAGGREGATEEXCHANGERATEPREVOTE.fields_by_name['feeder']._options = None
@@ -49,22 +49,22 @@
   _MSGDELEGATEFEEDCONSENT._serialized_options = b'\350\240\037\000\210\240\037\000'
   _MSG.methods_by_name['AggregateExchangeRatePrevote']._options = None
   _MSG.methods_by_name['AggregateExchangeRatePrevote']._serialized_options = b'\202\323\344\223\002\030\"\026/nibiru/oracle/prevote'
   _MSG.methods_by_name['AggregateExchangeRateVote']._options = None
   _MSG.methods_by_name['AggregateExchangeRateVote']._serialized_options = b'\202\323\344\223\002\025\"\023/nibiru/oracle/vote'
   _MSG.methods_by_name['DelegateFeedConsent']._options = None
   _MSG.methods_by_name['DelegateFeedConsent']._serialized_options = b'\202\323\344\223\002 \"\036/nibiru/oracle/feeder-delegate'
-  _MSGAGGREGATEEXCHANGERATEPREVOTE._serialized_start=93
-  _MSGAGGREGATEEXCHANGERATEPREVOTE._serialized_end=243
-  _MSGAGGREGATEEXCHANGERATEPREVOTERESPONSE._serialized_start=245
-  _MSGAGGREGATEEXCHANGERATEPREVOTERESPONSE._serialized_end=286
-  _MSGAGGREGATEEXCHANGERATEVOTE._serialized_start=289
-  _MSGAGGREGATEEXCHANGERATEVOTE._serialized_end=487
-  _MSGAGGREGATEEXCHANGERATEVOTERESPONSE._serialized_start=489
-  _MSGAGGREGATEEXCHANGERATEVOTERESPONSE._serialized_end=527
-  _MSGDELEGATEFEEDCONSENT._serialized_start=529
-  _MSGDELEGATEFEEDCONSENT._serialized_end=641
-  _MSGDELEGATEFEEDCONSENTRESPONSE._serialized_start=643
-  _MSGDELEGATEFEEDCONSENTRESPONSE._serialized_end=675
-  _MSG._serialized_start=678
-  _MSG._serialized_end=1177
+  _MSGAGGREGATEEXCHANGERATEPREVOTE._serialized_start=103
+  _MSGAGGREGATEEXCHANGERATEPREVOTE._serialized_end=253
+  _MSGAGGREGATEEXCHANGERATEPREVOTERESPONSE._serialized_start=255
+  _MSGAGGREGATEEXCHANGERATEPREVOTERESPONSE._serialized_end=296
+  _MSGAGGREGATEEXCHANGERATEVOTE._serialized_start=299
+  _MSGAGGREGATEEXCHANGERATEVOTE._serialized_end=497
+  _MSGAGGREGATEEXCHANGERATEVOTERESPONSE._serialized_start=499
+  _MSGAGGREGATEEXCHANGERATEVOTERESPONSE._serialized_end=537
+  _MSGDELEGATEFEEDCONSENT._serialized_start=539
+  _MSGDELEGATEFEEDCONSENT._serialized_end=651
+  _MSGDELEGATEFEEDCONSENTRESPONSE._serialized_start=653
+  _MSGDELEGATEFEEDCONSENTRESPONSE._serialized_end=685
+  _MSG._serialized_start=688
+  _MSG._serialized_end=1217
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/tx_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HASH_FIELD_NUMBER: builtins.int
     FEEDER_FIELD_NUMBER: builtins.int
     VALIDATOR_FIELD_NUMBER: builtins.int
     hash: builtins.str
     feeder: builtins.str
-    """Feeder is the Bech32 address of the price feeder. A validator may
-    specify multiple price feeders by delegating them consent. The validator
+    """Feeder is the Bech32 address of the price feeder. A validator may 
+    specify multiple price feeders by delegating them consent. The validator  
     address is also a valid feeder by default.
     """
     validator: builtins.str
     """Validator is the Bech32 address to which the prevote will be credited."""
     def __init__(
         self,
         *,
@@ -42,17 +42,15 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["feeder", b"feeder", "hash", b"hash", "validator", b"validator"]) -> None: ...
 
 global___MsgAggregateExchangeRatePrevote = MsgAggregateExchangeRatePrevote
 
 @typing_extensions.final
 class MsgAggregateExchangeRatePrevoteResponse(google.protobuf.message.Message):
-    """MsgAggregateExchangeRatePrevoteResponse defines the
-    Msg/AggregateExchangeRatePrevote response type.
-    """
+    """MsgAggregateExchangeRatePrevoteResponse defines the Msg/AggregateExchangeRatePrevote response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
@@ -69,16 +67,16 @@
     SALT_FIELD_NUMBER: builtins.int
     EXCHANGE_RATES_FIELD_NUMBER: builtins.int
     FEEDER_FIELD_NUMBER: builtins.int
     VALIDATOR_FIELD_NUMBER: builtins.int
     salt: builtins.str
     exchange_rates: builtins.str
     feeder: builtins.str
-    """Feeder is the Bech32 address of the price feeder. A validator may
-    specify multiple price feeders by delegating them consent. The validator
+    """Feeder is the Bech32 address of the price feeder. A validator may 
+    specify multiple price feeders by delegating them consent. The validator  
     address is also a valid feeder by default.
     """
     validator: builtins.str
     """Validator is the Bech32 address to which the vote will be credited."""
     def __init__(
         self,
         *,
@@ -89,29 +87,27 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["exchange_rates", b"exchange_rates", "feeder", b"feeder", "salt", b"salt", "validator", b"validator"]) -> None: ...
 
 global___MsgAggregateExchangeRateVote = MsgAggregateExchangeRateVote
 
 @typing_extensions.final
 class MsgAggregateExchangeRateVoteResponse(google.protobuf.message.Message):
-    """MsgAggregateExchangeRateVoteResponse defines the
-    Msg/AggregateExchangeRateVote response type.
-    """
+    """MsgAggregateExchangeRateVoteResponse defines the Msg/AggregateExchangeRateVote response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgAggregateExchangeRateVoteResponse = MsgAggregateExchangeRateVoteResponse
 
 @typing_extensions.final
 class MsgDelegateFeedConsent(google.protobuf.message.Message):
-    """MsgDelegateFeedConsent represents a message to delegate oracle voting rights
+    """MsgDelegateFeedConsent represents a message to delegate oracle voting rights 
     to another address.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OPERATOR_FIELD_NUMBER: builtins.int
     DELEGATE_FIELD_NUMBER: builtins.int
@@ -125,17 +121,15 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegate", b"delegate", "operator", b"operator"]) -> None: ...
 
 global___MsgDelegateFeedConsent = MsgDelegateFeedConsent
 
 @typing_extensions.final
 class MsgDelegateFeedConsentResponse(google.protobuf.message.Message):
-    """MsgDelegateFeedConsentResponse defines the Msg/DelegateFeedConsent response
-    type.
-    """
+    """MsgDelegateFeedConsentResponse defines the Msg/DelegateFeedConsent response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/tx_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from oracle.v1 import tx_pb2 as oracle_dot_v1_dot_tx__pb2
+from oracle.v1beta1 import tx_pb2 as oracle_dot_v1beta1_dot_tx__pb2
 
 
 class MsgStub(object):
     """Msg defines the oracle Msg service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.AggregateExchangeRatePrevote = channel.unary_unary(
-                '/nibiru.oracle.v1.Msg/AggregateExchangeRatePrevote',
-                request_serializer=oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRatePrevote.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRatePrevoteResponse.FromString,
+                '/nibiru.oracle.v1beta1.Msg/AggregateExchangeRatePrevote',
+                request_serializer=oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRatePrevote.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRatePrevoteResponse.FromString,
                 )
         self.AggregateExchangeRateVote = channel.unary_unary(
-                '/nibiru.oracle.v1.Msg/AggregateExchangeRateVote',
-                request_serializer=oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRateVote.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRateVoteResponse.FromString,
+                '/nibiru.oracle.v1beta1.Msg/AggregateExchangeRateVote',
+                request_serializer=oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRateVote.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRateVoteResponse.FromString,
                 )
         self.DelegateFeedConsent = channel.unary_unary(
-                '/nibiru.oracle.v1.Msg/DelegateFeedConsent',
-                request_serializer=oracle_dot_v1_dot_tx__pb2.MsgDelegateFeedConsent.SerializeToString,
-                response_deserializer=oracle_dot_v1_dot_tx__pb2.MsgDelegateFeedConsentResponse.FromString,
+                '/nibiru.oracle.v1beta1.Msg/DelegateFeedConsent',
+                request_serializer=oracle_dot_v1beta1_dot_tx__pb2.MsgDelegateFeedConsent.SerializeToString,
+                response_deserializer=oracle_dot_v1beta1_dot_tx__pb2.MsgDelegateFeedConsentResponse.FromString,
                 )
 
 
 class MsgServicer(object):
     """Msg defines the oracle Msg service.
     """
 
@@ -49,43 +49,43 @@
         aggregate exchange rate vote
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DelegateFeedConsent(self, request, context):
-        """DelegateFeedConsent defines a method for delegating oracle voting rights
-        to another address known as a price feeder.
+        """DelegateFeedConsent defines a method for delegating oracle voting rights 
+        to another address known as a price feeder. 
         See https://github.com/NibiruChain/pricefeeder.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_MsgServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'AggregateExchangeRatePrevote': grpc.unary_unary_rpc_method_handler(
                     servicer.AggregateExchangeRatePrevote,
-                    request_deserializer=oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRatePrevote.FromString,
-                    response_serializer=oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRatePrevoteResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRatePrevote.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRatePrevoteResponse.SerializeToString,
             ),
             'AggregateExchangeRateVote': grpc.unary_unary_rpc_method_handler(
                     servicer.AggregateExchangeRateVote,
-                    request_deserializer=oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRateVote.FromString,
-                    response_serializer=oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRateVoteResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRateVote.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRateVoteResponse.SerializeToString,
             ),
             'DelegateFeedConsent': grpc.unary_unary_rpc_method_handler(
                     servicer.DelegateFeedConsent,
-                    request_deserializer=oracle_dot_v1_dot_tx__pb2.MsgDelegateFeedConsent.FromString,
-                    response_serializer=oracle_dot_v1_dot_tx__pb2.MsgDelegateFeedConsentResponse.SerializeToString,
+                    request_deserializer=oracle_dot_v1beta1_dot_tx__pb2.MsgDelegateFeedConsent.FromString,
+                    response_serializer=oracle_dot_v1beta1_dot_tx__pb2.MsgDelegateFeedConsentResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'nibiru.oracle.v1.Msg', rpc_method_handlers)
+            'nibiru.oracle.v1beta1.Msg', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Msg(object):
     """Msg defines the oracle Msg service.
     """
@@ -97,46 +97,46 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Msg/AggregateExchangeRatePrevote',
-            oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRatePrevote.SerializeToString,
-            oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRatePrevoteResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Msg/AggregateExchangeRatePrevote',
+            oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRatePrevote.SerializeToString,
+            oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRatePrevoteResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def AggregateExchangeRateVote(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Msg/AggregateExchangeRateVote',
-            oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRateVote.SerializeToString,
-            oracle_dot_v1_dot_tx__pb2.MsgAggregateExchangeRateVoteResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Msg/AggregateExchangeRateVote',
+            oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRateVote.SerializeToString,
+            oracle_dot_v1beta1_dot_tx__pb2.MsgAggregateExchangeRateVoteResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def DelegateFeedConsent(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1.Msg/DelegateFeedConsent',
-            oracle_dot_v1_dot_tx__pb2.MsgDelegateFeedConsent.SerializeToString,
-            oracle_dot_v1_dot_tx__pb2.MsgDelegateFeedConsentResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.oracle.v1beta1.Msg/DelegateFeedConsent',
+            oracle_dot_v1beta1_dot_tx__pb2.MsgDelegateFeedConsent.SerializeToString,
+            oracle_dot_v1beta1_dot_tx__pb2.MsgDelegateFeedConsentResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/oracle/v1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/oracle/v1beta1/tx_pb2_grpc.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import grpc
-import oracle.v1.tx_pb2
+import oracle.v1beta1.tx_pb2
 
 class MsgStub:
     """Msg defines the oracle Msg service."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
     AggregateExchangeRatePrevote: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.tx_pb2.MsgAggregateExchangeRatePrevote,
-        oracle.v1.tx_pb2.MsgAggregateExchangeRatePrevoteResponse,
+        oracle.v1beta1.tx_pb2.MsgAggregateExchangeRatePrevote,
+        oracle.v1beta1.tx_pb2.MsgAggregateExchangeRatePrevoteResponse,
     ]
     """AggregateExchangeRatePrevote defines a method for submitting
     aggregate exchange rate prevote
     """
     AggregateExchangeRateVote: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.tx_pb2.MsgAggregateExchangeRateVote,
-        oracle.v1.tx_pb2.MsgAggregateExchangeRateVoteResponse,
+        oracle.v1beta1.tx_pb2.MsgAggregateExchangeRateVote,
+        oracle.v1beta1.tx_pb2.MsgAggregateExchangeRateVoteResponse,
     ]
     """AggregateExchangeRateVote defines a method for submitting
     aggregate exchange rate vote
     """
     DelegateFeedConsent: grpc.UnaryUnaryMultiCallable[
-        oracle.v1.tx_pb2.MsgDelegateFeedConsent,
-        oracle.v1.tx_pb2.MsgDelegateFeedConsentResponse,
+        oracle.v1beta1.tx_pb2.MsgDelegateFeedConsent,
+        oracle.v1beta1.tx_pb2.MsgDelegateFeedConsentResponse,
     ]
-    """DelegateFeedConsent defines a method for delegating oracle voting rights
-    to another address known as a price feeder.
+    """DelegateFeedConsent defines a method for delegating oracle voting rights 
+    to another address known as a price feeder. 
     See https://github.com/NibiruChain/pricefeeder.
     """
 
 class MsgServicer(metaclass=abc.ABCMeta):
     """Msg defines the oracle Msg service."""
 
     @abc.abstractmethod
     def AggregateExchangeRatePrevote(
         self,
-        request: oracle.v1.tx_pb2.MsgAggregateExchangeRatePrevote,
+        request: oracle.v1beta1.tx_pb2.MsgAggregateExchangeRatePrevote,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.tx_pb2.MsgAggregateExchangeRatePrevoteResponse:
+    ) -> oracle.v1beta1.tx_pb2.MsgAggregateExchangeRatePrevoteResponse:
         """AggregateExchangeRatePrevote defines a method for submitting
         aggregate exchange rate prevote
         """
     @abc.abstractmethod
     def AggregateExchangeRateVote(
         self,
-        request: oracle.v1.tx_pb2.MsgAggregateExchangeRateVote,
+        request: oracle.v1beta1.tx_pb2.MsgAggregateExchangeRateVote,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.tx_pb2.MsgAggregateExchangeRateVoteResponse:
+    ) -> oracle.v1beta1.tx_pb2.MsgAggregateExchangeRateVoteResponse:
         """AggregateExchangeRateVote defines a method for submitting
         aggregate exchange rate vote
         """
     @abc.abstractmethod
     def DelegateFeedConsent(
         self,
-        request: oracle.v1.tx_pb2.MsgDelegateFeedConsent,
+        request: oracle.v1beta1.tx_pb2.MsgDelegateFeedConsent,
         context: grpc.ServicerContext,
-    ) -> oracle.v1.tx_pb2.MsgDelegateFeedConsentResponse:
-        """DelegateFeedConsent defines a method for delegating oracle voting rights
-        to another address known as a price feeder.
+    ) -> oracle.v1beta1.tx_pb2.MsgDelegateFeedConsentResponse:
+        """DelegateFeedConsent defines a method for delegating oracle voting rights 
+        to another address known as a price feeder. 
         See https://github.com/NibiruChain/pricefeeder.
         """
 
 def add_MsgServicer_to_server(servicer: MsgServicer, server: grpc.Server) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/event_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/event_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: perp/v2/event.proto
+# source: perp/v1/event.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
-from perp.v2 import state_pb2 as perp_dot_v2_dot_state__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from perp.v1 import state_pb2 as perp_dot_v1_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13perp/v2/event.proto\x12\x0enibiru.perp.v2\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x13perp/v2/state.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xf0\x06\n\x14PositionChangedEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x16\n\x0etrader_address\x18\x02 \x01(\t\x12@\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x15\xf2\xde\x1f\ryaml:\"margin\"\xc8\xde\x1f\x00\x12I\n\x11position_notional\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x46\n\x0e\x65xchanged_size\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12J\n\x12\x65xchanged_notional\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12R\n\x0ftransaction_fee\x18\x07 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x1e\xf2\xde\x1f\x16yaml:\"transaction_fee\"\xc8\xde\x1f\x00\x12\x45\n\rposition_size\x18\x08 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0crealized_pnl\x18\t \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12L\n\x14unrealized_pnl_after\x18\n \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x31\n\x08\x62\x61\x64_debt\x18\x0b \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12G\n\x0f\x66unding_payment\x18\x0c \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_height\x18\r \x01(\x03\x12\x15\n\rblock_time_ms\x18\x0e \x01(\x03\"\xae\x07\n\x17PositionLiquidatedEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x16\n\x0etrader_address\x18\x02 \x01(\t\x12N\n\x16\x65xchanged_quote_amount\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x65xchanged_position_size\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x1a\n\x12liquidator_address\x18\x05 \x01(\t\x12V\n\x11\x66\x65\x65_to_liquidator\x18\x06 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB \xf2\xde\x1f\x18yaml:\"fee_to_liquidator\"\xc8\xde\x1f\x00\x12^\n\x15\x66\x65\x65_to_ecosystem_fund\x18\x07 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB$\xf2\xde\x1f\x1cyaml:\"fee_to_ecosystem_fund\"\xc8\xde\x1f\x00\x12\x31\n\x08\x62\x61\x64_debt\x18\x08 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12@\n\x06margin\x18\t \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x15\xf2\xde\x1f\ryaml:\"margin\"\xc8\xde\x1f\x00\x12I\n\x11position_notional\x18\n \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x45\n\rposition_size\x18\x0b \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x45\n\runrealizedPnl\x18\x0c \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x42\n\nmark_price\x18\r \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_height\x18\x0e \x01(\x03\x12\x15\n\rblock_time_ms\x18\x0f \x01(\x03\"\xf3\x01\n\x14PositionSettledEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x16\n\x0etrader_address\x18\x02 \x01(\t\x12z\n\rsettled_coins\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinBH\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\xf2\xde\x1f\x14yaml:\"settled_coins\"\xc8\xde\x1f\x00\"\x8b\x04\n\x17\x46undingRateChangedEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x42\n\nmark_price\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x43\n\x0bindex_price\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12K\n\x13latest_funding_rate\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17latest_premium_fraction\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12S\n\x1b\x63umulative_premium_fraction\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_height\x18\x07 \x01(\x03\x12\x15\n\rblock_time_ms\x18\x08 \x01(\x03\"\xc7\x02\n\x16LiquidationFailedEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x0e\n\x06trader\x18\x02 \x01(\t\x12\x12\n\nliquidator\x18\x03 \x01(\t\x12N\n\x06reason\x18\x04 \x01(\x0e\x32>.nibiru.perp.v2.LiquidationFailedEvent.LiquidationFailedReason\"p\n\x17LiquidationFailedReason\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x14\n\x10POSITION_HEALTHY\x10\x01\x12\x14\n\x10NONEXISTENT_PAIR\x10\x02\x12\x18\n\x14NONEXISTENT_POSITION\x10\x03\x42/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13perp/v1/event.proto\x12\x0enibiru.perp.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x13perp/v1/state.proto\"\xb4\x07\n\x14PositionChangedEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x16\n\x0etrader_address\x18\x02 \x01(\t\x12@\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x15\xf2\xde\x1f\ryaml:\"margin\"\xc8\xde\x1f\x00\x12I\n\x11position_notional\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x46\n\x0e\x65xchanged_size\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12J\n\x12\x65xchanged_notional\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12R\n\x0ftransaction_fee\x18\x07 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x1e\xf2\xde\x1f\x16yaml:\"transaction_fee\"\xc8\xde\x1f\x00\x12\x45\n\rposition_size\x18\x08 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0crealized_pnl\x18\t \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12L\n\x14unrealized_pnl_after\x18\n \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x31\n\x08\x62\x61\x64_debt\x18\x0b \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x42\n\nmark_price\x18\x0c \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12G\n\x0f\x66unding_payment\x18\r \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_height\x18\x0e \x01(\x03\x12\x15\n\rblock_time_ms\x18\x0f \x01(\x03\"\xae\x07\n\x17PositionLiquidatedEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x16\n\x0etrader_address\x18\x02 \x01(\t\x12N\n\x16\x65xchanged_quote_amount\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x65xchanged_position_size\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x1a\n\x12liquidator_address\x18\x05 \x01(\t\x12V\n\x11\x66\x65\x65_to_liquidator\x18\x06 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB \xf2\xde\x1f\x18yaml:\"fee_to_liquidator\"\xc8\xde\x1f\x00\x12^\n\x15\x66\x65\x65_to_ecosystem_fund\x18\x07 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB$\xf2\xde\x1f\x1cyaml:\"fee_to_ecosystem_fund\"\xc8\xde\x1f\x00\x12\x31\n\x08\x62\x61\x64_debt\x18\x08 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12@\n\x06margin\x18\t \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x15\xf2\xde\x1f\ryaml:\"margin\"\xc8\xde\x1f\x00\x12I\n\x11position_notional\x18\n \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x45\n\rposition_size\x18\x0b \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x45\n\runrealizedPnl\x18\x0c \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x42\n\nmark_price\x18\r \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_height\x18\x0e \x01(\x03\x12\x15\n\rblock_time_ms\x18\x0f \x01(\x03\"\xf3\x01\n\x14PositionSettledEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x16\n\x0etrader_address\x18\x02 \x01(\t\x12z\n\rsettled_coins\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinBH\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\xf2\xde\x1f\x14yaml:\"settled_coins\"\xc8\xde\x1f\x00\"\x8b\x04\n\x17\x46undingRateChangedEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x42\n\nmark_price\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x43\n\x0bindex_price\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12K\n\x13latest_funding_rate\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17latest_premium_fraction\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12S\n\x1b\x63umulative_premium_fraction\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_height\x18\x07 \x01(\x03\x12\x15\n\rblock_time_ms\x18\x08 \x01(\x03\"\xc7\x02\n\x16LiquidationFailedEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x0e\n\x06trader\x18\x02 \x01(\t\x12\x12\n\nliquidator\x18\x03 \x01(\t\x12N\n\x06reason\x18\x04 \x01(\x0e\x32>.nibiru.perp.v1.LiquidationFailedEvent.LiquidationFailedReason\"p\n\x17LiquidationFailedReason\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x14\n\x10POSITION_HEALTHY\x10\x01\x12\x14\n\x10NONEXISTENT_PAIR\x10\x02\x12\x18\n\x14NONEXISTENT_POSITION\x10\x03\"\xcf\x02\n\x0cMetricsEvent\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12@\n\x08net_size\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x43\n\x0bvolumeQuote\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x42\n\nvolumeBase\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_height\x18\x05 \x01(\x03\x12\x15\n\rblock_time_ms\x18\x06 \x01(\x03\x42,Z*github.com/NibiruChain/nibiru/x/perp/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v2.event_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v1.event_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/NibiruChain/nibiru/x/perp/v2/types'
+  DESCRIPTOR._serialized_options = b'Z*github.com/NibiruChain/nibiru/x/perp/types'
   _POSITIONCHANGEDEVENT.fields_by_name['pair']._options = None
   _POSITIONCHANGEDEVENT.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
   _POSITIONCHANGEDEVENT.fields_by_name['margin']._options = None
   _POSITIONCHANGEDEVENT.fields_by_name['margin']._serialized_options = b'\362\336\037\ryaml:\"margin\"\310\336\037\000'
   _POSITIONCHANGEDEVENT.fields_by_name['position_notional']._options = None
   _POSITIONCHANGEDEVENT.fields_by_name['position_notional']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _POSITIONCHANGEDEVENT.fields_by_name['exchanged_size']._options = None
@@ -42,14 +41,16 @@
   _POSITIONCHANGEDEVENT.fields_by_name['position_size']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _POSITIONCHANGEDEVENT.fields_by_name['realized_pnl']._options = None
   _POSITIONCHANGEDEVENT.fields_by_name['realized_pnl']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _POSITIONCHANGEDEVENT.fields_by_name['unrealized_pnl_after']._options = None
   _POSITIONCHANGEDEVENT.fields_by_name['unrealized_pnl_after']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _POSITIONCHANGEDEVENT.fields_by_name['bad_debt']._options = None
   _POSITIONCHANGEDEVENT.fields_by_name['bad_debt']._serialized_options = b'\310\336\037\000'
+  _POSITIONCHANGEDEVENT.fields_by_name['mark_price']._options = None
+  _POSITIONCHANGEDEVENT.fields_by_name['mark_price']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _POSITIONCHANGEDEVENT.fields_by_name['funding_payment']._options = None
   _POSITIONCHANGEDEVENT.fields_by_name['funding_payment']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _POSITIONLIQUIDATEDEVENT.fields_by_name['pair']._options = None
   _POSITIONLIQUIDATEDEVENT.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
   _POSITIONLIQUIDATEDEVENT.fields_by_name['exchanged_quote_amount']._options = None
   _POSITIONLIQUIDATEDEVENT.fields_by_name['exchanged_quote_amount']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _POSITIONLIQUIDATEDEVENT.fields_by_name['exchanged_position_size']._options = None
@@ -84,20 +85,30 @@
   _FUNDINGRATECHANGEDEVENT.fields_by_name['latest_funding_rate']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _FUNDINGRATECHANGEDEVENT.fields_by_name['latest_premium_fraction']._options = None
   _FUNDINGRATECHANGEDEVENT.fields_by_name['latest_premium_fraction']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _FUNDINGRATECHANGEDEVENT.fields_by_name['cumulative_premium_fraction']._options = None
   _FUNDINGRATECHANGEDEVENT.fields_by_name['cumulative_premium_fraction']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _LIQUIDATIONFAILEDEVENT.fields_by_name['pair']._options = None
   _LIQUIDATIONFAILEDEVENT.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
-  _POSITIONCHANGEDEVENT._serialized_start=178
-  _POSITIONCHANGEDEVENT._serialized_end=1058
-  _POSITIONLIQUIDATEDEVENT._serialized_start=1061
-  _POSITIONLIQUIDATEDEVENT._serialized_end=2003
-  _POSITIONSETTLEDEVENT._serialized_start=2006
-  _POSITIONSETTLEDEVENT._serialized_end=2249
-  _FUNDINGRATECHANGEDEVENT._serialized_start=2252
-  _FUNDINGRATECHANGEDEVENT._serialized_end=2775
-  _LIQUIDATIONFAILEDEVENT._serialized_start=2778
-  _LIQUIDATIONFAILEDEVENT._serialized_end=3105
-  _LIQUIDATIONFAILEDEVENT_LIQUIDATIONFAILEDREASON._serialized_start=2993
-  _LIQUIDATIONFAILEDEVENT_LIQUIDATIONFAILEDREASON._serialized_end=3105
+  _METRICSEVENT.fields_by_name['pair']._options = None
+  _METRICSEVENT.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
+  _METRICSEVENT.fields_by_name['net_size']._options = None
+  _METRICSEVENT.fields_by_name['net_size']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _METRICSEVENT.fields_by_name['volumeQuote']._options = None
+  _METRICSEVENT.fields_by_name['volumeQuote']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _METRICSEVENT.fields_by_name['volumeBase']._options = None
+  _METRICSEVENT.fields_by_name['volumeBase']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _POSITIONCHANGEDEVENT._serialized_start=145
+  _POSITIONCHANGEDEVENT._serialized_end=1093
+  _POSITIONLIQUIDATEDEVENT._serialized_start=1096
+  _POSITIONLIQUIDATEDEVENT._serialized_end=2038
+  _POSITIONSETTLEDEVENT._serialized_start=2041
+  _POSITIONSETTLEDEVENT._serialized_end=2284
+  _FUNDINGRATECHANGEDEVENT._serialized_start=2287
+  _FUNDINGRATECHANGEDEVENT._serialized_end=2810
+  _LIQUIDATIONFAILEDEVENT._serialized_start=2813
+  _LIQUIDATIONFAILEDEVENT._serialized_end=3140
+  _LIQUIDATIONFAILEDEVENT_LIQUIDATIONFAILEDREASON._serialized_start=3028
+  _LIQUIDATIONFAILEDEVENT_LIQUIDATIONFAILEDREASON._serialized_end=3140
+  _METRICSEVENT._serialized_start=3143
+  _METRICSEVENT._serialized_end=3478
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/event_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/event_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
 class PositionChangedEvent(google.protobuf.message.Message):
     """Emitted when a position changes.
-    TODO: Is there a way to split this into different events without creating too
-    much complexity?
+    TODO: Is there a way to split this into different events without creating too much complexity?
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAIR_FIELD_NUMBER: builtins.int
     TRADER_ADDRESS_FIELD_NUMBER: builtins.int
     MARGIN_FIELD_NUMBER: builtins.int
@@ -35,59 +34,64 @@
     EXCHANGED_SIZE_FIELD_NUMBER: builtins.int
     EXCHANGED_NOTIONAL_FIELD_NUMBER: builtins.int
     TRANSACTION_FEE_FIELD_NUMBER: builtins.int
     POSITION_SIZE_FIELD_NUMBER: builtins.int
     REALIZED_PNL_FIELD_NUMBER: builtins.int
     UNREALIZED_PNL_AFTER_FIELD_NUMBER: builtins.int
     BAD_DEBT_FIELD_NUMBER: builtins.int
+    MARK_PRICE_FIELD_NUMBER: builtins.int
     FUNDING_PAYMENT_FIELD_NUMBER: builtins.int
     BLOCK_HEIGHT_FIELD_NUMBER: builtins.int
     BLOCK_TIME_MS_FIELD_NUMBER: builtins.int
     pair: builtins.str
     """identifier of the corresponding virtual pool for the position"""
     trader_address: builtins.str
     """owner of the position."""
     @property
     def margin(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
         """Amount of collateral (quote units) backing the position after the change."""
     position_notional: builtins.str
-    """Position notional (quote units) after the change. In general,
+    """Position notional (quote units) after the change. In general, 
     'notional = baseAmount * priceQuotePerBase', where size is the baseAmount.
     """
     exchanged_size: builtins.str
-    """Exchanged size is the magnitude of the change to position size (base
-    units). The size is a signed quantity expressing how much exposure a
-    position has in base units of the pair.
+    """Exchanged size is the magnitude of the change to position size (base units). 
+    The size is a signed quantity expressing how much exposure a position has in 
+    base units of the pair.
     """
     exchanged_notional: builtins.str
     """*
     Exchanged notional is the value of the exchanged size in quote units.
-    exchangedNotional = posBefore.OpenNotional + (direction * realizedPnl),
-    where 'posBefore' is the position before the change, and
+    exchangedNotional = posBefore.OpenNotional + (direction * realizedPnl), 
+    where 'posBefore' is the position before the change, and 
     direction is 1 if posBefore.Size > 0 or -1 if posBefore.Size < 0,
     """
     @property
     def transaction_fee(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
         """Transaction fee paid. A "taker" fee."""
     position_size: builtins.str
     """Position size after the change."""
     realized_pnl: builtins.str
     """realize profits and losses after the change"""
     unrealized_pnl_after: builtins.str
     """unrealized profits and losses after the change"""
     @property
     def bad_debt(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
-        """Amount of bad debt cleared by the PerpEF during the change.
+        """Amount of bad debt cleared by the PerpEF during the change. 
         Bad debt is negative net margin past the liquidation point of a position.
         """
+    mark_price: builtins.str
+    """Mark price, synonymous with mark price in this context, is the quotient of
+    the quote reserves and base reserves
+    """
     funding_payment: builtins.str
-    """A funding payment made or received by the trader on the current position.
+    """A funding payment made or received by the trader on the current position. 
     'fundingPayment' is positive if 'owner' is the sender and negative if 'owner'
-    is the receiver of the payment. Its magnitude is abs(vSize * fundingRate).
-    Funding payments act to converge the mark price (vPrice) and index price
+    is the receiver of the payment. Its magnitude is abs(vSize * fundingRate). 
+    Funding payments act to converge the mark price (vPrice) and index price 
     (average price on major exchanges).
     """
     block_height: builtins.int
     """The block number at which this position was changed."""
     block_time_ms: builtins.int
     """The block time in unix milliseconds at which this position was changed."""
     def __init__(
@@ -100,20 +104,21 @@
         exchanged_size: builtins.str = ...,
         exchanged_notional: builtins.str = ...,
         transaction_fee: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
         position_size: builtins.str = ...,
         realized_pnl: builtins.str = ...,
         unrealized_pnl_after: builtins.str = ...,
         bad_debt: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        mark_price: builtins.str = ...,
         funding_payment: builtins.str = ...,
         block_height: builtins.int = ...,
         block_time_ms: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["bad_debt", b"bad_debt", "margin", b"margin", "transaction_fee", b"transaction_fee"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bad_debt", b"bad_debt", "block_height", b"block_height", "block_time_ms", b"block_time_ms", "exchanged_notional", b"exchanged_notional", "exchanged_size", b"exchanged_size", "funding_payment", b"funding_payment", "margin", b"margin", "pair", b"pair", "position_notional", b"position_notional", "position_size", b"position_size", "realized_pnl", b"realized_pnl", "trader_address", b"trader_address", "transaction_fee", b"transaction_fee", "unrealized_pnl_after", b"unrealized_pnl_after"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bad_debt", b"bad_debt", "block_height", b"block_height", "block_time_ms", b"block_time_ms", "exchanged_notional", b"exchanged_notional", "exchanged_size", b"exchanged_size", "funding_payment", b"funding_payment", "margin", b"margin", "mark_price", b"mark_price", "pair", b"pair", "position_notional", b"position_notional", "position_size", b"position_size", "realized_pnl", b"realized_pnl", "trader_address", b"trader_address", "transaction_fee", b"transaction_fee", "unrealized_pnl_after", b"unrealized_pnl_after"]) -> None: ...
 
 global___PositionChangedEvent = PositionChangedEvent
 
 @typing_extensions.final
 class PositionLiquidatedEvent(google.protobuf.message.Message):
     """Emitted when a position is liquidated."""
 
@@ -135,34 +140,28 @@
     BLOCK_HEIGHT_FIELD_NUMBER: builtins.int
     BLOCK_TIME_MS_FIELD_NUMBER: builtins.int
     pair: builtins.str
     """identifier of the corresponding virtual pool for the position"""
     trader_address: builtins.str
     """owner of the position."""
     exchanged_quote_amount: builtins.str
-    """margin * leverage * vPrice. 'notional' is the virtual size times  the
-    virtual price on 'perp.amm'.
-    """
+    """margin * leverage * vPrice. 'notional' is the virtual size times  the virtual price on 'vpool'."""
     exchanged_position_size: builtins.str
-    """virtual amount of base assets for the position, which would be margin *
-    leverage * priceBasePerQuote.
-    """
+    """virtual amount of base assets for the position, which would be margin * leverage * priceBasePerQuote."""
     liquidator_address: builtins.str
     """Address of the account that executed the tx."""
     @property
     def fee_to_liquidator(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
         """Commission (in margin units) received by 'liquidator'."""
     @property
     def fee_to_ecosystem_fund(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
         """Commission (in margin units) given to the ecosystem fund."""
     @property
     def bad_debt(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
-        """ Bad debt (margin units) cleared by the PerpEF during the tx. Bad debt is
-         negative net margin past the liquidation point of a position.
-        """
+        """ Bad debt (margin units) cleared by the PerpEF during the tx. Bad debt is negative net margin past the liquidation point of a position."""
     @property
     def margin(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
         """Remaining margin in the position after liquidation"""
     position_notional: builtins.str
     """Remaining position notional in the position after liquidation"""
     position_size: builtins.str
     """Remaining position size in the position after liquidation"""
@@ -209,15 +208,15 @@
     SETTLED_COINS_FIELD_NUMBER: builtins.int
     pair: builtins.str
     """Identifier for the virtual pool of the position."""
     trader_address: builtins.str
     """Owner of the position."""
     @property
     def settled_coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]:
-        """Settled coin as dictated by the settlement price of the perp.amm."""
+        """Settled coin as dictated by the settlement price of the vpool."""
     def __init__(
         self,
         *,
         pair: builtins.str = ...,
         trader_address: builtins.str = ...,
         settled_coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
@@ -247,24 +246,21 @@
     """The oracle index price of the pair."""
     latest_funding_rate: builtins.str
     """The latest funding rate."""
     latest_premium_fraction: builtins.str
     """The latest premium fraction just calculated."""
     cumulative_premium_fraction: builtins.str
     """The latest cumulative premium fraction.
-    The funding payment a position will pay is the difference between this
-    value and the latest cumulative premium fraction on the position,
-    multiplied by the position size.
+    The funding payment a position will pay is the difference between this value
+    and the latest cumulative premium fraction on the position, multiplied by the position size.
     """
     block_height: builtins.int
     """The block number at which the funding rate was calculated."""
     block_time_ms: builtins.int
-    """The block time in unix milliseconds at which the funding rate was
-    calculated.
-    """
+    """The block time in unix milliseconds at which the funding rate was calculated."""
     def __init__(
         self,
         *,
         pair: builtins.str = ...,
         mark_price: builtins.str = ...,
         index_price: builtins.str = ...,
         latest_funding_rate: builtins.str = ...,
@@ -325,7 +321,42 @@
         trader: builtins.str = ...,
         liquidator: builtins.str = ...,
         reason: global___LiquidationFailedEvent.LiquidationFailedReason.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["liquidator", b"liquidator", "pair", b"pair", "reason", b"reason", "trader", b"trader"]) -> None: ...
 
 global___LiquidationFailedEvent = LiquidationFailedEvent
+
+@typing_extensions.final
+class MetricsEvent(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    PAIR_FIELD_NUMBER: builtins.int
+    NET_SIZE_FIELD_NUMBER: builtins.int
+    VOLUMEQUOTE_FIELD_NUMBER: builtins.int
+    VOLUMEBASE_FIELD_NUMBER: builtins.int
+    BLOCK_HEIGHT_FIELD_NUMBER: builtins.int
+    BLOCK_TIME_MS_FIELD_NUMBER: builtins.int
+    pair: builtins.str
+    net_size: builtins.str
+    """Sum of all active position sizes for the pair."""
+    volumeQuote: builtins.str
+    """Total notional volume for the pair."""
+    volumeBase: builtins.str
+    """Total size volume for the pair."""
+    block_height: builtins.int
+    """The block number at which metrics were generated."""
+    block_time_ms: builtins.int
+    """The block time in unix milliseconds at which metrics were generated."""
+    def __init__(
+        self,
+        *,
+        pair: builtins.str = ...,
+        net_size: builtins.str = ...,
+        volumeQuote: builtins.str = ...,
+        volumeBase: builtins.str = ...,
+        block_height: builtins.int = ...,
+        block_time_ms: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["block_height", b"block_height", "block_time_ms", b"block_time_ms", "net_size", b"net_size", "pair", b"pair", "volumeBase", b"volumeBase", "volumeQuote", b"volumeQuote"]) -> None: ...
+
+global___MetricsEvent = MetricsEvent
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/genesis_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: perp/v2/genesis.proto
+# source: perp/v1/genesis.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
-from perp.v2 import state_pb2 as perp_dot_v2_dot_state__pb2
+from perp.v1 import state_pb2 as perp_dot_v1_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15perp/v2/genesis.proto\x12\x0enibiru.perp.v2\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x13perp/v2/state.proto\"\xdb\x01\n\x0cGenesisState\x12-\n\x07markets\x18\x02 \x03(\x0b\x32\x16.nibiru.perp.v2.MarketB\x04\xc8\xde\x1f\x00\x12\'\n\x04\x61mms\x18\x03 \x03(\x0b\x32\x13.nibiru.perp.v2.AMMB\x04\xc8\xde\x1f\x00\x12\x31\n\tpositions\x18\x04 \x03(\x0b\x32\x18.nibiru.perp.v2.PositionB\x04\xc8\xde\x1f\x00\x12@\n\x11reserve_snapshots\x18\x05 \x03(\x0b\x32\x1f.nibiru.perp.v2.ReserveSnapshotB\x04\xc8\xde\x1f\x00\x42/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15perp/v1/genesis.proto\x12\x0enibiru.perp.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x13perp/v1/state.proto\"\xeb\x01\n\x0cGenesisState\x12,\n\x06params\x18\x01 \x01(\x0b\x32\x16.nibiru.perp.v1.ParamsB\x04\xc8\xde\x1f\x00\x12\x39\n\rpair_metadata\x18\x02 \x03(\x0b\x32\x1c.nibiru.perp.v1.PairMetadataB\x04\xc8\xde\x1f\x00\x12\x31\n\tpositions\x18\x03 \x03(\x0b\x32\x18.nibiru.perp.v1.PositionB\x04\xc8\xde\x1f\x00\x12?\n\x11prepaid_bad_debts\x18\x04 \x03(\x0b\x32\x1e.nibiru.perp.v1.PrepaidBadDebtB\x04\xc8\xde\x1f\x00\x42,Z*github.com/NibiruChain/nibiru/x/perp/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v2.genesis_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v1.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/NibiruChain/nibiru/x/perp/v2/types'
-  _GENESISSTATE.fields_by_name['markets']._options = None
-  _GENESISSTATE.fields_by_name['markets']._serialized_options = b'\310\336\037\000'
-  _GENESISSTATE.fields_by_name['amms']._options = None
-  _GENESISSTATE.fields_by_name['amms']._serialized_options = b'\310\336\037\000'
+  DESCRIPTOR._serialized_options = b'Z*github.com/NibiruChain/nibiru/x/perp/types'
+  _GENESISSTATE.fields_by_name['params']._options = None
+  _GENESISSTATE.fields_by_name['params']._serialized_options = b'\310\336\037\000'
+  _GENESISSTATE.fields_by_name['pair_metadata']._options = None
+  _GENESISSTATE.fields_by_name['pair_metadata']._serialized_options = b'\310\336\037\000'
   _GENESISSTATE.fields_by_name['positions']._options = None
   _GENESISSTATE.fields_by_name['positions']._serialized_options = b'\310\336\037\000'
-  _GENESISSTATE.fields_by_name['reserve_snapshots']._options = None
-  _GENESISSTATE.fields_by_name['reserve_snapshots']._serialized_options = b'\310\336\037\000'
+  _GENESISSTATE.fields_by_name['prepaid_bad_debts']._options = None
+  _GENESISSTATE.fields_by_name['prepaid_bad_debts']._serialized_options = b'\310\336\037\000'
   _GENESISSTATE._serialized_start=147
-  _GENESISSTATE._serialized_end=366
+  _GENESISSTATE._serialized_end=382
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/genesis_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import perp.v2.state_pb2
+import perp.v1.state_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -19,30 +19,31 @@
 
 @typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the perp module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    MARKETS_FIELD_NUMBER: builtins.int
-    AMMS_FIELD_NUMBER: builtins.int
+    PARAMS_FIELD_NUMBER: builtins.int
+    PAIR_METADATA_FIELD_NUMBER: builtins.int
     POSITIONS_FIELD_NUMBER: builtins.int
-    RESERVE_SNAPSHOTS_FIELD_NUMBER: builtins.int
+    PREPAID_BAD_DEBTS_FIELD_NUMBER: builtins.int
     @property
-    def markets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[perp.v2.state_pb2.Market]: ...
+    def params(self) -> perp.v1.state_pb2.Params: ...
     @property
-    def amms(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[perp.v2.state_pb2.AMM]: ...
+    def pair_metadata(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[perp.v1.state_pb2.PairMetadata]: ...
     @property
-    def positions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[perp.v2.state_pb2.Position]: ...
+    def positions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[perp.v1.state_pb2.Position]: ...
     @property
-    def reserve_snapshots(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[perp.v2.state_pb2.ReserveSnapshot]: ...
+    def prepaid_bad_debts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[perp.v1.state_pb2.PrepaidBadDebt]: ...
     def __init__(
         self,
         *,
-        markets: collections.abc.Iterable[perp.v2.state_pb2.Market] | None = ...,
-        amms: collections.abc.Iterable[perp.v2.state_pb2.AMM] | None = ...,
-        positions: collections.abc.Iterable[perp.v2.state_pb2.Position] | None = ...,
-        reserve_snapshots: collections.abc.Iterable[perp.v2.state_pb2.ReserveSnapshot] | None = ...,
+        params: perp.v1.state_pb2.Params | None = ...,
+        pair_metadata: collections.abc.Iterable[perp.v1.state_pb2.PairMetadata] | None = ...,
+        positions: collections.abc.Iterable[perp.v1.state_pb2.Position] | None = ...,
+        prepaid_bad_debts: collections.abc.Iterable[perp.v1.state_pb2.PrepaidBadDebt] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["amms", b"amms", "markets", b"markets", "positions", b"positions", "reserve_snapshots", b"reserve_snapshots"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pair_metadata", b"pair_metadata", "params", b"params", "positions", b"positions", "prepaid_bad_debts", b"prepaid_bad_debts"]) -> None: ...
 
 global___GenesisState = GenesisState
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/query_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: perp/v2/query.proto
+# source: perp/v1/query.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from perp.v2 import state_pb2 as perp_dot_v2_dot_state__pb2
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
+from perp.v1 import state_pb2 as perp_dot_v1_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13perp/v2/query.proto\x12\x0enibiru.perp.v2\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x13perp/v2/state.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"\'\n\x15QueryPositionsRequest\x12\x0e\n\x06trader\x18\x01 \x01(\t\"X\n\x16QueryPositionsResponse\x12>\n\tpositions\x18\x01 \x03(\x0b\x32%.nibiru.perp.v2.QueryPositionResponseB\x04\xc8\xde\x1f\x00\"o\n\x14QueryPositionRequest\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x0e\n\x06trader\x18\x02 \x01(\t\"\xa2\x02\n\x15QueryPositionResponse\x12\x30\n\x08position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionB\x04\xc8\xde\x1f\x00\x12I\n\x11position_notional\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x46\n\x0eunrealized_pnl\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0cmargin_ratio\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\x1c\n\x1aQueryModuleAccountsRequest\"Y\n\x1bQueryModuleAccountsResponse\x12:\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\".nibiru.perp.v2.AccountWithBalanceB\x04\xc8\xde\x1f\x00\"\x91\x01\n\x12\x41\x63\x63ountWithBalance\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\\\n\x07\x62\x61lance\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\"a\n\tAmmMarket\x12,\n\x06market\x18\x01 \x01(\x0b\x32\x16.nibiru.perp.v2.MarketB\x04\xc8\xde\x1f\x00\x12&\n\x03\x61mm\x18\x02 \x01(\x0b\x32\x13.nibiru.perp.v2.AMMB\x04\xc8\xde\x1f\x00\"\x15\n\x13QueryMarketsRequest\"L\n\x14QueryMarketsResponse\x12\x34\n\x0b\x61mm_markets\x18\x01 \x03(\x0b\x32\x19.nibiru.perp.v2.AmmMarketB\x04\xc8\xde\x1f\x00\x32\x9d\x04\n\x05Query\x12~\n\rQueryPosition\x12$.nibiru.perp.v2.QueryPositionRequest\x1a%.nibiru.perp.v2.QueryPositionResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/nibiru/perp/v2/position\x12\x82\x01\n\x0eQueryPositions\x12%.nibiru.perp.v2.QueryPositionsRequest\x1a&.nibiru.perp.v2.QueryPositionsResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/nibiru/perp/v2/positions\x12\x92\x01\n\x0eModuleAccounts\x12*.nibiru.perp.v2.QueryModuleAccountsRequest\x1a+.nibiru.perp.v2.QueryModuleAccountsResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/nibiru/perp/v2/module_accounts\x12z\n\x0cQueryMarkets\x12#.nibiru.perp.v2.QueryMarketsRequest\x1a$.nibiru.perp.v2.QueryMarketsResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/nibiru/perp/v2/marketsB/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13perp/v1/query.proto\x12\x0enibiru.perp.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x13perp/v1/state.proto\"\x14\n\x12QueryParamsRequest\"C\n\x13QueryParamsResponse\x12,\n\x06params\x18\x01 \x01(\x0b\x32\x16.nibiru.perp.v1.ParamsB\x04\xc8\xde\x1f\x00\"\'\n\x15QueryPositionsRequest\x12\x0e\n\x06trader\x18\x01 \x01(\t\"R\n\x16QueryPositionsResponse\x12\x38\n\tpositions\x18\x01 \x03(\x0b\x32%.nibiru.perp.v1.QueryPositionResponse\"o\n\x14QueryPositionRequest\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x0e\n\x06trader\x18\x02 \x01(\t\"\x83\x03\n\x15QueryPositionResponse\x12*\n\x08position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v1.Position\x12I\n\x11position_notional\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x46\n\x0eunrealized_pnl\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12I\n\x11margin_ratio_mark\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12J\n\x12margin_ratio_index\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_number\x18\x07 \x01(\x03\"p\n%QueryCumulativePremiumFractionRequest\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\"\xe1\x01\n&QueryCumulativePremiumFractionResponse\x12S\n\x1b\x63umulative_premium_fraction\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x62\n*estimated_next_cumulative_premium_fraction\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"^\n\x13QueryMetricsRequest\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\"F\n\x14QueryMetricsResponse\x12.\n\x07metrics\x18\x01 \x01(\x0b\x32\x17.nibiru.perp.v1.MetricsB\x04\xc8\xde\x1f\x00\x32\xa8\x05\n\x05Query\x12n\n\x06Params\x12\".nibiru.perp.v1.QueryParamsRequest\x1a#.nibiru.perp.v1.QueryParamsResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/nibiru/perp/params\x12{\n\rQueryPosition\x12$.nibiru.perp.v1.QueryPositionRequest\x1a%.nibiru.perp.v1.QueryPositionResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/nibiru/perp/position\x12\x7f\n\x0eQueryPositions\x12%.nibiru.perp.v1.QueryPositionsRequest\x1a&.nibiru.perp.v1.QueryPositionsResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/nibiru/perp/positions\x12\xbc\x01\n\x19\x43umulativePremiumFraction\x12\x35.nibiru.perp.v1.QueryCumulativePremiumFractionRequest\x1a\x36.nibiru.perp.v1.QueryCumulativePremiumFractionResponse\"0\x82\xd3\xe4\x93\x02*\x12(/nibiru/perp/cumulative_premium_fraction\x12r\n\x07Metrics\x12#.nibiru.perp.v1.QueryMetricsRequest\x1a$.nibiru.perp.v1.QueryMetricsResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/nibiru/perp/metricsB,Z*github.com/NibiruChain/nibiru/x/perp/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v2.query_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v1.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/NibiruChain/nibiru/x/perp/v2/types'
-  _QUERYPOSITIONSRESPONSE.fields_by_name['positions']._options = None
-  _QUERYPOSITIONSRESPONSE.fields_by_name['positions']._serialized_options = b'\310\336\037\000'
+  DESCRIPTOR._serialized_options = b'Z*github.com/NibiruChain/nibiru/x/perp/types'
+  _QUERYPARAMSRESPONSE.fields_by_name['params']._options = None
+  _QUERYPARAMSRESPONSE.fields_by_name['params']._serialized_options = b'\310\336\037\000'
   _QUERYPOSITIONREQUEST.fields_by_name['pair']._options = None
   _QUERYPOSITIONREQUEST.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
-  _QUERYPOSITIONRESPONSE.fields_by_name['position']._options = None
-  _QUERYPOSITIONRESPONSE.fields_by_name['position']._serialized_options = b'\310\336\037\000'
   _QUERYPOSITIONRESPONSE.fields_by_name['position_notional']._options = None
   _QUERYPOSITIONRESPONSE.fields_by_name['position_notional']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _QUERYPOSITIONRESPONSE.fields_by_name['unrealized_pnl']._options = None
   _QUERYPOSITIONRESPONSE.fields_by_name['unrealized_pnl']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _QUERYPOSITIONRESPONSE.fields_by_name['margin_ratio']._options = None
-  _QUERYPOSITIONRESPONSE.fields_by_name['margin_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _QUERYMODULEACCOUNTSRESPONSE.fields_by_name['accounts']._options = None
-  _QUERYMODULEACCOUNTSRESPONSE.fields_by_name['accounts']._serialized_options = b'\310\336\037\000'
-  _ACCOUNTWITHBALANCE.fields_by_name['balance']._options = None
-  _ACCOUNTWITHBALANCE.fields_by_name['balance']._serialized_options = b'\310\336\037\000\252\337\037(github.com/cosmos/cosmos-sdk/types.Coins'
-  _AMMMARKET.fields_by_name['market']._options = None
-  _AMMMARKET.fields_by_name['market']._serialized_options = b'\310\336\037\000'
-  _AMMMARKET.fields_by_name['amm']._options = None
-  _AMMMARKET.fields_by_name['amm']._serialized_options = b'\310\336\037\000'
-  _QUERYMARKETSRESPONSE.fields_by_name['amm_markets']._options = None
-  _QUERYMARKETSRESPONSE.fields_by_name['amm_markets']._serialized_options = b'\310\336\037\000'
+  _QUERYPOSITIONRESPONSE.fields_by_name['margin_ratio_mark']._options = None
+  _QUERYPOSITIONRESPONSE.fields_by_name['margin_ratio_mark']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _QUERYPOSITIONRESPONSE.fields_by_name['margin_ratio_index']._options = None
+  _QUERYPOSITIONRESPONSE.fields_by_name['margin_ratio_index']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _QUERYCUMULATIVEPREMIUMFRACTIONREQUEST.fields_by_name['pair']._options = None
+  _QUERYCUMULATIVEPREMIUMFRACTIONREQUEST.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
+  _QUERYCUMULATIVEPREMIUMFRACTIONRESPONSE.fields_by_name['cumulative_premium_fraction']._options = None
+  _QUERYCUMULATIVEPREMIUMFRACTIONRESPONSE.fields_by_name['cumulative_premium_fraction']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _QUERYCUMULATIVEPREMIUMFRACTIONRESPONSE.fields_by_name['estimated_next_cumulative_premium_fraction']._options = None
+  _QUERYCUMULATIVEPREMIUMFRACTIONRESPONSE.fields_by_name['estimated_next_cumulative_premium_fraction']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _QUERYMETRICSREQUEST.fields_by_name['pair']._options = None
+  _QUERYMETRICSREQUEST.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
+  _QUERYMETRICSRESPONSE.fields_by_name['metrics']._options = None
+  _QUERYMETRICSRESPONSE.fields_by_name['metrics']._serialized_options = b'\310\336\037\000'
+  _QUERY.methods_by_name['Params']._options = None
+  _QUERY.methods_by_name['Params']._serialized_options = b'\202\323\344\223\002\025\022\023/nibiru/perp/params'
   _QUERY.methods_by_name['QueryPosition']._options = None
-  _QUERY.methods_by_name['QueryPosition']._serialized_options = b'\202\323\344\223\002\032\022\030/nibiru/perp/v2/position'
+  _QUERY.methods_by_name['QueryPosition']._serialized_options = b'\202\323\344\223\002\027\022\025/nibiru/perp/position'
   _QUERY.methods_by_name['QueryPositions']._options = None
-  _QUERY.methods_by_name['QueryPositions']._serialized_options = b'\202\323\344\223\002\033\022\031/nibiru/perp/v2/positions'
-  _QUERY.methods_by_name['ModuleAccounts']._options = None
-  _QUERY.methods_by_name['ModuleAccounts']._serialized_options = b'\202\323\344\223\002!\022\037/nibiru/perp/v2/module_accounts'
-  _QUERY.methods_by_name['QueryMarkets']._options = None
-  _QUERY.methods_by_name['QueryMarkets']._serialized_options = b'\202\323\344\223\002\031\022\027/nibiru/perp/v2/markets'
-  _QUERYPOSITIONSREQUEST._serialized_start=144
-  _QUERYPOSITIONSREQUEST._serialized_end=183
-  _QUERYPOSITIONSRESPONSE._serialized_start=185
-  _QUERYPOSITIONSRESPONSE._serialized_end=273
-  _QUERYPOSITIONREQUEST._serialized_start=275
-  _QUERYPOSITIONREQUEST._serialized_end=386
-  _QUERYPOSITIONRESPONSE._serialized_start=389
-  _QUERYPOSITIONRESPONSE._serialized_end=679
-  _QUERYMODULEACCOUNTSREQUEST._serialized_start=681
-  _QUERYMODULEACCOUNTSREQUEST._serialized_end=709
-  _QUERYMODULEACCOUNTSRESPONSE._serialized_start=711
-  _QUERYMODULEACCOUNTSRESPONSE._serialized_end=800
-  _ACCOUNTWITHBALANCE._serialized_start=803
-  _ACCOUNTWITHBALANCE._serialized_end=948
-  _AMMMARKET._serialized_start=950
-  _AMMMARKET._serialized_end=1047
-  _QUERYMARKETSREQUEST._serialized_start=1049
-  _QUERYMARKETSREQUEST._serialized_end=1070
-  _QUERYMARKETSRESPONSE._serialized_start=1072
-  _QUERYMARKETSRESPONSE._serialized_end=1148
-  _QUERY._serialized_start=1151
-  _QUERY._serialized_end=1692
+  _QUERY.methods_by_name['QueryPositions']._serialized_options = b'\202\323\344\223\002\030\022\026/nibiru/perp/positions'
+  _QUERY.methods_by_name['CumulativePremiumFraction']._options = None
+  _QUERY.methods_by_name['CumulativePremiumFraction']._serialized_options = b'\202\323\344\223\002*\022(/nibiru/perp/cumulative_premium_fraction'
+  _QUERY.methods_by_name['Metrics']._options = None
+  _QUERY.methods_by_name['Metrics']._serialized_options = b'\202\323\344\223\002\026\022\024/nibiru/perp/metrics'
+  _QUERYPARAMSREQUEST._serialized_start=112
+  _QUERYPARAMSREQUEST._serialized_end=132
+  _QUERYPARAMSRESPONSE._serialized_start=134
+  _QUERYPARAMSRESPONSE._serialized_end=201
+  _QUERYPOSITIONSREQUEST._serialized_start=203
+  _QUERYPOSITIONSREQUEST._serialized_end=242
+  _QUERYPOSITIONSRESPONSE._serialized_start=244
+  _QUERYPOSITIONSRESPONSE._serialized_end=326
+  _QUERYPOSITIONREQUEST._serialized_start=328
+  _QUERYPOSITIONREQUEST._serialized_end=439
+  _QUERYPOSITIONRESPONSE._serialized_start=442
+  _QUERYPOSITIONRESPONSE._serialized_end=829
+  _QUERYCUMULATIVEPREMIUMFRACTIONREQUEST._serialized_start=831
+  _QUERYCUMULATIVEPREMIUMFRACTIONREQUEST._serialized_end=943
+  _QUERYCUMULATIVEPREMIUMFRACTIONRESPONSE._serialized_start=946
+  _QUERYCUMULATIVEPREMIUMFRACTIONRESPONSE._serialized_end=1171
+  _QUERYMETRICSREQUEST._serialized_start=1173
+  _QUERYMETRICSREQUEST._serialized_end=1267
+  _QUERYMETRICSRESPONSE._serialized_start=1269
+  _QUERYMETRICSRESPONSE._serialized_end=1339
+  _QUERY._serialized_start=1342
+  _QUERY._serialized_end=2022
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/tx_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -4,202 +4,198 @@
 """
 import builtins
 import collections.abc
 import cosmos.base.v1beta1.coin_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import perp.v2.state_pb2
+import spot.v1.pool_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class QueryPositionsRequest(google.protobuf.message.Message):
-    """---------------------------------------- Positions"""
-
+class MsgCreatePool(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TRADER_FIELD_NUMBER: builtins.int
-    trader: builtins.str
+    CREATOR_FIELD_NUMBER: builtins.int
+    POOL_PARAMS_FIELD_NUMBER: builtins.int
+    POOL_ASSETS_FIELD_NUMBER: builtins.int
+    creator: builtins.str
+    @property
+    def pool_params(self) -> spot.v1.pool_pb2.PoolParams: ...
+    @property
+    def pool_assets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[spot.v1.pool_pb2.PoolAsset]: ...
     def __init__(
         self,
         *,
-        trader: builtins.str = ...,
+        creator: builtins.str = ...,
+        pool_params: spot.v1.pool_pb2.PoolParams | None = ...,
+        pool_assets: collections.abc.Iterable[spot.v1.pool_pb2.PoolAsset] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["trader", b"trader"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["pool_params", b"pool_params"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["creator", b"creator", "pool_assets", b"pool_assets", "pool_params", b"pool_params"]) -> None: ...
 
-global___QueryPositionsRequest = QueryPositionsRequest
+global___MsgCreatePool = MsgCreatePool
 
 @typing_extensions.final
-class QueryPositionsResponse(google.protobuf.message.Message):
+class MsgCreatePoolResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    POSITIONS_FIELD_NUMBER: builtins.int
-    @property
-    def positions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___QueryPositionResponse]: ...
+    POOL_ID_FIELD_NUMBER: builtins.int
+    pool_id: builtins.int
     def __init__(
         self,
         *,
-        positions: collections.abc.Iterable[global___QueryPositionResponse] | None = ...,
+        pool_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["positions", b"positions"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
 
-global___QueryPositionsResponse = QueryPositionsResponse
+global___MsgCreatePoolResponse = MsgCreatePoolResponse
 
 @typing_extensions.final
-class QueryPositionRequest(google.protobuf.message.Message):
-    """---------------------------------------- Position
-
-    QueryPositionRequest is the request type for the position of the x/perp
-    module account.
+class MsgJoinPool(google.protobuf.message.Message):
+    """
+    Message to join a pool (identified by poolId) with a set of tokens to deposit.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PAIR_FIELD_NUMBER: builtins.int
-    TRADER_FIELD_NUMBER: builtins.int
-    pair: builtins.str
-    trader: builtins.str
-    def __init__(
-        self,
-        *,
-        pair: builtins.str = ...,
-        trader: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pair", b"pair", "trader", b"trader"]) -> None: ...
-
-global___QueryPositionRequest = QueryPositionRequest
-
-@typing_extensions.final
-class QueryPositionResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    POSITION_FIELD_NUMBER: builtins.int
-    POSITION_NOTIONAL_FIELD_NUMBER: builtins.int
-    UNREALIZED_PNL_FIELD_NUMBER: builtins.int
-    MARGIN_RATIO_FIELD_NUMBER: builtins.int
+    SENDER_FIELD_NUMBER: builtins.int
+    POOL_ID_FIELD_NUMBER: builtins.int
+    TOKENS_IN_FIELD_NUMBER: builtins.int
+    USE_ALL_COINS_FIELD_NUMBER: builtins.int
+    sender: builtins.str
+    pool_id: builtins.int
     @property
-    def position(self) -> perp.v2.state_pb2.Position:
-        """The position as it exists in the blockchain state"""
-    position_notional: builtins.str
-    """The position's current notional value, if it were to be entirely closed (in
-    margin units).
-    """
-    unrealized_pnl: builtins.str
-    """The position's unrealized PnL."""
-    margin_ratio: builtins.str
-    """margin ratio of the position based on the spot price"""
+    def tokens_in(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
+    use_all_coins: builtins.bool
     def __init__(
         self,
         *,
-        position: perp.v2.state_pb2.Position | None = ...,
-        position_notional: builtins.str = ...,
-        unrealized_pnl: builtins.str = ...,
-        margin_ratio: builtins.str = ...,
+        sender: builtins.str = ...,
+        pool_id: builtins.int = ...,
+        tokens_in: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
+        use_all_coins: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["position", b"position"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["margin_ratio", b"margin_ratio", "position", b"position", "position_notional", b"position_notional", "unrealized_pnl", b"unrealized_pnl"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "tokens_in", b"tokens_in", "use_all_coins", b"use_all_coins"]) -> None: ...
 
-global___QueryPositionResponse = QueryPositionResponse
+global___MsgJoinPool = MsgJoinPool
 
 @typing_extensions.final
-class QueryModuleAccountsRequest(google.protobuf.message.Message):
-    """---------------------------------------- QueryModuleAccounts"""
-
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    def __init__(
-        self,
-    ) -> None: ...
-
-global___QueryModuleAccountsRequest = QueryModuleAccountsRequest
+class MsgJoinPoolResponse(google.protobuf.message.Message):
+    """
+    Response when a user joins a pool.
+    """
 
-@typing_extensions.final
-class QueryModuleAccountsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ACCOUNTS_FIELD_NUMBER: builtins.int
+    POOL_FIELD_NUMBER: builtins.int
+    NUM_POOL_SHARES_OUT_FIELD_NUMBER: builtins.int
+    REMAINING_COINS_FIELD_NUMBER: builtins.int
+    @property
+    def pool(self) -> spot.v1.pool_pb2.Pool:
+        """the final state of the pool after a join"""
+    @property
+    def num_pool_shares_out(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
+        """sum of LP tokens minted from the join"""
     @property
-    def accounts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AccountWithBalance]: ...
+    def remaining_coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]:
+        """remaining tokens from attempting to join the pool"""
     def __init__(
         self,
         *,
-        accounts: collections.abc.Iterable[global___AccountWithBalance] | None = ...,
+        pool: spot.v1.pool_pb2.Pool | None = ...,
+        num_pool_shares_out: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        remaining_coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["accounts", b"accounts"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["num_pool_shares_out", b"num_pool_shares_out", "pool", b"pool"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["num_pool_shares_out", b"num_pool_shares_out", "pool", b"pool", "remaining_coins", b"remaining_coins"]) -> None: ...
 
-global___QueryModuleAccountsResponse = QueryModuleAccountsResponse
+global___MsgJoinPoolResponse = MsgJoinPoolResponse
 
 @typing_extensions.final
-class AccountWithBalance(google.protobuf.message.Message):
+class MsgExitPool(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    NAME_FIELD_NUMBER: builtins.int
-    ADDRESS_FIELD_NUMBER: builtins.int
-    BALANCE_FIELD_NUMBER: builtins.int
-    name: builtins.str
-    address: builtins.str
+    SENDER_FIELD_NUMBER: builtins.int
+    POOL_ID_FIELD_NUMBER: builtins.int
+    POOL_SHARES_FIELD_NUMBER: builtins.int
+    sender: builtins.str
+    pool_id: builtins.int
     @property
-    def balance(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
+    def pool_shares(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     def __init__(
         self,
         *,
-        name: builtins.str = ...,
-        address: builtins.str = ...,
-        balance: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
+        sender: builtins.str = ...,
+        pool_id: builtins.int = ...,
+        pool_shares: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "balance", b"balance", "name", b"name"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["pool_shares", b"pool_shares"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "pool_shares", b"pool_shares", "sender", b"sender"]) -> None: ...
 
-global___AccountWithBalance = AccountWithBalance
+global___MsgExitPool = MsgExitPool
 
 @typing_extensions.final
-class AmmMarket(google.protobuf.message.Message):
+class MsgExitPoolResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    MARKET_FIELD_NUMBER: builtins.int
-    AMM_FIELD_NUMBER: builtins.int
+    TOKENS_OUT_FIELD_NUMBER: builtins.int
     @property
-    def market(self) -> perp.v2.state_pb2.Market: ...
-    @property
-    def amm(self) -> perp.v2.state_pb2.AMM: ...
+    def tokens_out(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
         self,
         *,
-        market: perp.v2.state_pb2.Market | None = ...,
-        amm: perp.v2.state_pb2.AMM | None = ...,
+        tokens_out: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["amm", b"amm", "market", b"market"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["amm", b"amm", "market", b"market"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["tokens_out", b"tokens_out"]) -> None: ...
 
-global___AmmMarket = AmmMarket
+global___MsgExitPoolResponse = MsgExitPoolResponse
 
 @typing_extensions.final
-class QueryMarketsRequest(google.protobuf.message.Message):
+class MsgSwapAssets(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    SENDER_FIELD_NUMBER: builtins.int
+    POOL_ID_FIELD_NUMBER: builtins.int
+    TOKEN_IN_FIELD_NUMBER: builtins.int
+    TOKEN_OUT_DENOM_FIELD_NUMBER: builtins.int
+    sender: builtins.str
+    pool_id: builtins.int
+    @property
+    def token_in(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
+    token_out_denom: builtins.str
     def __init__(
         self,
+        *,
+        sender: builtins.str = ...,
+        pool_id: builtins.int = ...,
+        token_in: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        token_out_denom: builtins.str = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["token_in", b"token_in"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "token_in", b"token_in", "token_out_denom", b"token_out_denom"]) -> None: ...
 
-global___QueryMarketsRequest = QueryMarketsRequest
+global___MsgSwapAssets = MsgSwapAssets
 
 @typing_extensions.final
-class QueryMarketsResponse(google.protobuf.message.Message):
+class MsgSwapAssetsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    AMM_MARKETS_FIELD_NUMBER: builtins.int
+    TOKEN_OUT_FIELD_NUMBER: builtins.int
     @property
-    def amm_markets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AmmMarket]: ...
+    def token_out(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     def __init__(
         self,
         *,
-        amm_markets: collections.abc.Iterable[global___AmmMarket] | None = ...,
+        token_out: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["amm_markets", b"amm_markets"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["token_out", b"token_out"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["token_out", b"token_out"]) -> None: ...
 
-global___QueryMarketsResponse = QueryMarketsResponse
+global___MsgSwapAssetsResponse = MsgSwapAssetsResponse
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/query_pb2_grpc.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,72 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import grpc
-import perp.v2.query_pb2
+import perp.v1.query_pb2
 
 class QueryStub:
     """Query defines the gRPC querier service."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
+    Params: grpc.UnaryUnaryMultiCallable[
+        perp.v1.query_pb2.QueryParamsRequest,
+        perp.v1.query_pb2.QueryParamsResponse,
+    ]
+    """Parameters queries the parameters of the x/perp module."""
     QueryPosition: grpc.UnaryUnaryMultiCallable[
-        perp.v2.query_pb2.QueryPositionRequest,
-        perp.v2.query_pb2.QueryPositionResponse,
+        perp.v1.query_pb2.QueryPositionRequest,
+        perp.v1.query_pb2.QueryPositionResponse,
     ]
     QueryPositions: grpc.UnaryUnaryMultiCallable[
-        perp.v2.query_pb2.QueryPositionsRequest,
-        perp.v2.query_pb2.QueryPositionsResponse,
+        perp.v1.query_pb2.QueryPositionsRequest,
+        perp.v1.query_pb2.QueryPositionsResponse,
     ]
-    ModuleAccounts: grpc.UnaryUnaryMultiCallable[
-        perp.v2.query_pb2.QueryModuleAccountsRequest,
-        perp.v2.query_pb2.QueryModuleAccountsResponse,
+    CumulativePremiumFraction: grpc.UnaryUnaryMultiCallable[
+        perp.v1.query_pb2.QueryCumulativePremiumFractionRequest,
+        perp.v1.query_pb2.QueryCumulativePremiumFractionResponse,
     ]
-    """Queries the reserve assets in a given pool, identified by a token pair."""
-    QueryMarkets: grpc.UnaryUnaryMultiCallable[
-        perp.v2.query_pb2.QueryMarketsRequest,
-        perp.v2.query_pb2.QueryMarketsResponse,
+    """Queries the latest cumulative premium fraction and the estimated next cumulative premium fraction."""
+    Metrics: grpc.UnaryUnaryMultiCallable[
+        perp.v1.query_pb2.QueryMetricsRequest,
+        perp.v1.query_pb2.QueryMetricsResponse,
     ]
 
 class QueryServicer(metaclass=abc.ABCMeta):
     """Query defines the gRPC querier service."""
 
     @abc.abstractmethod
+    def Params(
+        self,
+        request: perp.v1.query_pb2.QueryParamsRequest,
+        context: grpc.ServicerContext,
+    ) -> perp.v1.query_pb2.QueryParamsResponse:
+        """Parameters queries the parameters of the x/perp module."""
+    @abc.abstractmethod
     def QueryPosition(
         self,
-        request: perp.v2.query_pb2.QueryPositionRequest,
+        request: perp.v1.query_pb2.QueryPositionRequest,
         context: grpc.ServicerContext,
-    ) -> perp.v2.query_pb2.QueryPositionResponse: ...
+    ) -> perp.v1.query_pb2.QueryPositionResponse: ...
     @abc.abstractmethod
     def QueryPositions(
         self,
-        request: perp.v2.query_pb2.QueryPositionsRequest,
+        request: perp.v1.query_pb2.QueryPositionsRequest,
         context: grpc.ServicerContext,
-    ) -> perp.v2.query_pb2.QueryPositionsResponse: ...
+    ) -> perp.v1.query_pb2.QueryPositionsResponse: ...
     @abc.abstractmethod
-    def ModuleAccounts(
+    def CumulativePremiumFraction(
         self,
-        request: perp.v2.query_pb2.QueryModuleAccountsRequest,
+        request: perp.v1.query_pb2.QueryCumulativePremiumFractionRequest,
         context: grpc.ServicerContext,
-    ) -> perp.v2.query_pb2.QueryModuleAccountsResponse:
-        """Queries the reserve assets in a given pool, identified by a token pair."""
+    ) -> perp.v1.query_pb2.QueryCumulativePremiumFractionResponse:
+        """Queries the latest cumulative premium fraction and the estimated next cumulative premium fraction."""
     @abc.abstractmethod
-    def QueryMarkets(
+    def Metrics(
         self,
-        request: perp.v2.query_pb2.QueryMarketsRequest,
+        request: perp.v1.query_pb2.QueryMetricsRequest,
         context: grpc.ServicerContext,
-    ) -> perp.v2.query_pb2.QueryMarketsResponse: ...
+    ) -> perp.v1.query_pb2.QueryMetricsResponse: ...
 
 def add_QueryServicer_to_server(servicer: QueryServicer, server: grpc.Server) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/state_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/state_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,78 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: perp/v2/state.proto
+# source: vpool/v1/state.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from cosmos_proto import cosmos_pb2 as cosmos__proto_dot_cosmos__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13perp/v2/state.proto\x12\x0enibiru.perp.v2\x1a\x14gogoproto/gogo.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x19\x63osmos_proto/cosmos.proto\x1a\x1egoogle/protobuf/duration.proto\"\x8a\x07\n\x06Market\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08\x12U\n\x1dprice_fluctuation_limit_ratio\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12P\n\x18maintenance_margin_ratio\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0cmax_leverage\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12Z\n\"latest_cumulative_premium_fraction\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12J\n\x12\x65xchange_fee_ratio\x18\x07 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12P\n\x18\x65\x63osystem_fund_fee_ratio\x18\x08 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12M\n\x15liquidation_fee_ratio\x18\t \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12Q\n\x19partial_liquidation_ratio\x18\n \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x1d\n\x15\x66unding_rate_epoch_id\x18\x0b \x01(\t\x12\x41\n\x14twap_lookback_window\x18\x0c \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xc8\xde\x1f\x00\x98\xdf\x1f\x01\x12\x39\n\x10prepaid_bad_debt\x18\r \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\xf2\x03\n\x03\x41MM\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x44\n\x0c\x62\x61se_reserve\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x45\n\rquote_reserve\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x42\n\nsqrt_depth\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12H\n\x10price_multiplier\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x42\n\ntotal_long\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x43\n\x0btotal_short\x18\x07 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\xaf\x03\n\x08Position\x12\x16\n\x0etrader_address\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12<\n\x04size\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12>\n\x06margin\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x45\n\ropen_notional\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12Z\n\"latest_cumulative_premium_fraction\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12!\n\x19last_updated_block_number\x18\x07 \x01(\x03\"O\n\x0fReserveSnapshot\x12&\n\x03\x61mm\x18\x01 \x01(\x0b\x32\x13.nibiru.perp.v2.AMMB\x04\xc8\xde\x1f\x00\x12\x14\n\x0ctimestamp_ms\x18\x02 \x01(\x03*;\n\tDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x08\n\x04LONG\x10\x01\x12\t\n\x05SHORT\x10\x02*g\n\x0eTwapCalcOption\x12 \n\x1cTWAP_CALC_OPTION_UNSPECIFIED\x10\x00\x12\x08\n\x04SPOT\x10\x01\x12\x14\n\x10QUOTE_ASSET_SWAP\x10\x02\x12\x13\n\x0f\x42\x41SE_ASSET_SWAP\x10\x03\x42/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14vpool/v1/state.proto\x12\x0fnibiru.vpool.v1\x1a\x19\x63osmos_proto/cosmos.proto\x1a\x14gogoproto/gogo.proto\"\x9d\x02\n\x05Vpool\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12J\n\x12\x62\x61se_asset_reserve\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12K\n\x13quote_asset_reserve\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x32\n\x06\x63onfig\x18\x04 \x01(\x0b\x32\x1c.nibiru.vpool.v1.VpoolConfigB\x04\xc8\xde\x1f\x00\"\x92\x03\n\x0bVpoolConfig\x12I\n\x11trade_limit_ratio\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x66luctuation_limit_ratio\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17max_oracle_spread_ratio\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12P\n\x18maintenance_margin_ratio\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0cmax_leverage\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\xf1\x01\n\x0b\x43urrentTWAP\x12\x1b\n\x07pair_id\x18\x01 \x01(\tB\n\xe2\xde\x1f\x06PairID\x12\x41\n\tnumerator\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x43\n\x0b\x64\x65nominator\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12=\n\x05price\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\x89\x02\n\x0fReserveSnapshot\x12G\n\x04pair\x18\x05 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12J\n\x12\x62\x61se_asset_reserve\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12K\n\x13quote_asset_reserve\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x14\n\x0ctimestamp_ms\x18\x03 \x01(\x03\"\xb8\x02\n\nPoolPrices\x12G\n\x04pair\x18\t \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x42\n\nmark_price\x18\n \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x13\n\x0bindex_price\x18\x0b \x01(\t\x12\x11\n\ttwap_mark\x18\x0c \x01(\t\x12_\n\x0eswap_invariant\x18\r \x01(\tBG\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xf2\xde\x1f\x15yaml:\"swap_invariant\"\xc8\xde\x1f\x00\x12\x14\n\x0c\x62lock_number\x18\x0e \x01(\x03*M\n\tDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x0f\n\x0b\x41\x44\x44_TO_POOL\x10\x01\x12\x14\n\x10REMOVE_FROM_POOL\x10\x02*g\n\x0eTwapCalcOption\x12 \n\x1cTWAP_CALC_OPTION_UNSPECIFIED\x10\x00\x12\x08\n\x04SPOT\x10\x01\x12\x14\n\x10QUOTE_ASSET_SWAP\x10\x02\x12\x13\n\x0f\x42\x41SE_ASSET_SWAP\x10\x03\x42-Z+github.com/NibiruChain/nibiru/x/vpool/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v2.state_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'vpool.v1.state_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/NibiruChain/nibiru/x/perp/v2/types'
-  _MARKET.fields_by_name['pair']._options = None
-  _MARKET.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
-  _MARKET.fields_by_name['price_fluctuation_limit_ratio']._options = None
-  _MARKET.fields_by_name['price_fluctuation_limit_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _MARKET.fields_by_name['maintenance_margin_ratio']._options = None
-  _MARKET.fields_by_name['maintenance_margin_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _MARKET.fields_by_name['max_leverage']._options = None
-  _MARKET.fields_by_name['max_leverage']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _MARKET.fields_by_name['latest_cumulative_premium_fraction']._options = None
-  _MARKET.fields_by_name['latest_cumulative_premium_fraction']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _MARKET.fields_by_name['exchange_fee_ratio']._options = None
-  _MARKET.fields_by_name['exchange_fee_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _MARKET.fields_by_name['ecosystem_fund_fee_ratio']._options = None
-  _MARKET.fields_by_name['ecosystem_fund_fee_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _MARKET.fields_by_name['liquidation_fee_ratio']._options = None
-  _MARKET.fields_by_name['liquidation_fee_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _MARKET.fields_by_name['partial_liquidation_ratio']._options = None
-  _MARKET.fields_by_name['partial_liquidation_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _MARKET.fields_by_name['twap_lookback_window']._options = None
-  _MARKET.fields_by_name['twap_lookback_window']._serialized_options = b'\310\336\037\000\230\337\037\001'
-  _MARKET.fields_by_name['prepaid_bad_debt']._options = None
-  _MARKET.fields_by_name['prepaid_bad_debt']._serialized_options = b'\310\336\037\000'
-  _AMM.fields_by_name['pair']._options = None
-  _AMM.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
-  _AMM.fields_by_name['base_reserve']._options = None
-  _AMM.fields_by_name['base_reserve']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _AMM.fields_by_name['quote_reserve']._options = None
-  _AMM.fields_by_name['quote_reserve']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _AMM.fields_by_name['sqrt_depth']._options = None
-  _AMM.fields_by_name['sqrt_depth']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _AMM.fields_by_name['price_multiplier']._options = None
-  _AMM.fields_by_name['price_multiplier']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _AMM.fields_by_name['total_long']._options = None
-  _AMM.fields_by_name['total_long']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _AMM.fields_by_name['total_short']._options = None
-  _AMM.fields_by_name['total_short']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _POSITION.fields_by_name['pair']._options = None
-  _POSITION.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
-  _POSITION.fields_by_name['size']._options = None
-  _POSITION.fields_by_name['size']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _POSITION.fields_by_name['margin']._options = None
-  _POSITION.fields_by_name['margin']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _POSITION.fields_by_name['open_notional']._options = None
-  _POSITION.fields_by_name['open_notional']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _POSITION.fields_by_name['latest_cumulative_premium_fraction']._options = None
-  _POSITION.fields_by_name['latest_cumulative_premium_fraction']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _RESERVESNAPSHOT.fields_by_name['amm']._options = None
-  _RESERVESNAPSHOT.fields_by_name['amm']._serialized_options = b'\310\336\037\000'
-  _DIRECTION._serialized_start=2077
-  _DIRECTION._serialized_end=2136
-  _TWAPCALCOPTION._serialized_start=2138
-  _TWAPCALCOPTION._serialized_end=2241
-  _MARKET._serialized_start=153
-  _MARKET._serialized_end=1059
-  _AMM._serialized_start=1062
-  _AMM._serialized_end=1560
-  _POSITION._serialized_start=1563
-  _POSITION._serialized_end=1994
-  _RESERVESNAPSHOT._serialized_start=1996
-  _RESERVESNAPSHOT._serialized_end=2075
+  DESCRIPTOR._serialized_options = b'Z+github.com/NibiruChain/nibiru/x/vpool/types'
+  _VPOOL.fields_by_name['pair']._options = None
+  _VPOOL.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
+  _VPOOL.fields_by_name['base_asset_reserve']._options = None
+  _VPOOL.fields_by_name['base_asset_reserve']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _VPOOL.fields_by_name['quote_asset_reserve']._options = None
+  _VPOOL.fields_by_name['quote_asset_reserve']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _VPOOL.fields_by_name['config']._options = None
+  _VPOOL.fields_by_name['config']._serialized_options = b'\310\336\037\000'
+  _VPOOLCONFIG.fields_by_name['trade_limit_ratio']._options = None
+  _VPOOLCONFIG.fields_by_name['trade_limit_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _VPOOLCONFIG.fields_by_name['fluctuation_limit_ratio']._options = None
+  _VPOOLCONFIG.fields_by_name['fluctuation_limit_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _VPOOLCONFIG.fields_by_name['max_oracle_spread_ratio']._options = None
+  _VPOOLCONFIG.fields_by_name['max_oracle_spread_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _VPOOLCONFIG.fields_by_name['maintenance_margin_ratio']._options = None
+  _VPOOLCONFIG.fields_by_name['maintenance_margin_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _VPOOLCONFIG.fields_by_name['max_leverage']._options = None
+  _VPOOLCONFIG.fields_by_name['max_leverage']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _CURRENTTWAP.fields_by_name['pair_id']._options = None
+  _CURRENTTWAP.fields_by_name['pair_id']._serialized_options = b'\342\336\037\006PairID'
+  _CURRENTTWAP.fields_by_name['numerator']._options = None
+  _CURRENTTWAP.fields_by_name['numerator']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _CURRENTTWAP.fields_by_name['denominator']._options = None
+  _CURRENTTWAP.fields_by_name['denominator']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _CURRENTTWAP.fields_by_name['price']._options = None
+  _CURRENTTWAP.fields_by_name['price']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _RESERVESNAPSHOT.fields_by_name['pair']._options = None
+  _RESERVESNAPSHOT.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
+  _RESERVESNAPSHOT.fields_by_name['base_asset_reserve']._options = None
+  _RESERVESNAPSHOT.fields_by_name['base_asset_reserve']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _RESERVESNAPSHOT.fields_by_name['quote_asset_reserve']._options = None
+  _RESERVESNAPSHOT.fields_by_name['quote_asset_reserve']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _POOLPRICES.fields_by_name['pair']._options = None
+  _POOLPRICES.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
+  _POOLPRICES.fields_by_name['mark_price']._options = None
+  _POOLPRICES.fields_by_name['mark_price']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
+  _POOLPRICES.fields_by_name['swap_invariant']._options = None
+  _POOLPRICES.fields_by_name['swap_invariant']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Int\362\336\037\025yaml:\"swap_invariant\"\310\336\037\000'
+  _DIRECTION._serialized_start=1610
+  _DIRECTION._serialized_end=1687
+  _TWAPCALCOPTION._serialized_start=1689
+  _TWAPCALCOPTION._serialized_end=1792
+  _VPOOL._serialized_start=91
+  _VPOOL._serialized_end=376
+  _VPOOLCONFIG._serialized_start=379
+  _VPOOLCONFIG._serialized_end=781
+  _CURRENTTWAP._serialized_start=784
+  _CURRENTTWAP._serialized_end=1025
+  _RESERVESNAPSHOT._serialized_start=1028
+  _RESERVESNAPSHOT._serialized_end=1293
+  _POOLPRICES._serialized_start=1296
+  _POOLPRICES._serialized_end=1608
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/state_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/state_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,253 +1,357 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
-import cosmos.base.v1beta1.coin_pb2
+import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
+import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class _Direction:
+class _Side:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _DirectionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Direction.ValueType], builtins.type):
+class _SideEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Side.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-    DIRECTION_UNSPECIFIED: _Direction.ValueType  # 0
-    LONG: _Direction.ValueType  # 1
-    SHORT: _Direction.ValueType  # 2
-
-class Direction(_Direction, metaclass=_DirectionEnumTypeWrapper):
-    """The direction that the user is trading in
-    LONG means the user is going long the base asset (e.g. buy BTC)
-    SHORT means the user is shorting the base asset (e.g. sell BTC)
-    """
-
-DIRECTION_UNSPECIFIED: Direction.ValueType  # 0
-LONG: Direction.ValueType  # 1
-SHORT: Direction.ValueType  # 2
-global___Direction = Direction
+    SIDE_UNSPECIFIED: _Side.ValueType  # 0
+    BUY: _Side.ValueType  # 1
+    SELL: _Side.ValueType  # 2
+
+class Side(_Side, metaclass=_SideEnumTypeWrapper): ...
+
+SIDE_UNSPECIFIED: Side.ValueType  # 0
+BUY: Side.ValueType  # 1
+SELL: Side.ValueType  # 2
+global___Side = Side
 
-class _TwapCalcOption:
+class _PnLCalcOption:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _TwapCalcOptionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_TwapCalcOption.ValueType], builtins.type):
+class _PnLCalcOptionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_PnLCalcOption.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-    TWAP_CALC_OPTION_UNSPECIFIED: _TwapCalcOption.ValueType  # 0
-    SPOT: _TwapCalcOption.ValueType  # 1
-    """Spot price from quote asset reserve / base asset reserve"""
-    QUOTE_ASSET_SWAP: _TwapCalcOption.ValueType  # 2
-    """Swapping with quote assets, output denominated in base assets"""
-    BASE_ASSET_SWAP: _TwapCalcOption.ValueType  # 3
-    """Swapping with base assets, output denominated in quote assets"""
-
-class TwapCalcOption(_TwapCalcOption, metaclass=_TwapCalcOptionEnumTypeWrapper):
-    """Enumerates different options of calculating twap."""
-
-TWAP_CALC_OPTION_UNSPECIFIED: TwapCalcOption.ValueType  # 0
-SPOT: TwapCalcOption.ValueType  # 1
-"""Spot price from quote asset reserve / base asset reserve"""
-QUOTE_ASSET_SWAP: TwapCalcOption.ValueType  # 2
-"""Swapping with quote assets, output denominated in base assets"""
-BASE_ASSET_SWAP: TwapCalcOption.ValueType  # 3
-"""Swapping with base assets, output denominated in quote assets"""
-global___TwapCalcOption = TwapCalcOption
+    PNL_CALC_OPTION_UNSPECIFIED: _PnLCalcOption.ValueType  # 0
+    SPOT_PRICE: _PnLCalcOption.ValueType  # 1
+    TWAP: _PnLCalcOption.ValueType  # 2
+    ORACLE: _PnLCalcOption.ValueType  # 3
+
+class PnLCalcOption(_PnLCalcOption, metaclass=_PnLCalcOptionEnumTypeWrapper): ...
+
+PNL_CALC_OPTION_UNSPECIFIED: PnLCalcOption.ValueType  # 0
+SPOT_PRICE: PnLCalcOption.ValueType  # 1
+TWAP: PnLCalcOption.ValueType  # 2
+ORACLE: PnLCalcOption.ValueType  # 3
+global___PnLCalcOption = PnLCalcOption
+
+class _PnLPreferenceOption:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _PnLPreferenceOptionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_PnLPreferenceOption.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    PNL_PREFERENCE_UNSPECIFIED: _PnLPreferenceOption.ValueType  # 0
+    MAX: _PnLPreferenceOption.ValueType  # 1
+    MIN: _PnLPreferenceOption.ValueType  # 2
+
+class PnLPreferenceOption(_PnLPreferenceOption, metaclass=_PnLPreferenceOptionEnumTypeWrapper): ...
+
+PNL_PREFERENCE_UNSPECIFIED: PnLPreferenceOption.ValueType  # 0
+MAX: PnLPreferenceOption.ValueType  # 1
+MIN: PnLPreferenceOption.ValueType  # 2
+global___PnLPreferenceOption = PnLPreferenceOption
+
+class _MarginCalculationPriceOption:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _MarginCalculationPriceOptionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_MarginCalculationPriceOption.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    MARGIN_CALCULATION_PRICE_OPTION_UNSPECIFIED: _MarginCalculationPriceOption.ValueType  # 0
+    SPOT: _MarginCalculationPriceOption.ValueType  # 1
+    INDEX: _MarginCalculationPriceOption.ValueType  # 2
+    MAX_PNL: _MarginCalculationPriceOption.ValueType  # 3
+
+class MarginCalculationPriceOption(_MarginCalculationPriceOption, metaclass=_MarginCalculationPriceOptionEnumTypeWrapper): ...
+
+MARGIN_CALCULATION_PRICE_OPTION_UNSPECIFIED: MarginCalculationPriceOption.ValueType  # 0
+SPOT: MarginCalculationPriceOption.ValueType  # 1
+INDEX: MarginCalculationPriceOption.ValueType  # 2
+MAX_PNL: MarginCalculationPriceOption.ValueType  # 3
+global___MarginCalculationPriceOption = MarginCalculationPriceOption
 
 @typing_extensions.final
-class Market(google.protobuf.message.Message):
+class Params(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PAIR_FIELD_NUMBER: builtins.int
-    ENABLED_FIELD_NUMBER: builtins.int
-    PRICE_FLUCTUATION_LIMIT_RATIO_FIELD_NUMBER: builtins.int
-    MAINTENANCE_MARGIN_RATIO_FIELD_NUMBER: builtins.int
-    MAX_LEVERAGE_FIELD_NUMBER: builtins.int
-    LATEST_CUMULATIVE_PREMIUM_FRACTION_FIELD_NUMBER: builtins.int
-    EXCHANGE_FEE_RATIO_FIELD_NUMBER: builtins.int
+    STOPPED_FIELD_NUMBER: builtins.int
+    FEE_POOL_FEE_RATIO_FIELD_NUMBER: builtins.int
     ECOSYSTEM_FUND_FEE_RATIO_FIELD_NUMBER: builtins.int
     LIQUIDATION_FEE_RATIO_FIELD_NUMBER: builtins.int
     PARTIAL_LIQUIDATION_RATIO_FIELD_NUMBER: builtins.int
-    FUNDING_RATE_EPOCH_ID_FIELD_NUMBER: builtins.int
+    FUNDING_RATE_INTERVAL_FIELD_NUMBER: builtins.int
     TWAP_LOOKBACK_WINDOW_FIELD_NUMBER: builtins.int
-    PREPAID_BAD_DEBT_FIELD_NUMBER: builtins.int
-    pair: builtins.str
-    """the trading pair represented by this market
-    always BASE:QUOTE, e.g. BTC:NUSD or ETH:NUSD
-    """
-    enabled: builtins.bool
-    """whether or not the market is enabled"""
-    price_fluctuation_limit_ratio: builtins.str
-    """percentage that a single open or close position can alter the reserve
-    amounts
-    """
-    maintenance_margin_ratio: builtins.str
-    """the minimum margin ratio which a user must maintain on this market"""
-    max_leverage: builtins.str
-    """the maximum leverage a user is able to be taken on this market"""
-    latest_cumulative_premium_fraction: builtins.str
-    """Latest cumulative premium fraction for a given pair.
-    Calculated once per funding rate interval.
-    A premium fraction is the difference between mark and index, divided by the
-    number of payments per day. (mark - index) / # payments in a day
-    """
-    exchange_fee_ratio: builtins.str
-    """the percentage of the notional given to the exchange when trading"""
+    WHITELISTED_LIQUIDATORS_FIELD_NUMBER: builtins.int
+    stopped: builtins.bool
+    """stopped identifies if the perp exchange is stopped or not"""
+    fee_pool_fee_ratio: builtins.str
+    """FeePoolFeeRatio is the ratio transferred to the the fee pool"""
     ecosystem_fund_fee_ratio: builtins.str
-    """the percentage of the notional transferred to the ecosystem fund when
-    trading
-    """
+    """EcosystemFundFeeRatio is the ratio transferred to the PerpEF."""
     liquidation_fee_ratio: builtins.str
-    """the percentage of liquidated position that will be
+    """LiquidationFeeRatio is the percentage of liquidated position that will be
     given to out as a reward. Half of the liquidation fee is given to the
     liquidator, and the other half is given to the ecosystem fund.
     """
     partial_liquidation_ratio: builtins.str
-    """the portion of the position size we try to liquidate if the available
-    margin is higher than liquidation fee
+    """PartialLiquidationRatio is the share we try to liquidate if the margin is
+    higher than liquidation fee
     """
-    funding_rate_epoch_id: builtins.str
+    funding_rate_interval: builtins.str
     """specifies the interval on which the funding rate is updated"""
     @property
     def twap_lookback_window(self) -> google.protobuf.duration_pb2.Duration:
         """amount of time to look back for TWAP calculations"""
     @property
-    def prepaid_bad_debt(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
-        """the amount of collateral already credited from the ecosystem fund"""
+    def whitelisted_liquidators(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """whitelisted_liquidators defines the list of addresses
+        which are allowed to liquidate a position.
+        """
     def __init__(
         self,
         *,
-        pair: builtins.str = ...,
-        enabled: builtins.bool = ...,
-        price_fluctuation_limit_ratio: builtins.str = ...,
-        maintenance_margin_ratio: builtins.str = ...,
-        max_leverage: builtins.str = ...,
-        latest_cumulative_premium_fraction: builtins.str = ...,
-        exchange_fee_ratio: builtins.str = ...,
+        stopped: builtins.bool = ...,
+        fee_pool_fee_ratio: builtins.str = ...,
         ecosystem_fund_fee_ratio: builtins.str = ...,
         liquidation_fee_ratio: builtins.str = ...,
         partial_liquidation_ratio: builtins.str = ...,
-        funding_rate_epoch_id: builtins.str = ...,
+        funding_rate_interval: builtins.str = ...,
         twap_lookback_window: google.protobuf.duration_pb2.Duration | None = ...,
-        prepaid_bad_debt: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        whitelisted_liquidators: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["prepaid_bad_debt", b"prepaid_bad_debt", "twap_lookback_window", b"twap_lookback_window"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ecosystem_fund_fee_ratio", b"ecosystem_fund_fee_ratio", "enabled", b"enabled", "exchange_fee_ratio", b"exchange_fee_ratio", "funding_rate_epoch_id", b"funding_rate_epoch_id", "latest_cumulative_premium_fraction", b"latest_cumulative_premium_fraction", "liquidation_fee_ratio", b"liquidation_fee_ratio", "maintenance_margin_ratio", b"maintenance_margin_ratio", "max_leverage", b"max_leverage", "pair", b"pair", "partial_liquidation_ratio", b"partial_liquidation_ratio", "prepaid_bad_debt", b"prepaid_bad_debt", "price_fluctuation_limit_ratio", b"price_fluctuation_limit_ratio", "twap_lookback_window", b"twap_lookback_window"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["twap_lookback_window", b"twap_lookback_window"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["ecosystem_fund_fee_ratio", b"ecosystem_fund_fee_ratio", "fee_pool_fee_ratio", b"fee_pool_fee_ratio", "funding_rate_interval", b"funding_rate_interval", "liquidation_fee_ratio", b"liquidation_fee_ratio", "partial_liquidation_ratio", b"partial_liquidation_ratio", "stopped", b"stopped", "twap_lookback_window", b"twap_lookback_window", "whitelisted_liquidators", b"whitelisted_liquidators"]) -> None: ...
 
-global___Market = Market
-
-@typing_extensions.final
-class AMM(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    PAIR_FIELD_NUMBER: builtins.int
-    BASE_RESERVE_FIELD_NUMBER: builtins.int
-    QUOTE_RESERVE_FIELD_NUMBER: builtins.int
-    SQRT_DEPTH_FIELD_NUMBER: builtins.int
-    PRICE_MULTIPLIER_FIELD_NUMBER: builtins.int
-    TOTAL_LONG_FIELD_NUMBER: builtins.int
-    TOTAL_SHORT_FIELD_NUMBER: builtins.int
-    pair: builtins.str
-    """identifies the market this AMM belongs to"""
-    base_reserve: builtins.str
-    """the amount of base reserves this AMM has"""
-    quote_reserve: builtins.str
-    """the amount of quote reserves this AMM has"""
-    sqrt_depth: builtins.str
-    """sqrt(k)"""
-    price_multiplier: builtins.str
-    """the price multiplier of the dynamic AMM"""
-    total_long: builtins.str
-    """Total long refers to the sum of long open notional in base."""
-    total_short: builtins.str
-    """Total short refers to the sum of short open notional in base."""
-    def __init__(
-        self,
-        *,
-        pair: builtins.str = ...,
-        base_reserve: builtins.str = ...,
-        quote_reserve: builtins.str = ...,
-        sqrt_depth: builtins.str = ...,
-        price_multiplier: builtins.str = ...,
-        total_long: builtins.str = ...,
-        total_short: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["base_reserve", b"base_reserve", "pair", b"pair", "price_multiplier", b"price_multiplier", "quote_reserve", b"quote_reserve", "sqrt_depth", b"sqrt_depth", "total_long", b"total_long", "total_short", b"total_short"]) -> None: ...
-
-global___AMM = AMM
+global___Params = Params
 
 @typing_extensions.final
 class Position(google.protobuf.message.Message):
+    """Position identifies and records information on a user's position on one of
+    the virtual liquidity pools.
+    """
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TRADER_ADDRESS_FIELD_NUMBER: builtins.int
     PAIR_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     MARGIN_FIELD_NUMBER: builtins.int
     OPEN_NOTIONAL_FIELD_NUMBER: builtins.int
     LATEST_CUMULATIVE_PREMIUM_FRACTION_FIELD_NUMBER: builtins.int
-    LAST_UPDATED_BLOCK_NUMBER_FIELD_NUMBER: builtins.int
+    BLOCK_NUMBER_FIELD_NUMBER: builtins.int
     trader_address: builtins.str
     """address identifies the address owner of this position"""
     pair: builtins.str
     """pair identifies the pair associated with this position"""
     size: builtins.str
-    """the position size"""
+    """Position size."""
     margin: builtins.str
-    """amount of margin remaining in the position"""
+    """Amount of margin remaining in the position."""
     open_notional: builtins.str
-    """value of position in quote assets when opened"""
+    """OpenNotional is the quote denom value of the position when opening.
+    Used to calculate PnL.
+    """
     latest_cumulative_premium_fraction: builtins.str
     """The most recent cumulative premium fraction this position has.
     Used to calculate the next funding payment.
     """
-    last_updated_block_number: builtins.int
-    """last block number this position was updated"""
+    block_number: builtins.int
+    """BlockNumber is the last block number when this position was updated."""
     def __init__(
         self,
         *,
         trader_address: builtins.str = ...,
         pair: builtins.str = ...,
         size: builtins.str = ...,
         margin: builtins.str = ...,
         open_notional: builtins.str = ...,
         latest_cumulative_premium_fraction: builtins.str = ...,
-        last_updated_block_number: builtins.int = ...,
+        block_number: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["last_updated_block_number", b"last_updated_block_number", "latest_cumulative_premium_fraction", b"latest_cumulative_premium_fraction", "margin", b"margin", "open_notional", b"open_notional", "pair", b"pair", "size", b"size", "trader_address", b"trader_address"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["block_number", b"block_number", "latest_cumulative_premium_fraction", b"latest_cumulative_premium_fraction", "margin", b"margin", "open_notional", b"open_notional", "pair", b"pair", "size", b"size", "trader_address", b"trader_address"]) -> None: ...
 
 global___Position = Position
 
 @typing_extensions.final
-class ReserveSnapshot(google.protobuf.message.Message):
-    """a snapshot of the perp.amm's reserves at a given point in time"""
+class PairMetadata(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    PAIR_FIELD_NUMBER: builtins.int
+    LATEST_CUMULATIVE_PREMIUM_FRACTION_FIELD_NUMBER: builtins.int
+    pair: builtins.str
+    latest_cumulative_premium_fraction: builtins.str
+    """Latest cumulative premium fraction for a given pair.
+    Calculated once per funding rate interval.
+    A premium fraction is the difference between mark and index, divided by the number of payments per day.
+    (mark - index) / # payments in a day
+    """
+    def __init__(
+        self,
+        *,
+        pair: builtins.str = ...,
+        latest_cumulative_premium_fraction: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["latest_cumulative_premium_fraction", b"latest_cumulative_premium_fraction", "pair", b"pair"]) -> None: ...
+
+global___PairMetadata = PairMetadata
+
+@typing_extensions.final
+class PrepaidBadDebt(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DENOM_FIELD_NUMBER: builtins.int
+    AMOUNT_FIELD_NUMBER: builtins.int
+    denom: builtins.str
+    amount: builtins.str
+    def __init__(
+        self,
+        *,
+        denom: builtins.str = ...,
+        amount: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "denom", b"denom"]) -> None: ...
+
+global___PrepaidBadDebt = PrepaidBadDebt
+
+@typing_extensions.final
+class PositionResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    POSITION_FIELD_NUMBER: builtins.int
+    EXCHANGED_NOTIONAL_VALUE_FIELD_NUMBER: builtins.int
+    EXCHANGED_POSITION_SIZE_FIELD_NUMBER: builtins.int
+    BAD_DEBT_FIELD_NUMBER: builtins.int
+    FUNDING_PAYMENT_FIELD_NUMBER: builtins.int
+    REALIZED_PNL_FIELD_NUMBER: builtins.int
+    UNREALIZED_PNL_AFTER_FIELD_NUMBER: builtins.int
+    MARGIN_TO_VAULT_FIELD_NUMBER: builtins.int
+    POSITION_NOTIONAL_FIELD_NUMBER: builtins.int
+    @property
+    def position(self) -> global___Position: ...
+    exchanged_notional_value: builtins.str
+    """The amount of quote assets exchanged."""
+    exchanged_position_size: builtins.str
+    """The amount of base assets exchanged."""
+    bad_debt: builtins.str
+    """The amount of bad debt accrued during this position change.
+    Measured in absolute value of quote units.
+    If greater than zero, then the position change event will likely fail.
+    """
+    funding_payment: builtins.str
+    """The funding payment applied on this position change."""
+    realized_pnl: builtins.str
+    """The amount of PnL realized on this position changed, measured in quote
+    units.
+    """
+    unrealized_pnl_after: builtins.str
+    """The unrealized PnL in the position after the position change."""
+    margin_to_vault: builtins.str
+    """The amount of margin the trader has to give to the vault.
+    A negative value means the vault pays the trader.
+    """
+    position_notional: builtins.str
+    """The position's notional value after the position change, measured in quote
+    units.
+    """
+    def __init__(
+        self,
+        *,
+        position: global___Position | None = ...,
+        exchanged_notional_value: builtins.str = ...,
+        exchanged_position_size: builtins.str = ...,
+        bad_debt: builtins.str = ...,
+        funding_payment: builtins.str = ...,
+        realized_pnl: builtins.str = ...,
+        unrealized_pnl_after: builtins.str = ...,
+        margin_to_vault: builtins.str = ...,
+        position_notional: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["position", b"position"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bad_debt", b"bad_debt", "exchanged_notional_value", b"exchanged_notional_value", "exchanged_position_size", b"exchanged_position_size", "funding_payment", b"funding_payment", "margin_to_vault", b"margin_to_vault", "position", b"position", "position_notional", b"position_notional", "realized_pnl", b"realized_pnl", "unrealized_pnl_after", b"unrealized_pnl_after"]) -> None: ...
+
+global___PositionResp = PositionResp
+
+@typing_extensions.final
+class LiquidateResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    AMM_FIELD_NUMBER: builtins.int
-    TIMESTAMP_MS_FIELD_NUMBER: builtins.int
+    BAD_DEBT_FIELD_NUMBER: builtins.int
+    FEE_TO_LIQUIDATOR_FIELD_NUMBER: builtins.int
+    FEE_TO_PERP_ECOSYSTEM_FUND_FIELD_NUMBER: builtins.int
+    LIQUIDATOR_FIELD_NUMBER: builtins.int
+    POSITION_RESP_FIELD_NUMBER: builtins.int
+    bad_debt: builtins.str
+    """Amount of bad debt created by the liquidation event"""
+    fee_to_liquidator: builtins.str
+    """Fee paid to the liquidator"""
+    fee_to_perp_ecosystem_fund: builtins.str
+    """Fee paid to the Perp EF fund"""
+    liquidator: builtins.str
+    """Address of the liquidator"""
     @property
-    def amm(self) -> global___AMM: ...
-    timestamp_ms: builtins.int
-    """milliseconds since unix epoch"""
+    def position_resp(self) -> global___PositionResp:
+        """Position response from the close or open reverse position"""
+    def __init__(
+        self,
+        *,
+        bad_debt: builtins.str = ...,
+        fee_to_liquidator: builtins.str = ...,
+        fee_to_perp_ecosystem_fund: builtins.str = ...,
+        liquidator: builtins.str = ...,
+        position_resp: global___PositionResp | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["position_resp", b"position_resp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bad_debt", b"bad_debt", "fee_to_liquidator", b"fee_to_liquidator", "fee_to_perp_ecosystem_fund", b"fee_to_perp_ecosystem_fund", "liquidator", b"liquidator", "position_resp", b"position_resp"]) -> None: ...
+
+global___LiquidateResp = LiquidateResp
+
+@typing_extensions.final
+class Metrics(google.protobuf.message.Message):
+    """PoolMetrics is a structure that displays a snapshot of perp metrics for each pair."""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    PAIR_FIELD_NUMBER: builtins.int
+    NET_SIZE_FIELD_NUMBER: builtins.int
+    VOLUMEQUOTE_FIELD_NUMBER: builtins.int
+    VOLUMEBASE_FIELD_NUMBER: builtins.int
+    pair: builtins.str
+    """Pair identifier for the two assets. Always in format 'base:quote'"""
+    net_size: builtins.str
+    """Sum of all active position sizes for the pair."""
+    volumeQuote: builtins.str
+    """Total notional volume for the pair."""
+    volumeBase: builtins.str
+    """Total size volume for the pair."""
     def __init__(
         self,
         *,
-        amm: global___AMM | None = ...,
-        timestamp_ms: builtins.int = ...,
+        pair: builtins.str = ...,
+        net_size: builtins.str = ...,
+        volumeQuote: builtins.str = ...,
+        volumeBase: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["amm", b"amm"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["amm", b"amm", "timestamp_ms", b"timestamp_ms"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["net_size", b"net_size", "pair", b"pair", "volumeBase", b"volumeBase", "volumeQuote", b"volumeQuote"]) -> None: ...
 
-global___ReserveSnapshot = ReserveSnapshot
+global___Metrics = Metrics
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/tx_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: perp/v2/tx.proto
+# source: perp/v1/tx.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from perp.v2 import state_pb2 as perp_dot_v2_dot_state__pb2
+from perp.v1 import state_pb2 as perp_dot_v1_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10perp/v2/tx.proto\x12\x0enibiru.perp.v2\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x13perp/v2/state.proto\"\x9b\x01\n\x0fMsgRemoveMargin\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12/\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\xc3\x01\n\x17MsgRemoveMarginResponse\x12\x33\n\nmargin_out\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12G\n\x0f\x66unding_payment\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12*\n\x08position\x18\x03 \x01(\x0b\x32\x18.nibiru.perp.v2.Position\"\x98\x01\n\x0cMsgAddMargin\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12/\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\x8b\x01\n\x14MsgAddMarginResponse\x12G\n\x0f\x66unding_payment\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12*\n\x08position\x18\x02 \x01(\x0b\x32\x18.nibiru.perp.v2.Position\"\xd0\x01\n\x11MsgMultiLiquidate\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12\x43\n\x0cliquidations\x18\x02 \x03(\x0b\x32-.nibiru.perp.v2.MsgMultiLiquidate.Liquidation\x1a\x66\n\x0bLiquidation\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x0e\n\x06trader\x18\x02 \x01(\t\"\x97\x02\n\x19MsgMultiLiquidateResponse\x12S\n\x0cliquidations\x18\x01 \x03(\x0b\x32=.nibiru.perp.v2.MsgMultiLiquidateResponse.LiquidationResponse\x1a\xa4\x01\n\x13LiquidationResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\x37\n\x0eliquidator_fee\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x34\n\x0bperp_ef_fee\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\xf2\x02\n\x0fMsgOpenPosition\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\'\n\x04side\x18\x03 \x01(\x0e\x32\x19.nibiru.perp.v2.Direction\x12J\n\x12quote_asset_amount\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\x12@\n\x08leverage\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x62\x61se_asset_amount_limit\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"\xd9\x04\n\x17MsgOpenPositionResponse\x12*\n\x08position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v2.Position\x12P\n\x18\x65xchanged_notional_value\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x65xchanged_position_size\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12G\n\x0f\x66unding_payment\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0crealized_pnl\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12L\n\x14unrealized_pnl_after\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12G\n\x0fmargin_to_vault\x18\x07 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12I\n\x11position_notional\x18\x08 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"k\n\x10MsgClosePosition\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\"\x96\x03\n\x18MsgClosePositionResponse\x12P\n\x18\x65xchanged_notional_value\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x65xchanged_position_size\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12G\n\x0f\x66unding_payment\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0crealized_pnl\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12H\n\x10margin_to_trader\x18\x07 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"p\n\x18MsgDonateToEcosystemFund\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12\x44\n\x08\x64onation\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x17\xf2\xde\x1f\x0fyaml:\"donation\"\xc8\xde\x1f\x00\"\"\n MsgDonateToEcosystemFundResponse2\xb3\x06\n\x03Msg\x12\x7f\n\x0cRemoveMargin\x12\x1f.nibiru.perp.v2.MsgRemoveMargin\x1a\'.nibiru.perp.v2.MsgRemoveMarginResponse\"%\x82\xd3\xe4\x93\x02\x1f\"\x1d/nibiru/perp/v2/remove_margin\x12s\n\tAddMargin\x12\x1c.nibiru.perp.v2.MsgAddMargin\x1a$.nibiru.perp.v2.MsgAddMarginResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/perp/v2/add_margin\x12\x86\x01\n\x0eMultiLiquidate\x12!.nibiru.perp.v2.MsgMultiLiquidate\x1a).nibiru.perp.v2.MsgMultiLiquidateResponse\"&\x82\xd3\xe4\x93\x02 \"\x1e/nibiru/perp/v2/multiliquidate\x12\x7f\n\x0cOpenPosition\x12\x1f.nibiru.perp.v2.MsgOpenPosition\x1a\'.nibiru.perp.v2.MsgOpenPositionResponse\"%\x82\xd3\xe4\x93\x02\x1f\"\x1d/nibiru/perp/v2/open_position\x12\x83\x01\n\rClosePosition\x12 .nibiru.perp.v2.MsgClosePosition\x1a(.nibiru.perp.v2.MsgClosePositionResponse\"&\x82\xd3\xe4\x93\x02 \"\x1e/nibiru/perp/v2/close_position\x12\xa5\x01\n\x15\x44onateToEcosystemFund\x12(.nibiru.perp.v2.MsgDonateToEcosystemFund\x1a\x30.nibiru.perp.v2.MsgDonateToEcosystemFundResponse\"0\x82\xd3\xe4\x93\x02*\"(/nibiru/perp/v2/donate_to_ecosystem_fundB/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10perp/v1/tx.proto\x12\x0enibiru.perp.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x13perp/v1/state.proto\"\x9b\x01\n\x0fMsgRemoveMargin\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12/\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\xc3\x01\n\x17MsgRemoveMarginResponse\x12\x33\n\nmargin_out\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12G\n\x0f\x66unding_payment\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12*\n\x08position\x18\x03 \x01(\x0b\x32\x18.nibiru.perp.v1.Position\"\x98\x01\n\x0cMsgAddMargin\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12/\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\x8b\x01\n\x14MsgAddMarginResponse\x12G\n\x0f\x66unding_payment\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12*\n\x08position\x18\x02 \x01(\x0b\x32\x18.nibiru.perp.v1.Position\"\xd0\x01\n\x11MsgMultiLiquidate\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12\x43\n\x0cliquidations\x18\x02 \x03(\x0b\x32-.nibiru.perp.v1.MsgMultiLiquidate.Liquidation\x1a\x66\n\x0bLiquidation\x12G\n\x04pair\x18\x01 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\x0e\n\x06trader\x18\x02 \x01(\t\"\x97\x02\n\x19MsgMultiLiquidateResponse\x12S\n\x0cliquidations\x18\x01 \x03(\x0b\x32=.nibiru.perp.v1.MsgMultiLiquidateResponse.LiquidationResponse\x1a\xa4\x01\n\x13LiquidationResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\x37\n\x0eliquidator_fee\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x34\n\x0bperp_ef_fee\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\xed\x02\n\x0fMsgOpenPosition\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\x12\"\n\x04side\x18\x03 \x01(\x0e\x32\x14.nibiru.perp.v1.Side\x12J\n\x12quote_asset_amount\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\x12@\n\x08leverage\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x62\x61se_asset_amount_limit\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"\xd9\x04\n\x17MsgOpenPositionResponse\x12*\n\x08position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v1.Position\x12P\n\x18\x65xchanged_notional_value\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x65xchanged_position_size\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12G\n\x0f\x66unding_payment\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0crealized_pnl\x18\x05 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12L\n\x14unrealized_pnl_after\x18\x06 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12G\n\x0fmargin_to_vault\x18\x07 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12I\n\x11position_notional\x18\x08 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"k\n\x10MsgClosePosition\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12G\n\x04pair\x18\x02 \x01(\tB9\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.Pair\xc8\xde\x1f\x00\"\x96\x03\n\x18MsgClosePositionResponse\x12P\n\x18\x65xchanged_notional_value\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12O\n\x17\x65xchanged_position_size\x18\x02 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12G\n\x0f\x66unding_payment\x18\x03 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12\x44\n\x0crealized_pnl\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x12H\n\x10margin_to_trader\x18\x07 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"p\n\x18MsgDonateToEcosystemFund\x12\x0e\n\x06sender\x18\x01 \x01(\t\x12\x44\n\x08\x64onation\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x17\xf2\xde\x1f\x0fyaml:\"donation\"\xc8\xde\x1f\x00\"\"\n MsgDonateToEcosystemFundResponse2\xa1\x06\n\x03Msg\x12|\n\x0cRemoveMargin\x12\x1f.nibiru.perp.v1.MsgRemoveMargin\x1a\'.nibiru.perp.v1.MsgRemoveMarginResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/perp/remove_margin\x12p\n\tAddMargin\x12\x1c.nibiru.perp.v1.MsgAddMargin\x1a$.nibiru.perp.v1.MsgAddMarginResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/nibiru/perp/add_margin\x12\x83\x01\n\x0eMultiLiquidate\x12!.nibiru.perp.v1.MsgMultiLiquidate\x1a).nibiru.perp.v1.MsgMultiLiquidateResponse\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/nibiru/perp/multiliquidate\x12|\n\x0cOpenPosition\x12\x1f.nibiru.perp.v1.MsgOpenPosition\x1a\'.nibiru.perp.v1.MsgOpenPositionResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/perp/open_position\x12\x80\x01\n\rClosePosition\x12 .nibiru.perp.v1.MsgClosePosition\x1a(.nibiru.perp.v1.MsgClosePositionResponse\"#\x82\xd3\xe4\x93\x02\x1d\"\x1b/nibiru/perp/close_position\x12\xa2\x01\n\x15\x44onateToEcosystemFund\x12(.nibiru.perp.v1.MsgDonateToEcosystemFund\x1a\x30.nibiru.perp.v1.MsgDonateToEcosystemFundResponse\"-\x82\xd3\xe4\x93\x02\'\"%/nibiru/perp/donate_to_ecosystem_fundB,Z*github.com/NibiruChain/nibiru/x/perp/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v2.tx_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'perp.v1.tx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/NibiruChain/nibiru/x/perp/v2/types'
+  DESCRIPTOR._serialized_options = b'Z*github.com/NibiruChain/nibiru/x/perp/types'
   _MSGREMOVEMARGIN.fields_by_name['pair']._options = None
   _MSGREMOVEMARGIN.fields_by_name['pair']._serialized_options = b'\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair\310\336\037\000'
   _MSGREMOVEMARGIN.fields_by_name['margin']._options = None
   _MSGREMOVEMARGIN.fields_by_name['margin']._serialized_options = b'\310\336\037\000'
   _MSGREMOVEMARGINRESPONSE.fields_by_name['margin_out']._options = None
   _MSGREMOVEMARGINRESPONSE.fields_by_name['margin_out']._serialized_options = b'\310\336\037\000'
   _MSGREMOVEMARGINRESPONSE.fields_by_name['funding_payment']._options = None
@@ -78,25 +78,25 @@
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['realized_pnl']._options = None
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['realized_pnl']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['margin_to_trader']._options = None
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['margin_to_trader']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _MSGDONATETOECOSYSTEMFUND.fields_by_name['donation']._options = None
   _MSGDONATETOECOSYSTEMFUND.fields_by_name['donation']._serialized_options = b'\362\336\037\017yaml:\"donation\"\310\336\037\000'
   _MSG.methods_by_name['RemoveMargin']._options = None
-  _MSG.methods_by_name['RemoveMargin']._serialized_options = b'\202\323\344\223\002\037\"\035/nibiru/perp/v2/remove_margin'
+  _MSG.methods_by_name['RemoveMargin']._serialized_options = b'\202\323\344\223\002\034\"\032/nibiru/perp/remove_margin'
   _MSG.methods_by_name['AddMargin']._options = None
-  _MSG.methods_by_name['AddMargin']._serialized_options = b'\202\323\344\223\002\034\"\032/nibiru/perp/v2/add_margin'
+  _MSG.methods_by_name['AddMargin']._serialized_options = b'\202\323\344\223\002\031\"\027/nibiru/perp/add_margin'
   _MSG.methods_by_name['MultiLiquidate']._options = None
-  _MSG.methods_by_name['MultiLiquidate']._serialized_options = b'\202\323\344\223\002 \"\036/nibiru/perp/v2/multiliquidate'
+  _MSG.methods_by_name['MultiLiquidate']._serialized_options = b'\202\323\344\223\002\035\"\033/nibiru/perp/multiliquidate'
   _MSG.methods_by_name['OpenPosition']._options = None
-  _MSG.methods_by_name['OpenPosition']._serialized_options = b'\202\323\344\223\002\037\"\035/nibiru/perp/v2/open_position'
+  _MSG.methods_by_name['OpenPosition']._serialized_options = b'\202\323\344\223\002\034\"\032/nibiru/perp/open_position'
   _MSG.methods_by_name['ClosePosition']._options = None
-  _MSG.methods_by_name['ClosePosition']._serialized_options = b'\202\323\344\223\002 \"\036/nibiru/perp/v2/close_position'
+  _MSG.methods_by_name['ClosePosition']._serialized_options = b'\202\323\344\223\002\035\"\033/nibiru/perp/close_position'
   _MSG.methods_by_name['DonateToEcosystemFund']._options = None
-  _MSG.methods_by_name['DonateToEcosystemFund']._serialized_options = b'\202\323\344\223\002*\"(/nibiru/perp/v2/donate_to_ecosystem_fund'
+  _MSG.methods_by_name['DonateToEcosystemFund']._serialized_options = b'\202\323\344\223\002\'\"%/nibiru/perp/donate_to_ecosystem_fund'
   _MSGREMOVEMARGIN._serialized_start=142
   _MSGREMOVEMARGIN._serialized_end=297
   _MSGREMOVEMARGINRESPONSE._serialized_start=300
   _MSGREMOVEMARGINRESPONSE._serialized_end=495
   _MSGADDMARGIN._serialized_start=498
   _MSGADDMARGIN._serialized_end=650
   _MSGADDMARGINRESPONSE._serialized_start=653
@@ -106,21 +106,21 @@
   _MSGMULTILIQUIDATE_LIQUIDATION._serialized_start=901
   _MSGMULTILIQUIDATE_LIQUIDATION._serialized_end=1003
   _MSGMULTILIQUIDATERESPONSE._serialized_start=1006
   _MSGMULTILIQUIDATERESPONSE._serialized_end=1285
   _MSGMULTILIQUIDATERESPONSE_LIQUIDATIONRESPONSE._serialized_start=1121
   _MSGMULTILIQUIDATERESPONSE_LIQUIDATIONRESPONSE._serialized_end=1285
   _MSGOPENPOSITION._serialized_start=1288
-  _MSGOPENPOSITION._serialized_end=1658
-  _MSGOPENPOSITIONRESPONSE._serialized_start=1661
-  _MSGOPENPOSITIONRESPONSE._serialized_end=2262
-  _MSGCLOSEPOSITION._serialized_start=2264
-  _MSGCLOSEPOSITION._serialized_end=2371
-  _MSGCLOSEPOSITIONRESPONSE._serialized_start=2374
-  _MSGCLOSEPOSITIONRESPONSE._serialized_end=2780
-  _MSGDONATETOECOSYSTEMFUND._serialized_start=2782
-  _MSGDONATETOECOSYSTEMFUND._serialized_end=2894
-  _MSGDONATETOECOSYSTEMFUNDRESPONSE._serialized_start=2896
-  _MSGDONATETOECOSYSTEMFUNDRESPONSE._serialized_end=2930
-  _MSG._serialized_start=2933
-  _MSG._serialized_end=3752
+  _MSGOPENPOSITION._serialized_end=1653
+  _MSGOPENPOSITIONRESPONSE._serialized_start=1656
+  _MSGOPENPOSITIONRESPONSE._serialized_end=2257
+  _MSGCLOSEPOSITION._serialized_start=2259
+  _MSGCLOSEPOSITION._serialized_end=2366
+  _MSGCLOSEPOSITIONRESPONSE._serialized_start=2369
+  _MSGCLOSEPOSITIONRESPONSE._serialized_end=2775
+  _MSGDONATETOECOSYSTEMFUND._serialized_start=2777
+  _MSGDONATETOECOSYSTEMFUND._serialized_end=2889
+  _MSGDONATETOECOSYSTEMFUNDRESPONSE._serialized_start=2891
+  _MSGDONATETOECOSYSTEMFUNDRESPONSE._serialized_end=2925
+  _MSG._serialized_start=2928
+  _MSG._serialized_end=3729
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/tx_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import builtins
 import collections.abc
 import cosmos.base.v1beta1.coin_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import perp.v2.state_pb2
+import perp.v1.state_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -55,22 +55,22 @@
     POSITION_FIELD_NUMBER: builtins.int
     @property
     def margin_out(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
         """tokens transferred back to the trader"""
     funding_payment: builtins.str
     """the funding payment applied on this position interaction"""
     @property
-    def position(self) -> perp.v2.state_pb2.Position:
+    def position(self) -> perp.v1.state_pb2.Position:
         """The resulting position"""
     def __init__(
         self,
         *,
         margin_out: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
         funding_payment: builtins.str = ...,
-        position: perp.v2.state_pb2.Position | None = ...,
+        position: perp.v1.state_pb2.Position | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["margin_out", b"margin_out", "position", b"position"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["funding_payment", b"funding_payment", "margin_out", b"margin_out", "position", b"position"]) -> None: ...
 
 global___MsgRemoveMarginResponse = MsgRemoveMarginResponse
 
 @typing_extensions.final
@@ -105,20 +105,20 @@
 class MsgAddMarginResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FUNDING_PAYMENT_FIELD_NUMBER: builtins.int
     POSITION_FIELD_NUMBER: builtins.int
     funding_payment: builtins.str
     @property
-    def position(self) -> perp.v2.state_pb2.Position: ...
+    def position(self) -> perp.v1.state_pb2.Position: ...
     def __init__(
         self,
         *,
         funding_payment: builtins.str = ...,
-        position: perp.v2.state_pb2.Position | None = ...,
+        position: perp.v1.state_pb2.Position | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["position", b"position"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["funding_payment", b"funding_payment", "position", b"position"]) -> None: ...
 
 global___MsgAddMarginResponse = MsgAddMarginResponse
 
 @typing_extensions.final
@@ -210,24 +210,24 @@
     PAIR_FIELD_NUMBER: builtins.int
     SIDE_FIELD_NUMBER: builtins.int
     QUOTE_ASSET_AMOUNT_FIELD_NUMBER: builtins.int
     LEVERAGE_FIELD_NUMBER: builtins.int
     BASE_ASSET_AMOUNT_LIMIT_FIELD_NUMBER: builtins.int
     sender: builtins.str
     pair: builtins.str
-    side: perp.v2.state_pb2.Direction.ValueType
+    side: perp.v1.state_pb2.Side.ValueType
     quote_asset_amount: builtins.str
     leverage: builtins.str
     base_asset_amount_limit: builtins.str
     def __init__(
         self,
         *,
         sender: builtins.str = ...,
         pair: builtins.str = ...,
-        side: perp.v2.state_pb2.Direction.ValueType = ...,
+        side: perp.v1.state_pb2.Side.ValueType = ...,
         quote_asset_amount: builtins.str = ...,
         leverage: builtins.str = ...,
         base_asset_amount_limit: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_asset_amount_limit", b"base_asset_amount_limit", "leverage", b"leverage", "pair", b"pair", "quote_asset_amount", b"quote_asset_amount", "sender", b"sender", "side", b"side"]) -> None: ...
 
 global___MsgOpenPosition = MsgOpenPosition
@@ -241,43 +241,35 @@
     EXCHANGED_POSITION_SIZE_FIELD_NUMBER: builtins.int
     FUNDING_PAYMENT_FIELD_NUMBER: builtins.int
     REALIZED_PNL_FIELD_NUMBER: builtins.int
     UNREALIZED_PNL_AFTER_FIELD_NUMBER: builtins.int
     MARGIN_TO_VAULT_FIELD_NUMBER: builtins.int
     POSITION_NOTIONAL_FIELD_NUMBER: builtins.int
     @property
-    def position(self) -> perp.v2.state_pb2.Position: ...
+    def position(self) -> perp.v1.state_pb2.Position: ...
     exchanged_notional_value: builtins.str
     """The amount of quote assets exchanged."""
     exchanged_position_size: builtins.str
     """The amount of base assets exchanged."""
     funding_payment: builtins.str
-    """The funding payment applied on this position change, measured in quote
-    units.
-    """
+    """The funding payment applied on this position change, measured in quote units."""
     realized_pnl: builtins.str
-    """The amount of PnL realized on this position changed, measured in quote
-    units.
-    """
+    """The amount of PnL realized on this position changed, measured in quote units."""
     unrealized_pnl_after: builtins.str
-    """The unrealized PnL in the position after the position change, measured in
-    quote units.
-    """
+    """The unrealized PnL in the position after the position change, measured in quote units."""
     margin_to_vault: builtins.str
     """The amount of margin the trader has to give to the vault.
     A negative value means the vault pays the trader.
     """
     position_notional: builtins.str
-    """The position's notional value after the position change, measured in quote
-    units.
-    """
+    """The position's notional value after the position change, measured in quote units."""
     def __init__(
         self,
         *,
-        position: perp.v2.state_pb2.Position | None = ...,
+        position: perp.v1.state_pb2.Position | None = ...,
         exchanged_notional_value: builtins.str = ...,
         exchanged_position_size: builtins.str = ...,
         funding_payment: builtins.str = ...,
         realized_pnl: builtins.str = ...,
         unrealized_pnl_after: builtins.str = ...,
         margin_to_vault: builtins.str = ...,
         position_notional: builtins.str = ...,
@@ -317,24 +309,20 @@
     REALIZED_PNL_FIELD_NUMBER: builtins.int
     MARGIN_TO_TRADER_FIELD_NUMBER: builtins.int
     exchanged_notional_value: builtins.str
     """The amount of quote assets exchanged."""
     exchanged_position_size: builtins.str
     """The amount of base assets exchanged."""
     funding_payment: builtins.str
-    """The funding payment applied on this position change, measured in quote
-    units.
-    """
+    """The funding payment applied on this position change, measured in quote units."""
     realized_pnl: builtins.str
-    """The amount of PnL realized on this position changed, measured in quote
-    units.
-    """
+    """The amount of PnL realized on this position changed, measured in quote units."""
     margin_to_trader: builtins.str
-    """The amount of margin the trader receives after closing the position, from
-    the vault. Should never be negative.
+    """The amount of margin the trader receives after closing the position, from the vault.
+    Should never be negative.
     """
     def __init__(
         self,
         *,
         exchanged_notional_value: builtins.str = ...,
         exchanged_position_size: builtins.str = ...,
         funding_payment: builtins.str = ...,
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/tx_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from perp.v2 import tx_pb2 as perp_dot_v2_dot_tx__pb2
+from perp.v1 import tx_pb2 as perp_dot_v1_dot_tx__pb2
 
 
 class MsgStub(object):
     """Msg defines the x/perp Msg service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.RemoveMargin = channel.unary_unary(
-                '/nibiru.perp.v2.Msg/RemoveMargin',
-                request_serializer=perp_dot_v2_dot_tx__pb2.MsgRemoveMargin.SerializeToString,
-                response_deserializer=perp_dot_v2_dot_tx__pb2.MsgRemoveMarginResponse.FromString,
+                '/nibiru.perp.v1.Msg/RemoveMargin',
+                request_serializer=perp_dot_v1_dot_tx__pb2.MsgRemoveMargin.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_tx__pb2.MsgRemoveMarginResponse.FromString,
                 )
         self.AddMargin = channel.unary_unary(
-                '/nibiru.perp.v2.Msg/AddMargin',
-                request_serializer=perp_dot_v2_dot_tx__pb2.MsgAddMargin.SerializeToString,
-                response_deserializer=perp_dot_v2_dot_tx__pb2.MsgAddMarginResponse.FromString,
+                '/nibiru.perp.v1.Msg/AddMargin',
+                request_serializer=perp_dot_v1_dot_tx__pb2.MsgAddMargin.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_tx__pb2.MsgAddMarginResponse.FromString,
                 )
         self.MultiLiquidate = channel.unary_unary(
-                '/nibiru.perp.v2.Msg/MultiLiquidate',
-                request_serializer=perp_dot_v2_dot_tx__pb2.MsgMultiLiquidate.SerializeToString,
-                response_deserializer=perp_dot_v2_dot_tx__pb2.MsgMultiLiquidateResponse.FromString,
+                '/nibiru.perp.v1.Msg/MultiLiquidate',
+                request_serializer=perp_dot_v1_dot_tx__pb2.MsgMultiLiquidate.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_tx__pb2.MsgMultiLiquidateResponse.FromString,
                 )
         self.OpenPosition = channel.unary_unary(
-                '/nibiru.perp.v2.Msg/OpenPosition',
-                request_serializer=perp_dot_v2_dot_tx__pb2.MsgOpenPosition.SerializeToString,
-                response_deserializer=perp_dot_v2_dot_tx__pb2.MsgOpenPositionResponse.FromString,
+                '/nibiru.perp.v1.Msg/OpenPosition',
+                request_serializer=perp_dot_v1_dot_tx__pb2.MsgOpenPosition.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_tx__pb2.MsgOpenPositionResponse.FromString,
                 )
         self.ClosePosition = channel.unary_unary(
-                '/nibiru.perp.v2.Msg/ClosePosition',
-                request_serializer=perp_dot_v2_dot_tx__pb2.MsgClosePosition.SerializeToString,
-                response_deserializer=perp_dot_v2_dot_tx__pb2.MsgClosePositionResponse.FromString,
+                '/nibiru.perp.v1.Msg/ClosePosition',
+                request_serializer=perp_dot_v1_dot_tx__pb2.MsgClosePosition.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_tx__pb2.MsgClosePositionResponse.FromString,
                 )
         self.DonateToEcosystemFund = channel.unary_unary(
-                '/nibiru.perp.v2.Msg/DonateToEcosystemFund',
-                request_serializer=perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFund.SerializeToString,
-                response_deserializer=perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFundResponse.FromString,
+                '/nibiru.perp.v1.Msg/DonateToEcosystemFund',
+                request_serializer=perp_dot_v1_dot_tx__pb2.MsgDonateToEcosystemFund.SerializeToString,
+                response_deserializer=perp_dot_v1_dot_tx__pb2.MsgDonateToEcosystemFundResponse.FromString,
                 )
 
 
 class MsgServicer(object):
     """Msg defines the x/perp Msg service.
     """
 
@@ -88,45 +88,45 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_MsgServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'RemoveMargin': grpc.unary_unary_rpc_method_handler(
                     servicer.RemoveMargin,
-                    request_deserializer=perp_dot_v2_dot_tx__pb2.MsgRemoveMargin.FromString,
-                    response_serializer=perp_dot_v2_dot_tx__pb2.MsgRemoveMarginResponse.SerializeToString,
+                    request_deserializer=perp_dot_v1_dot_tx__pb2.MsgRemoveMargin.FromString,
+                    response_serializer=perp_dot_v1_dot_tx__pb2.MsgRemoveMarginResponse.SerializeToString,
             ),
             'AddMargin': grpc.unary_unary_rpc_method_handler(
                     servicer.AddMargin,
-                    request_deserializer=perp_dot_v2_dot_tx__pb2.MsgAddMargin.FromString,
-                    response_serializer=perp_dot_v2_dot_tx__pb2.MsgAddMarginResponse.SerializeToString,
+                    request_deserializer=perp_dot_v1_dot_tx__pb2.MsgAddMargin.FromString,
+                    response_serializer=perp_dot_v1_dot_tx__pb2.MsgAddMarginResponse.SerializeToString,
             ),
             'MultiLiquidate': grpc.unary_unary_rpc_method_handler(
                     servicer.MultiLiquidate,
-                    request_deserializer=perp_dot_v2_dot_tx__pb2.MsgMultiLiquidate.FromString,
-                    response_serializer=perp_dot_v2_dot_tx__pb2.MsgMultiLiquidateResponse.SerializeToString,
+                    request_deserializer=perp_dot_v1_dot_tx__pb2.MsgMultiLiquidate.FromString,
+                    response_serializer=perp_dot_v1_dot_tx__pb2.MsgMultiLiquidateResponse.SerializeToString,
             ),
             'OpenPosition': grpc.unary_unary_rpc_method_handler(
                     servicer.OpenPosition,
-                    request_deserializer=perp_dot_v2_dot_tx__pb2.MsgOpenPosition.FromString,
-                    response_serializer=perp_dot_v2_dot_tx__pb2.MsgOpenPositionResponse.SerializeToString,
+                    request_deserializer=perp_dot_v1_dot_tx__pb2.MsgOpenPosition.FromString,
+                    response_serializer=perp_dot_v1_dot_tx__pb2.MsgOpenPositionResponse.SerializeToString,
             ),
             'ClosePosition': grpc.unary_unary_rpc_method_handler(
                     servicer.ClosePosition,
-                    request_deserializer=perp_dot_v2_dot_tx__pb2.MsgClosePosition.FromString,
-                    response_serializer=perp_dot_v2_dot_tx__pb2.MsgClosePositionResponse.SerializeToString,
+                    request_deserializer=perp_dot_v1_dot_tx__pb2.MsgClosePosition.FromString,
+                    response_serializer=perp_dot_v1_dot_tx__pb2.MsgClosePositionResponse.SerializeToString,
             ),
             'DonateToEcosystemFund': grpc.unary_unary_rpc_method_handler(
                     servicer.DonateToEcosystemFund,
-                    request_deserializer=perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFund.FromString,
-                    response_serializer=perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFundResponse.SerializeToString,
+                    request_deserializer=perp_dot_v1_dot_tx__pb2.MsgDonateToEcosystemFund.FromString,
+                    response_serializer=perp_dot_v1_dot_tx__pb2.MsgDonateToEcosystemFundResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'nibiru.perp.v2.Msg', rpc_method_handlers)
+            'nibiru.perp.v1.Msg', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Msg(object):
     """Msg defines the x/perp Msg service.
     """
@@ -138,97 +138,97 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v2.Msg/RemoveMargin',
-            perp_dot_v2_dot_tx__pb2.MsgRemoveMargin.SerializeToString,
-            perp_dot_v2_dot_tx__pb2.MsgRemoveMarginResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Msg/RemoveMargin',
+            perp_dot_v1_dot_tx__pb2.MsgRemoveMargin.SerializeToString,
+            perp_dot_v1_dot_tx__pb2.MsgRemoveMarginResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def AddMargin(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v2.Msg/AddMargin',
-            perp_dot_v2_dot_tx__pb2.MsgAddMargin.SerializeToString,
-            perp_dot_v2_dot_tx__pb2.MsgAddMarginResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Msg/AddMargin',
+            perp_dot_v1_dot_tx__pb2.MsgAddMargin.SerializeToString,
+            perp_dot_v1_dot_tx__pb2.MsgAddMarginResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def MultiLiquidate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v2.Msg/MultiLiquidate',
-            perp_dot_v2_dot_tx__pb2.MsgMultiLiquidate.SerializeToString,
-            perp_dot_v2_dot_tx__pb2.MsgMultiLiquidateResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Msg/MultiLiquidate',
+            perp_dot_v1_dot_tx__pb2.MsgMultiLiquidate.SerializeToString,
+            perp_dot_v1_dot_tx__pb2.MsgMultiLiquidateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def OpenPosition(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v2.Msg/OpenPosition',
-            perp_dot_v2_dot_tx__pb2.MsgOpenPosition.SerializeToString,
-            perp_dot_v2_dot_tx__pb2.MsgOpenPositionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Msg/OpenPosition',
+            perp_dot_v1_dot_tx__pb2.MsgOpenPosition.SerializeToString,
+            perp_dot_v1_dot_tx__pb2.MsgOpenPositionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ClosePosition(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v2.Msg/ClosePosition',
-            perp_dot_v2_dot_tx__pb2.MsgClosePosition.SerializeToString,
-            perp_dot_v2_dot_tx__pb2.MsgClosePositionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Msg/ClosePosition',
+            perp_dot_v1_dot_tx__pb2.MsgClosePosition.SerializeToString,
+            perp_dot_v1_dot_tx__pb2.MsgClosePositionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def DonateToEcosystemFund(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v2.Msg/DonateToEcosystemFund',
-            perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFund.SerializeToString,
-            perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFundResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v1.Msg/DonateToEcosystemFund',
+            perp_dot_v1_dot_tx__pb2.MsgDonateToEcosystemFund.SerializeToString,
+            perp_dot_v1_dot_tx__pb2.MsgDonateToEcosystemFundResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/perp/v2/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/perp/v1/tx_pb2_grpc.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import grpc
-import perp.v2.tx_pb2
+import perp.v1.tx_pb2
 
 class MsgStub:
     """Msg defines the x/perp Msg service."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
     RemoveMargin: grpc.UnaryUnaryMultiCallable[
-        perp.v2.tx_pb2.MsgRemoveMargin,
-        perp.v2.tx_pb2.MsgRemoveMarginResponse,
+        perp.v1.tx_pb2.MsgRemoveMargin,
+        perp.v1.tx_pb2.MsgRemoveMarginResponse,
     ]
     AddMargin: grpc.UnaryUnaryMultiCallable[
-        perp.v2.tx_pb2.MsgAddMargin,
-        perp.v2.tx_pb2.MsgAddMarginResponse,
+        perp.v1.tx_pb2.MsgAddMargin,
+        perp.v1.tx_pb2.MsgAddMarginResponse,
     ]
     MultiLiquidate: grpc.UnaryUnaryMultiCallable[
-        perp.v2.tx_pb2.MsgMultiLiquidate,
-        perp.v2.tx_pb2.MsgMultiLiquidateResponse,
+        perp.v1.tx_pb2.MsgMultiLiquidate,
+        perp.v1.tx_pb2.MsgMultiLiquidateResponse,
     ]
     OpenPosition: grpc.UnaryUnaryMultiCallable[
-        perp.v2.tx_pb2.MsgOpenPosition,
-        perp.v2.tx_pb2.MsgOpenPositionResponse,
+        perp.v1.tx_pb2.MsgOpenPosition,
+        perp.v1.tx_pb2.MsgOpenPositionResponse,
     ]
     ClosePosition: grpc.UnaryUnaryMultiCallable[
-        perp.v2.tx_pb2.MsgClosePosition,
-        perp.v2.tx_pb2.MsgClosePositionResponse,
+        perp.v1.tx_pb2.MsgClosePosition,
+        perp.v1.tx_pb2.MsgClosePositionResponse,
     ]
     DonateToEcosystemFund: grpc.UnaryUnaryMultiCallable[
-        perp.v2.tx_pb2.MsgDonateToEcosystemFund,
-        perp.v2.tx_pb2.MsgDonateToEcosystemFundResponse,
+        perp.v1.tx_pb2.MsgDonateToEcosystemFund,
+        perp.v1.tx_pb2.MsgDonateToEcosystemFundResponse,
     ]
 
 class MsgServicer(metaclass=abc.ABCMeta):
     """Msg defines the x/perp Msg service."""
 
     @abc.abstractmethod
     def RemoveMargin(
         self,
-        request: perp.v2.tx_pb2.MsgRemoveMargin,
+        request: perp.v1.tx_pb2.MsgRemoveMargin,
         context: grpc.ServicerContext,
-    ) -> perp.v2.tx_pb2.MsgRemoveMarginResponse: ...
+    ) -> perp.v1.tx_pb2.MsgRemoveMarginResponse: ...
     @abc.abstractmethod
     def AddMargin(
         self,
-        request: perp.v2.tx_pb2.MsgAddMargin,
+        request: perp.v1.tx_pb2.MsgAddMargin,
         context: grpc.ServicerContext,
-    ) -> perp.v2.tx_pb2.MsgAddMarginResponse: ...
+    ) -> perp.v1.tx_pb2.MsgAddMarginResponse: ...
     @abc.abstractmethod
     def MultiLiquidate(
         self,
-        request: perp.v2.tx_pb2.MsgMultiLiquidate,
+        request: perp.v1.tx_pb2.MsgMultiLiquidate,
         context: grpc.ServicerContext,
-    ) -> perp.v2.tx_pb2.MsgMultiLiquidateResponse: ...
+    ) -> perp.v1.tx_pb2.MsgMultiLiquidateResponse: ...
     @abc.abstractmethod
     def OpenPosition(
         self,
-        request: perp.v2.tx_pb2.MsgOpenPosition,
+        request: perp.v1.tx_pb2.MsgOpenPosition,
         context: grpc.ServicerContext,
-    ) -> perp.v2.tx_pb2.MsgOpenPositionResponse: ...
+    ) -> perp.v1.tx_pb2.MsgOpenPositionResponse: ...
     @abc.abstractmethod
     def ClosePosition(
         self,
-        request: perp.v2.tx_pb2.MsgClosePosition,
+        request: perp.v1.tx_pb2.MsgClosePosition,
         context: grpc.ServicerContext,
-    ) -> perp.v2.tx_pb2.MsgClosePositionResponse: ...
+    ) -> perp.v1.tx_pb2.MsgClosePositionResponse: ...
     @abc.abstractmethod
     def DonateToEcosystemFund(
         self,
-        request: perp.v2.tx_pb2.MsgDonateToEcosystemFund,
+        request: perp.v1.tx_pb2.MsgDonateToEcosystemFund,
         context: grpc.ServicerContext,
-    ) -> perp.v2.tx_pb2.MsgDonateToEcosystemFundResponse: ...
+    ) -> perp.v1.tx_pb2.MsgDonateToEcosystemFundResponse: ...
 
 def add_MsgServicer_to_server(servicer: MsgServicer, server: grpc.Server) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/event_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/event_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/params_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/params_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/pool_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/pool_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/pool_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/pool_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,16 @@
 
 class _PoolTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_PoolType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     BALANCER: _PoolType.ValueType  # 0
     STABLESWAP: _PoolType.ValueType  # 1
 
 class PoolType(_PoolType, metaclass=_PoolTypeEnumTypeWrapper):
-    """- `balancer`: Balancer are pools defined by the equation xy=k, extended by
-    the weighs introduced by Balancer.
-    - `stableswap`: Stableswap pools are defined by a combination of
-    constant-product and constant-sum pool
+    """- `balancer`: Balancer are pools defined by the equation xy=k, extended by the weighs introduced by Balancer.
+    - `stableswap`: Stableswap pools are defined by a combination of constant-product and constant-sum pool
     """
 
 BALANCER: PoolType.ValueType  # 0
 STABLESWAP: PoolType.ValueType  # 1
 global___PoolType = PoolType
 
 @typing_extensions.final
@@ -48,19 +46,18 @@
     SWAP_FEE_FIELD_NUMBER: builtins.int
     EXIT_FEE_FIELD_NUMBER: builtins.int
     A_FIELD_NUMBER: builtins.int
     POOL_TYPE_FIELD_NUMBER: builtins.int
     swap_fee: builtins.str
     exit_fee: builtins.str
     A: builtins.str
-    """Amplification Parameter (A): Larger value of A make the curve better
-    resemble a straight line in the center (when pool is near balance).  Highly
-    volatile assets should use a lower value, while assets that are closer
-    together may be best with a higher value. This is only used if the
-    pool_type is set to 1 (stableswap)
+    """Amplification Parameter (A): Larger value of A make the curve better resemble a straight 
+    line in the center (when pool is near balance).  Highly volatile assets should use a lower value, while assets that 
+    are closer together may be best with a higher value.
+    This is only used if the pool_type is set to 1 (stableswap)
     """
     pool_type: global___PoolType.ValueType
     def __init__(
         self,
         *,
         swap_fee: builtins.str = ...,
         exit_fee: builtins.str = ...,
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/query_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -303,16 +303,16 @@
     def ClearField(self, field_name: typing_extensions.Literal["total_shares", b"total_shares"]) -> None: ...
 
 global___QueryTotalSharesResponse = QueryTotalSharesResponse
 
 @typing_extensions.final
 class QuerySpotPriceRequest(google.protobuf.message.Message):
     """Returns the amount of tokenInDenom to produce 1 tokenOutDenom
-    For example, if the price of NIBI = 9.123 NUSD, then setting
-    tokenInDenom=NUSD and tokenOutDenom=NIBI would give "9.123".
+    For example, if the price of NIBI = 9.123 NUSD, then setting tokenInDenom=NUSD
+    and tokenOutDenom=NIBI would give "9.123".
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     TOKEN_IN_DENOM_FIELD_NUMBER: builtins.int
     TOKEN_OUT_DENOM_FIELD_NUMBER: builtins.int
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/tx_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -4,198 +4,212 @@
 """
 import builtins
 import collections.abc
 import cosmos.base.v1beta1.coin_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import spot.v1.pool_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class MsgCreatePool(google.protobuf.message.Message):
+class MsgMintStable(google.protobuf.message.Message):
+    """
+    MsgMintStable: Msg to mint NUSD. A user deposits NIBI and collateral and gets 
+    NUSD in return. The amount of NUSD received depends on the current price set 
+    by the oracle library and the current collateral ratio for the protocol.
+    """
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CREATOR_FIELD_NUMBER: builtins.int
-    POOL_PARAMS_FIELD_NUMBER: builtins.int
-    POOL_ASSETS_FIELD_NUMBER: builtins.int
+    STABLE_FIELD_NUMBER: builtins.int
     creator: builtins.str
     @property
-    def pool_params(self) -> spot.v1.pool_pb2.PoolParams: ...
-    @property
-    def pool_assets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[spot.v1.pool_pb2.PoolAsset]: ...
+    def stable(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     def __init__(
         self,
         *,
         creator: builtins.str = ...,
-        pool_params: spot.v1.pool_pb2.PoolParams | None = ...,
-        pool_assets: collections.abc.Iterable[spot.v1.pool_pb2.PoolAsset] | None = ...,
+        stable: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["pool_params", b"pool_params"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["creator", b"creator", "pool_assets", b"pool_assets", "pool_params", b"pool_params"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["stable", b"stable"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["creator", b"creator", "stable", b"stable"]) -> None: ...
 
-global___MsgCreatePool = MsgCreatePool
+global___MsgMintStable = MsgMintStable
 
 @typing_extensions.final
-class MsgCreatePoolResponse(google.protobuf.message.Message):
+class MsgMintStableResponse(google.protobuf.message.Message):
+    """MsgMintStableResponse specifies the amount of NUSD token the user will receive after their
+    mint transaction
+    """
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    POOL_ID_FIELD_NUMBER: builtins.int
-    pool_id: builtins.int
+    STABLE_FIELD_NUMBER: builtins.int
+    USED_COINS_FIELD_NUMBER: builtins.int
+    FEES_PAYED_FIELD_NUMBER: builtins.int
+    @property
+    def stable(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
+    @property
+    def used_coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
+    @property
+    def fees_payed(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
         self,
         *,
-        pool_id: builtins.int = ...,
+        stable: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        used_coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
+        fees_payed: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["stable", b"stable"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["fees_payed", b"fees_payed", "stable", b"stable", "used_coins", b"used_coins"]) -> None: ...
 
-global___MsgCreatePoolResponse = MsgCreatePoolResponse
+global___MsgMintStableResponse = MsgMintStableResponse
 
 @typing_extensions.final
-class MsgJoinPool(google.protobuf.message.Message):
+class MsgBurnStable(google.protobuf.message.Message):
     """
-    Message to join a pool (identified by poolId) with a set of tokens to deposit.
+    MsgBurnStable allows users to burn NUSD in exchange for NIBI and collateral. 
+    The amount of NIBI and Collateral received depends on the current price set by 
+    the x/oracle library and the current collateral ratio.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    SENDER_FIELD_NUMBER: builtins.int
-    POOL_ID_FIELD_NUMBER: builtins.int
-    TOKENS_IN_FIELD_NUMBER: builtins.int
-    USE_ALL_COINS_FIELD_NUMBER: builtins.int
-    sender: builtins.str
-    pool_id: builtins.int
+    CREATOR_FIELD_NUMBER: builtins.int
+    STABLE_FIELD_NUMBER: builtins.int
+    creator: builtins.str
     @property
-    def tokens_in(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
-    use_all_coins: builtins.bool
+    def stable(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     def __init__(
         self,
         *,
-        sender: builtins.str = ...,
-        pool_id: builtins.int = ...,
-        tokens_in: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
-        use_all_coins: builtins.bool = ...,
+        creator: builtins.str = ...,
+        stable: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "tokens_in", b"tokens_in", "use_all_coins", b"use_all_coins"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["stable", b"stable"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["creator", b"creator", "stable", b"stable"]) -> None: ...
 
-global___MsgJoinPool = MsgJoinPool
+global___MsgBurnStable = MsgBurnStable
 
 @typing_extensions.final
-class MsgJoinPoolResponse(google.protobuf.message.Message):
-    """
-    Response when a user joins a pool.
+class MsgBurnStableResponse(google.protobuf.message.Message):
+    """MsgBurnStableResponse specifies the amount of collateral and governance 
+    token the user will receive after their burn transaction.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    POOL_FIELD_NUMBER: builtins.int
-    NUM_POOL_SHARES_OUT_FIELD_NUMBER: builtins.int
-    REMAINING_COINS_FIELD_NUMBER: builtins.int
+    COLLATERAL_FIELD_NUMBER: builtins.int
+    GOV_FIELD_NUMBER: builtins.int
+    FEES_PAYED_FIELD_NUMBER: builtins.int
     @property
-    def pool(self) -> spot.v1.pool_pb2.Pool:
-        """the final state of the pool after a join"""
+    def collateral(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     @property
-    def num_pool_shares_out(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
-        """sum of LP tokens minted from the join"""
+    def gov(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     @property
-    def remaining_coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]:
-        """remaining tokens from attempting to join the pool"""
+    def fees_payed(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
         self,
         *,
-        pool: spot.v1.pool_pb2.Pool | None = ...,
-        num_pool_shares_out: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
-        remaining_coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
+        collateral: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        gov: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        fees_payed: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["num_pool_shares_out", b"num_pool_shares_out", "pool", b"pool"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["num_pool_shares_out", b"num_pool_shares_out", "pool", b"pool", "remaining_coins", b"remaining_coins"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["collateral", b"collateral", "gov", b"gov"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["collateral", b"collateral", "fees_payed", b"fees_payed", "gov", b"gov"]) -> None: ...
 
-global___MsgJoinPoolResponse = MsgJoinPoolResponse
+global___MsgBurnStableResponse = MsgBurnStableResponse
 
 @typing_extensions.final
-class MsgExitPool(google.protobuf.message.Message):
+class MsgRecollateralize(google.protobuf.message.Message):
+    """MsgRecollateralize"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    SENDER_FIELD_NUMBER: builtins.int
-    POOL_ID_FIELD_NUMBER: builtins.int
-    POOL_SHARES_FIELD_NUMBER: builtins.int
-    sender: builtins.str
-    pool_id: builtins.int
+    CREATOR_FIELD_NUMBER: builtins.int
+    COLL_FIELD_NUMBER: builtins.int
+    creator: builtins.str
     @property
-    def pool_shares(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
+    def coll(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     def __init__(
         self,
         *,
-        sender: builtins.str = ...,
-        pool_id: builtins.int = ...,
-        pool_shares: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        creator: builtins.str = ...,
+        coll: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["pool_shares", b"pool_shares"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "pool_shares", b"pool_shares", "sender", b"sender"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["coll", b"coll"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["coll", b"coll", "creator", b"creator"]) -> None: ...
 
-global___MsgExitPool = MsgExitPool
+global___MsgRecollateralize = MsgRecollateralize
 
 @typing_extensions.final
-class MsgExitPoolResponse(google.protobuf.message.Message):
+class MsgRecollateralizeResponse(google.protobuf.message.Message):
+    """MsgRecollateralizeResponse is the output of a successful 'Recollateralize'"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TOKENS_OUT_FIELD_NUMBER: builtins.int
+    GOV_FIELD_NUMBER: builtins.int
     @property
-    def tokens_out(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
+    def gov(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
+        """Gov (sdk.Coin): Tokens rewarded to the caller in exchange for her collateral."""
     def __init__(
         self,
         *,
-        tokens_out: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
+        gov: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tokens_out", b"tokens_out"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["gov", b"gov"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["gov", b"gov"]) -> None: ...
 
-global___MsgExitPoolResponse = MsgExitPoolResponse
+global___MsgRecollateralizeResponse = MsgRecollateralizeResponse
 
 @typing_extensions.final
-class MsgSwapAssets(google.protobuf.message.Message):
+class MsgBuyback(google.protobuf.message.Message):
+    """MsgBuyback"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    SENDER_FIELD_NUMBER: builtins.int
-    POOL_ID_FIELD_NUMBER: builtins.int
-    TOKEN_IN_FIELD_NUMBER: builtins.int
-    TOKEN_OUT_DENOM_FIELD_NUMBER: builtins.int
-    sender: builtins.str
-    pool_id: builtins.int
+    CREATOR_FIELD_NUMBER: builtins.int
+    GOV_FIELD_NUMBER: builtins.int
+    creator: builtins.str
     @property
-    def token_in(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
-    token_out_denom: builtins.str
+    def gov(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
+        """Gov (sdk.Coin): Tokens the caller wants to sell to the protocol in exchange 
+        for collateral.
+        """
     def __init__(
         self,
         *,
-        sender: builtins.str = ...,
-        pool_id: builtins.int = ...,
-        token_in: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
-        token_out_denom: builtins.str = ...,
+        creator: builtins.str = ...,
+        gov: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["token_in", b"token_in"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "token_in", b"token_in", "token_out_denom", b"token_out_denom"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["gov", b"gov"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["creator", b"creator", "gov", b"gov"]) -> None: ...
 
-global___MsgSwapAssets = MsgSwapAssets
+global___MsgBuyback = MsgBuyback
 
 @typing_extensions.final
-class MsgSwapAssetsResponse(google.protobuf.message.Message):
+class MsgBuybackResponse(google.protobuf.message.Message):
+    """MsgBuybackResponse is the output of a successful 'Buyback'"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TOKEN_OUT_FIELD_NUMBER: builtins.int
+    COLL_FIELD_NUMBER: builtins.int
     @property
-    def token_out(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
+    def coll(self) -> cosmos.base.v1beta1.coin_pb2.Coin:
+        """Coll (sdk.Coin): Tokens sold to the caller in exchange for her collateral."""
     def __init__(
         self,
         *,
-        token_out: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
+        coll: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["token_out", b"token_out"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["token_out", b"token_out"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["coll", b"coll"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["coll", b"coll"]) -> None: ...
 
-global___MsgSwapAssetsResponse = MsgSwapAssetsResponse
+global___MsgBuybackResponse = MsgBuybackResponse
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/spot/v1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/spot/v1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/events_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/events_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: stablecoin/v1/events.proto
+# source: stablecoin/events.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1astablecoin/v1/events.proto\x12\x14nibiru.stablecoin.v1\x1a\x14gogoproto/gogo.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"X\n\rEventTransfer\x12-\n\x04\x63oin\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x0c\n\x04\x66rom\x18\x02 \x01(\t\x12\n\n\x02to\x18\x03 \x01(\t\"Q\n\x0f\x45ventMintStable\x12>\n\x06\x61mount\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"Q\n\x0f\x45ventBurnStable\x12>\n\x06\x61mount\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"O\n\rEventMintNIBI\x12>\n\x06\x61mount\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"O\n\rEventBurnNIBI\x12>\n\x06\x61mount\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"\xcf\x01\n\x14\x45ventRecollateralize\x12\x0e\n\x06\x63\x61ller\x18\x01 \x01(\t\x12\x30\n\x07in_coin\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x31\n\x08out_coin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x42\n\ncoll_ratio\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\xc7\x01\n\x0c\x45ventBuyback\x12\x0e\n\x06\x63\x61ller\x18\x01 \x01(\t\x12\x30\n\x07in_coin\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x31\n\x08out_coin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x42\n\ncoll_ratio\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x42\x32Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17stablecoin/events.proto\x12\x14nibiru.stablecoin.v1\x1a\x14gogoproto/gogo.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\"X\n\rEventTransfer\x12-\n\x04\x63oin\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x0c\n\x04\x66rom\x18\x02 \x01(\t\x12\n\n\x02to\x18\x03 \x01(\t\"Q\n\x0f\x45ventMintStable\x12>\n\x06\x61mount\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"Q\n\x0f\x45ventBurnStable\x12>\n\x06\x61mount\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"O\n\rEventMintNIBI\x12>\n\x06\x61mount\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"O\n\rEventBurnNIBI\x12>\n\x06\x61mount\x18\x01 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Int\xc8\xde\x1f\x00\"\xcf\x01\n\x14\x45ventRecollateralize\x12\x0e\n\x06\x63\x61ller\x18\x01 \x01(\t\x12\x30\n\x07in_coin\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x31\n\x08out_coin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x42\n\ncoll_ratio\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\"\xc7\x01\n\x0c\x45ventBuyback\x12\x0e\n\x06\x63\x61ller\x18\x01 \x01(\t\x12\x30\n\x07in_coin\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x31\n\x08out_coin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12\x42\n\ncoll_ratio\x18\x04 \x01(\tB.\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.Dec\xc8\xde\x1f\x00\x42\x32Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.v1.events_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.events_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z0github.com/NibiruChain/nibiru/x/stablecoin/types'
   _EVENTTRANSFER.fields_by_name['coin']._options = None
   _EVENTTRANSFER.fields_by_name['coin']._serialized_options = b'\310\336\037\000'
   _EVENTMINTSTABLE.fields_by_name['amount']._options = None
@@ -41,22 +41,22 @@
   _EVENTRECOLLATERALIZE.fields_by_name['coll_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
   _EVENTBUYBACK.fields_by_name['in_coin']._options = None
   _EVENTBUYBACK.fields_by_name['in_coin']._serialized_options = b'\310\336\037\000'
   _EVENTBUYBACK.fields_by_name['out_coin']._options = None
   _EVENTBUYBACK.fields_by_name['out_coin']._serialized_options = b'\310\336\037\000'
   _EVENTBUYBACK.fields_by_name['coll_ratio']._options = None
   _EVENTBUYBACK.fields_by_name['coll_ratio']._serialized_options = b'\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec\310\336\037\000'
-  _EVENTTRANSFER._serialized_start=106
-  _EVENTTRANSFER._serialized_end=194
-  _EVENTMINTSTABLE._serialized_start=196
-  _EVENTMINTSTABLE._serialized_end=277
-  _EVENTBURNSTABLE._serialized_start=279
-  _EVENTBURNSTABLE._serialized_end=360
-  _EVENTMINTNIBI._serialized_start=362
-  _EVENTMINTNIBI._serialized_end=441
-  _EVENTBURNNIBI._serialized_start=443
-  _EVENTBURNNIBI._serialized_end=522
-  _EVENTRECOLLATERALIZE._serialized_start=525
-  _EVENTRECOLLATERALIZE._serialized_end=732
-  _EVENTBUYBACK._serialized_start=735
-  _EVENTBUYBACK._serialized_end=934
+  _EVENTTRANSFER._serialized_start=103
+  _EVENTTRANSFER._serialized_end=191
+  _EVENTMINTSTABLE._serialized_start=193
+  _EVENTMINTSTABLE._serialized_end=274
+  _EVENTBURNSTABLE._serialized_start=276
+  _EVENTBURNSTABLE._serialized_end=357
+  _EVENTMINTNIBI._serialized_start=359
+  _EVENTMINTNIBI._serialized_end=438
+  _EVENTBURNNIBI._serialized_start=440
+  _EVENTBURNNIBI._serialized_end=519
+  _EVENTRECOLLATERALIZE._serialized_start=522
+  _EVENTRECOLLATERALIZE._serialized_end=729
+  _EVENTBUYBACK._serialized_start=732
+  _EVENTBUYBACK._serialized_end=931
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/events_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/genesis_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/genesis_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: stablecoin/v1/genesis.proto
+# source: stablecoin/genesis.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from stablecoin.v1 import params_pb2 as stablecoin_dot_v1_dot_params__pb2
+from stablecoin import params_pb2 as stablecoin_dot_params__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstablecoin/v1/genesis.proto\x12\x14nibiru.stablecoin.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1astablecoin/v1/params.proto\"\xa4\x01\n\x0cGenesisState\x12\x32\n\x06params\x18\x01 \x01(\x0b\x32\x1c.nibiru.stablecoin.v1.ParamsB\x04\xc8\xde\x1f\x00\x12`\n\x16module_account_balance\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB%\xf2\xde\x1f\x1dyaml:\"module_account_balance\"\xc8\xde\x1f\x00\x42\x32Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18stablecoin/genesis.proto\x12\x14nibiru.stablecoin.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x17stablecoin/params.proto\"\xa4\x01\n\x0cGenesisState\x12\x32\n\x06params\x18\x01 \x01(\x0b\x32\x1c.nibiru.stablecoin.v1.ParamsB\x04\xc8\xde\x1f\x00\x12`\n\x16module_account_balance\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB%\xf2\xde\x1f\x1dyaml:\"module_account_balance\"\xc8\xde\x1f\x00\x42\x32Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.v1.genesis_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z0github.com/NibiruChain/nibiru/x/stablecoin/types'
   _GENESISSTATE.fields_by_name['params']._options = None
   _GENESISSTATE.fields_by_name['params']._serialized_options = b'\310\336\037\000'
   _GENESISSTATE.fields_by_name['module_account_balance']._options = None
   _GENESISSTATE.fields_by_name['module_account_balance']._serialized_options = b'\362\336\037\035yaml:\"module_account_balance\"\310\336\037\000'
-  _GENESISSTATE._serialized_start=136
-  _GENESISSTATE._serialized_end=300
+  _GENESISSTATE._serialized_start=130
+  _GENESISSTATE._serialized_end=294
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/genesis_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/genesis_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import cosmos.base.v1beta1.coin_pb2
 import google.protobuf.descriptor
 import google.protobuf.message
-import stablecoin.v1.params_pb2
+import stablecoin.params_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -21,20 +21,20 @@
     """GenesisState defines the stablecoin module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     MODULE_ACCOUNT_BALANCE_FIELD_NUMBER: builtins.int
     @property
-    def params(self) -> stablecoin.v1.params_pb2.Params: ...
+    def params(self) -> stablecoin.params_pb2.Params: ...
     @property
     def module_account_balance(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     def __init__(
         self,
         *,
-        params: stablecoin.v1.params_pb2.Params | None = ...,
+        params: stablecoin.params_pb2.Params | None = ...,
         module_account_balance: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["module_account_balance", b"module_account_balance", "params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["module_account_balance", b"module_account_balance", "params", b"params"]) -> None: ...
 
 global___GenesisState = GenesisState
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/params_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/keys_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: stablecoin/v1/params.proto
+# source: tendermint/crypto/keys.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1astablecoin/v1/params.proto\x12\x14nibiru.stablecoin.v1\x1a\x14gogoproto/gogo.proto\"\x95\x02\n\x06Params\x12\x12\n\ncoll_ratio\x18\x01 \x01(\x03\x12\x11\n\tfee_ratio\x18\x02 \x01(\x03\x12\x14\n\x0c\x65\x66_fee_ratio\x18\x03 \x01(\x03\x12\x19\n\x11\x62onus_rate_recoll\x18\x04 \x01(\x03\x12\x41\n\x16\x64istr_epoch_identifier\x18\x05 \x01(\tB!\xf2\xde\x1f\x1dyaml:\"distr_epoch_identifier\"\x12\x17\n\x0f\x61\x64justment_step\x18\x06 \x01(\x03\x12\x19\n\x11price_lower_bound\x18\x07 \x01(\x03\x12\x19\n\x11price_upper_bound\x18\x08 \x01(\x03\x12!\n\x19is_collateral_ratio_valid\x18\t \x01(\x08\x42\x32Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctendermint/crypto/keys.proto\x12\x11tendermint.crypto\x1a\x14gogoproto/gogo.proto\"D\n\tPublicKey\x12\x11\n\x07\x65\x64\x32\x35\x35\x31\x39\x18\x01 \x01(\x0cH\x00\x12\x13\n\tsecp256k1\x18\x02 \x01(\x0cH\x00:\x08\xe8\xa1\x1f\x01\xe8\xa0\x1f\x01\x42\x05\n\x03sumB:Z8github.com/tendermint/tendermint/proto/tendermint/cryptob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.v1.params_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.crypto.keys_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z0github.com/NibiruChain/nibiru/x/stablecoin/types'
-  _PARAMS.fields_by_name['distr_epoch_identifier']._options = None
-  _PARAMS.fields_by_name['distr_epoch_identifier']._serialized_options = b'\362\336\037\035yaml:\"distr_epoch_identifier\"'
-  _PARAMS._serialized_start=75
-  _PARAMS._serialized_end=352
+  DESCRIPTOR._serialized_options = b'Z8github.com/tendermint/tendermint/proto/tendermint/crypto'
+  _PUBLICKEY._options = None
+  _PUBLICKEY._serialized_options = b'\350\241\037\001\350\240\037\001'
+  _PUBLICKEY._serialized_start=73
+  _PUBLICKEY._serialized_end=141
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/params_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/query_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/query_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import builtins
 import collections.abc
 import cosmos.base.v1beta1.coin_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import stablecoin.v1.params_pb2
+import stablecoin.params_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -37,31 +37,31 @@
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
-    def params(self) -> stablecoin.v1.params_pb2.Params:
+    def params(self) -> stablecoin.params_pb2.Params:
         """params holds all the parameters of this module."""
     def __init__(
         self,
         *,
-        params: stablecoin.v1.params_pb2.Params | None = ...,
+        params: stablecoin.params_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
 @typing_extensions.final
 class QueryModuleAccountBalances(google.protobuf.message.Message):
     """---------------------------------------- ModuleAccountBalances
 
-    QueryModuleAccountBalances is the request type for the balance of the
+    QueryModuleAccountBalances is the request type for the balance of the 
     x/stablecoin module account.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
@@ -72,17 +72,15 @@
 @typing_extensions.final
 class QueryModuleAccountBalancesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MODULE_ACCOUNT_BALANCES_FIELD_NUMBER: builtins.int
     @property
     def module_account_balances(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]:
-        """ModuleAccountBalances is the balance of all coins in the x/stablecoin
-        module.
-        """
+        """ModuleAccountBalances is the balance of all coins in the x/stablecoin module."""
     def __init__(
         self,
         *,
         module_account_balances: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["module_account_balances", b"module_account_balances"]) -> None: ...
 
@@ -125,16 +123,15 @@
 
 global___QueryCirculatingSuppliesResponse = QueryCirculatingSuppliesResponse
 
 @typing_extensions.final
 class QueryGovToMintStable(google.protobuf.message.Message):
     """---------------------------------------- GovToMintStable
 
-    QueryGovToMintStable is the request type for the Query/GovToMintStable RPC
-    method
+    QueryGovToMintStable is the request type for the Query/GovToMintStable RPC method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COLLATERAL_FIELD_NUMBER: builtins.int
     @property
     def collateral(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/query_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/query_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from stablecoin.v1 import query_pb2 as stablecoin_dot_v1_dot_query__pb2
+from stablecoin import query_pb2 as stablecoin_dot_query__pb2
 
 
 class QueryStub(object):
     """Query defines the gRPC querier service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Params = channel.unary_unary(
                 '/nibiru.stablecoin.v1.Query/Params',
-                request_serializer=stablecoin_dot_v1_dot_query__pb2.QueryParamsRequest.SerializeToString,
-                response_deserializer=stablecoin_dot_v1_dot_query__pb2.QueryParamsResponse.FromString,
+                request_serializer=stablecoin_dot_query__pb2.QueryParamsRequest.SerializeToString,
+                response_deserializer=stablecoin_dot_query__pb2.QueryParamsResponse.FromString,
                 )
         self.ModuleAccountBalances = channel.unary_unary(
                 '/nibiru.stablecoin.v1.Query/ModuleAccountBalances',
-                request_serializer=stablecoin_dot_v1_dot_query__pb2.QueryModuleAccountBalances.SerializeToString,
-                response_deserializer=stablecoin_dot_v1_dot_query__pb2.QueryModuleAccountBalancesResponse.FromString,
+                request_serializer=stablecoin_dot_query__pb2.QueryModuleAccountBalances.SerializeToString,
+                response_deserializer=stablecoin_dot_query__pb2.QueryModuleAccountBalancesResponse.FromString,
                 )
         self.CirculatingSupplies = channel.unary_unary(
                 '/nibiru.stablecoin.v1.Query/CirculatingSupplies',
-                request_serializer=stablecoin_dot_v1_dot_query__pb2.QueryCirculatingSupplies.SerializeToString,
-                response_deserializer=stablecoin_dot_v1_dot_query__pb2.QueryCirculatingSuppliesResponse.FromString,
+                request_serializer=stablecoin_dot_query__pb2.QueryCirculatingSupplies.SerializeToString,
+                response_deserializer=stablecoin_dot_query__pb2.QueryCirculatingSuppliesResponse.FromString,
                 )
         self.LiquidityRatioInfo = channel.unary_unary(
                 '/nibiru.stablecoin.v1.Query/LiquidityRatioInfo',
-                request_serializer=stablecoin_dot_v1_dot_query__pb2.QueryLiquidityRatioInfoRequest.SerializeToString,
-                response_deserializer=stablecoin_dot_v1_dot_query__pb2.QueryLiquidityRatioInfoResponse.FromString,
+                request_serializer=stablecoin_dot_query__pb2.QueryLiquidityRatioInfoRequest.SerializeToString,
+                response_deserializer=stablecoin_dot_query__pb2.QueryLiquidityRatioInfoResponse.FromString,
                 )
 
 
 class QueryServicer(object):
     """Query defines the gRPC querier service.
     """
 
@@ -68,31 +68,31 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_QueryServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Params': grpc.unary_unary_rpc_method_handler(
                     servicer.Params,
-                    request_deserializer=stablecoin_dot_v1_dot_query__pb2.QueryParamsRequest.FromString,
-                    response_serializer=stablecoin_dot_v1_dot_query__pb2.QueryParamsResponse.SerializeToString,
+                    request_deserializer=stablecoin_dot_query__pb2.QueryParamsRequest.FromString,
+                    response_serializer=stablecoin_dot_query__pb2.QueryParamsResponse.SerializeToString,
             ),
             'ModuleAccountBalances': grpc.unary_unary_rpc_method_handler(
                     servicer.ModuleAccountBalances,
-                    request_deserializer=stablecoin_dot_v1_dot_query__pb2.QueryModuleAccountBalances.FromString,
-                    response_serializer=stablecoin_dot_v1_dot_query__pb2.QueryModuleAccountBalancesResponse.SerializeToString,
+                    request_deserializer=stablecoin_dot_query__pb2.QueryModuleAccountBalances.FromString,
+                    response_serializer=stablecoin_dot_query__pb2.QueryModuleAccountBalancesResponse.SerializeToString,
             ),
             'CirculatingSupplies': grpc.unary_unary_rpc_method_handler(
                     servicer.CirculatingSupplies,
-                    request_deserializer=stablecoin_dot_v1_dot_query__pb2.QueryCirculatingSupplies.FromString,
-                    response_serializer=stablecoin_dot_v1_dot_query__pb2.QueryCirculatingSuppliesResponse.SerializeToString,
+                    request_deserializer=stablecoin_dot_query__pb2.QueryCirculatingSupplies.FromString,
+                    response_serializer=stablecoin_dot_query__pb2.QueryCirculatingSuppliesResponse.SerializeToString,
             ),
             'LiquidityRatioInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.LiquidityRatioInfo,
-                    request_deserializer=stablecoin_dot_v1_dot_query__pb2.QueryLiquidityRatioInfoRequest.FromString,
-                    response_serializer=stablecoin_dot_v1_dot_query__pb2.QueryLiquidityRatioInfoResponse.SerializeToString,
+                    request_deserializer=stablecoin_dot_query__pb2.QueryLiquidityRatioInfoRequest.FromString,
+                    response_serializer=stablecoin_dot_query__pb2.QueryLiquidityRatioInfoResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'nibiru.stablecoin.v1.Query', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -109,16 +109,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.stablecoin.v1.Query/Params',
-            stablecoin_dot_v1_dot_query__pb2.QueryParamsRequest.SerializeToString,
-            stablecoin_dot_v1_dot_query__pb2.QueryParamsResponse.FromString,
+            stablecoin_dot_query__pb2.QueryParamsRequest.SerializeToString,
+            stablecoin_dot_query__pb2.QueryParamsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ModuleAccountBalances(request,
             target,
             options=(),
@@ -126,16 +126,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.stablecoin.v1.Query/ModuleAccountBalances',
-            stablecoin_dot_v1_dot_query__pb2.QueryModuleAccountBalances.SerializeToString,
-            stablecoin_dot_v1_dot_query__pb2.QueryModuleAccountBalancesResponse.FromString,
+            stablecoin_dot_query__pb2.QueryModuleAccountBalances.SerializeToString,
+            stablecoin_dot_query__pb2.QueryModuleAccountBalancesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def CirculatingSupplies(request,
             target,
             options=(),
@@ -143,16 +143,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.stablecoin.v1.Query/CirculatingSupplies',
-            stablecoin_dot_v1_dot_query__pb2.QueryCirculatingSupplies.SerializeToString,
-            stablecoin_dot_v1_dot_query__pb2.QueryCirculatingSuppliesResponse.FromString,
+            stablecoin_dot_query__pb2.QueryCirculatingSupplies.SerializeToString,
+            stablecoin_dot_query__pb2.QueryCirculatingSuppliesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def LiquidityRatioInfo(request,
             target,
             options=(),
@@ -160,11 +160,11 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.stablecoin.v1.Query/LiquidityRatioInfo',
-            stablecoin_dot_v1_dot_query__pb2.QueryLiquidityRatioInfoRequest.SerializeToString,
-            stablecoin_dot_v1_dot_query__pb2.QueryLiquidityRatioInfoResponse.FromString,
+            stablecoin_dot_query__pb2.QueryLiquidityRatioInfoRequest.SerializeToString,
+            stablecoin_dot_query__pb2.QueryLiquidityRatioInfoResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/query_pb2_grpc.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import grpc
-import stablecoin.v1.query_pb2
+import stablecoin.query_pb2
 
 class QueryStub:
     """Query defines the gRPC querier service."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
     Params: grpc.UnaryUnaryMultiCallable[
-        stablecoin.v1.query_pb2.QueryParamsRequest,
-        stablecoin.v1.query_pb2.QueryParamsResponse,
+        stablecoin.query_pb2.QueryParamsRequest,
+        stablecoin.query_pb2.QueryParamsResponse,
     ]
     """Parameters queries the parameters of the x/stablecoin module."""
     ModuleAccountBalances: grpc.UnaryUnaryMultiCallable[
-        stablecoin.v1.query_pb2.QueryModuleAccountBalances,
-        stablecoin.v1.query_pb2.QueryModuleAccountBalancesResponse,
+        stablecoin.query_pb2.QueryModuleAccountBalances,
+        stablecoin.query_pb2.QueryModuleAccountBalancesResponse,
     ]
     """ModuleAccountBalances queries the account balance of x/stablecoin."""
     CirculatingSupplies: grpc.UnaryUnaryMultiCallable[
-        stablecoin.v1.query_pb2.QueryCirculatingSupplies,
-        stablecoin.v1.query_pb2.QueryCirculatingSuppliesResponse,
+        stablecoin.query_pb2.QueryCirculatingSupplies,
+        stablecoin.query_pb2.QueryCirculatingSuppliesResponse,
     ]
     LiquidityRatioInfo: grpc.UnaryUnaryMultiCallable[
-        stablecoin.v1.query_pb2.QueryLiquidityRatioInfoRequest,
-        stablecoin.v1.query_pb2.QueryLiquidityRatioInfoResponse,
+        stablecoin.query_pb2.QueryLiquidityRatioInfoRequest,
+        stablecoin.query_pb2.QueryLiquidityRatioInfoResponse,
     ]
 
 class QueryServicer(metaclass=abc.ABCMeta):
     """Query defines the gRPC querier service."""
 
     @abc.abstractmethod
     def Params(
         self,
-        request: stablecoin.v1.query_pb2.QueryParamsRequest,
+        request: stablecoin.query_pb2.QueryParamsRequest,
         context: grpc.ServicerContext,
-    ) -> stablecoin.v1.query_pb2.QueryParamsResponse:
+    ) -> stablecoin.query_pb2.QueryParamsResponse:
         """Parameters queries the parameters of the x/stablecoin module."""
     @abc.abstractmethod
     def ModuleAccountBalances(
         self,
-        request: stablecoin.v1.query_pb2.QueryModuleAccountBalances,
+        request: stablecoin.query_pb2.QueryModuleAccountBalances,
         context: grpc.ServicerContext,
-    ) -> stablecoin.v1.query_pb2.QueryModuleAccountBalancesResponse:
+    ) -> stablecoin.query_pb2.QueryModuleAccountBalancesResponse:
         """ModuleAccountBalances queries the account balance of x/stablecoin."""
     @abc.abstractmethod
     def CirculatingSupplies(
         self,
-        request: stablecoin.v1.query_pb2.QueryCirculatingSupplies,
+        request: stablecoin.query_pb2.QueryCirculatingSupplies,
         context: grpc.ServicerContext,
-    ) -> stablecoin.v1.query_pb2.QueryCirculatingSuppliesResponse: ...
+    ) -> stablecoin.query_pb2.QueryCirculatingSuppliesResponse: ...
     @abc.abstractmethod
     def LiquidityRatioInfo(
         self,
-        request: stablecoin.v1.query_pb2.QueryLiquidityRatioInfoRequest,
+        request: stablecoin.query_pb2.QueryLiquidityRatioInfoRequest,
         context: grpc.ServicerContext,
-    ) -> stablecoin.v1.query_pb2.QueryLiquidityRatioInfoResponse: ...
+    ) -> stablecoin.query_pb2.QueryLiquidityRatioInfoResponse: ...
 
 def add_QueryServicer_to_server(servicer: QueryServicer, server: grpc.Server) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/tx_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/tx_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: stablecoin/v1/tx.proto
+# source: stablecoin/tx.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
@@ -12,18 +12,18 @@
 
 
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16stablecoin/v1/tx.proto\x12\x14nibiru.stablecoin.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"Q\n\rMsgMintStable\x12\x0f\n\x07\x63reator\x18\x01 \x01(\t\x12/\n\x06stable\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\x8a\x02\n\x15MsgMintStableResponse\x12/\n\x06stable\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12_\n\nused_coins\x18\x02 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\x12_\n\nfees_payed\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\"Q\n\rMsgBurnStable\x12\x0f\n\x07\x63reator\x18\x01 \x01(\t\x12/\n\x06stable\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\xdb\x01\n\x15MsgBurnStableResponse\x12\x33\n\ncollateral\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12,\n\x03gov\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12_\n\nfees_payed\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\"T\n\x12MsgRecollateralize\x12\x0f\n\x07\x63reator\x18\x01 \x01(\t\x12-\n\x04\x63oll\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"J\n\x1aMsgRecollateralizeResponse\x12,\n\x03gov\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"K\n\nMsgBuyback\x12\x0f\n\x07\x63reator\x18\x01 \x01(\t\x12,\n\x03gov\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"C\n\x12MsgBuybackResponse\x12-\n\x04\x63oll\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x32\x9d\x04\n\x03Msg\x12\x82\x01\n\nMintStable\x12#.nibiru.stablecoin.v1.MsgMintStable\x1a+.nibiru.stablecoin.v1.MsgMintStableResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/stablecoin/mint-sc\x12\x82\x01\n\nBurnStable\x12#.nibiru.stablecoin.v1.MsgBurnStable\x1a+.nibiru.stablecoin.v1.MsgBurnStableResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/stablecoin/burn-sc\x12\x90\x01\n\x0fRecollateralize\x12(.nibiru.stablecoin.v1.MsgRecollateralize\x1a\x30.nibiru.stablecoin.v1.MsgRecollateralizeResponse\"!\x82\xd3\xe4\x93\x02\x1b\"\x19/nibiru/stablecoin/recoll\x12y\n\x07\x42uyback\x12 .nibiru.stablecoin.v1.MsgBuyback\x1a(.nibiru.stablecoin.v1.MsgBuybackResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/stablecoin/buybackB2Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13stablecoin/tx.proto\x12\x14nibiru.stablecoin.v1\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\"Q\n\rMsgMintStable\x12\x0f\n\x07\x63reator\x18\x01 \x01(\t\x12/\n\x06stable\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\x8a\x02\n\x15MsgMintStableResponse\x12/\n\x06stable\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12_\n\nused_coins\x18\x02 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\x12_\n\nfees_payed\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\"Q\n\rMsgBurnStable\x12\x0f\n\x07\x63reator\x18\x01 \x01(\t\x12/\n\x06stable\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"\xdb\x01\n\x15MsgBurnStableResponse\x12\x33\n\ncollateral\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12,\n\x03gov\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x12_\n\nfees_payed\x18\x03 \x03(\x0b\x32\x19.cosmos.base.v1beta1.CoinB0\xc8\xde\x1f\x00\xaa\xdf\x1f(github.com/cosmos/cosmos-sdk/types.Coins\"T\n\x12MsgRecollateralize\x12\x0f\n\x07\x63reator\x18\x01 \x01(\t\x12-\n\x04\x63oll\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"J\n\x1aMsgRecollateralizeResponse\x12,\n\x03gov\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"K\n\nMsgBuyback\x12\x0f\n\x07\x63reator\x18\x01 \x01(\t\x12,\n\x03gov\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\"C\n\x12MsgBuybackResponse\x12-\n\x04\x63oll\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00\x32\x9d\x04\n\x03Msg\x12\x82\x01\n\nMintStable\x12#.nibiru.stablecoin.v1.MsgMintStable\x1a+.nibiru.stablecoin.v1.MsgMintStableResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/stablecoin/mint-sc\x12\x82\x01\n\nBurnStable\x12#.nibiru.stablecoin.v1.MsgBurnStable\x1a+.nibiru.stablecoin.v1.MsgBurnStableResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/stablecoin/burn-sc\x12\x90\x01\n\x0fRecollateralize\x12(.nibiru.stablecoin.v1.MsgRecollateralize\x1a\x30.nibiru.stablecoin.v1.MsgRecollateralizeResponse\"!\x82\xd3\xe4\x93\x02\x1b\"\x19/nibiru/stablecoin/recoll\x12y\n\x07\x42uyback\x12 .nibiru.stablecoin.v1.MsgBuyback\x1a(.nibiru.stablecoin.v1.MsgBuybackResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x1a/nibiru/stablecoin/buybackB2Z0github.com/NibiruChain/nibiru/x/stablecoin/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.v1.tx_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stablecoin.tx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z0github.com/NibiruChain/nibiru/x/stablecoin/types'
   _MSGMINTSTABLE.fields_by_name['stable']._options = None
   _MSGMINTSTABLE.fields_by_name['stable']._serialized_options = b'\310\336\037\000'
   _MSGMINTSTABLERESPONSE.fields_by_name['stable']._options = None
@@ -52,26 +52,26 @@
   _MSG.methods_by_name['MintStable']._serialized_options = b'\202\323\344\223\002\034\"\032/nibiru/stablecoin/mint-sc'
   _MSG.methods_by_name['BurnStable']._options = None
   _MSG.methods_by_name['BurnStable']._serialized_options = b'\202\323\344\223\002\034\"\032/nibiru/stablecoin/burn-sc'
   _MSG.methods_by_name['Recollateralize']._options = None
   _MSG.methods_by_name['Recollateralize']._serialized_options = b'\202\323\344\223\002\033\"\031/nibiru/stablecoin/recoll'
   _MSG.methods_by_name['Buyback']._options = None
   _MSG.methods_by_name['Buyback']._serialized_options = b'\202\323\344\223\002\034\"\032/nibiru/stablecoin/buyback'
-  _MSGMINTSTABLE._serialized_start=132
-  _MSGMINTSTABLE._serialized_end=213
-  _MSGMINTSTABLERESPONSE._serialized_start=216
-  _MSGMINTSTABLERESPONSE._serialized_end=482
-  _MSGBURNSTABLE._serialized_start=484
-  _MSGBURNSTABLE._serialized_end=565
-  _MSGBURNSTABLERESPONSE._serialized_start=568
-  _MSGBURNSTABLERESPONSE._serialized_end=787
-  _MSGRECOLLATERALIZE._serialized_start=789
-  _MSGRECOLLATERALIZE._serialized_end=873
-  _MSGRECOLLATERALIZERESPONSE._serialized_start=875
-  _MSGRECOLLATERALIZERESPONSE._serialized_end=949
-  _MSGBUYBACK._serialized_start=951
-  _MSGBUYBACK._serialized_end=1026
-  _MSGBUYBACKRESPONSE._serialized_start=1028
-  _MSGBUYBACKRESPONSE._serialized_end=1095
-  _MSG._serialized_start=1098
-  _MSG._serialized_end=1639
+  _MSGMINTSTABLE._serialized_start=129
+  _MSGMINTSTABLE._serialized_end=210
+  _MSGMINTSTABLERESPONSE._serialized_start=213
+  _MSGMINTSTABLERESPONSE._serialized_end=479
+  _MSGBURNSTABLE._serialized_start=481
+  _MSGBURNSTABLE._serialized_end=562
+  _MSGBURNSTABLERESPONSE._serialized_start=565
+  _MSGBURNSTABLERESPONSE._serialized_end=784
+  _MSGRECOLLATERALIZE._serialized_start=786
+  _MSGRECOLLATERALIZE._serialized_end=870
+  _MSGRECOLLATERALIZERESPONSE._serialized_start=872
+  _MSGRECOLLATERALIZERESPONSE._serialized_end=946
+  _MSGBUYBACK._serialized_start=948
+  _MSGBUYBACK._serialized_end=1023
+  _MSGBUYBACKRESPONSE._serialized_start=1025
+  _MSGBUYBACKRESPONSE._serialized_end=1092
+  _MSG._serialized_start=1095
+  _MSG._serialized_end=1636
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/tx_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/tx_pb2_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from stablecoin.v1 import tx_pb2 as stablecoin_dot_v1_dot_tx__pb2
+from stablecoin import tx_pb2 as stablecoin_dot_tx__pb2
 
 
 class MsgStub(object):
     """Msg defines the x/stablecoin Msg service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.MintStable = channel.unary_unary(
                 '/nibiru.stablecoin.v1.Msg/MintStable',
-                request_serializer=stablecoin_dot_v1_dot_tx__pb2.MsgMintStable.SerializeToString,
-                response_deserializer=stablecoin_dot_v1_dot_tx__pb2.MsgMintStableResponse.FromString,
+                request_serializer=stablecoin_dot_tx__pb2.MsgMintStable.SerializeToString,
+                response_deserializer=stablecoin_dot_tx__pb2.MsgMintStableResponse.FromString,
                 )
         self.BurnStable = channel.unary_unary(
                 '/nibiru.stablecoin.v1.Msg/BurnStable',
-                request_serializer=stablecoin_dot_v1_dot_tx__pb2.MsgBurnStable.SerializeToString,
-                response_deserializer=stablecoin_dot_v1_dot_tx__pb2.MsgBurnStableResponse.FromString,
+                request_serializer=stablecoin_dot_tx__pb2.MsgBurnStable.SerializeToString,
+                response_deserializer=stablecoin_dot_tx__pb2.MsgBurnStableResponse.FromString,
                 )
         self.Recollateralize = channel.unary_unary(
                 '/nibiru.stablecoin.v1.Msg/Recollateralize',
-                request_serializer=stablecoin_dot_v1_dot_tx__pb2.MsgRecollateralize.SerializeToString,
-                response_deserializer=stablecoin_dot_v1_dot_tx__pb2.MsgRecollateralizeResponse.FromString,
+                request_serializer=stablecoin_dot_tx__pb2.MsgRecollateralize.SerializeToString,
+                response_deserializer=stablecoin_dot_tx__pb2.MsgRecollateralizeResponse.FromString,
                 )
         self.Buyback = channel.unary_unary(
                 '/nibiru.stablecoin.v1.Msg/Buyback',
-                request_serializer=stablecoin_dot_v1_dot_tx__pb2.MsgBuyback.SerializeToString,
-                response_deserializer=stablecoin_dot_v1_dot_tx__pb2.MsgBuybackResponse.FromString,
+                request_serializer=stablecoin_dot_tx__pb2.MsgBuyback.SerializeToString,
+                response_deserializer=stablecoin_dot_tx__pb2.MsgBuybackResponse.FromString,
                 )
 
 
 class MsgServicer(object):
     """Msg defines the x/stablecoin Msg service.
     """
 
@@ -77,31 +77,31 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_MsgServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'MintStable': grpc.unary_unary_rpc_method_handler(
                     servicer.MintStable,
-                    request_deserializer=stablecoin_dot_v1_dot_tx__pb2.MsgMintStable.FromString,
-                    response_serializer=stablecoin_dot_v1_dot_tx__pb2.MsgMintStableResponse.SerializeToString,
+                    request_deserializer=stablecoin_dot_tx__pb2.MsgMintStable.FromString,
+                    response_serializer=stablecoin_dot_tx__pb2.MsgMintStableResponse.SerializeToString,
             ),
             'BurnStable': grpc.unary_unary_rpc_method_handler(
                     servicer.BurnStable,
-                    request_deserializer=stablecoin_dot_v1_dot_tx__pb2.MsgBurnStable.FromString,
-                    response_serializer=stablecoin_dot_v1_dot_tx__pb2.MsgBurnStableResponse.SerializeToString,
+                    request_deserializer=stablecoin_dot_tx__pb2.MsgBurnStable.FromString,
+                    response_serializer=stablecoin_dot_tx__pb2.MsgBurnStableResponse.SerializeToString,
             ),
             'Recollateralize': grpc.unary_unary_rpc_method_handler(
                     servicer.Recollateralize,
-                    request_deserializer=stablecoin_dot_v1_dot_tx__pb2.MsgRecollateralize.FromString,
-                    response_serializer=stablecoin_dot_v1_dot_tx__pb2.MsgRecollateralizeResponse.SerializeToString,
+                    request_deserializer=stablecoin_dot_tx__pb2.MsgRecollateralize.FromString,
+                    response_serializer=stablecoin_dot_tx__pb2.MsgRecollateralizeResponse.SerializeToString,
             ),
             'Buyback': grpc.unary_unary_rpc_method_handler(
                     servicer.Buyback,
-                    request_deserializer=stablecoin_dot_v1_dot_tx__pb2.MsgBuyback.FromString,
-                    response_serializer=stablecoin_dot_v1_dot_tx__pb2.MsgBuybackResponse.SerializeToString,
+                    request_deserializer=stablecoin_dot_tx__pb2.MsgBuyback.FromString,
+                    response_serializer=stablecoin_dot_tx__pb2.MsgBuybackResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'nibiru.stablecoin.v1.Msg', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -118,16 +118,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.stablecoin.v1.Msg/MintStable',
-            stablecoin_dot_v1_dot_tx__pb2.MsgMintStable.SerializeToString,
-            stablecoin_dot_v1_dot_tx__pb2.MsgMintStableResponse.FromString,
+            stablecoin_dot_tx__pb2.MsgMintStable.SerializeToString,
+            stablecoin_dot_tx__pb2.MsgMintStableResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def BurnStable(request,
             target,
             options=(),
@@ -135,16 +135,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.stablecoin.v1.Msg/BurnStable',
-            stablecoin_dot_v1_dot_tx__pb2.MsgBurnStable.SerializeToString,
-            stablecoin_dot_v1_dot_tx__pb2.MsgBurnStableResponse.FromString,
+            stablecoin_dot_tx__pb2.MsgBurnStable.SerializeToString,
+            stablecoin_dot_tx__pb2.MsgBurnStableResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Recollateralize(request,
             target,
             options=(),
@@ -152,16 +152,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.stablecoin.v1.Msg/Recollateralize',
-            stablecoin_dot_v1_dot_tx__pb2.MsgRecollateralize.SerializeToString,
-            stablecoin_dot_v1_dot_tx__pb2.MsgRecollateralizeResponse.FromString,
+            stablecoin_dot_tx__pb2.MsgRecollateralize.SerializeToString,
+            stablecoin_dot_tx__pb2.MsgRecollateralizeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Buyback(request,
             target,
             options=(),
@@ -169,11 +169,11 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/nibiru.stablecoin.v1.Msg/Buyback',
-            stablecoin_dot_v1_dot_tx__pb2.MsgBuyback.SerializeToString,
-            stablecoin_dot_v1_dot_tx__pb2.MsgBuybackResponse.FromString,
+            stablecoin_dot_tx__pb2.MsgBuyback.SerializeToString,
+            stablecoin_dot_tx__pb2.MsgBuybackResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/stablecoin/v1/tx_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/stablecoin/tx_pb2_grpc.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import grpc
-import stablecoin.v1.tx_pb2
+import stablecoin.tx_pb2
 
 class MsgStub:
     """Msg defines the x/stablecoin Msg service."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
     MintStable: grpc.UnaryUnaryMultiCallable[
-        stablecoin.v1.tx_pb2.MsgMintStable,
-        stablecoin.v1.tx_pb2.MsgMintStableResponse,
+        stablecoin.tx_pb2.MsgMintStable,
+        stablecoin.tx_pb2.MsgMintStableResponse,
     ]
     """MintStable defines a method for trading a mixture of GOV and COLL to mint an 
     equivalent value of stablecoins.
     """
     BurnStable: grpc.UnaryUnaryMultiCallable[
-        stablecoin.v1.tx_pb2.MsgBurnStable,
-        stablecoin.v1.tx_pb2.MsgBurnStableResponse,
+        stablecoin.tx_pb2.MsgBurnStable,
+        stablecoin.tx_pb2.MsgBurnStableResponse,
     ]
     """BurnStable defines a method for redeeming/burning stablecoins to receive an 
     equivalent value as a mixture of governance and collateral tokens.
     """
     Recollateralize: grpc.UnaryUnaryMultiCallable[
-        stablecoin.v1.tx_pb2.MsgRecollateralize,
-        stablecoin.v1.tx_pb2.MsgRecollateralizeResponse,
+        stablecoin.tx_pb2.MsgRecollateralize,
+        stablecoin.tx_pb2.MsgRecollateralizeResponse,
     ]
     """Recollateralize defines a method for manually adding collateral to the 
     protocol in exchange for an equivalent stablecoin value in governance tokens 
     plus a small bonus.
     """
     Buyback: grpc.UnaryUnaryMultiCallable[
-        stablecoin.v1.tx_pb2.MsgBuyback,
-        stablecoin.v1.tx_pb2.MsgBuybackResponse,
+        stablecoin.tx_pb2.MsgBuyback,
+        stablecoin.tx_pb2.MsgBuybackResponse,
     ]
     """Buyback defines a method for manually adding NIBI to the protocol 
     in exchange for an equivalent stablecoin value in collateral, effectively 
     executing a share buyback for Nibiru Chain. The NIBI purchased by the protocol 
     is then burned, distributing value to all NIBI hodlers.
     """
 
 class MsgServicer(metaclass=abc.ABCMeta):
     """Msg defines the x/stablecoin Msg service."""
 
     @abc.abstractmethod
     def MintStable(
         self,
-        request: stablecoin.v1.tx_pb2.MsgMintStable,
+        request: stablecoin.tx_pb2.MsgMintStable,
         context: grpc.ServicerContext,
-    ) -> stablecoin.v1.tx_pb2.MsgMintStableResponse:
+    ) -> stablecoin.tx_pb2.MsgMintStableResponse:
         """MintStable defines a method for trading a mixture of GOV and COLL to mint an 
         equivalent value of stablecoins.
         """
     @abc.abstractmethod
     def BurnStable(
         self,
-        request: stablecoin.v1.tx_pb2.MsgBurnStable,
+        request: stablecoin.tx_pb2.MsgBurnStable,
         context: grpc.ServicerContext,
-    ) -> stablecoin.v1.tx_pb2.MsgBurnStableResponse:
+    ) -> stablecoin.tx_pb2.MsgBurnStableResponse:
         """BurnStable defines a method for redeeming/burning stablecoins to receive an 
         equivalent value as a mixture of governance and collateral tokens.
         """
     @abc.abstractmethod
     def Recollateralize(
         self,
-        request: stablecoin.v1.tx_pb2.MsgRecollateralize,
+        request: stablecoin.tx_pb2.MsgRecollateralize,
         context: grpc.ServicerContext,
-    ) -> stablecoin.v1.tx_pb2.MsgRecollateralizeResponse:
+    ) -> stablecoin.tx_pb2.MsgRecollateralizeResponse:
         """Recollateralize defines a method for manually adding collateral to the 
         protocol in exchange for an equivalent stablecoin value in governance tokens 
         plus a small bonus.
         """
     @abc.abstractmethod
     def Buyback(
         self,
-        request: stablecoin.v1.tx_pb2.MsgBuyback,
+        request: stablecoin.tx_pb2.MsgBuyback,
         context: grpc.ServicerContext,
-    ) -> stablecoin.v1.tx_pb2.MsgBuybackResponse:
+    ) -> stablecoin.tx_pb2.MsgBuybackResponse:
         """Buyback defines a method for manually adding NIBI to the protocol 
         in exchange for an equivalent stablecoin value in collateral, effectively 
         executing a share buyback for Nibiru Chain. The NIBI purchased by the protocol 
         is then burned, distributing value to all NIBI hodlers.
         """
 
 def add_MsgServicer_to_server(servicer: MsgServicer, server: grpc.Server) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/event_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/keys_pb2.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import sudo.v1.state_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class EventUpdateSudoers(google.protobuf.message.Message):
+class PublicKey(google.protobuf.message.Message):
+    """PublicKey defines the keys available for use with Tendermint Validators"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    SUDOERS_FIELD_NUMBER: builtins.int
-    ACTION_FIELD_NUMBER: builtins.int
-    @property
-    def sudoers(self) -> sudo.v1.state_pb2.Sudoers: ...
-    action: builtins.str
-    """Action is the type of update that occured to the "sudoers" """
+    ED25519_FIELD_NUMBER: builtins.int
+    SECP256K1_FIELD_NUMBER: builtins.int
+    ed25519: builtins.bytes
+    secp256k1: builtins.bytes
     def __init__(
         self,
         *,
-        sudoers: sudo.v1.state_pb2.Sudoers | None = ...,
-        action: builtins.str = ...,
+        ed25519: builtins.bytes = ...,
+        secp256k1: builtins.bytes = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["sudoers", b"sudoers"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action", b"action", "sudoers", b"sudoers"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["ed25519", b"ed25519", "secp256k1", b"secp256k1", "sum", b"sum"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["ed25519", b"ed25519", "secp256k1", b"secp256k1", "sum", b"sum"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sum", b"sum"]) -> typing_extensions.Literal["ed25519", "secp256k1"] | None: ...
 
-global___EventUpdateSudoers = EventUpdateSudoers
+global___PublicKey = PublicKey
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/query_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/genesis_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: sudo/v1/query.proto
+# source: vpool/v1/genesis.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from sudo.v1 import state_pb2 as sudo_dot_v1_dot_state__pb2
+from vpool.v1 import state_pb2 as vpool_dot_v1_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13sudo/v1/query.proto\x12\x0enibiru.sudo.v1\x1a\x14gogoproto/gogo.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x13sudo/v1/state.proto\"\x15\n\x13QuerySudoersRequest\"F\n\x14QuerySudoersResponse\x12.\n\x07sudoers\x18\x01 \x01(\x0b\x32\x17.nibiru.sudo.v1.SudoersB\x04\xc8\xde\x1f\x00\x32\x80\x01\n\x05Query\x12w\n\x0cQuerySudoers\x12#.nibiru.sudo.v1.QuerySudoersRequest\x1a$.nibiru.sudo.v1.QuerySudoersResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/nibiru/sudo/sudoersB)Z\'github.com/NibiruChain/nibiru/x/sudo/pbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16vpool/v1/genesis.proto\x12\x0fnibiru.vpool.v1\x1a\x14gogoproto/gogo.proto\x1a\x14vpool/v1/state.proto\"<\n\x0cGenesisState\x12,\n\x06vpools\x18\x01 \x03(\x0b\x32\x16.nibiru.vpool.v1.VpoolB\x04\xc8\xde\x1f\x00\x42-Z+github.com/NibiruChain/nibiru/x/vpool/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sudo.v1.query_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'vpool.v1.genesis_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\'github.com/NibiruChain/nibiru/x/sudo/pb'
-  _QUERYSUDOERSRESPONSE.fields_by_name['sudoers']._options = None
-  _QUERYSUDOERSRESPONSE.fields_by_name['sudoers']._serialized_options = b'\310\336\037\000'
-  _QUERY.methods_by_name['QuerySudoers']._options = None
-  _QUERY.methods_by_name['QuerySudoers']._serialized_options = b'\202\323\344\223\002\026\022\024/nibiru/sudo/sudoers'
-  _QUERYSUDOERSREQUEST._serialized_start=112
-  _QUERYSUDOERSREQUEST._serialized_end=133
-  _QUERYSUDOERSRESPONSE._serialized_start=135
-  _QUERYSUDOERSRESPONSE._serialized_end=205
-  _QUERY._serialized_start=208
-  _QUERY._serialized_end=336
+  DESCRIPTOR._serialized_options = b'Z+github.com/NibiruChain/nibiru/x/vpool/types'
+  _GENESISSTATE.fields_by_name['vpools']._options = None
+  _GENESISSTATE.fields_by_name['vpools']._serialized_options = b'\310\336\037\000'
+  _GENESISSTATE._serialized_start=87
+  _GENESISSTATE._serialized_end=147
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/query_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/util/v1/query_pb2_grpc.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import grpc
-import sudo.v1.query_pb2
+import util.v1.query_pb2
 
 class QueryStub:
     """Query defines the gRPC querier service."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
-    QuerySudoers: grpc.UnaryUnaryMultiCallable[
-        sudo.v1.query_pb2.QuerySudoersRequest,
-        sudo.v1.query_pb2.QuerySudoersResponse,
+    ModuleAccounts: grpc.UnaryUnaryMultiCallable[
+        util.v1.query_pb2.QueryModuleAccountsRequest,
+        util.v1.query_pb2.QueryModuleAccountsResponse,
     ]
+    """Queries the reserve assets in a given pool, identified by a token pair."""
 
 class QueryServicer(metaclass=abc.ABCMeta):
     """Query defines the gRPC querier service."""
 
     @abc.abstractmethod
-    def QuerySudoers(
+    def ModuleAccounts(
         self,
-        request: sudo.v1.query_pb2.QuerySudoersRequest,
+        request: util.v1.query_pb2.QueryModuleAccountsRequest,
         context: grpc.ServicerContext,
-    ) -> sudo.v1.query_pb2.QuerySudoersResponse: ...
+    ) -> util.v1.query_pb2.QueryModuleAccountsResponse:
+        """Queries the reserve assets in a given pool, identified by a token pair."""
 
 def add_QueryServicer_to_server(servicer: QueryServicer, server: grpc.Server) -> None: ...
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/sudo/v1/tx_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/util/v1/query_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import collections.abc
+import cosmos.base.v1beta1.coin_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class MsgEditSudoers(google.protobuf.message.Message):
-    """-------------------------- EditSudoers --------------------------
+class QueryModuleAccountsRequest(google.protobuf.message.Message):
+    """----------------------------------------"""
 
-    MsgEditSudoers: Msg to update the "Sudoers" state.
-    """
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
 
+global___QueryModuleAccountsRequest = QueryModuleAccountsRequest
+
+@typing_extensions.final
+class QueryModuleAccountsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ACTION_FIELD_NUMBER: builtins.int
-    CONTRACTS_FIELD_NUMBER: builtins.int
-    SENDER_FIELD_NUMBER: builtins.int
-    action: builtins.str
-    """Action: identifier for the type of edit that will take place. Using this 
-      action field prevents us from needing to create several similar message 
-      types.
-    """
+    ACCOUNTS_FIELD_NUMBER: builtins.int
     @property
-    def contracts(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Contracts: An input payload."""
-    sender: builtins.str
-    """Sender: Address for the signer of the transaction."""
+    def accounts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AccountWithBalance]: ...
     def __init__(
         self,
         *,
-        action: builtins.str = ...,
-        contracts: collections.abc.Iterable[builtins.str] | None = ...,
-        sender: builtins.str = ...,
+        accounts: collections.abc.Iterable[global___AccountWithBalance] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action", b"action", "contracts", b"contracts", "sender", b"sender"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["accounts", b"accounts"]) -> None: ...
 
-global___MsgEditSudoers = MsgEditSudoers
+global___QueryModuleAccountsResponse = QueryModuleAccountsResponse
 
 @typing_extensions.final
-class MsgEditSudoersResponse(google.protobuf.message.Message):
-    """MsgEditSudoersResponse indicates the successful execution of MsgEditSudeors."""
-
+class AccountWithBalance(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    NAME_FIELD_NUMBER: builtins.int
+    ADDRESS_FIELD_NUMBER: builtins.int
+    BALANCE_FIELD_NUMBER: builtins.int
+    name: builtins.str
+    address: builtins.str
+    @property
+    def balance(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
         self,
+        *,
+        name: builtins.str = ...,
+        address: builtins.str = ...,
+        balance: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "balance", b"balance", "name", b"name"]) -> None: ...
 
-global___MsgEditSudoersResponse = MsgEditSudoersResponse
+global___AccountWithBalance = AccountWithBalance
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/abci/types_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/abci/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/abci/types_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/abci/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/abci/types_pb2_grpc.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/abci/types_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/abci/types_pb2_grpc.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/abci/types_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/keys_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/validator_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/crypto/keys.proto
+# source: tendermint/types/validator.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
+from tendermint.crypto import keys_pb2 as tendermint_dot_crypto_dot_keys__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctendermint/crypto/keys.proto\x12\x11tendermint.crypto\x1a\x14gogoproto/gogo.proto\"D\n\tPublicKey\x12\x11\n\x07\x65\x64\x32\x35\x35\x31\x39\x18\x01 \x01(\x0cH\x00\x12\x13\n\tsecp256k1\x18\x02 \x01(\x0cH\x00:\x08\xe8\xa1\x1f\x01\xe8\xa0\x1f\x01\x42\x05\n\x03sumB:Z8github.com/tendermint/tendermint/proto/tendermint/cryptob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tendermint/types/validator.proto\x12\x10tendermint.types\x1a\x14gogoproto/gogo.proto\x1a\x1ctendermint/crypto/keys.proto\"\x8a\x01\n\x0cValidatorSet\x12/\n\nvalidators\x18\x01 \x03(\x0b\x32\x1b.tendermint.types.Validator\x12-\n\x08proposer\x18\x02 \x01(\x0b\x32\x1b.tendermint.types.Validator\x12\x1a\n\x12total_voting_power\x18\x03 \x01(\x03\"\x82\x01\n\tValidator\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0c\x12\x33\n\x07pub_key\x18\x02 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKeyB\x04\xc8\xde\x1f\x00\x12\x14\n\x0cvoting_power\x18\x03 \x01(\x03\x12\x19\n\x11proposer_priority\x18\x04 \x01(\x03\"V\n\x0fSimpleValidator\x12-\n\x07pub_key\x18\x01 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKey\x12\x14\n\x0cvoting_power\x18\x02 \x01(\x03\x42\x39Z7github.com/tendermint/tendermint/proto/tendermint/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.crypto.keys_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.validator_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z8github.com/tendermint/tendermint/proto/tendermint/crypto'
-  _PUBLICKEY._options = None
-  _PUBLICKEY._serialized_options = b'\350\241\037\001\350\240\037\001'
-  _PUBLICKEY._serialized_start=73
-  _PUBLICKEY._serialized_end=141
+  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types'
+  _VALIDATOR.fields_by_name['pub_key']._options = None
+  _VALIDATOR.fields_by_name['pub_key']._serialized_options = b'\310\336\037\000'
+  _VALIDATORSET._serialized_start=107
+  _VALIDATORSET._serialized_end=245
+  _VALIDATOR._serialized_start=248
+  _VALIDATOR._serialized_end=378
+  _SIMPLEVALIDATOR._serialized_start=380
+  _SIMPLEVALIDATOR._serialized_end=466
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/keys_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/libs/bits/types_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class PublicKey(google.protobuf.message.Message):
-    """PublicKey defines the keys available for use with Tendermint Validators"""
-
+class BitArray(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ED25519_FIELD_NUMBER: builtins.int
-    SECP256K1_FIELD_NUMBER: builtins.int
-    ed25519: builtins.bytes
-    secp256k1: builtins.bytes
+    BITS_FIELD_NUMBER: builtins.int
+    ELEMS_FIELD_NUMBER: builtins.int
+    bits: builtins.int
+    @property
+    def elems(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
-        ed25519: builtins.bytes = ...,
-        secp256k1: builtins.bytes = ...,
+        bits: builtins.int = ...,
+        elems: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["ed25519", b"ed25519", "secp256k1", b"secp256k1", "sum", b"sum"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ed25519", b"ed25519", "secp256k1", b"secp256k1", "sum", b"sum"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["sum", b"sum"]) -> typing_extensions.Literal["ed25519", "secp256k1"] | None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bits", b"bits", "elems", b"elems"]) -> None: ...
 
-global___PublicKey = PublicKey
+global___BitArray = BitArray
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/proof_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/proof_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/crypto/proof_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/crypto/proof_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/libs/bits/types_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/libs/bits/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/libs/bits/types_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/vpool/v1/genesis_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
+import vpool.v1.state_pb2
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class BitArray(google.protobuf.message.Message):
+class GenesisState(google.protobuf.message.Message):
+    """GenesisState defines the vpool module's genesis state."""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    BITS_FIELD_NUMBER: builtins.int
-    ELEMS_FIELD_NUMBER: builtins.int
-    bits: builtins.int
+    VPOOLS_FIELD_NUMBER: builtins.int
     @property
-    def elems(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    def vpools(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[vpool.v1.state_pb2.Vpool]: ...
     def __init__(
         self,
         *,
-        bits: builtins.int = ...,
-        elems: collections.abc.Iterable[builtins.int] | None = ...,
+        vpools: collections.abc.Iterable[vpool.v1.state_pb2.Vpool] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bits", b"bits", "elems", b"elems"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["vpools", b"vpools"]) -> None: ...
 
-global___BitArray = BitArray
+global___GenesisState = GenesisState
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/p2p/types_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/p2p/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/p2p/types_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/p2p/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/block_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/block_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/block_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/evidence_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/evidence_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/params_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/params_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/types_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/types_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/validator_pb2.py` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/version/types_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tendermint/types/validator.proto
+# source: tendermint/version/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-from tendermint.crypto import keys_pb2 as tendermint_dot_crypto_dot_keys__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tendermint/types/validator.proto\x12\x10tendermint.types\x1a\x14gogoproto/gogo.proto\x1a\x1ctendermint/crypto/keys.proto\"\x8a\x01\n\x0cValidatorSet\x12/\n\nvalidators\x18\x01 \x03(\x0b\x32\x1b.tendermint.types.Validator\x12-\n\x08proposer\x18\x02 \x01(\x0b\x32\x1b.tendermint.types.Validator\x12\x1a\n\x12total_voting_power\x18\x03 \x01(\x03\"\x82\x01\n\tValidator\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0c\x12\x33\n\x07pub_key\x18\x02 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKeyB\x04\xc8\xde\x1f\x00\x12\x14\n\x0cvoting_power\x18\x03 \x01(\x03\x12\x19\n\x11proposer_priority\x18\x04 \x01(\x03\"V\n\x0fSimpleValidator\x12-\n\x07pub_key\x18\x01 \x01(\x0b\x32\x1c.tendermint.crypto.PublicKey\x12\x14\n\x0cvoting_power\x18\x02 \x01(\x03\x42\x39Z7github.com/tendermint/tendermint/proto/tendermint/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1etendermint/version/types.proto\x12\x12tendermint.version\x1a\x14gogoproto/gogo.proto\")\n\x03\x41pp\x12\x10\n\x08protocol\x18\x01 \x01(\x04\x12\x10\n\x08software\x18\x02 \x01(\t\"-\n\tConsensus\x12\r\n\x05\x62lock\x18\x01 \x01(\x04\x12\x0b\n\x03\x61pp\x18\x02 \x01(\x04:\x04\xe8\xa0\x1f\x01\x42;Z9github.com/tendermint/tendermint/proto/tendermint/versionb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.types.validator_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tendermint.version.types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z7github.com/tendermint/tendermint/proto/tendermint/types'
-  _VALIDATOR.fields_by_name['pub_key']._options = None
-  _VALIDATOR.fields_by_name['pub_key']._serialized_options = b'\310\336\037\000'
-  _VALIDATORSET._serialized_start=107
-  _VALIDATORSET._serialized_end=245
-  _VALIDATOR._serialized_start=248
-  _VALIDATOR._serialized_end=378
-  _SIMPLEVALIDATOR._serialized_start=380
-  _SIMPLEVALIDATOR._serialized_end=466
+  DESCRIPTOR._serialized_options = b'Z9github.com/tendermint/tendermint/proto/tendermint/version'
+  _CONSENSUS._options = None
+  _CONSENSUS._serialized_options = b'\350\240\037\001'
+  _APP._serialized_start=76
+  _APP._serialized_end=117
+  _CONSENSUS._serialized_start=119
+  _CONSENSUS._serialized_end=164
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/types/validator_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/types/validator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/nibiru_proto/proto/tendermint/version/types_pb2.pyi` & `nibiru_proto-0.20.0rc1/nibiru_proto/proto/tendermint/version/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.20.0b5/pyproject.toml` & `nibiru_proto-0.20.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nibiru-proto"
-version = "0.20.0b5"
+version = "0.20.0-rc1"
 description = "Nibiru Chain Python SDK"
 authors = ["Nibiru Chain <dev@nibiru.fi>"]
 packages = [{ include = "nibiru_proto" }]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `nibiru_proto-0.20.0b5/setup.py` & `nibiru_proto-0.20.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,30 +35,30 @@
  'nibiru_proto.proto.cosmos.slashing.v1beta1',
  'nibiru_proto.proto.cosmos.staking.v1beta1',
  'nibiru_proto.proto.cosmos.tx.signing.v1beta1',
  'nibiru_proto.proto.cosmos.tx.v1beta1',
  'nibiru_proto.proto.cosmos.upgrade.v1beta1',
  'nibiru_proto.proto.cosmos.vesting.v1beta1',
  'nibiru_proto.proto.cosmos_proto',
- 'nibiru_proto.proto.epochs.v1',
+ 'nibiru_proto.proto.epochs',
  'nibiru_proto.proto.gogoproto',
  'nibiru_proto.proto.google.api',
  'nibiru_proto.proto.google.protobuf',
- 'nibiru_proto.proto.inflation.v1',
- 'nibiru_proto.proto.oracle.v1',
- 'nibiru_proto.proto.perp.v2',
+ 'nibiru_proto.proto.oracle.v1beta1',
+ 'nibiru_proto.proto.perp.v1',
  'nibiru_proto.proto.spot.v1',
- 'nibiru_proto.proto.stablecoin.v1',
- 'nibiru_proto.proto.sudo.v1',
+ 'nibiru_proto.proto.stablecoin',
  'nibiru_proto.proto.tendermint.abci',
  'nibiru_proto.proto.tendermint.crypto',
  'nibiru_proto.proto.tendermint.libs.bits',
  'nibiru_proto.proto.tendermint.p2p',
  'nibiru_proto.proto.tendermint.types',
- 'nibiru_proto.proto.tendermint.version']
+ 'nibiru_proto.proto.tendermint.version',
+ 'nibiru_proto.proto.util.v1',
+ 'nibiru_proto.proto.vpool.v1']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['asyncio>=3.4.3,<4.0.0',
  'bech32>=1.2.0,<2.0.0',
@@ -66,15 +66,15 @@
  'grpcio>=1.51.1,<2.0.0',
  'mypy-protobuf>=3.4.0,<4.0.0',
  'protobuf>=4.21.12,<5.0.0',
  'types-protobuf>=4.21.0.2,<5.0.0.0']
 
 setup_kwargs = {
     'name': 'nibiru-proto',
-    'version': '0.20.0b5',
+    'version': '0.20.0rc1',
     'description': 'Nibiru Chain Python SDK',
     'long_description': 'None',
     'author': 'Nibiru Chain',
     'author_email': 'dev@nibiru.fi',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nibiru_proto-0.20.0b5/PKG-INFO` & `nibiru_proto-0.20.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibiru-proto
-Version: 0.20.0b5
+Version: 0.20.0rc1
 Summary: Nibiru Chain Python SDK
 License: MIT
 Author: Nibiru Chain
 Author-email: dev@nibiru.fi
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

