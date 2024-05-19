# Comparing `tmp/toc_trade_pb_v2-0.1.4.tar.gz` & `tmp/toc_trade_pb_v2-0.1.7.tar.gz`

## Comparing `toc_trade_pb_v2-0.1.4.tar` & `toc_trade_pb_v2-0.1.7.tar`

### file list

```diff
@@ -1,71 +1,113 @@
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/Makefile
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/go.mod
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/go.sum
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/package-lock.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/package.json
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/.github/workflows/main.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/app/app.proto
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/basic.proto
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/entity.proto
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/history.proto
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/mq.proto
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/realtime.proto
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/subscribe.proto
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/protos/v3/forwarder/trade.proto
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/scripts/gomod_update.sh
--rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/scripts/modify_py_import.sh
--rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/app.pb.go
--rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/basic.pb.go
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/basic_grpc.pb.go
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/entity.pb.go
--rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/history.pb.go
--rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/history_grpc.pb.go
--rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/mq.pb.go
--rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/realtime.pb.go
--rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/realtime_grpc.pb.go
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/subscribe.pb.go
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/subscribe_grpc.pb.go
--rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/trade.pb.go
--rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/golang/pb/trade_grpc.pb.go
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/__init__.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2.pyi
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/__init__.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2.pyi
--rw-r--r--   0        0        0     9478 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
--rw-r--r--   0        0        0    20666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
--rw-r--r--   0        0        0    35687 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
--rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/app/app.ts
--rw-r--r--   0        0        0    46501 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/basic.ts
--rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/entity.ts
--rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/history.ts
--rw-r--r--   0        0        0    75768 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/mq.ts
--rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/realtime.ts
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/subscribe.ts
--rw-r--r--   0        0        0    91499 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/forwarder/trade.ts
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/src/ts/google/protobuf/empty.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/tests/.gitkeep
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/Makefile
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/go.mod
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/go.sum
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/package-lock.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/package.json
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/pubspec.lock
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/pubspec.yaml
+-rwxr-xr-x   0        0        0      504 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/.chglog/config.yml
+-rw-r--r--   0        0        0    16456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/app/app.pb.dart
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/app/app.pbenum.dart
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/app/app.pbjson.dart
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/app/app.pbserver.dart
+-rw-r--r--   0        0        0    33911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pb.dart
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pbenum.dart
+-rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pbjson.dart
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pbserver.dart
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pb.dart
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pbenum.dart
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pbjson.dart
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pbserver.dart
+-rw-r--r--   0        0        0    30778 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/history.pb.dart
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/history.pbenum.dart
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/history.pbjson.dart
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/history.pbserver.dart
+-rw-r--r--   0        0        0    46124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pb.dart
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pbenum.dart
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pbjson.dart
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pbserver.dart
+-rw-r--r--   0        0        0    36869 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pb.dart
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pbenum.dart
+-rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pbjson.dart
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pbserver.dart
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pb.dart
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pbenum.dart
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pbjson.dart
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pbserver.dart
+-rw-r--r--   0        0        0    69695 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pb.dart
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pbenum.dart
+-rw-r--r--   0        0        0    20594 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pbjson.dart
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pbserver.dart
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pb.dart
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pbenum.dart
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pbjson.dart
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pbserver.dart
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/app/app.proto
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/basic.proto
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/entity.proto
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/history.proto
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/mq.proto
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/realtime.proto
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/subscribe.proto
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/trade.proto
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/scripts/gomod_update.sh
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/scripts/modify_py_import.sh
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/scripts/update_dependency.sh
+-rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/app.pb.go
+-rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/basic.pb.go
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/basic_grpc.pb.go
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/entity.pb.go
+-rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/history.pb.go
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/history_grpc.pb.go
+-rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/mq.pb.go
+-rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/realtime.pb.go
+-rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/realtime_grpc.pb.go
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/subscribe.pb.go
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/subscribe_grpc.pb.go
+-rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/trade.pb.go
+-rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/trade_grpc.pb.go
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/__init__.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2.pyi
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/__init__.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2.pyi
+-rw-r--r--   0        0        0     9478 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
+-rw-r--r--   0        0        0    20666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
+-rw-r--r--   0        0        0    35687 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
+-rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/app/app.ts
+-rw-r--r--   0        0        0    46501 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/basic.ts
+-rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/entity.ts
+-rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/history.ts
+-rw-r--r--   0        0        0    75768 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/mq.ts
+-rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/realtime.ts
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/subscribe.ts
+-rw-r--r--   0        0        0    91499 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/trade.ts
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/google/protobuf/empty.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/tests/.gitkeep
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/LICENSE
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/README.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/PKG-INFO
```

