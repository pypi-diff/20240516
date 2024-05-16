# Comparing `tmp/vastdb-0.1.4.tar.gz` & `tmp/vastdb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastdb-0.1.4.tar", last modified: Mon May 13 08:36:48 2024, max compression
+gzip compressed data, was "vastdb-0.1.5.tar", last modified: Thu May 16 15:22:13 2024, max compression
```

## Comparing `vastdb-0.1.4.tar` & `vastdb-0.1.5.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.725018 vastdb-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     4344 2024-05-13 07:47:14.000000 vastdb-0.1.4/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11333 2024-05-13 07:47:14.000000 vastdb-0.1.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-13 07:47:14.000000 vastdb-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-13 08:36:48.725018 vastdb-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6027 2024-05-13 07:47:14.000000 vastdb-0.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-13 07:47:14.000000 vastdb-0.1.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 08:36:48.725018 vastdb-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1702 2024-05-13 07:47:14.000000 vastdb-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.669021 vastdb-0.1.4/vast_flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.669021 vastdb-0.1.4/vast_flatbuf/org/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.670021 vastdb-0.1.4/vast_flatbuf/org/apache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.670021 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.670021 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.692020 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
--rw-rw-rw-   0 root         (0) root         (0)     3260 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2602 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
--rw-rw-rw-   0 root         (0) root         (0)     4455 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     3847 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
--rw-rw-rw-   0 root         (0) root         (0)     3678 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
--rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
--rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
--rw-rw-rw-   0 root         (0) root         (0)     5650 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
--rw-rw-rw-   0 root         (0) root         (0)     7527 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.710019 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
--rw-rw-rw-   0 root         (0) root         (0)     3148 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/List.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
--rw-rw-rw-   0 root         (0) root         (0)     5589 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     6042 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
--rw-rw-rw-   0 root         (0) root         (0)     5785 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
--rw-rw-rw-   0 root         (0) root         (0)     6091 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
--rw-rw-rw-   0 root         (0) root         (0)     9409 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
--rw-rw-rw-   0 root         (0) root         (0)     5767 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
--rw-rw-rw-   0 root         (0) root         (0)     2639 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     7925 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.716018 vastdb-0.1.4/vast_flatbuf/tabular/
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/AlterColumnRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/AlterProjectionTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/AlterSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/AlterTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/Column.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ColumnType.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/CreateProjectionRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/CreateSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/GetTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ImportDataRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ListProjectionsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ListSchemasResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ListTablesResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ObjectDetails.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/S3File.py
--rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/VipRange.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/tabular/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.719018 vastdb-0.1.4/vastdb/
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.721018 vastdb-0.1.4/vastdb/bench/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vastdb/bench/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/bench/test_perf.py
--rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/bucket.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/errors.py
--rw-rw-rw-   0 root         (0) root         (0)   100414 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/internal_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     3346 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/session.py
--rw-rw-rw-   0 root         (0) root         (0)    28891 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.724018 vastdb-0.1.4/vastdb/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vastdb/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_duckdb.py
--rw-rw-rw-   0 root         (0) root         (0)     5705 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_imports.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_nested.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_projections.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_sanity.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)    27499 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_tables.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/util.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.724018 vastdb-0.1.4/vastdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9048 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.534700 vastdb-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2024-05-16 14:40:09.000000 vastdb-0.1.5/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11333 2024-05-16 14:40:09.000000 vastdb-0.1.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-16 14:40:09.000000 vastdb-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-16 15:22:13.534700 vastdb-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6037 2024-05-16 14:40:09.000000 vastdb-0.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-16 14:40:09.000000 vastdb-0.1.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 15:22:13.535700 vastdb-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2024-05-16 14:40:09.000000 vastdb-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.498700 vastdb-0.1.5/vast_flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.499700 vastdb-0.1.5/vast_flatbuf/org/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.499700 vastdb-0.1.5/vast_flatbuf/org/apache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.499700 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.499700 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.514700 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2602 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
+-rw-rw-rw-   0 root         (0) root         (0)     4455 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     3847 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
+-rw-rw-rw-   0 root         (0) root         (0)     7527 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.525700 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3148 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/List.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
+-rw-rw-rw-   0 root         (0) root         (0)     5589 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5785 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
+-rw-rw-rw-   0 root         (0) root         (0)     6091 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
+-rw-rw-rw-   0 root         (0) root         (0)     5767 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7925 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.529700 vastdb-0.1.5/vast_flatbuf/tabular/
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/AlterColumnRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/AlterProjectionTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/AlterSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/AlterTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/Column.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ColumnType.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/CreateProjectionRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/CreateSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/GetTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ImportDataRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ListProjectionsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ListSchemasResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ListTablesResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/ObjectDetails.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/S3File.py
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-16 14:40:09.000000 vastdb-0.1.5/vast_flatbuf/tabular/VipRange.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vast_flatbuf/tabular/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.530700 vastdb-0.1.5/vastdb/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.532700 vastdb-0.1.5/vastdb/bench/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vastdb/bench/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/bench/test_perf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/bucket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    98490 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/internal_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     3346 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    30031 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.534700 vastdb-0.1.5/vastdb/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 15:06:28.000000 vastdb-0.1.5/vastdb/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_duckdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5705 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_projections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_sanity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)    27859 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_tables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/test_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/tests/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2852 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-16 14:40:09.000000 vastdb-0.1.5/vastdb/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:22:13.534700 vastdb-0.1.5/vastdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9048 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-16 15:22:13.000000 vastdb-0.1.5/vastdb.egg-info/top_level.txt
```

### Comparing `vastdb-0.1.4/CHANGELOG.md` & `vastdb-0.1.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## [0.1.5] (2024-05-16)
+[0.1.5]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.4...v0.1.5
+
+### Added
+ - Allow passing `ssl_verify` via `Session` c-tor
+ - Retry `requests.exceptions.ConnectionError`
+ - Document `QueryConfig` properties
+ - Support "deferred" `ibis` predicates using [Underscore (`_`) API](https://github.com/ibis-project/ibis/pull/3804)
+
+### Fixed
+ - Fix predicate pushdown when nested columns are present
+ - Attach original traceback to `MissingBucket` exception
+
 ## [0.1.4] (2024-05-13)
 [0.1.4]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.3...v0.1.4
 
 ### Added
  - Resume `Table.select()` on HTTP 503 code
  - Allow pushing down True/False boolean literals
  - Support `between` predicate pushdown
```

### Comparing `vastdb-0.1.4/LICENSE` & `vastdb-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/PKG-INFO` & `vastdb-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.4
+Version: 0.1.5
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vastdb-0.1.4/README.md` & `vastdb-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -145,233 +145,234 @@
 00000900: 6720 7468 6520 636f 6e74 6578 740a 6060  g the context.``
 00000910: 600a 0a23 2320 4669 6c74 6572 7320 616e  `..## Filters an
 00000920: 6420 7072 6f6a 6563 7469 6f6e 730a 0a4f  d projections..O
 00000930: 7572 2053 444b 2073 7570 706f 7274 7320  ur SDK supports 
 00000940: 7072 6564 6963 6174 6520 616e 6420 7072  predicate and pr
 00000950: 6f6a 6563 7469 6f6e 2070 7573 6864 6f77  ojection pushdow
 00000960: 6e3a 0a0a 6060 6070 7974 686f 6e0a 2020  n:..```python.  
-00000970: 2020 2320 5345 4c45 4354 2063 3120 4652    # SELECT c1 FR
-00000980: 4f4d 2074 2057 4845 5245 2028 6332 203e  OM t WHERE (c2 >
-00000990: 2032 2920 414e 4420 2863 3320 4953 204e   2) AND (c3 IS N
-000009a0: 554c 4c29 0a20 2020 2074 6162 6c65 2e73  ULL).    table.s
-000009b0: 656c 6563 7428 636f 6c75 6d6e 733d 5b27  elect(columns=['
-000009c0: 6331 275d 2c0a 2020 2020 2020 2020 2020  c1'],.          
-000009d0: 2020 2020 2020 2070 7265 6469 6361 7465         predicate
-000009e0: 3d28 7461 626c 655b 2763 3227 5d20 3e20  =(table['c2'] > 
-000009f0: 3229 2026 2074 6162 6c65 5b27 6333 275d  2) & table['c3']
-00000a00: 2e69 736e 756c 6c28 2929 0a0a 2020 2020  .isnull())..    
-00000a10: 2320 5345 4c45 4354 2063 322c 2063 3320  # SELECT c2, c3 
-00000a20: 4652 4f4d 2074 2057 4845 5245 2028 6332  FROM t WHERE (c2
-00000a30: 2042 4554 5745 454e 2030 2041 4e44 2031   BETWEEN 0 AND 1
-00000a40: 2920 4f52 2028 6332 203e 2031 3029 0a20  ) OR (c2 > 10). 
-00000a50: 2020 2074 6162 6c65 2e73 656c 6563 7428     table.select(
-00000a60: 636f 6c75 6d6e 733d 5b27 6332 272c 2027  columns=['c2', '
-00000a70: 6333 275d 2c0a 2020 2020 2020 2020 2020  c3'],.          
-00000a80: 2020 2020 2020 2070 7265 6469 6361 7465         predicate
-00000a90: 3d74 6162 6c65 5b27 6332 275d 2e62 6574  =table['c2'].bet
-00000aa0: 7765 656e 2830 2c20 3129 207c 2028 7461  ween(0, 1) | (ta
-00000ab0: 626c 655b 2763 3227 5d20 3e20 3130 2929  ble['c2'] > 10))
-00000ac0: 0a0a 2020 2020 2320 5345 4c45 4354 202a  ..    # SELECT *
-00000ad0: 2046 524f 4d20 7420 5748 4552 4520 6333   FROM t WHERE c3
-00000ae0: 204c 494b 4520 2725 7375 6273 7472 696e   LIKE '%substrin
-00000af0: 6725 270a 2020 2020 7461 626c 652e 7365  g%'.    table.se
-00000b00: 6c65 6374 2870 7265 6469 6361 7465 3d74  lect(predicate=t
-00000b10: 6162 6c65 5b27 6333 275d 2e63 6f6e 7461  able['c3'].conta
-00000b20: 696e 7328 2773 7562 7374 7269 6e67 2729  ins('substring')
-00000b30: 290a 6060 600a 0a53 6565 205b 6865 7265  ).```..See [here
-00000b40: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
-00000b50: 735d 2864 6f63 732f 7072 6564 6963 6174  s](docs/predicat
-00000b60: 652e 6d64 292e 0a0a 2323 2049 6d70 6f72  e.md)...## Impor
-00000b70: 7420 6120 7369 6e67 6c65 2050 6172 7175  t a single Parqu
-00000b80: 6574 2066 696c 6520 7669 6120 5333 2070  et file via S3 p
-00000b90: 726f 746f 636f 6c0a 0a49 7420 6973 2070  rotocol..It is p
-00000ba0: 6f73 7369 626c 6520 746f 2065 6666 6963  ossible to effic
-00000bb0: 6965 6e74 6c79 2063 7265 6174 6520 6120  iently create a 
-00000bc0: 7461 626c 6520 6672 6f6d 2061 2050 6172  table from a Par
-00000bd0: 7175 6574 2066 696c 6520 2877 6974 686f  quet file (witho
-00000be0: 7574 2063 6f70 7969 6e67 2069 7420 7669  ut copying it vi
-00000bf0: 6120 7468 6520 636c 6965 6e74 293a 0a0a  a the client):..
-00000c00: 6060 6070 7974 686f 6e0a 2020 2020 7769  ```python.    wi
-00000c10: 7468 2074 656d 7066 696c 652e 4e61 6d65  th tempfile.Name
-00000c20: 6454 656d 706f 7261 7279 4669 6c65 2829  dTemporaryFile()
-00000c30: 2061 7320 663a 0a20 2020 2020 2020 2070   as f:.        p
-00000c40: 612e 7061 7271 7565 742e 7772 6974 655f  a.parquet.write_
-00000c50: 7461 626c 6528 6172 726f 775f 7461 626c  table(arrow_tabl
-00000c60: 652c 2066 2e6e 616d 6529 0a20 2020 2020  e, f.name).     
-00000c70: 2020 2073 332e 7075 745f 6f62 6a65 6374     s3.put_object
-00000c80: 2842 7563 6b65 743d 2762 7563 6b65 742d  (Bucket='bucket-
-00000c90: 6e61 6d65 272c 204b 6579 3d27 7374 6167  name', Key='stag
-00000ca0: 696e 672f 6669 6c65 2e70 6172 7175 6574  ing/file.parquet
-00000cb0: 272c 2042 6f64 793d 6629 0a0a 2020 2020  ', Body=f)..    
-00000cc0: 7363 6865 6d61 203d 2074 782e 6275 636b  schema = tx.buck
-00000cd0: 6574 2827 6275 636b 6574 2d6e 616d 6527  et('bucket-name'
-00000ce0: 292e 7363 6865 6d61 2827 7363 6865 6d61  ).schema('schema
-00000cf0: 2d6e 616d 6527 290a 2020 2020 7461 626c  -name').    tabl
-00000d00: 6520 3d20 7574 696c 2e63 7265 6174 655f  e = util.create_
-00000d10: 7461 626c 655f 6672 6f6d 5f66 696c 6573  table_from_files
-00000d20: 280a 2020 2020 2020 2020 7363 6865 6d61  (.        schema
-00000d30: 3d73 6368 656d 612c 2074 6162 6c65 5f6e  =schema, table_n
-00000d40: 616d 653d 2769 6d70 6f72 7465 642d 7461  ame='imported-ta
-00000d50: 626c 6527 2c0a 2020 2020 2020 2020 7061  ble',.        pa
-00000d60: 7271 7565 745f 6669 6c65 733d 5b27 2f62  rquet_files=['/b
-00000d70: 7563 6b65 742d 6e61 6d65 2f73 7461 6769  ucket-name/stagi
-00000d80: 6e67 2f66 696c 652e 7061 7271 7565 7427  ng/file.parquet'
-00000d90: 5d29 0a60 6060 0a0a 2323 2049 6d70 6f72  ]).```..## Impor
-00000da0: 7420 6d75 6c74 6970 6c65 2050 6172 7175  t multiple Parqu
-00000db0: 6574 2066 696c 6573 2063 6f6e 6375 7272  et files concurr
-00000dc0: 656e 746c 7920 7669 6120 5333 2070 726f  ently via S3 pro
-00000dd0: 746f 636f 6c0a 0a57 6520 6361 6e20 696d  tocol..We can im
-00000de0: 706f 7274 206d 756c 7469 706c 6520 6669  port multiple fi
-00000df0: 6c65 7320 636f 6e63 7572 7265 6e74 6c79  les concurrently
-00000e00: 2069 6e74 6f20 6120 7461 626c 6520 2862   into a table (b
-00000e10: 7920 7574 696c 697a 696e 6720 6d75 6c74  y utilizing mult
-00000e20: 6970 6c65 2043 4e6f 6465 7327 2063 6f72  iple CNodes' cor
-00000e30: 6573 293a 0a0a 6060 6070 7974 686f 6e0a  es):..```python.
-00000e40: 2020 2020 7363 6865 6d61 203d 2074 782e      schema = tx.
-00000e50: 6275 636b 6574 2827 6275 636b 6574 2d6e  bucket('bucket-n
-00000e60: 616d 6527 292e 7363 6865 6d61 2827 7363  ame').schema('sc
-00000e70: 6865 6d61 2d6e 616d 6527 290a 2020 2020  hema-name').    
-00000e80: 7461 626c 6520 3d20 7574 696c 2e63 7265  table = util.cre
-00000e90: 6174 655f 7461 626c 655f 6672 6f6d 5f66  ate_table_from_f
-00000ea0: 696c 6573 280a 2020 2020 2020 2020 7363  iles(.        sc
-00000eb0: 6865 6d61 3d73 6368 656d 612c 2074 6162  hema=schema, tab
-00000ec0: 6c65 5f6e 616d 653d 276c 6172 6765 2d69  le_name='large-i
-00000ed0: 6d70 6f72 7465 642d 7461 626c 6527 2c0a  mported-table',.
-00000ee0: 2020 2020 2020 2020 7061 7271 7565 745f          parquet_
-00000ef0: 6669 6c65 733d 5b66 272f 6275 636b 6574  files=[f'/bucket
-00000f00: 2d6e 616d 652f 7374 6167 696e 672f 6669  -name/staging/fi
-00000f10: 6c65 7b69 7d2e 7061 7271 7565 7427 2066  le{i}.parquet' f
-00000f20: 6f72 2069 2069 6e20 7261 6e67 6528 3130  or i in range(10
-00000f30: 295d 290a 6060 600a 0a23 2320 506f 7374  )]).```..## Post
-00000f40: 2d70 726f 6365 7373 696e 670a 0a23 2323  -processing..###
-00000f50: 2045 7870 6f72 740a 0a60 5461 626c 652e   Export..`Table.
-00000f60: 7365 6c65 6374 2829 6020 7265 7475 726e  select()` return
-00000f70: 7320 6120 7374 7265 616d 206f 6620 5b50  s a stream of [P
-00000f80: 7941 7272 6f77 2072 6563 6f72 6420 6261  yArrow record ba
-00000f90: 7463 6865 735d 2868 7474 7073 3a2f 2f61  tches](https://a
-00000fa0: 7272 6f77 2e61 7061 6368 652e 6f72 672f  rrow.apache.org/
-00000fb0: 646f 6373 2f70 7974 686f 6e2f 6461 7461  docs/python/data
-00000fc0: 2e68 746d 6c23 7265 636f 7264 2d62 6174  .html#record-bat
-00000fd0: 6368 6573 292c 2077 6869 6368 2063 616e  ches), which can
-00000fe0: 2062 6520 6469 7265 6374 6c79 2065 7870   be directly exp
-00000ff0: 6f72 7465 6420 696e 746f 2061 2050 6172  orted into a Par
-00001000: 7175 6574 2066 696c 653a 0a0a 6060 6070  quet file:..```p
-00001010: 7974 686f 6e0a 6261 7463 6865 7320 3d20  ython.batches = 
-00001020: 7461 626c 652e 7365 6c65 6374 2829 0a77  table.select().w
-00001030: 6974 6820 636f 6e74 6578 746c 6962 2e63  ith contextlib.c
-00001040: 6c6f 7369 6e67 2870 612e 7061 7271 7565  losing(pa.parque
-00001050: 742e 5061 7271 7565 7457 7269 7465 7228  t.ParquetWriter(
-00001060: 272f 7061 7468 2f74 6f2f 6669 6c65 2e70  '/path/to/file.p
-00001070: 6172 7175 6574 272c 2062 6174 6368 6573  arquet', batches
-00001080: 2e73 6368 656d 6129 2920 6173 2077 7269  .schema)) as wri
-00001090: 7465 723a 0a20 2020 2066 6f72 2062 6174  ter:.    for bat
-000010a0: 6368 2069 6e20 7461 626c 655f 6261 7463  ch in table_batc
-000010b0: 6865 733a 0a20 2020 2020 2020 2077 7269  hes:.        wri
-000010c0: 7465 722e 7772 6974 655f 6261 7463 6828  ter.write_batch(
-000010d0: 6261 7463 6829 0a60 6060 0a0a 2323 2320  batch).```..### 
-000010e0: 4475 636b 4442 0a0a 5765 2063 616e 2075  DuckDB..We can u
-000010f0: 7365 205b 4475 636b 4442 5d28 6874 7470  se [DuckDB](http
-00001100: 733a 2f2f 6475 636b 6462 2e6f 7267 2f64  s://duckdb.org/d
-00001110: 6f63 732f 6775 6964 6573 2f70 7974 686f  ocs/guides/pytho
-00001120: 6e2f 7371 6c5f 6f6e 5f61 7272 6f77 2e68  n/sql_on_arrow.h
-00001130: 746d 6c29 2074 6f20 706f 7374 2d70 726f  tml) to post-pro
-00001140: 6365 7373 2074 6865 2072 6573 756c 7469  cess the resulti
-00001150: 6e67 2073 7472 6561 6d20 6f66 205b 5079  ng stream of [Py
-00001160: 4172 726f 7720 7265 636f 7264 2062 6174  Arrow record bat
-00001170: 6368 6573 5d28 6874 7470 733a 2f2f 6172  ches](https://ar
-00001180: 726f 772e 6170 6163 6865 2e6f 7267 2f64  row.apache.org/d
-00001190: 6f63 732f 7079 7468 6f6e 2f64 6174 612e  ocs/python/data.
-000011a0: 6874 6d6c 2372 6563 6f72 642d 6261 7463  html#record-batc
-000011b0: 6865 7329 3a0a 0a60 6060 7079 7468 6f6e  hes):..```python
-000011c0: 0a69 6d70 6f72 7420 6475 636b 6462 0a63  .import duckdb.c
-000011d0: 6f6e 6e20 3d20 6475 636b 6462 2e63 6f6e  onn = duckdb.con
-000011e0: 6e65 6374 2829 0a0a 6261 7463 6865 7320  nect()..batches 
-000011f0: 3d20 7461 626c 652e 7365 6c65 6374 2863  = table.select(c
-00001200: 6f6c 756d 6e73 3d5b 2763 3127 5d2c 2070  olumns=['c1'], p
-00001210: 7265 6469 6361 7465 3d28 7461 626c 655b  redicate=(table[
-00001220: 2763 3227 5d20 3e20 3229 290a 7072 696e  'c2'] > 2)).prin
-00001230: 7428 636f 6e6e 2e65 7865 6375 7465 2822  t(conn.execute("
-00001240: 5345 4c45 4354 2073 756d 2863 3129 2046  SELECT sum(c1) F
-00001250: 524f 4d20 6261 7463 6865 7322 292e 6172  ROM batches").ar
-00001260: 726f 7728 2929 0a60 6060 0a0a 2323 2053  row()).```..## S
-00001270: 656d 692d 736f 7274 6564 2070 726f 6a65  emi-sorted proje
-00001280: 6374 696f 6e73 0a0a 5765 2063 616e 2063  ctions..We can c
-00001290: 7265 6174 652c 206c 6973 7420 616e 6420  reate, list and 
-000012a0: 6465 6c65 7465 205b 6176 6169 6c61 626c  delete [availabl
-000012b0: 6520 7365 6d69 2d73 6f72 7465 6420 7072  e semi-sorted pr
-000012c0: 6f6a 6563 7469 6f6e 735d 2868 7474 7073  ojections](https
-000012d0: 3a2f 2f73 7570 706f 7274 2e76 6173 7464  ://support.vastd
-000012e0: 6174 612e 636f 6d2f 732f 6172 7469 636c  ata.com/s/articl
-000012f0: 652f 5555 4944 2d65 3463 6134 3261 622d  e/UUID-e4ca42ab-
-00001300: 6431 3562 2d36 6237 322d 6264 3662 2d66  d15b-6b72-bd6b-f
-00001310: 3363 3737 6234 3535 6465 3429 3a0a 0a60  3c77b455de4):..`
-00001320: 6060 7079 7468 6f6e 0a70 203d 2074 6162  ``python.p = tab
-00001330: 6c65 2e63 7265 6174 655f 7072 6f6a 6563  le.create_projec
-00001340: 7469 6f6e 2827 7072 6f6a 272c 2073 6f72  tion('proj', sor
-00001350: 7465 643d 5b27 6333 275d 2c20 756e 736f  ted=['c3'], unso
-00001360: 7274 6564 3d5b 2763 3127 5d29 0a70 7269  rted=['c1']).pri
-00001370: 6e74 2874 6162 6c65 2e70 726f 6a65 6374  nt(table.project
-00001380: 696f 6e73 2829 290a 7072 696e 7428 702e  ions()).print(p.
-00001390: 6765 745f 7374 6174 7328 2929 0a70 2e64  get_stats()).p.d
-000013a0: 726f 7028 290a 6060 600a 0a23 2320 536e  rop().```..## Sn
-000013b0: 6170 7368 6f74 730a 0a49 7420 6973 2070  apshots..It is p
-000013c0: 6f73 7369 626c 6520 746f 2075 7365 205b  ossible to use [
-000013d0: 736e 6170 7368 6f74 735d 2868 7474 7073  snapshots](https
-000013e0: 3a2f 2f76 6173 7464 6174 612e 636f 6d2f  ://vastdata.com/
-000013f0: 626c 6f67 2f62 7269 6e67 696e 672d 736e  blog/bringing-sn
-00001400: 6170 7368 6f74 732d 746f 2d76 6173 7473  apshots-to-vasts
-00001410: 2d65 6c65 6d65 6e74 2d73 746f 7265 2920  -element-store) 
-00001420: 666f 7220 6163 6365 7373 696e 6720 7468  for accessing th
-00001430: 6520 4461 7461 6261 7365 3a0a 0a60 6060  e Database:..```
-00001440: 7079 7468 6f6e 0a73 6e61 7073 203d 2062  python.snaps = b
-00001450: 7563 6b65 742e 6c69 7374 5f73 6e61 7073  ucket.list_snaps
-00001460: 686f 7473 2829 0a62 6174 6368 6573 203d  hots().batches =
-00001470: 2073 6e61 7073 5b30 5d2e 7363 6865 6d61   snaps[0].schema
-00001480: 2827 7363 6865 6d61 2d6e 616d 6527 292e  ('schema-name').
-00001490: 7461 626c 6528 2774 6162 6c65 2d6e 616d  table('table-nam
-000014a0: 6527 292e 7365 6c65 6374 2829 0a60 6060  e').select().```
-000014b0: 0a0a 2323 2056 4153 5420 4361 7461 6c6f  ..## VAST Catalo
-000014c0: 670a 0a5b 5641 5354 2043 6174 616c 6f67  g..[VAST Catalog
-000014d0: 5d28 6874 7470 733a 2f2f 7661 7374 6461  ](https://vastda
-000014e0: 7461 2e63 6f6d 2f62 6c6f 672f 7661 7374  ta.com/blog/vast
-000014f0: 2d63 6174 616c 6f67 2d74 7265 6174 2d79  -catalog-treat-y
-00001500: 6f75 722d 6669 6c65 2d73 7973 7465 6d2d  our-file-system-
-00001510: 6c69 6b65 2d61 2d64 6174 6162 6173 6529  like-a-database)
-00001520: 2063 616e 2062 6520 7175 6572 6965 6420   can be queried 
-00001530: 6173 2061 2072 6567 756c 6172 2074 6162  as a regular tab
-00001540: 6c65 3a0a 0a60 6060 7079 7468 6f6e 0a74  le:..```python.t
-00001550: 6162 6c65 203d 2070 612e 5461 626c 652e  able = pa.Table.
-00001560: 6672 6f6d 5f62 6174 6368 6573 2874 782e  from_batches(tx.
-00001570: 6361 7461 6c6f 672e 7365 6c65 6374 285b  catalog.select([
-00001580: 2765 6c65 6d65 6e74 5f74 7970 6527 5d29  'element_type'])
-00001590: 290a 6466 203d 2074 6162 6c65 2e74 6f5f  ).df = table.to_
-000015a0: 7061 6e64 6173 2829 0a0a 746f 7461 6c5f  pandas()..total_
-000015b0: 656c 656d 656e 7473 203d 206c 656e 2864  elements = len(d
-000015c0: 6629 0a70 7269 6e74 2866 2254 6f74 616c  f).print(f"Total
-000015d0: 2065 6c65 6d65 6e74 7320 696e 2074 6865   elements in the
-000015e0: 2063 6174 616c 6f67 3a20 7b74 6f74 616c   catalog: {total
-000015f0: 5f65 6c65 6d65 6e74 737d 2229 0a0a 6669  _elements}")..fi
-00001600: 6c65 5f63 6f75 6e74 203d 2028 6466 5b27  le_count = (df['
-00001610: 656c 656d 656e 745f 7479 7065 275d 203d  element_type'] =
-00001620: 3d20 2746 494c 4527 292e 7375 6d28 290a  = 'FILE').sum().
-00001630: 7072 696e 7428 6622 4e75 6d62 6572 206f  print(f"Number o
-00001640: 6620 6669 6c65 732f 6f62 6a65 6374 733a  f files/objects:
-00001650: 207b 6669 6c65 5f63 6f75 6e74 7d22 290a   {file_count}").
-00001660: 0a64 6973 7469 6e63 745f 656c 656d 656e  .distinct_elemen
-00001670: 7473 203d 2064 665b 2765 6c65 6d65 6e74  ts = df['element
-00001680: 5f74 7970 6527 5d2e 756e 6971 7565 2829  _type'].unique()
-00001690: 0a70 7269 6e74 2822 4469 7374 696e 6374  .print("Distinct
-000016a0: 2065 6c65 6d65 6e74 2074 7970 6573 206f   element types o
-000016b0: 6e20 7468 6520 7379 7374 656d 3a22 290a  n the system:").
-000016c0: 7072 696e 7428 6469 7374 696e 6374 5f65  print(distinct_e
-000016d0: 6c65 6d65 6e74 7329 0a60 6060 0a0a 5365  lements).```..Se
-000016e0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-000016f0: 626c 6f67 2070 6f73 7473 2066 6f72 206d  blog posts for m
-00001700: 6f72 6520 6578 616d 706c 6573 3a0a 0a2d  ore examples:..-
-00001710: 2068 7474 7073 3a2f 2f76 6173 7464 6174   https://vastdat
-00001720: 612e 636f 6d2f 626c 6f67 2f74 6865 2d76  a.com/blog/the-v
-00001730: 6173 742d 6361 7461 6c6f 672d 696e 2d61  ast-catalog-in-a
-00001740: 6374 696f 6e2d 7061 7274 2d31 0a2d 2068  ction-part-1.- h
-00001750: 7474 7073 3a2f 2f76 6173 7464 6174 612e  ttps://vastdata.
-00001760: 636f 6d2f 626c 6f67 2f74 6865 2d76 6173  com/blog/the-vas
-00001770: 742d 6361 7461 6c6f 672d 696e 2d61 6374  t-catalog-in-act
-00001780: 696f 6e2d 7061 7274 2d32 0a              ion-part-2.
+00000970: 2020 6672 6f6d 2069 6269 7320 696d 706f    from ibis impo
+00000980: 7274 205f 0a0a 2020 2020 2320 5345 4c45  rt _..    # SELE
+00000990: 4354 2063 3120 4652 4f4d 2074 2057 4845  CT c1 FROM t WHE
+000009a0: 5245 2028 6332 203e 2032 2920 414e 4420  RE (c2 > 2) AND 
+000009b0: 2863 3320 4953 204e 554c 4c29 0a20 2020  (c3 IS NULL).   
+000009c0: 2074 6162 6c65 2e73 656c 6563 7428 636f   table.select(co
+000009d0: 6c75 6d6e 733d 5b27 6331 275d 2c0a 2020  lumns=['c1'],.  
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000009f0: 7265 6469 6361 7465 3d28 5f2e 6332 203e  redicate=(_.c2 >
+00000a00: 2032 2920 2620 5f2e 6333 2e69 736e 756c   2) & _.c3.isnul
+00000a10: 6c28 2929 0a0a 2020 2020 2320 5345 4c45  l())..    # SELE
+00000a20: 4354 2063 322c 2063 3320 4652 4f4d 2074  CT c2, c3 FROM t
+00000a30: 2057 4845 5245 2028 6332 2042 4554 5745   WHERE (c2 BETWE
+00000a40: 454e 2030 2041 4e44 2031 2920 4f52 2028  EN 0 AND 1) OR (
+00000a50: 6332 203e 2031 3029 0a20 2020 2074 6162  c2 > 10).    tab
+00000a60: 6c65 2e73 656c 6563 7428 636f 6c75 6d6e  le.select(column
+00000a70: 733d 5b27 6332 272c 2027 6333 275d 2c0a  s=['c2', 'c3'],.
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2070 7265 6469 6361 7465 3d28 5f2e 6332   predicate=(_.c2
+00000aa0: 2e62 6574 7765 656e 2830 2c20 3129 207c  .between(0, 1) |
+00000ab0: 2028 7461 626c 655b 2763 3227 5d20 3e20   (table['c2'] > 
+00000ac0: 3130 2929 0a0a 2020 2020 2320 5345 4c45  10))..    # SELE
+00000ad0: 4354 202a 2046 524f 4d20 7420 5748 4552  CT * FROM t WHER
+00000ae0: 4520 6333 204c 494b 4520 2725 7375 6273  E c3 LIKE '%subs
+00000af0: 7472 696e 6725 270a 2020 2020 7461 626c  tring%'.    tabl
+00000b00: 652e 7365 6c65 6374 2870 7265 6469 6361  e.select(predica
+00000b10: 7465 3d5f 2e63 332e 636f 6e74 6169 6e73  te=_.c3.contains
+00000b20: 2827 7375 6273 7472 696e 6727 2929 0a60  ('substring')).`
+00000b30: 6060 0a0a 5365 6520 5b68 6572 6520 666f  ``..See [here fo
+00000b40: 7220 6d6f 7265 2064 6574 6169 6c73 5d28  r more details](
+00000b50: 646f 6373 2f70 7265 6469 6361 7465 2e6d  docs/predicate.m
+00000b60: 6429 2e0a 0a23 2320 496d 706f 7274 2061  d)...## Import a
+00000b70: 2073 696e 676c 6520 5061 7271 7565 7420   single Parquet 
+00000b80: 6669 6c65 2076 6961 2053 3320 7072 6f74  file via S3 prot
+00000b90: 6f63 6f6c 0a0a 4974 2069 7320 706f 7373  ocol..It is poss
+00000ba0: 6962 6c65 2074 6f20 6566 6669 6369 656e  ible to efficien
+00000bb0: 746c 7920 6372 6561 7465 2061 2074 6162  tly create a tab
+00000bc0: 6c65 2066 726f 6d20 6120 5061 7271 7565  le from a Parque
+00000bd0: 7420 6669 6c65 2028 7769 7468 6f75 7420  t file (without 
+00000be0: 636f 7079 696e 6720 6974 2076 6961 2074  copying it via t
+00000bf0: 6865 2063 6c69 656e 7429 3a0a 0a60 6060  he client):..```
+00000c00: 7079 7468 6f6e 0a20 2020 2077 6974 6820  python.    with 
+00000c10: 7465 6d70 6669 6c65 2e4e 616d 6564 5465  tempfile.NamedTe
+00000c20: 6d70 6f72 6172 7946 696c 6528 2920 6173  mporaryFile() as
+00000c30: 2066 3a0a 2020 2020 2020 2020 7061 2e70   f:.        pa.p
+00000c40: 6172 7175 6574 2e77 7269 7465 5f74 6162  arquet.write_tab
+00000c50: 6c65 2861 7272 6f77 5f74 6162 6c65 2c20  le(arrow_table, 
+00000c60: 662e 6e61 6d65 290a 2020 2020 2020 2020  f.name).        
+00000c70: 7333 2e70 7574 5f6f 626a 6563 7428 4275  s3.put_object(Bu
+00000c80: 636b 6574 3d27 6275 636b 6574 2d6e 616d  cket='bucket-nam
+00000c90: 6527 2c20 4b65 793d 2773 7461 6769 6e67  e', Key='staging
+00000ca0: 2f66 696c 652e 7061 7271 7565 7427 2c20  /file.parquet', 
+00000cb0: 426f 6479 3d66 290a 0a20 2020 2073 6368  Body=f)..    sch
+00000cc0: 656d 6120 3d20 7478 2e62 7563 6b65 7428  ema = tx.bucket(
+00000cd0: 2762 7563 6b65 742d 6e61 6d65 2729 2e73  'bucket-name').s
+00000ce0: 6368 656d 6128 2773 6368 656d 612d 6e61  chema('schema-na
+00000cf0: 6d65 2729 0a20 2020 2074 6162 6c65 203d  me').    table =
+00000d00: 2075 7469 6c2e 6372 6561 7465 5f74 6162   util.create_tab
+00000d10: 6c65 5f66 726f 6d5f 6669 6c65 7328 0a20  le_from_files(. 
+00000d20: 2020 2020 2020 2073 6368 656d 613d 7363         schema=sc
+00000d30: 6865 6d61 2c20 7461 626c 655f 6e61 6d65  hema, table_name
+00000d40: 3d27 696d 706f 7274 6564 2d74 6162 6c65  ='imported-table
+00000d50: 272c 0a20 2020 2020 2020 2070 6172 7175  ',.        parqu
+00000d60: 6574 5f66 696c 6573 3d5b 272f 6275 636b  et_files=['/buck
+00000d70: 6574 2d6e 616d 652f 7374 6167 696e 672f  et-name/staging/
+00000d80: 6669 6c65 2e70 6172 7175 6574 275d 290a  file.parquet']).
+00000d90: 6060 600a 0a23 2320 496d 706f 7274 206d  ```..## Import m
+00000da0: 756c 7469 706c 6520 5061 7271 7565 7420  ultiple Parquet 
+00000db0: 6669 6c65 7320 636f 6e63 7572 7265 6e74  files concurrent
+00000dc0: 6c79 2076 6961 2053 3320 7072 6f74 6f63  ly via S3 protoc
+00000dd0: 6f6c 0a0a 5765 2063 616e 2069 6d70 6f72  ol..We can impor
+00000de0: 7420 6d75 6c74 6970 6c65 2066 696c 6573  t multiple files
+00000df0: 2063 6f6e 6375 7272 656e 746c 7920 696e   concurrently in
+00000e00: 746f 2061 2074 6162 6c65 2028 6279 2075  to a table (by u
+00000e10: 7469 6c69 7a69 6e67 206d 756c 7469 706c  tilizing multipl
+00000e20: 6520 434e 6f64 6573 2720 636f 7265 7329  e CNodes' cores)
+00000e30: 3a0a 0a60 6060 7079 7468 6f6e 0a20 2020  :..```python.   
+00000e40: 2073 6368 656d 6120 3d20 7478 2e62 7563   schema = tx.buc
+00000e50: 6b65 7428 2762 7563 6b65 742d 6e61 6d65  ket('bucket-name
+00000e60: 2729 2e73 6368 656d 6128 2773 6368 656d  ').schema('schem
+00000e70: 612d 6e61 6d65 2729 0a20 2020 2074 6162  a-name').    tab
+00000e80: 6c65 203d 2075 7469 6c2e 6372 6561 7465  le = util.create
+00000e90: 5f74 6162 6c65 5f66 726f 6d5f 6669 6c65  _table_from_file
+00000ea0: 7328 0a20 2020 2020 2020 2073 6368 656d  s(.        schem
+00000eb0: 613d 7363 6865 6d61 2c20 7461 626c 655f  a=schema, table_
+00000ec0: 6e61 6d65 3d27 6c61 7267 652d 696d 706f  name='large-impo
+00000ed0: 7274 6564 2d74 6162 6c65 272c 0a20 2020  rted-table',.   
+00000ee0: 2020 2020 2070 6172 7175 6574 5f66 696c       parquet_fil
+00000ef0: 6573 3d5b 6627 2f62 7563 6b65 742d 6e61  es=[f'/bucket-na
+00000f00: 6d65 2f73 7461 6769 6e67 2f66 696c 657b  me/staging/file{
+00000f10: 697d 2e70 6172 7175 6574 2720 666f 7220  i}.parquet' for 
+00000f20: 6920 696e 2072 616e 6765 2831 3029 5d29  i in range(10)])
+00000f30: 0a60 6060 0a0a 2323 2050 6f73 742d 7072  .```..## Post-pr
+00000f40: 6f63 6573 7369 6e67 0a0a 2323 2320 4578  ocessing..### Ex
+00000f50: 706f 7274 0a0a 6054 6162 6c65 2e73 656c  port..`Table.sel
+00000f60: 6563 7428 2960 2072 6574 7572 6e73 2061  ect()` returns a
+00000f70: 2073 7472 6561 6d20 6f66 205b 5079 4172   stream of [PyAr
+00000f80: 726f 7720 7265 636f 7264 2062 6174 6368  row record batch
+00000f90: 6573 5d28 6874 7470 733a 2f2f 6172 726f  es](https://arro
+00000fa0: 772e 6170 6163 6865 2e6f 7267 2f64 6f63  w.apache.org/doc
+00000fb0: 732f 7079 7468 6f6e 2f64 6174 612e 6874  s/python/data.ht
+00000fc0: 6d6c 2372 6563 6f72 642d 6261 7463 6865  ml#record-batche
+00000fd0: 7329 2c20 7768 6963 6820 6361 6e20 6265  s), which can be
+00000fe0: 2064 6972 6563 746c 7920 6578 706f 7274   directly export
+00000ff0: 6564 2069 6e74 6f20 6120 5061 7271 7565  ed into a Parque
+00001000: 7420 6669 6c65 3a0a 0a60 6060 7079 7468  t file:..```pyth
+00001010: 6f6e 0a62 6174 6368 6573 203d 2074 6162  on.batches = tab
+00001020: 6c65 2e73 656c 6563 7428 290a 7769 7468  le.select().with
+00001030: 2063 6f6e 7465 7874 6c69 622e 636c 6f73   contextlib.clos
+00001040: 696e 6728 7061 2e70 6172 7175 6574 2e50  ing(pa.parquet.P
+00001050: 6172 7175 6574 5772 6974 6572 2827 2f70  arquetWriter('/p
+00001060: 6174 682f 746f 2f66 696c 652e 7061 7271  ath/to/file.parq
+00001070: 7565 7427 2c20 6261 7463 6865 732e 7363  uet', batches.sc
+00001080: 6865 6d61 2929 2061 7320 7772 6974 6572  hema)) as writer
+00001090: 3a0a 2020 2020 666f 7220 6261 7463 6820  :.    for batch 
+000010a0: 696e 2074 6162 6c65 5f62 6174 6368 6573  in table_batches
+000010b0: 3a0a 2020 2020 2020 2020 7772 6974 6572  :.        writer
+000010c0: 2e77 7269 7465 5f62 6174 6368 2862 6174  .write_batch(bat
+000010d0: 6368 290a 6060 600a 0a23 2323 2044 7563  ch).```..### Duc
+000010e0: 6b44 420a 0a57 6520 6361 6e20 7573 6520  kDB..We can use 
+000010f0: 5b44 7563 6b44 425d 2868 7474 7073 3a2f  [DuckDB](https:/
+00001100: 2f64 7563 6b64 622e 6f72 672f 646f 6373  /duckdb.org/docs
+00001110: 2f67 7569 6465 732f 7079 7468 6f6e 2f73  /guides/python/s
+00001120: 716c 5f6f 6e5f 6172 726f 772e 6874 6d6c  ql_on_arrow.html
+00001130: 2920 746f 2070 6f73 742d 7072 6f63 6573  ) to post-proces
+00001140: 7320 7468 6520 7265 7375 6c74 696e 6720  s the resulting 
+00001150: 7374 7265 616d 206f 6620 5b50 7941 7272  stream of [PyArr
+00001160: 6f77 2072 6563 6f72 6420 6261 7463 6865  ow record batche
+00001170: 735d 2868 7474 7073 3a2f 2f61 7272 6f77  s](https://arrow
+00001180: 2e61 7061 6368 652e 6f72 672f 646f 6373  .apache.org/docs
+00001190: 2f70 7974 686f 6e2f 6461 7461 2e68 746d  /python/data.htm
+000011a0: 6c23 7265 636f 7264 2d62 6174 6368 6573  l#record-batches
+000011b0: 293a 0a0a 6060 6070 7974 686f 6e0a 6672  ):..```python.fr
+000011c0: 6f6d 2069 6269 7320 696d 706f 7274 205f  om ibis import _
+000011d0: 0a0a 696d 706f 7274 2064 7563 6b64 620a  ..import duckdb.
+000011e0: 636f 6e6e 203d 2064 7563 6b64 622e 636f  conn = duckdb.co
+000011f0: 6e6e 6563 7428 290a 0a62 6174 6368 6573  nnect()..batches
+00001200: 203d 2074 6162 6c65 2e73 656c 6563 7428   = table.select(
+00001210: 636f 6c75 6d6e 733d 5b27 6331 275d 2c20  columns=['c1'], 
+00001220: 7072 6564 6963 6174 653d 285f 2e63 3220  predicate=(_.c2 
+00001230: 3e20 3229 290a 7072 696e 7428 636f 6e6e  > 2)).print(conn
+00001240: 2e65 7865 6375 7465 2822 5345 4c45 4354  .execute("SELECT
+00001250: 2073 756d 2863 3129 2046 524f 4d20 6261   sum(c1) FROM ba
+00001260: 7463 6865 7322 292e 6172 726f 7728 2929  tches").arrow())
+00001270: 0a60 6060 0a0a 2323 2053 656d 692d 736f  .```..## Semi-so
+00001280: 7274 6564 2070 726f 6a65 6374 696f 6e73  rted projections
+00001290: 0a0a 5765 2063 616e 2063 7265 6174 652c  ..We can create,
+000012a0: 206c 6973 7420 616e 6420 6465 6c65 7465   list and delete
+000012b0: 205b 6176 6169 6c61 626c 6520 7365 6d69   [available semi
+000012c0: 2d73 6f72 7465 6420 7072 6f6a 6563 7469  -sorted projecti
+000012d0: 6f6e 735d 2868 7474 7073 3a2f 2f73 7570  ons](https://sup
+000012e0: 706f 7274 2e76 6173 7464 6174 612e 636f  port.vastdata.co
+000012f0: 6d2f 732f 6172 7469 636c 652f 5555 4944  m/s/article/UUID
+00001300: 2d65 3463 6134 3261 622d 6431 3562 2d36  -e4ca42ab-d15b-6
+00001310: 6237 322d 6264 3662 2d66 3363 3737 6234  b72-bd6b-f3c77b4
+00001320: 3535 6465 3429 3a0a 0a60 6060 7079 7468  55de4):..```pyth
+00001330: 6f6e 0a70 203d 2074 6162 6c65 2e63 7265  on.p = table.cre
+00001340: 6174 655f 7072 6f6a 6563 7469 6f6e 2827  ate_projection('
+00001350: 7072 6f6a 272c 2073 6f72 7465 643d 5b27  proj', sorted=['
+00001360: 6333 275d 2c20 756e 736f 7274 6564 3d5b  c3'], unsorted=[
+00001370: 2763 3127 5d29 0a70 7269 6e74 2874 6162  'c1']).print(tab
+00001380: 6c65 2e70 726f 6a65 6374 696f 6e73 2829  le.projections()
+00001390: 290a 7072 696e 7428 702e 6765 745f 7374  ).print(p.get_st
+000013a0: 6174 7328 2929 0a70 2e64 726f 7028 290a  ats()).p.drop().
+000013b0: 6060 600a 0a23 2320 536e 6170 7368 6f74  ```..## Snapshot
+000013c0: 730a 0a49 7420 6973 2070 6f73 7369 626c  s..It is possibl
+000013d0: 6520 746f 2075 7365 205b 736e 6170 7368  e to use [snapsh
+000013e0: 6f74 735d 2868 7474 7073 3a2f 2f76 6173  ots](https://vas
+000013f0: 7464 6174 612e 636f 6d2f 626c 6f67 2f62  tdata.com/blog/b
+00001400: 7269 6e67 696e 672d 736e 6170 7368 6f74  ringing-snapshot
+00001410: 732d 746f 2d76 6173 7473 2d65 6c65 6d65  s-to-vasts-eleme
+00001420: 6e74 2d73 746f 7265 2920 666f 7220 6163  nt-store) for ac
+00001430: 6365 7373 696e 6720 7468 6520 4461 7461  cessing the Data
+00001440: 6261 7365 3a0a 0a60 6060 7079 7468 6f6e  base:..```python
+00001450: 0a73 6e61 7073 203d 2062 7563 6b65 742e  .snaps = bucket.
+00001460: 6c69 7374 5f73 6e61 7073 686f 7473 2829  list_snapshots()
+00001470: 0a62 6174 6368 6573 203d 2073 6e61 7073  .batches = snaps
+00001480: 5b30 5d2e 7363 6865 6d61 2827 7363 6865  [0].schema('sche
+00001490: 6d61 2d6e 616d 6527 292e 7461 626c 6528  ma-name').table(
+000014a0: 2774 6162 6c65 2d6e 616d 6527 292e 7365  'table-name').se
+000014b0: 6c65 6374 2829 0a60 6060 0a0a 2323 2056  lect().```..## V
+000014c0: 4153 5420 4361 7461 6c6f 670a 0a5b 5641  AST Catalog..[VA
+000014d0: 5354 2043 6174 616c 6f67 5d28 6874 7470  ST Catalog](http
+000014e0: 733a 2f2f 7661 7374 6461 7461 2e63 6f6d  s://vastdata.com
+000014f0: 2f62 6c6f 672f 7661 7374 2d63 6174 616c  /blog/vast-catal
+00001500: 6f67 2d74 7265 6174 2d79 6f75 722d 6669  og-treat-your-fi
+00001510: 6c65 2d73 7973 7465 6d2d 6c69 6b65 2d61  le-system-like-a
+00001520: 2d64 6174 6162 6173 6529 2063 616e 2062  -database) can b
+00001530: 6520 7175 6572 6965 6420 6173 2061 2072  e queried as a r
+00001540: 6567 756c 6172 2074 6162 6c65 3a0a 0a60  egular table:..`
+00001550: 6060 7079 7468 6f6e 0a74 6162 6c65 203d  ``python.table =
+00001560: 2070 612e 5461 626c 652e 6672 6f6d 5f62   pa.Table.from_b
+00001570: 6174 6368 6573 2874 782e 6361 7461 6c6f  atches(tx.catalo
+00001580: 672e 7365 6c65 6374 285b 2765 6c65 6d65  g.select(['eleme
+00001590: 6e74 5f74 7970 6527 5d29 290a 6466 203d  nt_type'])).df =
+000015a0: 2074 6162 6c65 2e74 6f5f 7061 6e64 6173   table.to_pandas
+000015b0: 2829 0a0a 746f 7461 6c5f 656c 656d 656e  ()..total_elemen
+000015c0: 7473 203d 206c 656e 2864 6629 0a70 7269  ts = len(df).pri
+000015d0: 6e74 2866 2254 6f74 616c 2065 6c65 6d65  nt(f"Total eleme
+000015e0: 6e74 7320 696e 2074 6865 2063 6174 616c  nts in the catal
+000015f0: 6f67 3a20 7b74 6f74 616c 5f65 6c65 6d65  og: {total_eleme
+00001600: 6e74 737d 2229 0a0a 6669 6c65 5f63 6f75  nts}")..file_cou
+00001610: 6e74 203d 2028 6466 5b27 656c 656d 656e  nt = (df['elemen
+00001620: 745f 7479 7065 275d 203d 3d20 2746 494c  t_type'] == 'FIL
+00001630: 4527 292e 7375 6d28 290a 7072 696e 7428  E').sum().print(
+00001640: 6622 4e75 6d62 6572 206f 6620 6669 6c65  f"Number of file
+00001650: 732f 6f62 6a65 6374 733a 207b 6669 6c65  s/objects: {file
+00001660: 5f63 6f75 6e74 7d22 290a 0a64 6973 7469  _count}")..disti
+00001670: 6e63 745f 656c 656d 656e 7473 203d 2064  nct_elements = d
+00001680: 665b 2765 6c65 6d65 6e74 5f74 7970 6527  f['element_type'
+00001690: 5d2e 756e 6971 7565 2829 0a70 7269 6e74  ].unique().print
+000016a0: 2822 4469 7374 696e 6374 2065 6c65 6d65  ("Distinct eleme
+000016b0: 6e74 2074 7970 6573 206f 6e20 7468 6520  nt types on the 
+000016c0: 7379 7374 656d 3a22 290a 7072 696e 7428  system:").print(
+000016d0: 6469 7374 696e 6374 5f65 6c65 6d65 6e74  distinct_element
+000016e0: 7329 0a60 6060 0a0a 5365 6520 7468 6520  s).```..See the 
+000016f0: 666f 6c6c 6f77 696e 6720 626c 6f67 2070  following blog p
+00001700: 6f73 7473 2066 6f72 206d 6f72 6520 6578  osts for more ex
+00001710: 616d 706c 6573 3a0a 0a2d 2068 7474 7073  amples:..- https
+00001720: 3a2f 2f76 6173 7464 6174 612e 636f 6d2f  ://vastdata.com/
+00001730: 626c 6f67 2f74 6865 2d76 6173 742d 6361  blog/the-vast-ca
+00001740: 7461 6c6f 672d 696e 2d61 6374 696f 6e2d  talog-in-action-
+00001750: 7061 7274 2d31 0a2d 2068 7474 7073 3a2f  part-1.- https:/
+00001760: 2f76 6173 7464 6174 612e 636f 6d2f 626c  /vastdata.com/bl
+00001770: 6f67 2f74 6865 2d76 6173 742d 6361 7461  og/the-vast-cata
+00001780: 6c6f 672d 696e 2d61 6374 696f 6e2d 7061  log-in-action-pa
+00001790: 7274 2d32 0a                             rt-2.
```

### Comparing `vastdb-0.1.4/setup.py` & `vastdb-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 
 from setuptools import find_packages, setup
 
 long_description = """
 `vastdb` is a Python-based SDK designed for interacting
 with [VAST Database](https://vastdata.com/database)
 and [VAST Catalog](https://vastdata.com/blog/vast-catalog-treat-your-file-system-like-a-database),
@@ -24,21 +25,21 @@
 if os.environ.get('VASTDB_APPEND_VERSION_SUFFIX'):
     suffix = _get_version_suffix()
 
 setup(
     name='vastdb',
     python_requires='>=3.9.0',
     description='VAST Data SDK',
-    version='0.1.4' + suffix,
+    version='0.1.5' + suffix,
     url='https://github.com/vast-data/vastdb_sdk',
     author='VAST DATA',
     author_email='hello@vastdata.com',
     license='Copyright (C) VAST Data Ltd.',
     packages=find_packages(),
-    install_requires=open('requirements.txt').read().strip().split('\n'),
+    install_requires=Path('requirements.txt').read_text().strip().split(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
```

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Block.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Block.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Date.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Date.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Field.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Field.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Int.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Int.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/List.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/List.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Map.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Map.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Message.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Message.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Null.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Null.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Time.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Time.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Type.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Type.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Union.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Union.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py` & `vastdb-0.1.5/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/AlterColumnRequest.py` & `vastdb-0.1.5/vast_flatbuf/tabular/AlterColumnRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/AlterProjectionTableRequest.py` & `vastdb-0.1.5/vast_flatbuf/tabular/AlterProjectionTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/AlterSchemaRequest.py` & `vastdb-0.1.5/vast_flatbuf/tabular/AlterSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/AlterTableRequest.py` & `vastdb-0.1.5/vast_flatbuf/tabular/AlterTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/Column.py` & `vastdb-0.1.5/vast_flatbuf/tabular/Column.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/CreateProjectionRequest.py` & `vastdb-0.1.5/vast_flatbuf/tabular/CreateProjectionRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/CreateSchemaRequest.py` & `vastdb-0.1.5/vast_flatbuf/tabular/CreateSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py` & `vastdb-0.1.5/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/GetTableStatsResponse.py` & `vastdb-0.1.5/vast_flatbuf/tabular/GetTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/ImportDataRequest.py` & `vastdb-0.1.5/vast_flatbuf/tabular/ImportDataRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/ListProjectionsResponse.py` & `vastdb-0.1.5/vast_flatbuf/tabular/ListProjectionsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/ListSchemasResponse.py` & `vastdb-0.1.5/vast_flatbuf/tabular/ListSchemasResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/ListTablesResponse.py` & `vastdb-0.1.5/vast_flatbuf/tabular/ListTablesResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/ObjectDetails.py` & `vastdb-0.1.5/vast_flatbuf/tabular/ObjectDetails.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/S3File.py` & `vastdb-0.1.5/vast_flatbuf/tabular/S3File.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vast_flatbuf/tabular/VipRange.py` & `vastdb-0.1.5/vast_flatbuf/tabular/VipRange.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/bench/test_perf.py` & `vastdb-0.1.5/vastdb/bench/test_perf.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/bucket.py` & `vastdb-0.1.5/vastdb/bucket.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/conftest.py` & `vastdb-0.1.5/vastdb/conftest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/errors.py` & `vastdb-0.1.5/vastdb/errors.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/internal_commands.py` & `vastdb-0.1.5/vastdb/internal_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,54 +126,21 @@
     }
     return unit_to_flatbuff_time_unit[type]
 
 
 class Predicate:
     def __init__(self, schema: 'pa.Schema', expr: ibis.expr.types.BooleanColumn):
         self.schema = schema
+        index = itertools.count()  # used to generate leaf column positions for VAST QueryData RPC
+        # Arrow schema contains the top-level columns, where each column may include multiple subfields
+        # We use DFS is used to enumerate all the sub-columns, using `index` as an ID allocator
+        nodes = [FieldNode(field, index) for field in schema]
+        self.nodes_map = {node.field.name: node for node in nodes}
         self.expr = expr
 
-    def get_field_indexes(self, field: 'pa.Field', field_name_per_index: list) -> None:
-        field_name_per_index.append(field.name)
-
-        if isinstance(field.type, pa.StructType):
-            flat_fields = field.flatten()
-        elif isinstance(field.type, pa.MapType):
-            flat_fields = [pa.field(f'{field.name}.entries', pa.struct([field.type.key_field, field.type.item_field]))]
-        elif isinstance(field.type, pa.ListType):
-            flat_fields = [pa.field(f'{field.name}.{field.type.value_field.name}', field.type.value_field.type)]
-        else:
-            return
-
-        for flat_field in flat_fields:
-            self.get_field_indexes(flat_field, field_name_per_index)
-
-    @property
-    def field_name_per_index(self):
-        if self._field_name_per_index is None:
-            _field_name_per_index = []
-            for field in self.schema:
-                self.get_field_indexes(field, _field_name_per_index)
-            self._field_name_per_index = {field: index for index, field in enumerate(_field_name_per_index)}
-        return self._field_name_per_index
-
-    def get_projections(self, builder: 'flatbuffers.builder.Builder', field_names: Optional[List[str]] = None):
-        if field_names is None:
-            field_names = self.field_name_per_index.keys()
-        projection_fields = []
-        for field_name in field_names:
-            fb_field_index.Start(builder)
-            fb_field_index.AddPosition(builder, self.field_name_per_index[field_name])
-            offset = fb_field_index.End(builder)
-            projection_fields.append(offset)
-        fb_source.StartProjectionVector(builder, len(projection_fields))
-        for offset in reversed(projection_fields):
-            builder.PrependUOffsetTRelative(offset)
-        return builder.EndVector()
-
     def serialize(self, builder: 'flatbuffers.builder.Builder'):
         from ibis.expr.operations.generic import (
             IsNull,
             Literal,
             TableColumn,
         )
         from ibis.expr.operations.logical import (
@@ -200,16 +167,14 @@
             NotEquals: self.build_not_equal,
             IsNull: self.build_is_null,
             Not: self.build_is_not_null,
             StringContains: self.build_match_substring,
             Between: self.build_between,
         }
 
-        positions_map = dict((f.name, index) for index, f in enumerate(self.schema))  # TODO: BFS
-
         self.builder = builder
 
         offsets = []
 
         if self.expr is not None:
             and_args = list(_flatten_args(self.expr.op(), And))
             _logger.debug('AND args: %s ops %s', and_args, self.expr.op())
@@ -257,15 +222,19 @@
 
                     field_name = column.name
                     if prev_field_name is None:
                         prev_field_name = field_name
                     elif prev_field_name != field_name:
                         raise NotImplementedError(self.expr)
 
-                    column_offset = self.build_column(position=positions_map[field_name])
+                    node = self.nodes_map[field_name]
+                    # TODO: support predicate pushdown for leaf nodes (ORION-160338)
+                    if node.children:
+                        raise NotImplementedError(node.field)  # no predicate pushdown for nested columns
+                    column_offset = self.build_column(position=node.index)
                     field = self.schema.field(field_name)
                     for literal in literals:
                         args_offsets = [column_offset]
                         if literal is not None:
                             args_offsets.append(self.build_literal(field=field, value=literal.value))
                         if builder_func == self.build_between:
                             args_offsets.append(self.build_literal(field=field, value=lower.value))
@@ -835,20 +804,21 @@
         for k, v in sorted(url_params.items()):
             params_list.append(f"{k}={urllib.parse.quote_plus(v)}")
 
         prefix += '&'.join(params_list)
         return prefix
 
     def _fill_common_headers(self, txid=0, client_tags=[], version_id=1):
-        common_headers = {'tabular-txid': str(txid), 'tabular-api-version-id': str(version_id),
-                          'tabular-client-name': 'tabular-api'}
-        for tag in client_tags:
-            common_headers['tabular-client-tags-%d' % client_tags.index(tag)] = tag
+        common_headers = {
+            'tabular-txid': str(txid),
+            'tabular-api-version-id': str(version_id),
+            'tabular-client-name': 'tabular-api'
+        }
 
-        return common_headers
+        return common_headers | {f'tabular-client-tags-{index}': tag for index, tag in enumerate(client_tags)}
 
     def _check_res(self, res, cmd="", expected_retvals=[]):
         if exc := errors.from_response(res):
             raise exc
         return res
 
     def create_schema(self, bucket, name, txid=0, client_tags=[], schema_properties="", expected_retvals=[]):
@@ -948,16 +918,15 @@
         schema = schema or ""
         res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, command="schema"), headers=headers, stream=True)
         self._check_res(res, "list_schemas", expected_retvals)
         if res.status_code == 200:
             res_headers = res.headers
             next_key = int(res_headers['tabular-next-key'])
             is_truncated = res_headers['tabular-is-truncated'] == 'true'
-            flatbuf = b''.join(res.iter_content(chunk_size=128))
-            lists = list_schemas.GetRootAs(flatbuf)
+            lists = list_schemas.GetRootAs(res.content)
             bucket_name = lists.BucketName().decode()
             if not bucket.startswith(bucket_name):
                 raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
             schemas_length = lists.SchemasLength()
             count = int(res_headers['tabular-list-count']) if 'tabular-list-count' in res_headers else schemas_length
             for i in range(schemas_length):
                 schema_obj = lists.Schemas(i)
@@ -972,16 +941,15 @@
         url_params = {'list_type': '2', 'prefix': '.snapshot/' + name_prefix, 'delimiter': '/', 'max_keys': str(max_keys)}
         if next_token:
             url_params['continuation-token'] = next_token
 
         res = self.session.get(self._api_prefix(bucket=bucket, command="list", url_params=url_params), headers={}, stream=True)
         self._check_res(res, "list_snapshots")
 
-        out = b''.join(res.iter_content(chunk_size=128))
-        xml_str = out.decode()
+        xml_str = res.content.decode()
         xml_dict = xmltodict.parse(xml_str)
         list_res = xml_dict['ListBucketResult']
         is_truncated = list_res['IsTruncated'] == 'true'
         marker = list_res['Marker']
         common_prefixes = list_res.get('CommonPrefixes', [])
         if isinstance(common_prefixes, dict):  # in case there is a single snapshot
             common_prefixes = [common_prefixes]
@@ -1055,16 +1023,15 @@
         The Command will return the statistics in flatbuf format
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if imports_table_stats else {}
         res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=name, command="stats", url_params=url_params), headers=headers)
         self._check_res(res, "get_table_stats", expected_retvals)
 
-        flatbuf = b''.join(res.iter_content(chunk_size=128))
-        stats = get_table_stats.GetRootAs(flatbuf)
+        stats = get_table_stats.GetRootAs(res.content)
         num_rows = stats.NumRows()
         size_in_bytes = stats.SizeInBytes()
         is_external_rowid_alloc = stats.IsExternalRowidAlloc()
         endpoints = []
         if stats.VipsLength() == 0:
             endpoints.append(self.url)
         else:
@@ -1155,16 +1122,15 @@
         tables = []
         res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, command="table"), headers=headers)
         self._check_res(res, "list_table", expected_retvals)
         if res.status_code == 200:
             res_headers = res.headers
             next_key = int(res_headers['tabular-next-key'])
             is_truncated = res_headers['tabular-is-truncated'] == 'true'
-            flatbuf = b''.join(res.iter_content(chunk_size=128))
-            lists = list_tables.GetRootAs(flatbuf)
+            lists = list_tables.GetRootAs(res.content)
             bucket_name = lists.BucketName().decode()
             schema_name = lists.SchemaName().decode()
             if not bucket.startswith(bucket_name):  # ignore snapshot name
                 raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
             tables_length = lists.TablesLength()
             count = int(res_headers['tabular-list-count']) if 'tabular-list-count' in res_headers else tables_length
             for i in range(tables_length):
@@ -1284,19 +1250,15 @@
                                headers=headers, stream=True)
         self._check_res(res, "list_columns", expected_retvals)
         if res.status_code == 200:
             res_headers = res.headers
             next_key = int(res_headers['tabular-next-key'])
             is_truncated = res_headers['tabular-is-truncated'] == 'true'
             count = int(res_headers['tabular-list-count'])
-            columns = []
-            if not count_only:
-                schema_buf = b''.join(res.iter_content(chunk_size=128))
-                schema_out = pa.ipc.open_stream(schema_buf).schema
-                columns = schema_out
+            columns = [] if count_only else pa.ipc.open_stream(res.content).schema
 
             return columns, next_key, is_truncated, count
 
     def begin_transaction(self, client_tags=[], expected_retvals=[]):
         """
         POST /?transaction HTTP/1.1
         tabular-client-tag: ClientTag
@@ -1688,16 +1650,15 @@
         The Command will return the statistics in flatbuf format
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         url_params = {'name': name}
         res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="projection-stats", url_params=url_params),
                                headers=headers)
         if res.status_code == 200:
-            flatbuf = b''.join(res.iter_content(chunk_size=128))
-            stats = get_projection_table_stats.GetRootAs(flatbuf)
+            stats = get_projection_table_stats.GetRootAs(res.content)
             num_rows = stats.NumRows()
             size_in_bytes = stats.SizeInBytes()
             dirty_blocks_percentage = stats.DirtyBlocksPercentage()
             initial_sync_progress = stats.InitialSyncProgress()
             return num_rows, size_in_bytes, dirty_blocks_percentage, initial_sync_progress
 
         return self._check_res(res, "get_projection_stats", expected_retvals)
@@ -1775,16 +1736,15 @@
         res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="projection"), headers=headers)
         self._check_res(res, "list_projections", expected_retvals)
         if res.status_code == 200:
             res_headers = res.headers
             next_key = int(res_headers['tabular-next-key'])
             is_truncated = res_headers['tabular-is-truncated'] == 'true'
             count = int(res_headers['tabular-list-count'])
-            flatbuf = b''.join(res.iter_content(chunk_size=128))
-            lists = list_projections.GetRootAs(flatbuf)
+            lists = list_projections.GetRootAs(res.content)
             bucket_name = lists.BucketName().decode()
             schema_name = lists.SchemaName().decode()
             table_name = lists.TableName().decode()
             if not bucket.startswith(bucket_name):  # ignore snapshot name
                 raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
             projections_length = lists.ProjectionsLength()
             for i in range(projections_length):
@@ -1823,21 +1783,16 @@
         self._check_res(res, "list_projection_columns", expected_retvals)
         # list projection columns response will also show column type Sorted/UnSorted
         if res.status_code == 200:
             res_headers = res.headers
             next_key = int(res_headers['tabular-next-key'])
             is_truncated = res_headers['tabular-is-truncated'] == 'true'
             count = int(res_headers['tabular-list-count'])
-            columns = []
-            if not count_only:
-                schema_buf = b''.join(res.iter_content(chunk_size=128))
-                schema_out = pa.ipc.open_stream(schema_buf).schema
-                for f in schema_out:
-                    columns.append([f.name, f.type, f.metadata])
-                #   sort_type = f.metadata[b'VAST:sort_type'].decode()
+            columns = [] if count_only else [[f.name, f.type, f.metadata] for f in
+                                             pa.ipc.open_stream(res.content).schema]
 
             return columns, next_key, is_truncated, count
 
 
 class QueryDataInternalError(Exception):
     pass
```

### Comparing `vastdb-0.1.4/vastdb/schema.py` & `vastdb-0.1.5/vastdb/schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/session.py` & `vastdb-0.1.5/vastdb/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,24 @@
         if self.vast_version < (5, 1):
             raise errors.NotSupportedVersion("return_row_ids requires 5.1+", self.vast_version)
 
 
 class Session:
     """VAST database session."""
 
-    def __init__(self, access=None, secret=None, endpoint=None):
+    def __init__(self, access=None, secret=None, endpoint=None, ssl_verify=True):
         """Connect to a VAST Database endpoint, using specified credentials."""
         if access is None:
             access = os.environ['AWS_ACCESS_KEY_ID']
         if secret is None:
             secret = os.environ['AWS_SECRET_ACCESS_KEY']
         if endpoint is None:
             endpoint = os.environ['AWS_S3_ENDPOINT_URL']
 
-        self.api = internal_commands.VastdbApi(endpoint, access, secret)
+        self.api = internal_commands.VastdbApi(endpoint, access, secret, ssl_verify=ssl_verify)
         version_tuple = tuple(int(part) for part in self.api.vast_version.split('.'))
         self.features = Features(version_tuple)
         self.s3 = boto3.client('s3',
             aws_access_key_id=access,
             aws_secret_access_key=secret,
             endpoint_url=endpoint)
```

### Comparing `vastdb-0.1.4/vastdb/table.py` & `vastdb-0.1.5/vastdb/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from math import ceil
 from threading import Event
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import backoff
 import ibis
 import pyarrow as pa
+import requests
 
 from . import errors, internal_commands, schema, util
 
 log = logging.getLogger(__name__)
 
 
 INTERNAL_ROW_ID = "$row_id"
@@ -35,28 +36,52 @@
 
     num_rows: int
     size_in_bytes: int
     is_external_rowid_alloc: bool = False
     endpoints: Tuple[str, ...] = ()
 
 
+RETRIABLE_ERRORS = (
+    errors.Slowdown,
+    requests.exceptions.ConnectionError,
+)
+
+
 @dataclass
 class QueryConfig:
     """Query execution configiration."""
 
+    # allows server-side parallel processing by issuing multiple reads concurrently for a single RPC
     num_sub_splits: int = 4
+
+    # used to split the table into disjoint subsets of rows, to be processed concurrently using multiple RPCs
     num_splits: int = 1
+
+    # each endpoint will be handled by a separate worker thread
+    # a single endpoint can be specified more than once to benefit from multithreaded execution
     data_endpoints: Optional[List[str]] = None
+
+    # a subsplit fiber will finish after sending this number of rows back to the client
     limit_rows_per_sub_split: int = 128 * 1024
+
+    # each fiber will read the following number of rowgroups coninuously before skipping
+    # in order to use semi-sorted projections this value must be 8
     num_row_groups_per_sub_split: int = 8
+
+    # can be disabled for benchmarking purposes
     use_semi_sorted_projections: bool = True
+
+    # used to estimate the number of splits, given the table rows' count
     rows_per_split: int = 4000000
+
+    # used for worker threads' naming
     query_id: str = ""
-    max_slowdown_retry: int = 10
-    backoff_func: Any = field(default=backoff.on_exception(backoff.expo, errors.Slowdown, max_tries=max_slowdown_retry))
+
+    # allows retrying QueryData when the server is overloaded
+    backoff_func: Any = field(default=backoff.on_exception(backoff.expo, RETRIABLE_ERRORS, max_tries=10))
 
 
 @dataclass
 class ImportConfig:
     """Import execution configiration."""
 
     import_concurrency: int = 2
@@ -267,15 +292,15 @@
         """Get the statistics of this table."""
         stats_tuple = self.tx._rpc.api.get_table_stats(
             bucket=self.bucket.name, schema=self.schema.name, name=self.name, txid=self.tx.txid,
             imports_table_stats=self._imports_table)
         return TableStats(**stats_tuple._asdict())
 
     def select(self, columns: Optional[List[str]] = None,
-               predicate: ibis.expr.types.BooleanColumn = None,
+               predicate: Union[ibis.expr.types.BooleanColumn, ibis.common.deferred.Deferred] = None,
                config: Optional[QueryConfig] = None,
                *,
                internal_row_id: bool = False) -> pa.RecordBatchReader:
         """Execute a query over this table.
 
         To read a subset of the columns, specify their names via `columns` argument. Otherwise, all columns will be read.
 
@@ -306,14 +331,17 @@
 
         if predicate is True:
             predicate = None
         if predicate is False:
             response_schema = internal_commands.get_response_schema(schema=query_schema, field_names=columns)
             return pa.RecordBatchReader.from_batches(response_schema, [])
 
+        if isinstance(predicate, ibis.common.deferred.Deferred):
+            predicate = predicate.resolve(self._ibis_table)  # may raise if the predicate is invalid (e.g. wrong types / missing column)
+
         query_data_request = internal_commands.build_query_data_request(
             schema=query_schema,
             predicate=predicate,
             field_names=columns)
 
         splits_queue: queue.Queue[int] = queue.Queue()
```

### Comparing `vastdb-0.1.4/vastdb/tests/test_duckdb.py` & `vastdb-0.1.5/vastdb/tests/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/tests/test_imports.py` & `vastdb-0.1.5/vastdb/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/tests/test_projections.py` & `vastdb-0.1.5/vastdb/tests/test_projections.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/tests/test_sanity.py` & `vastdb-0.1.5/vastdb/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/tests/test_schemas.py` & `vastdb-0.1.5/vastdb/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/tests/test_tables.py` & `vastdb-0.1.5/vastdb/tests/test_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import random
 import threading
 import time
 from contextlib import closing
 from tempfile import NamedTemporaryFile
 
+import ibis
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.parquet as pq
 import pytest
 from requests.exceptions import HTTPError
 
 from .. import errors
@@ -211,54 +212,55 @@
         [dt.time(12, 34, 56, 789789), dt.time(12, 34, 57, 789789), dt.time(12, 34, 58, 789789)],
         [dt.datetime(2024, 4, 10, 12, 34, 56), dt.datetime(2025, 4, 10, 12, 34, 56), dt.datetime(2026, 4, 10, 12, 34, 56)],
         [dt.datetime(2024, 4, 10, 12, 34, 56, 789000), dt.datetime(2025, 4, 10, 12, 34, 56, 789000), dt.datetime(2026, 4, 10, 12, 34, 56, 789000)],
         [dt.datetime(2024, 4, 10, 12, 34, 56, 789789), dt.datetime(2025, 4, 10, 12, 34, 56, 789789), dt.datetime(2026, 4, 10, 12, 34, 56, 789789)],
         [dt.datetime(2024, 4, 10, 12, 34, 56, 789789), dt.datetime(2025, 4, 10, 12, 34, 56, 789789), dt.datetime(2026, 4, 10, 12, 34, 56, 789789)],
     ])
 
-    with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
+    with prepare_data(session, clean_bucket_name, 's', 't', expected) as table:
         def select(predicate):
-            return pa.Table.from_batches(t.select(predicate=predicate))
+            return pa.Table.from_batches(table.select(predicate=predicate))
 
         assert select(None) == expected
-        assert select(t['tb'] == False) == expected.filter(pc.field('tb') == False)  # noqa: E712
-        assert select(t['a1'] == 2) == expected.filter(pc.field('a1') == 2)
-        assert select(t['a2'] == 2000) == expected.filter(pc.field('a2') == 2000)
-        assert select(t['a4'] == 222111122) == expected.filter(pc.field('a4') == 222111122)
-        assert select(t['b'] == 1.5) == expected.filter(pc.field('b') == 1.5)
-        assert select(t['s'] == "v") == expected.filter(pc.field('s') == "v")
-        assert select(t['d'] == 231.15) == expected.filter(pc.field('d') == 231.15)
-        assert select(t['bin'] == b"\x01\x02") == expected.filter(pc.field('bin') == b"\x01\x02")
-
-        date_literal = dt.date(2024, 4, 10)
-        assert select(t['date'] == date_literal) == expected.filter(pc.field('date') == date_literal)
-
-        time_literal = dt.time(12, 34, 56)
-        assert select(t['t0'] == time_literal) == expected.filter(pc.field('t0') == time_literal)
-
-        time_literal = dt.time(12, 34, 56, 789000)
-        assert select(t['t3'] == time_literal) == expected.filter(pc.field('t3') == time_literal)
-
-        time_literal = dt.time(12, 34, 56, 789789)
-        assert select(t['t6'] == time_literal) == expected.filter(pc.field('t6') == time_literal)
+        for t in [table, ibis._]:
+            assert select(t['tb'] == False) == expected.filter(pc.field('tb') == False)  # noqa: E712
+            assert select(t['a1'] == 2) == expected.filter(pc.field('a1') == 2)
+            assert select(t['a2'] == 2000) == expected.filter(pc.field('a2') == 2000)
+            assert select(t['a4'] == 222111122) == expected.filter(pc.field('a4') == 222111122)
+            assert select(t['b'] == 1.5) == expected.filter(pc.field('b') == 1.5)
+            assert select(t['s'] == "v") == expected.filter(pc.field('s') == "v")
+            assert select(t['d'] == 231.15) == expected.filter(pc.field('d') == 231.15)
+            assert select(t['bin'] == b"\x01\x02") == expected.filter(pc.field('bin') == b"\x01\x02")
+
+            date_literal = dt.date(2024, 4, 10)
+            assert select(t['date'] == date_literal) == expected.filter(pc.field('date') == date_literal)
+
+            time_literal = dt.time(12, 34, 56)
+            assert select(t['t0'] == time_literal) == expected.filter(pc.field('t0') == time_literal)
+
+            time_literal = dt.time(12, 34, 56, 789000)
+            assert select(t['t3'] == time_literal) == expected.filter(pc.field('t3') == time_literal)
+
+            time_literal = dt.time(12, 34, 56, 789789)
+            assert select(t['t6'] == time_literal) == expected.filter(pc.field('t6') == time_literal)
+
+            time_literal = dt.time(12, 34, 56, 789789)
+            assert select(t['t9'] == time_literal) == expected.filter(pc.field('t9') == time_literal)
+
+            ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56)
+            assert select(t['ts0'] == ts_literal) == expected.filter(pc.field('ts0') == ts_literal)
 
-        time_literal = dt.time(12, 34, 56, 789789)
-        assert select(t['t9'] == time_literal) == expected.filter(pc.field('t9') == time_literal)
+            ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789000)
+            assert select(t['ts3'] == ts_literal) == expected.filter(pc.field('ts3') == ts_literal)
 
-        ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56)
-        assert select(t['ts0'] == ts_literal) == expected.filter(pc.field('ts0') == ts_literal)
+            ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789789)
+            assert select(t['ts6'] == ts_literal) == expected.filter(pc.field('ts6') == ts_literal)
 
-        ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789000)
-        assert select(t['ts3'] == ts_literal) == expected.filter(pc.field('ts3') == ts_literal)
-
-        ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789789)
-        assert select(t['ts6'] == ts_literal) == expected.filter(pc.field('ts6') == ts_literal)
-
-        ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789789)
-        assert select(t['ts9'] == ts_literal) == expected.filter(pc.field('ts9') == ts_literal)
+            ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789789)
+            assert select(t['ts9'] == ts_literal) == expected.filter(pc.field('ts9') == ts_literal)
 
 
 def test_filters(session, clean_bucket_name):
     columns = pa.schema([
         ('a', pa.int32()),
         ('b', pa.float64()),
         ('s', pa.utf8()),
@@ -266,70 +268,71 @@
 
     expected = pa.table(schema=columns, data=[
         [111, 222, 333, 444, 555],
         [0.5, 1.5, 2.5, 3.5, 4.5],
         ['a', 'bb', 'ccc', None, 'xyz'],
     ])
 
-    with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
+    with prepare_data(session, clean_bucket_name, 's', 't', expected) as table:
         def select(predicate):
-            return pa.Table.from_batches(t.select(predicate=predicate), t.arrow_schema)
+            return pa.Table.from_batches(table.select(predicate=predicate), table.arrow_schema)
 
         assert select(None) == expected
         assert select(True) == expected
         assert select(False) == pa.Table.from_batches([], schema=columns)
 
-        assert select(t['a'].between(222, 444)) == expected.filter((pc.field('a') >= 222) & (pc.field('a') <= 444))
-        assert select((t['a'].between(222, 444)) & (t['b'] > 2.5)) == expected.filter((pc.field('a') >= 222) & (pc.field('a') <= 444) & (pc.field('b') > 2.5))
-
-        assert select(t['a'] > 222) == expected.filter(pc.field('a') > 222)
-        assert select(t['a'] < 222) == expected.filter(pc.field('a') < 222)
-        assert select(t['a'] == 222) == expected.filter(pc.field('a') == 222)
-        assert select(t['a'] != 222) == expected.filter(pc.field('a') != 222)
-        assert select(t['a'] <= 222) == expected.filter(pc.field('a') <= 222)
-        assert select(t['a'] >= 222) == expected.filter(pc.field('a') >= 222)
-
-        assert select(t['b'] > 1.5) == expected.filter(pc.field('b') > 1.5)
-        assert select(t['b'] < 1.5) == expected.filter(pc.field('b') < 1.5)
-        assert select(t['b'] == 1.5) == expected.filter(pc.field('b') == 1.5)
-        assert select(t['b'] != 1.5) == expected.filter(pc.field('b') != 1.5)
-        assert select(t['b'] <= 1.5) == expected.filter(pc.field('b') <= 1.5)
-        assert select(t['b'] >= 1.5) == expected.filter(pc.field('b') >= 1.5)
-
-        assert select(t['s'] > 'bb') == expected.filter(pc.field('s') > 'bb')
-        assert select(t['s'] < 'bb') == expected.filter(pc.field('s') < 'bb')
-        assert select(t['s'] == 'bb') == expected.filter(pc.field('s') == 'bb')
-        assert select(t['s'] != 'bb') == expected.filter(pc.field('s') != 'bb')
-        assert select(t['s'] <= 'bb') == expected.filter(pc.field('s') <= 'bb')
-        assert select(t['s'] >= 'bb') == expected.filter(pc.field('s') >= 'bb')
-
-        assert select((t['a'] > 111) & (t['b'] > 0) & (t['s'] < 'ccc')) == expected.filter((pc.field('a') > 111) & (pc.field('b') > 0) & (pc.field('s') < 'ccc'))
-        assert select((t['a'] > 111) & (t['b'] < 2.5)) == expected.filter((pc.field('a') > 111) & (pc.field('b') < 2.5))
-        assert select((t['a'] > 111) & (t['a'] < 333)) == expected.filter((pc.field('a') > 111) & (pc.field('a') < 333))
-
-        assert select((t['a'] > 111) | (t['a'] < 333)) == expected.filter((pc.field('a') > 111) | (pc.field('a') < 333))
-        assert select(((t['a'] > 111) | (t['a'] < 333)) & (t['b'] < 2.5)) == expected.filter(((pc.field('a') > 111) | (pc.field('a') < 333)) & (pc.field('b') < 2.5))
-        with pytest.raises(NotImplementedError):
-            assert select((t['a'] > 111) | (t['b'] > 0) | (t['s'] < 'ccc')) == expected.filter((pc.field('a') > 111) | (pc.field('b') > 0) | (pc.field('s') < 'ccc'))
-        assert select((t['a'] > 111) | (t['a'] < 333) | (t['a'] == 777)) == expected.filter((pc.field('a') > 111) | (pc.field('a') < 333) | (pc.field('a') == 777))
-
-        assert select(t['s'].isnull()) == expected.filter(pc.field('s').is_null())
-        assert select((t['s'].isnull()) | (t['s'] == 'bb'))  == expected.filter((pc.field('s').is_null()) | (pc.field('s') == 'bb'))
-        assert select((t['s'].isnull()) & (t['b'] == 3.5))  == expected.filter((pc.field('s').is_null()) & (pc.field('b') == 3.5))
-
-        assert select(~t['s'].isnull()) == expected.filter(~pc.field('s').is_null())
-        assert select(t['s'].contains('b')) == expected.filter(pc.field('s') == 'bb')
-        assert select(t['s'].contains('y')) == expected.filter(pc.field('s') == 'xyz')
-
-        assert select(t['a'].isin([555])) == expected.filter(pc.field('a').isin([555]))
-        assert select(t['a'].isin([111, 222, 999])) == expected.filter(pc.field('a').isin([111, 222, 999]))
-        assert select((t['a'] == 111) | t['a'].isin([333, 444]) | (t['a'] > 600)) == expected.filter((pc.field('a') == 111) | pc.field('a').isin([333, 444]) | (pc.field('a') > 600))
+        for t in [table, ibis._]:
+            assert select(t['a'].between(222, 444)) == expected.filter((pc.field('a') >= 222) & (pc.field('a') <= 444))
+            assert select((t['a'].between(222, 444)) & (t['b'] > 2.5)) == expected.filter((pc.field('a') >= 222) & (pc.field('a') <= 444) & (pc.field('b') > 2.5))
+
+            assert select(t['a'] > 222) == expected.filter(pc.field('a') > 222)
+            assert select(t['a'] < 222) == expected.filter(pc.field('a') < 222)
+            assert select(t['a'] == 222) == expected.filter(pc.field('a') == 222)
+            assert select(t['a'] != 222) == expected.filter(pc.field('a') != 222)
+            assert select(t['a'] <= 222) == expected.filter(pc.field('a') <= 222)
+            assert select(t['a'] >= 222) == expected.filter(pc.field('a') >= 222)
+
+            assert select(t['b'] > 1.5) == expected.filter(pc.field('b') > 1.5)
+            assert select(t['b'] < 1.5) == expected.filter(pc.field('b') < 1.5)
+            assert select(t['b'] == 1.5) == expected.filter(pc.field('b') == 1.5)
+            assert select(t['b'] != 1.5) == expected.filter(pc.field('b') != 1.5)
+            assert select(t['b'] <= 1.5) == expected.filter(pc.field('b') <= 1.5)
+            assert select(t['b'] >= 1.5) == expected.filter(pc.field('b') >= 1.5)
+
+            assert select(t['s'] > 'bb') == expected.filter(pc.field('s') > 'bb')
+            assert select(t['s'] < 'bb') == expected.filter(pc.field('s') < 'bb')
+            assert select(t['s'] == 'bb') == expected.filter(pc.field('s') == 'bb')
+            assert select(t['s'] != 'bb') == expected.filter(pc.field('s') != 'bb')
+            assert select(t['s'] <= 'bb') == expected.filter(pc.field('s') <= 'bb')
+            assert select(t['s'] >= 'bb') == expected.filter(pc.field('s') >= 'bb')
+
+            assert select((t['a'] > 111) & (t['b'] > 0) & (t['s'] < 'ccc')) == expected.filter((pc.field('a') > 111) & (pc.field('b') > 0) & (pc.field('s') < 'ccc'))
+            assert select((t['a'] > 111) & (t['b'] < 2.5)) == expected.filter((pc.field('a') > 111) & (pc.field('b') < 2.5))
+            assert select((t['a'] > 111) & (t['a'] < 333)) == expected.filter((pc.field('a') > 111) & (pc.field('a') < 333))
+
+            assert select((t['a'] > 111) | (t['a'] < 333)) == expected.filter((pc.field('a') > 111) | (pc.field('a') < 333))
+            assert select(((t['a'] > 111) | (t['a'] < 333)) & (t['b'] < 2.5)) == expected.filter(((pc.field('a') > 111) | (pc.field('a') < 333)) & (pc.field('b') < 2.5))
+            with pytest.raises(NotImplementedError):
+                assert select((t['a'] > 111) | (t['b'] > 0) | (t['s'] < 'ccc')) == expected.filter((pc.field('a') > 111) | (pc.field('b') > 0) | (pc.field('s') < 'ccc'))
+            assert select((t['a'] > 111) | (t['a'] < 333) | (t['a'] == 777)) == expected.filter((pc.field('a') > 111) | (pc.field('a') < 333) | (pc.field('a') == 777))
+
+            assert select(t['s'].isnull()) == expected.filter(pc.field('s').is_null())
+            assert select((t['s'].isnull()) | (t['s'] == 'bb'))  == expected.filter((pc.field('s').is_null()) | (pc.field('s') == 'bb'))
+            assert select((t['s'].isnull()) & (t['b'] == 3.5))  == expected.filter((pc.field('s').is_null()) & (pc.field('b') == 3.5))
+
+            assert select(~t['s'].isnull()) == expected.filter(~pc.field('s').is_null())
+            assert select(t['s'].contains('b')) == expected.filter(pc.field('s') == 'bb')
+            assert select(t['s'].contains('y')) == expected.filter(pc.field('s') == 'xyz')
+
+            assert select(t['a'].isin([555])) == expected.filter(pc.field('a').isin([555]))
+            assert select(t['a'].isin([111, 222, 999])) == expected.filter(pc.field('a').isin([111, 222, 999]))
+            assert select((t['a'] == 111) | t['a'].isin([333, 444]) | (t['a'] > 600)) == expected.filter((pc.field('a') == 111) | pc.field('a').isin([333, 444]) | (pc.field('a') > 600))
 
-        with pytest.raises(NotImplementedError):
-            select(t['a'].isin([]))
+            with pytest.raises(NotImplementedError):
+                select(t['a'].isin([]))
 
 
 def test_parquet_export(session, clean_bucket_name):
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s1')
         columns = pa.schema([
             ('a', pa.int16()),
```

### Comparing `vastdb-0.1.4/vastdb/tests/test_util.py` & `vastdb-0.1.5/vastdb/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/tests/util.py` & `vastdb-0.1.5/vastdb/tests/util.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb/transaction.py` & `vastdb-0.1.5/vastdb/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def bucket(self, name: str) -> "bucket.Bucket":
         """Return a VAST Bucket, if exists."""
         try:
             self._rpc.s3.head_bucket(Bucket=name)
         except botocore.exceptions.ClientError as e:
             log.warning("res: %s", e.response)
             if e.response['Error']['Code'] == '404':
-                raise errors.MissingBucket(name)
+                raise errors.MissingBucket(name) from e
             raise
         return bucket.Bucket(name, self)
 
     def catalog(self, fail_if_missing=True) -> Optional["table.Table"]:
         """Return VAST Catalog table."""
         b = bucket.Bucket(TABULAR_BC_BUCKET, self)
         s = schema.Schema(VAST_CATALOG_SCHEMA_NAME, b)
```

### Comparing `vastdb-0.1.4/vastdb/util.py` & `vastdb-0.1.5/vastdb/util.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.4/vastdb.egg-info/PKG-INFO` & `vastdb-0.1.5/vastdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.4
+Version: 0.1.5
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vastdb-0.1.4/vastdb.egg-info/SOURCES.txt` & `vastdb-0.1.5/vastdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

