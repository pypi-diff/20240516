# Comparing `tmp/toc_trade_pb-0.0.1.tar.gz` & `tmp/toc_trade_pb-0.0.2.tar.gz`

## Comparing `toc_trade_pb-0.0.1.tar` & `toc_trade_pb-0.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/Makefile
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/go.mod
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/go.sum
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/.github/workflows/main.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/protos/v3/app/app.proto
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/protos/v3/forwarder/basic.proto
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/protos/v3/forwarder/entity.proto
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/protos/v3/forwarder/history.proto
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/protos/v3/forwarder/mq.proto
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/protos/v3/forwarder/realtime.proto
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/protos/v3/forwarder/subscribe.proto
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/protos/v3/forwarder/trade.proto
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/scripts/gomod_update.sh
--rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/app.pb.go
--rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/basic.pb.go
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/basic_grpc.pb.go
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/entity.pb.go
--rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/history.pb.go
--rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/history_grpc.pb.go
--rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/mq.pb.go
--rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/realtime.pb.go
--rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/realtime_grpc.pb.go
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/subscribe.pb.go
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/subscribe_grpc.pb.go
--rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/trade.pb.go
--rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/golang/pb/trade_grpc.pb.go
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/__init__.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/app/app_pb2.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/app/app_pb2.pyi
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/app/app_pb2_grpc.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/basic_pb2.py
--rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
--rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/entity_pb2.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/history_pb2.py
--rw-r--r--   0        0        0     7903 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/history_pb2.pyi
--rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/mq_pb2.py
--rw-r--r--   0        0        0    16254 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/realtime_pb2.py
--rw-r--r--   0        0        0     9755 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
--rw-r--r--   0        0        0    20640 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/trade_pb2.py
--rw-r--r--   0        0        0    19916 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
--rw-r--r--   0        0        0    35674 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/tests/.gitkeep
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/LICENSE
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/Makefile
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/go.mod
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/go.sum
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/protos/v3/app/app.proto
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/protos/v3/forwarder/basic.proto
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/protos/v3/forwarder/entity.proto
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/protos/v3/forwarder/history.proto
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/protos/v3/forwarder/mq.proto
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/protos/v3/forwarder/realtime.proto
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/protos/v3/forwarder/subscribe.proto
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/protos/v3/forwarder/trade.proto
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/scripts/gomod_update.sh
+-rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/app.pb.go
+-rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/basic.pb.go
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/basic_grpc.pb.go
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/entity.pb.go
+-rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/history.pb.go
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/history_grpc.pb.go
+-rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/mq.pb.go
+-rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/realtime.pb.go
+-rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/realtime_grpc.pb.go
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/subscribe.pb.go
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/subscribe_grpc.pb.go
+-rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/trade.pb.go
+-rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/golang/pb/trade_grpc.pb.go
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/__init__.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/app/app_pb2.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/app/app_pb2.pyi
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/app/app_pb2_grpc.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/basic_pb2.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
+-rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/entity_pb2.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/history_pb2.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/history_pb2.pyi
+-rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/mq_pb2.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/realtime_pb2.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
+-rw-r--r--   0        0        0    20640 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/trade_pb2.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
+-rw-r--r--   0        0        0    35674 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/tests/.gitkeep
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/LICENSE
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 toc_trade_pb-0.0.2/PKG-INFO
```

### Comparing `toc_trade_pb-0.0.1/Makefile` & `toc_trade_pb-0.0.2/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 	@. ./scripts/gomod_update.sh
 .PHONY: compile-go
 
 compile-py: check ### compile-py
 	@rm -rf src/python/toc_trade_pb && mkdir -p src/python/toc_trade_pb
 	@$(PYTHON) -m grpc_tools.protoc \
 	--python_out=src/python/toc_trade_pb \
+	--pyi_out=src/python/toc_trade_pb \
 	--grpc_python_out=src/python/toc_trade_pb \