### Comparing `toc_trade_pb_v2-0.1.4/Makefile` & `toc_trade_pb_v2-0.1.7/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 PYTHON=$(shell which python3)
 PIP=$(shell which pip3)
+PROTOC_PATH=$(shell which protoc)
+PROTOC_INCLUDE_PATH=$(shell dirname $(shell dirname "$(PROTOC_PATH)"))
+
+compile: compile-go compile-py compile-ts compile-dart
 
 compile-go:
 	@rm -rf src/golang && mkdir -p src/golang
-	@protoc \
+	@$(PROTOC_PATH) \
 	--go_out=src/golang \
 	--go-grpc_out=src/golang \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto
 	@. ./scripts/gomod_update.sh
 
+compile-dart:
+	@rm -rf lib && mkdir -p lib
+	@dart pub global activate --overwrite protoc_plugin
+	@$(PROTOC_PATH) \
+	--dart_out=lib \
+	--proto_path=protos/v3 \
+	./protos/v3/*/*.proto \
+	$(PROTOC_INCLUDE_PATH)/include/google/protobuf/empty.proto
+
 compile-py: check
 	@rm -rf src/python/toc_trade_pb && mkdir -p src/python/toc_trade_pb
 	@$(PYTHON) -m grpc_tools.protoc \
 	--grpc_python_out=src/python/toc_trade_pb \
 	--python_out=pyi_out:src/python/toc_trade_pb \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto
@@ -21,15 +34,15 @@
 	@./scripts/modify_py_import.sh
 	@touch src/python/toc_trade_pb/__init__.py
 	@touch src/python/toc_trade_pb/app/__init__.py
 	@touch src/python/toc_trade_pb/forwarder/__init__.py
 
 compile-ts:
 	@rm -rf src/ts && mkdir -p src/ts
-	@protoc \
+	@$(PROTOC_PATH) \
 	--proto_path=protos/v3 \
     --ts_opt=no_grpc \
     --ts_opt=no_namespace \
     --ts_out=src/ts \
 	./protos/v3/*/*.proto
 
 build-py: check
```

### Comparing `toc_trade_pb_v2-0.1.4/go.sum` & `toc_trade_pb_v2-0.1.7/go.sum`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/package-lock.json` & `toc_trade_pb_v2-0.1.7/package-lock.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7958333333333334%*

 * *Differences: {"'name'": "'@chindada/toc-trade-protobuf'",*

 * * "'packages'": "{'': {'name': '@chindada/toc-trade-protobuf', 'version': '0.1.4'}}",*

 * * "'version'": "'0.1.4'"}*

```diff
@@ -1,27 +1,27 @@
 {
     "lockfileVersion": 3,
-    "name": "toc-trade-protobuf",
+    "name": "@chindada/toc-trade-protobuf",
     "packages": {
         "": {
             "dependencies": {
                 "@types/google-protobuf": "^3.15.12",
                 "google-protobuf": "^3.21.2"
             },
             "license": "MIT",
-            "name": "toc-trade-protobuf",
-            "version": "0.1.0"
+            "name": "@chindada/toc-trade-protobuf",
+            "version": "0.1.4"
         },
         "node_modules/@types/google-protobuf": {
             "integrity": "sha512-40um9QqwHjRS92qnOaDpL7RmDK15NuZYo9HihiJRbYkMQZlWnuH8AdvbMy8/o6lgLmKbDUKa+OALCltHdbOTpQ==",
             "resolved": "https://registry.npmjs.org/@types/google-protobuf/-/google-protobuf-3.15.12.tgz",
             "version": "3.15.12"
         },
         "node_modules/google-protobuf": {
             "integrity": "sha512-3MSOYFO5U9mPGikIYCzK0SaThypfGgS6bHqrUGXG3DPHCrb+txNqeEcns1W0lkGfk0rCyNXm7xB9rMxnCiZOoA==",
             "resolved": "https://registry.npmjs.org/google-protobuf/-/google-protobuf-3.21.2.tgz",
             "version": "3.21.2"
         }
     },
     "requires": true,
-    "version": "0.1.0"
+    "version": "0.1.4"
 }
