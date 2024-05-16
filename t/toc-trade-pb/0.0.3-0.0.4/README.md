# Comparing `tmp/toc_trade_pb-0.0.3.tar.gz` & `tmp/toc_trade_pb-0.0.4.tar.gz`

## Comparing `toc_trade_pb-0.0.3.tar` & `toc_trade_pb-0.0.4.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/Makefile
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/go.mod
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/go.sum
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/.github/workflows/main.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/protos/v3/app/app.proto
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/protos/v3/forwarder/basic.proto
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/protos/v3/forwarder/entity.proto
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/protos/v3/forwarder/history.proto
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/protos/v3/forwarder/mq.proto
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/protos/v3/forwarder/realtime.proto
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/protos/v3/forwarder/subscribe.proto
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/protos/v3/forwarder/trade.proto
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/scripts/gomod_update.sh
--rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/app.pb.go
--rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/basic.pb.go
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/basic_grpc.pb.go
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/entity.pb.go
--rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/history.pb.go
--rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/history_grpc.pb.go
--rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/mq.pb.go
--rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/realtime.pb.go
--rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/realtime_grpc.pb.go
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/subscribe.pb.go
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/subscribe_grpc.pb.go
--rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/trade.pb.go
--rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/golang/pb/trade_grpc.pb.go
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/__init__.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/app/app_pb2.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/app/app_pb2.pyi
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/app/app_pb2_grpc.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/basic_pb2.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
--rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/entity_pb2.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/history_pb2.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/history_pb2.pyi
--rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/mq_pb2.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/realtime_pb2.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
--rw-r--r--   0        0        0    20640 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/trade_pb2.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
--rw-r--r--   0        0        0    35674 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/tests/.gitkeep
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/LICENSE
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/Makefile
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/go.mod
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/go.sum
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/protos/v3/app/app.proto
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/protos/v3/forwarder/basic.proto
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/protos/v3/forwarder/entity.proto
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/protos/v3/forwarder/history.proto
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/protos/v3/forwarder/mq.proto
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/protos/v3/forwarder/realtime.proto
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/protos/v3/forwarder/subscribe.proto
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/protos/v3/forwarder/trade.proto
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/scripts/gomod_update.sh
+-rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/app.pb.go
+-rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/basic.pb.go
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/basic_grpc.pb.go
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/entity.pb.go
+-rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/history.pb.go
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/history_grpc.pb.go
+-rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/mq.pb.go
+-rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/realtime.pb.go
+-rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/realtime_grpc.pb.go
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/subscribe.pb.go
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/subscribe_grpc.pb.go
+-rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/trade.pb.go
+-rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/golang/pb/trade_grpc.pb.go
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/app/__init__.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/app/app_pb2.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/app/app_pb2.pyi
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/app/app_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/__init__.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/basic_pb2.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
+-rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/entity_pb2.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/history_pb2.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/history_pb2.pyi
+-rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/mq_pb2.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/realtime_pb2.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
+-rw-r--r--   0        0        0    20640 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/trade_pb2.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
+-rw-r--r--   0        0        0    35674 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/tests/.gitkeep
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/LICENSE
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.4/PKG-INFO
```

### Comparing `toc_trade_pb-0.0.3/Makefile` & `toc_trade_pb-0.0.4/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	--grpc_python_out=src/python/toc_trade_pb \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto
 	@touch src/python/toc_trade_pb/app/__init__.py
 	@touch src/python/toc_trade_pb/forwarder/__init__.py
 	@touch src/python/toc_trade_pb/__init__.py
 
-build-py: check
+build-py: check compile-py
 	@rm -rf dist
 	@$(PYTHON) -m build
 
 upload-py: check
 	@$(PYTHON) -m twine upload --repository pypi dist/*
 
 clean: ## clear virtual environment
```

### Comparing `toc_trade_pb-0.0.3/go.sum` & `toc_trade_pb-0.0.4/go.sum`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `toc_trade_pb-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `toc_trade_pb-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/.github/workflows/main.yml` & `toc_trade_pb-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/.github/workflows/publish.yml` & `toc_trade_pb-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/protos/v3/app/app.proto` & `toc_trade_pb-0.0.4/protos/v3/app/app.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/protos/v3/forwarder/basic.proto` & `toc_trade_pb-0.0.4/protos/v3/forwarder/basic.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/protos/v3/forwarder/history.proto` & `toc_trade_pb-0.0.4/protos/v3/forwarder/history.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/protos/v3/forwarder/mq.proto` & `toc_trade_pb-0.0.4/protos/v3/forwarder/mq.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/protos/v3/forwarder/realtime.proto` & `toc_trade_pb-0.0.4/protos/v3/forwarder/realtime.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/protos/v3/forwarder/subscribe.proto` & `toc_trade_pb-0.0.4/protos/v3/forwarder/subscribe.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/protos/v3/forwarder/trade.proto` & `toc_trade_pb-0.0.4/protos/v3/forwarder/trade.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/app.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/app.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/basic.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/basic.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/basic_grpc.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/basic_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/entity.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/entity.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/history.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/history.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/history_grpc.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/history_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/mq.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/mq.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/realtime.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/realtime.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/realtime_grpc.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/realtime_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/subscribe.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/subscribe.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/subscribe_grpc.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/subscribe_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/trade.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/trade.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/golang/pb/trade_grpc.pb.go` & `toc_trade_pb-0.0.4/src/golang/pb/trade_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/app/app_pb2.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/app/app_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/app/app_pb2.pyi` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/app/app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/app/app_pb2_grpc.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/app/app_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/basic_pb2.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/basic_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/basic_pb2.pyi` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/basic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/entity_pb2.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/entity_pb2.pyi` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/history_pb2.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/history_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/history_pb2.pyi` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/history_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/mq_pb2.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/mq_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/mq_pb2.pyi` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/mq_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/realtime_pb2.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/realtime_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/subscribe_pb2.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/trade_pb2.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/trade_pb2.pyi` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py` & `toc_trade_pb-0.0.4/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/LICENSE` & `toc_trade_pb-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.3/pyproject.toml` & `toc_trade_pb-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toc-trade-pb"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Tim Hsu", email = "maochindada@gmail.com" }]
 description = "Pre-compiled Python protobuf files for ToC Trade"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `toc_trade_pb-0.0.3/PKG-INFO` & `toc_trade_pb-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: toc-trade-pb
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pre-compiled Python protobuf files for ToC Trade
 Project-URL: Homepage, https://github.com/ToC-Taiwan/toc-trade-protobuf
 Project-URL: Issues, https://github.com/ToC-Taiwan/toc-trade-protobuf/issues
 Author-email: Tim Hsu <maochindada@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