-	--mypy_out=src/python/toc_trade_pb \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto
 	@touch src/python/toc_trade_pb/__init__.py
 .PHONY: compile-py
 
 clean: ## clear virtual environment
 	@rm -rf venv
@@ -32,13 +32,13 @@
 
 check: ## check environment
 ifneq ($(PYTHON),$(PWD)/venv/bin/python3)
 	$(error "Please run 'make venv' first")
 endif
 	@echo "Venv python version: $(shell $(PYTHON) --version | awk '{print $$2}')"
 	@echo "Python path: $(PYTHON)"
-	@$(PIP) install -U --no-warn-script-location --no-cache-dir grpcio grpcio-tools build twine mypy-protobuf
+	@$(PIP) install -U --no-warn-script-location --no-cache-dir grpcio grpcio-tools build twine
 .PHONY: check
 
 help: ## display this help screen
 	@awk 'BEGIN {FS = ":.*##"; printf "\nUsage:\n  make \033[36m<target>\033[0m\n"} /^[a-zA-Z_-]+:.*?##/ { printf "  \033[36m%-30s\033[0m %s\n", $$1, $$2 } /^##@/ { printf "\n\033[1m%s\033[0m\n", substr($$0, 5) } ' $(MAKEFILE_LIST)
 .PHONY: help
```

### Comparing `toc_trade_pb-0.0.1/go.sum` & `toc_trade_pb-0.0.2/go.sum`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `toc_trade_pb-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `toc_trade_pb-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/.github/workflows/main.yml` & `toc_trade_pb-0.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/.github/workflows/publish.yml` & `toc_trade_pb-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/protos/v3/app/app.proto` & `toc_trade_pb-0.0.2/protos/v3/app/app.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/protos/v3/forwarder/basic.proto` & `toc_trade_pb-0.0.2/protos/v3/forwarder/basic.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/protos/v3/forwarder/history.proto` & `toc_trade_pb-0.0.2/protos/v3/forwarder/history.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/protos/v3/forwarder/mq.proto` & `toc_trade_pb-0.0.2/protos/v3/forwarder/mq.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/protos/v3/forwarder/realtime.proto` & `toc_trade_pb-0.0.2/protos/v3/forwarder/realtime.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/protos/v3/forwarder/subscribe.proto` & `toc_trade_pb-0.0.2/protos/v3/forwarder/subscribe.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/protos/v3/forwarder/trade.proto` & `toc_trade_pb-0.0.2/protos/v3/forwarder/trade.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/app.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/app.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/basic.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/basic.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/basic_grpc.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/basic_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/entity.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/entity.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/history.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/history.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/history_grpc.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/history_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/mq.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/mq.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/realtime.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/realtime.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/realtime_grpc.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/realtime_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/subscribe.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/subscribe.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/subscribe_grpc.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/subscribe_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/trade.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/trade.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/golang/pb/trade_grpc.pb.go` & `toc_trade_pb-0.0.2/src/golang/pb/trade_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/app/app_pb2.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/app/app_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/app/app_pb2_grpc.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/app/app_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/basic_pb2.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/basic_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/entity_pb2.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/history_pb2.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/history_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/mq_pb2.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/mq_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/realtime_pb2.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/realtime_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/subscribe_pb2.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/subscribe_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/trade_pb2.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py` & `toc_trade_pb-0.0.2/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/LICENSE` & `toc_trade_pb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toc_trade_pb-0.0.1/pyproject.toml` & `toc_trade_pb-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toc-trade-pb"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Tim Hsu", email = "maochindada@gmail.com" }]
 description = "Pre-compiled Python protobuf files for ToC Trade"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `toc_trade_pb-0.0.1/PKG-INFO` & `toc_trade_pb-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: toc-trade-pb
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pre-compiled Python protobuf files for ToC Trade
 Project-URL: Homepage, https://github.com/ToC-Taiwan/toc-trade-protobuf
 Project-URL: Issues, https://github.com/ToC-Taiwan/toc-trade-protobuf/issues
 Author-email: Tim Hsu <maochindada@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