```

### Comparing `toc_trade_pb_v2-0.1.4/package.json` & `toc_trade_pb_v2-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,56 @@
-00000000: 7b0a 2020 226e 616d 6522 3a20 2274 6f63  {.  "name": "toc
-00000010: 2d74 7261 6465 2d70 726f 746f 6275 6622  -trade-protobuf"
-00000020: 2c0a 2020 2276 6572 7369 6f6e 223a 2022  ,.  "version": "
-00000030: 302e 312e 3022 2c0a 2020 2264 6573 6372  0.1.0",.  "descr
-00000040: 6970 7469 6f6e 223a 2022 7072 652d 636f  iption": "pre-co
-00000050: 6d70 696c 6564 2070 726f 746f 6275 6622  mpiled protobuf"
-00000060: 2c0a 2020 226d 6169 6e22 3a20 2269 6e64  ,.  "main": "ind
-00000070: 6578 2e6a 7322 2c0a 2020 2264 6972 6563  ex.js",.  "direc
-00000080: 746f 7269 6573 223a 207b 0a20 2020 2022  tories": {.    "
-00000090: 7465 7374 223a 2022 7465 7374 7322 0a20  test": "tests". 
-000000a0: 207d 2c0a 2020 2273 6372 6970 7473 223a   },.  "scripts":
-000000b0: 207b 0a20 2020 2022 7465 7374 223a 2022   {.    "test": "
-000000c0: 6563 686f 205c 2245 7272 6f72 3a20 6e6f  echo \"Error: no
-000000d0: 2074 6573 7420 7370 6563 6966 6965 645c   test specified\
-000000e0: 2220 2626 2065 7869 7420 3122 0a20 207d  " && exit 1".  }
-000000f0: 2c0a 2020 2272 6570 6f73 6974 6f72 7922  ,.  "repository"
-00000100: 3a20 7b0a 2020 2020 2274 7970 6522 3a20  : {.    "type": 
-00000110: 2267 6974 222c 0a20 2020 2022 7572 6c22  "git",.    "url"
-00000120: 3a20 2267 6974 2b68 7474 7073 3a2f 2f67  : "git+https://g
-00000130: 6974 6875 622e 636f 6d2f 546f 432d 5461  ithub.com/ToC-Ta
-00000140: 6977 616e 2f74 6f63 2d74 7261 6465 2d70  iwan/toc-trade-p
-00000150: 726f 746f 6275 662e 6769 7422 0a20 207d  rotobuf.git".  }
-00000160: 2c0a 2020 226b 6579 776f 7264 7322 3a20  ,.  "keywords": 
-00000170: 5b0a 2020 2020 2270 726f 746f 6275 6622  [.    "protobuf"
-00000180: 0a20 205d 2c0a 2020 2261 7574 686f 7222  .  ],.  "author"
-00000190: 3a20 2254 696d 2048 7375 222c 0a20 2022  : "Tim Hsu",.  "
-000001a0: 6c69 6365 6e73 6522 3a20 224d 4954 222c  license": "MIT",
-000001b0: 0a20 2022 6275 6773 223a 207b 0a20 2020  .  "bugs": {.   
-000001c0: 2022 7572 6c22 3a20 2268 7474 7073 3a2f   "url": "https:/
-000001d0: 2f67 6974 6875 622e 636f 6d2f 546f 432d  /github.com/ToC-
-000001e0: 5461 6977 616e 2f74 6f63 2d74 7261 6465  Taiwan/toc-trade
-000001f0: 2d70 726f 746f 6275 662f 6973 7375 6573  -protobuf/issues
-00000200: 220a 2020 7d2c 0a20 2022 686f 6d65 7061  ".  },.  "homepa
-00000210: 6765 223a 2022 6874 7470 733a 2f2f 6769  ge": "https://gi
-00000220: 7468 7562 2e63 6f6d 2f54 6f43 2d54 6169  thub.com/ToC-Tai
-00000230: 7761 6e2f 746f 632d 7472 6164 652d 7072  wan/toc-trade-pr
-00000240: 6f74 6f62 7566 2372 6561 646d 6522 2c0a  otobuf#readme",.
-00000250: 2020 2264 6570 656e 6465 6e63 6965 7322    "dependencies"
-00000260: 3a20 7b0a 2020 2020 2240 7479 7065 732f  : {.    "@types/
-00000270: 676f 6f67 6c65 2d70 726f 746f 6275 6622  google-protobuf"
-00000280: 3a20 225e 332e 3135 2e31 3222 2c0a 2020  : "^3.15.12",.  
-00000290: 2020 2267 6f6f 676c 652d 7072 6f74 6f62    "google-protob
-000002a0: 7566 223a 2022 5e33 2e32 312e 3222 0a20  uf": "^3.21.2". 
-000002b0: 207d 0a7d 0a                              }.}.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 330a 4e61 6d65 3a20 746f 632d  : 2.3.Name: toc-
+00000020: 7472 6164 652d 7062 2d76 320a 5665 7273  trade-pb-v2.Vers
+00000030: 696f 6e3a 2030 2e31 2e37 0a53 756d 6d61  ion: 0.1.7.Summa
+00000040: 7279 3a20 5072 652d 636f 6d70 696c 6564  ry: Pre-compiled
+00000050: 2050 7974 686f 6e20 7072 6f74 6f62 7566   Python protobuf
+00000060: 2066 696c 6573 2066 6f72 2054 6f43 2054   files for ToC T
+00000070: 7261 6465 0a50 726f 6a65 6374 2d55 524c  rade.Project-URL
+00000080: 3a20 486f 6d65 7061 6765 2c20 6874 7470  : Homepage, http
+00000090: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+000000a0: 6f43 2d54 6169 7761 6e2f 746f 632d 7472  oC-Taiwan/toc-tr
+000000b0: 6164 652d 7072 6f74 6f62 7566 0a50 726f  ade-protobuf.Pro
+000000c0: 6a65 6374 2d55 524c 3a20 4973 7375 6573  ject-URL: Issues
+000000d0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+000000e0: 2e63 6f6d 2f54 6f43 2d54 6169 7761 6e2f  .com/ToC-Taiwan/
+000000f0: 746f 632d 7472 6164 652d 7072 6f74 6f62  toc-trade-protob
+00000100: 7566 2f69 7373 7565 730a 4175 7468 6f72  uf/issues.Author
+00000110: 2d65 6d61 696c 3a20 5469 6d20 4873 7520  -email: Tim Hsu 
+00000120: 3c6d 616f 6368 696e 6461 6461 4067 6d61  <maochindada@gma
+00000130: 696c 2e63 6f6d 3e0a 4c69 6365 6e73 652d  il.com>.License-
+00000140: 4669 6c65 3a20 4c49 4345 4e53 450a 436c  File: LICENSE.Cl
+00000150: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000160: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000170: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000180: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000190: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000001a0: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+000001b0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001d0: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+000001e0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+000001f0: 203e 3d33 2e31 310a 4465 7363 7269 7074   >=3.11.Descript
+00000200: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+00000210: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+00000220: 0a23 2054 4f43 2054 5241 4445 2050 524f  .# TOC TRADE PRO
+00000230: 544f 4255 460a 0a23 2320 5653 636f 6465  TOBUF..## VScode
+00000240: 2073 6574 7469 6e67 730a 0a60 6060 6a73   settings..```js
+00000250: 6f6e 0a70 726f 746f 635f 7061 7468 3d24  on.protoc_path=$
+00000260: 2877 6869 6368 2070 726f 746f 6329 0a65  (which protoc).e
+00000270: 6368 6f20 277b 0a20 2020 2022 7072 6f74  cho '{.    "prot
+00000280: 6f63 223a 207b 0a20 2020 2020 2020 2022  oc": {.        "
+00000290: 7061 7468 223a 2022 2724 7072 6f74 6f63  path": "'$protoc
+000002a0: 5f70 6174 6827 222c 0a20 2020 2020 2020  _path'",.       
+000002b0: 2022 636f 6d70 696c 655f 6f6e 5f73 6176   "compile_on_sav
+000002c0: 6522 3a20 6661 6c73 652c 0a20 2020 2020  e": false,.     
+000002d0: 2020 2022 6f70 7469 6f6e 7322 3a20 5b0a     "options": [.
+000002e0: 2020 2020 2020 2020 2020 2020 222d 2d70              "--p
+000002f0: 726f 746f 5f70 6174 683d 7072 6f74 6f73  roto_path=protos
+00000300: 2f76 3322 2c0a 2020 2020 2020 2020 2020  /v3",.          
+00000310: 2020 222d 2d70 7974 686f 6e5f 6f75 743d    "--python_out=
+00000320: 7372 632f 7079 7468 6f6e 222c 0a20 2020  src/python",.   
+00000330: 2020 2020 2020 2020 2022 2d2d 676f 5f6f           "--go_o
+00000340: 7574 3d73 7263 2f67 6f22 0a20 2020 2020  ut=src/go".     
+00000350: 2020 205d 0a20 2020 207d 0a7d 2720 3e20     ].    }.}' > 
+00000360: 2e76 7363 6f64 652f 7365 7474 696e 6773  .vscode/settings
+00000370: 2e6a 736f 6e0a 6060 600a                 .json.```.
```

### Comparing `toc_trade_pb_v2-0.1.4/protos/v3/app/app.proto` & `toc_trade_pb_v2-0.1.7/protos/v3/app/app.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/basic.proto` & `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/basic.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/history.proto` & `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/history.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/mq.proto` & `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/mq.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/realtime.proto` & `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/realtime.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/subscribe.proto` & `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/subscribe.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/protos/v3/forwarder/trade.proto` & `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/trade.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/app.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/app.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/basic.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/basic.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/basic_grpc.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/basic_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/entity.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/entity.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/history.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/history.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/history_grpc.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/history_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/mq.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/mq.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/realtime.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/realtime.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/realtime_grpc.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/realtime_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/subscribe.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/subscribe.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/subscribe_grpc.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/subscribe_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/trade.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/trade.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/golang/pb/trade_grpc.pb.go` & `toc_trade_pb_v2-0.1.7/src/golang/pb/trade_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2.pyi` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/app/app_pb2_grpc.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2.pyi` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2.pyi` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2.pyi` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2.pyi` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2.pyi` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py` & `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/app/app.ts` & `toc_trade_pb_v2-0.1.7/src/ts/app/app.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/forwarder/basic.ts` & `toc_trade_pb_v2-0.1.7/src/ts/forwarder/basic.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/forwarder/entity.ts` & `toc_trade_pb_v2-0.1.7/src/ts/forwarder/entity.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/forwarder/history.ts` & `toc_trade_pb_v2-0.1.7/src/ts/forwarder/history.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/forwarder/mq.ts` & `toc_trade_pb_v2-0.1.7/src/ts/forwarder/mq.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/forwarder/realtime.ts` & `toc_trade_pb_v2-0.1.7/src/ts/forwarder/realtime.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/forwarder/subscribe.ts` & `toc_trade_pb_v2-0.1.7/src/ts/forwarder/subscribe.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/forwarder/trade.ts` & `toc_trade_pb_v2-0.1.7/src/ts/forwarder/trade.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/src/ts/google/protobuf/empty.ts` & `toc_trade_pb_v2-0.1.7/src/ts/google/protobuf/empty.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/LICENSE` & `toc_trade_pb_v2-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.4/pyproject.toml` & `toc_trade_pb_v2-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toc-trade-pb-v2"
-version = "0.1.4"
+version = "0.1.7"
 authors = [{ name = "Tim Hsu", email = "maochindada@gmail.com" }]
 description = "Pre-compiled Python protobuf files for ToC Trade"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

