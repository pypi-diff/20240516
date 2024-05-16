# Comparing `tmp/streams_py-1.2.1.tar.gz` & `tmp/streams_py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams_py-1.2.1.tar", max compression
+gzip compressed data, was "streams_py-1.3.0.tar", max compression
```

## Comparing `streams_py-1.2.1.tar` & `streams_py-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0    35149 2024-02-23 20:47:06.741874 streams_py-1.2.1/LICENSE
--rw-r--r--   0        0        0    12194 2024-02-23 20:47:06.741874 streams_py-1.2.1/README.md
--rw-r--r--   0        0        0      861 2024-02-23 20:47:06.741874 streams_py-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      157 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/__init__.py
--rw-r--r--   0        0        0      336 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/__iterate.py
--rw-r--r--   0        0        0     3910 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/__optional.py
--rw-r--r--   0        0        0     3483 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/__stream.py
--rw-r--r--   0        0        0     1809 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/__stream_converter.py
--rw-r--r--   0        0        0        0 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_itertools/__init__.py
--rw-r--r--   0        0        0     1713 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_itertools/tools.py
--rw-r--r--   0        0        0        0 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_lazy/__init__.py
--rw-r--r--   0        0        0      626 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_lazy/process.py
--rw-r--r--   0        0        0      593 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_lazy/queue.py
--rw-r--r--   0        0        0        0 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_parallel/__init__.py
--rw-r--r--   0        0        0     3903 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_parallel/fork_and_join.py
--rw-r--r--   0        0        0      781 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_parallel/parallelizer.py
--rw-r--r--   0        0        0    16071 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/__base_stream.py
--rw-r--r--   0        0        0        0 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/__init__.py
--rw-r--r--   0        0        0     3476 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/__parallel_stream.py
--rw-r--r--   0        0        0     2227 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/__sequential_stream.py
--rw-r--r--   0        0        0     3062 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/error/__error.py
--rw-r--r--   0        0        0      258 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/error/__levels.py
--rw-r--r--   0        0        0      307 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/error/__sentinel.py
--rw-r--r--   0        0        0     3595 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/numeric/__numeric_base_stream.py
--rw-r--r--   0        0        0      861 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
--rw-r--r--   0        0        0      686 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
--rw-r--r--   0        0        0      221 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/conditions/__init__.py
--rw-r--r--   0        0        0      307 2024-02-23 20:47:06.741874 streams_py-1.2.1/pystreamapi/conditions/combiners.py
--rw-r--r--   0        0        0    10297 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/conditions/date.py
--rw-r--r--   0        0        0     4937 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/conditions/numeric.py
--rw-r--r--   0        0        0     1385 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/conditions/string.py
--rw-r--r--   0        0        0      735 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/conditions/types.py
--rw-r--r--   0        0        0     1870 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__csv/__csv_loader.py
--rw-r--r--   0        0        0        0 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__csv/__init__.py
--rw-r--r--   0        0        0      216 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__json/__init__.py
--rw-r--r--   0        0        0     1683 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__json/__json_loader.py
--rw-r--r--   0        0        0      647 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__lazy_file_iterable.py
--rw-r--r--   0        0        0      838 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__loader_utils.py
--rw-r--r--   0        0        0        0 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__xml/__init__.py
--rw-r--r--   0        0        0     4076 2024-02-23 20:47:06.745874 streams_py-1.2.1/pystreamapi/loaders/__xml/__xml_loader.py
--rw-r--r--   0        0        0    13228 1970-01-01 00:00:00.000000 streams_py-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-16 14:54:37.903775 streams_py-1.3.0/LICENSE
+-rw-r--r--   0        0        0    12510 2024-05-16 14:54:37.903775 streams_py-1.3.0/README.md
+-rw-r--r--   0        0        0      917 2024-05-16 14:54:37.903775 streams_py-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      157 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/__iterate.py
+-rw-r--r--   0        0        0     3910 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/__optional.py
+-rw-r--r--   0        0        0     3483 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/__stream.py
+-rw-r--r--   0        0        0     1809 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/__stream_converter.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/_itertools/__init__.py
+-rw-r--r--   0        0        0     1713 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/_itertools/tools.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/_lazy/__init__.py
+-rw-r--r--   0        0        0      626 2024-05-16 14:54:37.903775 streams_py-1.3.0/pystreamapi/_lazy/process.py
+-rw-r--r--   0        0        0      593 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_lazy/queue.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_parallel/__init__.py
+-rw-r--r--   0        0        0     3903 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_parallel/fork_and_join.py
+-rw-r--r--   0        0        0      781 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_parallel/parallelizer.py
+-rw-r--r--   0        0        0    16071 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/__base_stream.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/__init__.py
+-rw-r--r--   0        0        0     3476 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/__parallel_stream.py
+-rw-r--r--   0        0        0     2227 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/__sequential_stream.py
+-rw-r--r--   0        0        0     3062 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/error/__error.py
+-rw-r--r--   0        0        0      258 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/error/__levels.py
+-rw-r--r--   0        0        0      307 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/error/__sentinel.py
+-rw-r--r--   0        0        0     3595 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/numeric/__numeric_base_stream.py
+-rw-r--r--   0        0        0      861 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
+-rw-r--r--   0        0        0      686 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
+-rw-r--r--   0        0        0      221 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/conditions/__init__.py
+-rw-r--r--   0        0        0      307 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/conditions/combiners.py
+-rw-r--r--   0        0        0    10297 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/conditions/date.py
+-rw-r--r--   0        0        0     4937 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/conditions/numeric.py
+-rw-r--r--   0        0        0     1385 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/conditions/string.py
+-rw-r--r--   0        0        0      735 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/conditions/types.py
+-rw-r--r--   0        0        0     1870 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__csv/__csv_loader.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__csv/__init__.py
+-rw-r--r--   0        0        0      286 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__json/__init__.py
+-rw-r--r--   0        0        0     1683 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__json/__json_loader.py
+-rw-r--r--   0        0        0      647 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__lazy_file_iterable.py
+-rw-r--r--   0        0        0      838 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__loader_utils.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__xml/__init__.py
+-rw-r--r--   0        0        0     4076 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__xml/__xml_loader.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__yaml/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-16 14:54:37.907775 streams_py-1.3.0/pystreamapi/loaders/__yaml/__yaml_loader.py
+-rw-r--r--   0        0        0    13657 1970-01-01 00:00:00.000000 streams_py-1.3.0/PKG-INFO
```

### Comparing `streams_py-1.2.1/LICENSE` & `streams_py-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/README.md` & `streams_py-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 * It provides both sequential and parallel streams.
 * Lazy execution is supported, enhancing performance.
 * It boasts high speed and efficiency.
 * The implementation achieves 100% test coverage.
 * It follows Pythonic principles, resulting in clean and readable code.
 * It adds some cool innovative features such as conditions or error handling and an even more declarative look.
-* It provides loaders for various data sources such as CSV, JSON and XML files.
+* It provides loaders for various data sources such as CSV, JSON, XML and YAML files.
 
 Let's take a look at a small example:
 
 ```python
 from pystreamapi import Stream
 
 Stream.of([" ", '3', None, "2", 1, ""]) \
@@ -209,23 +209,23 @@
 ```python
 Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) 
 # Like Stream.of([1, 2, 3, 4])
 ```
 
 Creates a new Stream from multiple Streams. Order doesn't change.
 
-## Use loaders: Load data from CSV, JSON and XML files in just one line
+## Use loaders: Load data from CSV, JSON, XML and YAML files in just one line
 
-PyStreamAPI offers a convenient way to load data from CSV, JSON and XML files. Like that you can start processing your
+PyStreamAPI offers a convenient way to load data from CSV, JSON, XML and YAML files. Like that you can start processing your
 files right away without having to worry about reading and parsing the files.
 
 You can import the loaders with:
 
 ```python
-from pystreamapi.loaders import csv, json, xml
+from pystreamapi.loaders import csv, json, xml, yaml
 ```
 Now you can use the loaders directly when creating your Stream:
 
 For CSV:
 
 ```python
 Stream.of(csv("data.csv", delimiter=";")) \
@@ -249,22 +249,38 @@
 ```bash
 pip install streams.py[xml_loader]
 ```
 
 Afterward, you can use the XML loader like this:
 
 ```python
-Stream.of(xml("data.xml"))
-  .map(lambda x: x.attr1)
+Stream.of(xml("data.xml")) \
+  .map(lambda x: x.attr1) \
   .for_each(print)
 ```
 
 The access to the attributes is using a node path syntax. For more details on how to use the node path syntax, please
 refer to the [documentation](https://pystreamapi.pickwicksoft.org/reference/data-loaders).
 
+For YAML:
+
+In order to use the YAML loader, you need to install the optional yaml dependency:
+
+```bash
+pip install streams.py[yaml_loader]
+```
+
+Afterward, you can use the YAML loader like this:
+
+```python
+Stream.of(yaml("data.yaml")) \
+  .map(lambda x: x.attr1) \
+  .for_each(print)
+```
+
 ## API Reference
 For a more detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/)
 
 ## Complex Examples
 
 #### Get all numbers from list of different types. Use parallelization.
```

#### html2text {}

```diff
@@ -10,36 +10,36 @@
 there are already a few implementations? Well, here are a few advantages of
 this particular implementation: * It provides both sequential and parallel
 streams. * Lazy execution is supported, enhancing performance. * It boasts high
 speed and efficiency. * The implementation achieves 100% test coverage. * It
 follows Pythonic principles, resulting in clean and readable code. * It adds
 some cool innovative features such as conditions or error handling and an even
 more declarative look. * It provides loaders for various data sources such as
-CSV, JSON and XML files. Let's take a look at a small example: ```python from
-pystreamapi import Stream Stream.of([" ", '3', None, "2", 1, ""]) \ .filter
-(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter
-(lambda x: len(x) > 0) \ .map(int) \ .sorted() \ .for_each(print) # Output: 1 2
-3 ``` And here's the equivalent code in Java: ```java Object[] words = { " ",
-'3', null, "2", 1, "" }; Arrays.stream( words ) .filter( Objects::nonNull )
-.map( Objects::toString ) .map( String::trim ) .filter( s -> ! s.isEmpty() )
-.map( Integer::parseInt ) .sorted() .forEach( System.out::println ); // Output:
-1 2 3 ``` ## What is a Stream? A `Stream` is a powerful abstraction for
-processing sequences of data in a functional and declarative manner. It enables
-efficient and concise data manipulation and transformation. Similar to its
-counterparts in Java and Kotlin, a Stream represents a pipeline of operations
-that can be applied to a collection or any iterable data source. It allows
-developers to express complex data processing logic using a combination of
-high-level operations, promoting code reusability and readability. With
-Streams, you can perform a wide range of operations on your data, such as
-filtering elements, transforming values, aggregating results, sorting, and
-more. These operations can be seamlessly chained together to form a processing
-pipeline, where each operation processes the data and passes it on to the next
-operation. One of the key benefits of Stream is lazy evaluation. This means
-that the operations are executed only when the result is actually needed,
-optimizing resource usage and enabling efficient processing of large or
+CSV, JSON, XML and YAML files. Let's take a look at a small example: ```python
+from pystreamapi import Stream Stream.of([" ", '3', None, "2", 1, ""]) \
+.filter(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \
+.filter(lambda x: len(x) > 0) \ .map(int) \ .sorted() \ .for_each(print) #
+Output: 1 2 3 ``` And here's the equivalent code in Java: ```java Object[]
+words = { " ", '3', null, "2", 1, "" }; Arrays.stream( words ) .filter
+( Objects::nonNull ) .map( Objects::toString ) .map( String::trim ) .filter( s
+-> ! s.isEmpty() ) .map( Integer::parseInt ) .sorted() .forEach( System.out::
+println ); // Output: 1 2 3 ``` ## What is a Stream? A `Stream` is a powerful
+abstraction for processing sequences of data in a functional and declarative
+manner. It enables efficient and concise data manipulation and transformation.
+Similar to its counterparts in Java and Kotlin, a Stream represents a pipeline
+of operations that can be applied to a collection or any iterable data source.
+It allows developers to express complex data processing logic using a
+combination of high-level operations, promoting code reusability and
+readability. With Streams, you can perform a wide range of operations on your
+data, such as filtering elements, transforming values, aggregating results,
+sorting, and more. These operations can be seamlessly chained together to form
+a processing pipeline, where each operation processes the data and passes it on
+to the next operation. One of the key benefits of Stream is lazy evaluation.
+This means that the operations are executed only when the result is actually
+needed, optimizing resource usage and enabling efficient processing of large or
 infinite datasets. Furthermore, Stream supports both sequential and parallel
 execution. This allows you to leverage parallel processing capabilities when
 dealing with computationally intensive tasks or large amounts of data,
 significantly improving performance. `pystreamapi.Stream` represents a stream
 that facilitates the execution of one or more operations. Stream operations can
 be categorized as either intermediate or terminal. Terminal operations return a
 result of a specific type, while intermediate operations return the stream
@@ -104,31 +104,35 @@
 numeric) Stream.of_noneable(None) ``` If the source is `None`, you get an empty
 `Stream` --- ```python Stream.iterate(0, lambda n: n + 2) ``` Creates a Stream
 of an infinite Iterator created by iterative application of a function f to an
 initial element seed, producing a Stream consisting of seed, f(seed), f(f
 (seed)), etc. > **Note** > Do not forget to limit the stream with `.limit()` --
 - ```python Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) # Like
 Stream.of([1, 2, 3, 4]) ``` Creates a new Stream from multiple Streams. Order
-doesn't change. ## Use loaders: Load data from CSV, JSON and XML files in just
-one line PyStreamAPI offers a convenient way to load data from CSV, JSON and
-XML files. Like that you can start processing your files right away without
-having to worry about reading and parsing the files. You can import the loaders
-with: ```python from pystreamapi.loaders import csv, json, xml ``` Now you can
-use the loaders directly when creating your Stream: For CSV: ```python
-Stream.of(csv("data.csv", delimiter=";")) \ .map(lambda x: x.attr1) \ .for_each
-(print) ``` For JSON: ```python Stream.of(json("data.json")) \ .map(lambda x:
-x.attr1) \ .for_each(print) ``` You can access the attributes of the data
-structures directly like you would do with a normal object. For XML: In order
-to use the XML loader, you need to install the optional xml dependency: ```bash
-pip install streams.py[xml_loader] ``` Afterward, you can use the XML loader
-like this: ```python Stream.of(xml("data.xml")) .map(lambda x: x.attr1)
-.for_each(print) ``` The access to the attributes is using a node path syntax.
-For more details on how to use the node path syntax, please refer to the
-[documentation](https://pystreamapi.pickwicksoft.org/reference/data-loaders).
-## API Reference For a more detailed documentation view the docs on GitBook:
+doesn't change. ## Use loaders: Load data from CSV, JSON, XML and YAML files in
+just one line PyStreamAPI offers a convenient way to load data from CSV, JSON,
+XML and YAML files. Like that you can start processing your files right away
+without having to worry about reading and parsing the files. You can import the
+loaders with: ```python from pystreamapi.loaders import csv, json, xml, yaml
+``` Now you can use the loaders directly when creating your Stream: For CSV:
+```python Stream.of(csv("data.csv", delimiter=";")) \ .map(lambda x: x.attr1) \
+.for_each(print) ``` For JSON: ```python Stream.of(json("data.json")) \ .map
+(lambda x: x.attr1) \ .for_each(print) ``` You can access the attributes of the
+data structures directly like you would do with a normal object. For XML: In
+order to use the XML loader, you need to install the optional xml dependency:
+```bash pip install streams.py[xml_loader] ``` Afterward, you can use the XML
+loader like this: ```python Stream.of(xml("data.xml")) \ .map(lambda x:
+x.attr1) \ .for_each(print) ``` The access to the attributes is using a node
+path syntax. For more details on how to use the node path syntax, please refer
+to the [documentation](https://pystreamapi.pickwicksoft.org/reference/data-
+loaders). For YAML: In order to use the YAML loader, you need to install the
+optional yaml dependency: ```bash pip install streams.py[yaml_loader] ```
+Afterward, you can use the YAML loader like this: ```python Stream.of(yaml
+("data.yaml")) \ .map(lambda x: x.attr1) \ .for_each(print) ``` ## API
+Reference For a more detailed documentation view the docs on GitBook:
 [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/) ## Complex Examples
 #### Get all numbers from list of different types. Use parallelization.
 ```python Stream.parallel_of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x:
 x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len
 (x) > 0) \ .map(int) \ .sorted()\ .for_each(print) # 1 2 3 ``` #### Generate a
 Stream of 10 Fibonacci numbers ```python def fib(): a, b = 0, 1 while True:
 yield a a, b = b, a + b Stream.of(fib()) \ .limit(10) \ .for_each(print) # 0 1
```

### Comparing `streams_py-1.2.1/pyproject.toml` & `streams_py-1.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "streams.py"
-version = "1.2.1"
+version = "1.3.0"
 authors = ["Stefan Garlonta <stefan@pickwicksoft.org>"]
 description = "A stream library for Python inspired by Java Stream API"
 keywords = ["streams", "parallel", "data"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/PickwickSoft/pystreamapi"
 repository = "https://github.com/PickwickSoft/pystreamapi"
 readme = "README.md"
 packages = [
     { include = "pystreamapi" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
-joblib = ">=1.2,<1.4"
+joblib = ">=1.2,<=1.4.2"
 defusedxml = { version = ">=0.7,<0.8", optional = true }
+pyyaml = "^6.0.1"
 
 [tool.poetry.extras]
 xml_loader = ["defusedxml"]
-all = ["defusedxml"]
+yaml_loader = ["pyyaml"]
+all = ["defusedxml", "pyyaml"]
 
 [tool.poetry.group.test.dependencies]
 parameterized = "*"
 pylint = "*"
 coverage = "*"
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `streams_py-1.2.1/pystreamapi/__optional.py` & `streams_py-1.3.0/pystreamapi/__optional.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/__stream.py` & `streams_py-1.3.0/pystreamapi/__stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/__stream_converter.py` & `streams_py-1.3.0/pystreamapi/__stream_converter.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_itertools/tools.py` & `streams_py-1.3.0/pystreamapi/_itertools/tools.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_lazy/process.py` & `streams_py-1.3.0/pystreamapi/_lazy/process.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_lazy/queue.py` & `streams_py-1.3.0/pystreamapi/_lazy/queue.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_parallel/fork_and_join.py` & `streams_py-1.3.0/pystreamapi/_parallel/fork_and_join.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_parallel/parallelizer.py` & `streams_py-1.3.0/pystreamapi/_parallel/parallelizer.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_streams/__base_stream.py` & `streams_py-1.3.0/pystreamapi/_streams/__base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_streams/__parallel_stream.py` & `streams_py-1.3.0/pystreamapi/_streams/__parallel_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_streams/__sequential_stream.py` & `streams_py-1.3.0/pystreamapi/_streams/__sequential_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_streams/error/__error.py` & `streams_py-1.3.0/pystreamapi/_streams/error/__error.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_streams/numeric/__numeric_base_stream.py` & `streams_py-1.3.0/pystreamapi/_streams/numeric/__numeric_base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_streams/numeric/__parallel_numeric_stream.py` & `streams_py-1.3.0/pystreamapi/_streams/numeric/__parallel_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/_streams/numeric/__sequential_numeric_stream.py` & `streams_py-1.3.0/pystreamapi/_streams/numeric/__sequential_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/conditions/date.py` & `streams_py-1.3.0/pystreamapi/conditions/date.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/conditions/numeric.py` & `streams_py-1.3.0/pystreamapi/conditions/numeric.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/conditions/string.py` & `streams_py-1.3.0/pystreamapi/conditions/string.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/conditions/types.py` & `streams_py-1.3.0/pystreamapi/conditions/types.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/loaders/__csv/__csv_loader.py` & `streams_py-1.3.0/pystreamapi/loaders/__csv/__csv_loader.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/loaders/__json/__json_loader.py` & `streams_py-1.3.0/pystreamapi/loaders/__json/__json_loader.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/loaders/__lazy_file_iterable.py` & `streams_py-1.3.0/pystreamapi/loaders/__lazy_file_iterable.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/loaders/__loader_utils.py` & `streams_py-1.3.0/pystreamapi/loaders/__loader_utils.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/pystreamapi/loaders/__xml/__xml_loader.py` & `streams_py-1.3.0/pystreamapi/loaders/__xml/__xml_loader.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.2.1/PKG-INFO` & `streams_py-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streams.py
-Version: 1.2.1
+Version: 1.3.0
 Summary: A stream library for Python inspired by Java Stream API
 Home-page: https://github.com/PickwickSoft/pystreamapi
 License: GPL-3.0-or-later
 Keywords: streams,parallel,data
 Author: Stefan Garlonta
 Author-email: stefan@pickwicksoft.org
 Requires-Python: >=3.7,<4.0
@@ -14,16 +14,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: xml-loader
+Provides-Extra: yaml-loader
 Requires-Dist: defusedxml (>=0.7,<0.8) ; extra == "xml-loader" or extra == "all"
-Requires-Dist: joblib (>=1.2,<1.4)
+Requires-Dist: joblib (>=1.2,<=1.4.2)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0) ; extra == "yaml-loader" or extra == "all"
 Project-URL: Repository, https://github.com/PickwickSoft/pystreamapi
 Description-Content-Type: text/markdown
 
 ![Header](https://raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/header.png)
 
 <h1 align="center">PyStreamAPI</h1>
 
@@ -47,15 +49,15 @@
 
 * It provides both sequential and parallel streams.
 * Lazy execution is supported, enhancing performance.
 * It boasts high speed and efficiency.
 * The implementation achieves 100% test coverage.
 * It follows Pythonic principles, resulting in clean and readable code.
 * It adds some cool innovative features such as conditions or error handling and an even more declarative look.
-* It provides loaders for various data sources such as CSV, JSON and XML files.
+* It provides loaders for various data sources such as CSV, JSON, XML and YAML files.
 
 Let's take a look at a small example:
 
 ```python
 from pystreamapi import Stream
 
 Stream.of([" ", '3', None, "2", 1, ""]) \
@@ -234,23 +236,23 @@
 ```python
 Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) 
 # Like Stream.of([1, 2, 3, 4])
 ```
 
 Creates a new Stream from multiple Streams. Order doesn't change.
 
-## Use loaders: Load data from CSV, JSON and XML files in just one line
+## Use loaders: Load data from CSV, JSON, XML and YAML files in just one line
 
-PyStreamAPI offers a convenient way to load data from CSV, JSON and XML files. Like that you can start processing your
+PyStreamAPI offers a convenient way to load data from CSV, JSON, XML and YAML files. Like that you can start processing your
 files right away without having to worry about reading and parsing the files.
 
 You can import the loaders with:
 
 ```python
-from pystreamapi.loaders import csv, json, xml
+from pystreamapi.loaders import csv, json, xml, yaml
 ```
 Now you can use the loaders directly when creating your Stream:
 
 For CSV:
 
 ```python
 Stream.of(csv("data.csv", delimiter=";")) \
@@ -274,22 +276,38 @@
 ```bash
 pip install streams.py[xml_loader]
 ```
 
 Afterward, you can use the XML loader like this:
 
 ```python
-Stream.of(xml("data.xml"))
-  .map(lambda x: x.attr1)
+Stream.of(xml("data.xml")) \
+  .map(lambda x: x.attr1) \
   .for_each(print)
 ```
 
 The access to the attributes is using a node path syntax. For more details on how to use the node path syntax, please
 refer to the [documentation](https://pystreamapi.pickwicksoft.org/reference/data-loaders).
 
+For YAML:
+
+In order to use the YAML loader, you need to install the optional yaml dependency:
+
+```bash
+pip install streams.py[yaml_loader]
+```
+
+Afterward, you can use the YAML loader like this:
+
+```python
+Stream.of(yaml("data.yaml")) \
+  .map(lambda x: x.attr1) \
+  .for_each(print)
+```
+
 ## API Reference
 For a more detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/)
 
 ## Complex Examples
 
 #### Get all numbers from list of different types. Use parallelization.
```

#### html2text {}

```diff
@@ -1,59 +1,60 @@
-Metadata-Version: 2.1 Name: streams.py Version: 1.2.1 Summary: A stream library
+Metadata-Version: 2.1 Name: streams.py Version: 1.3.0 Summary: A stream library
 for Python inspired by Java Stream API Home-page: https://github.com/
 PickwickSoft/pystreamapi License: GPL-3.0-or-later Keywords:
 streams,parallel,data Author: Stefan Garlonta Author-email:
 stefan@pickwicksoft.org Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Provides-Extra: all Provides-Extra: xml-
-loader Requires-Dist: defusedxml (>=0.7,<0.8) ; extra == "xml-loader" or extra
-== "all" Requires-Dist: joblib (>=1.2,<1.4) Project-URL: Repository, https://
-github.com/PickwickSoft/pystreamapi Description-Content-Type: text/markdown !
-[Header](https://raw.githubusercontent.com/PickwickSoft/pystreamapi/main/
-assets/header.png)
+loader Provides-Extra: yaml-loader Requires-Dist: defusedxml (>=0.7,<0.8) ;
+extra == "xml-loader" or extra == "all" Requires-Dist: joblib (>=1.2,<=1.4.2)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0) ; extra == "yaml-loader" or extra ==
+"all" Project-URL: Repository, https://github.com/PickwickSoft/pystreamapi
+Description-Content-Type: text/markdown ![Header](https://
+raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/header.png)
                            ************ PPyySSttrreeaammAAPPII ************
   _[_D_e_e_p_S_o_u_r_c_e_]_[_T_e_s_t_s_]_[_P_y_l_i_n_t_]_[_Q_u_a_l_i_t_y_ _G_a_t_e_]_[_C_o_v_e_r_a_g_e_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_P_y_P_I_]
 PyStreamAPI is a Python stream library that draws inspiration from the Java
 Stream API. Although it closely mirrors the Java API, PyStreamAPI adds some
 innovative features to make streams in Python even more innovative, declarative
 and easy to use. PyStreamAPI offers both sequential and parallel streams and
 utilizes lazy execution. Now you might be wondering why another library when
 there are already a few implementations? Well, here are a few advantages of
 this particular implementation: * It provides both sequential and parallel
 streams. * Lazy execution is supported, enhancing performance. * It boasts high
 speed and efficiency. * The implementation achieves 100% test coverage. * It
 follows Pythonic principles, resulting in clean and readable code. * It adds
 some cool innovative features such as conditions or error handling and an even
 more declarative look. * It provides loaders for various data sources such as
-CSV, JSON and XML files. Let's take a look at a small example: ```python from
-pystreamapi import Stream Stream.of([" ", '3', None, "2", 1, ""]) \ .filter
-(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter
-(lambda x: len(x) > 0) \ .map(int) \ .sorted() \ .for_each(print) # Output: 1 2
-3 ``` And here's the equivalent code in Java: ```java Object[] words = { " ",
-'3', null, "2", 1, "" }; Arrays.stream( words ) .filter( Objects::nonNull )
-.map( Objects::toString ) .map( String::trim ) .filter( s -> ! s.isEmpty() )
-.map( Integer::parseInt ) .sorted() .forEach( System.out::println ); // Output:
-1 2 3 ``` ## What is a Stream? A `Stream` is a powerful abstraction for
-processing sequences of data in a functional and declarative manner. It enables
-efficient and concise data manipulation and transformation. Similar to its
-counterparts in Java and Kotlin, a Stream represents a pipeline of operations
-that can be applied to a collection or any iterable data source. It allows
-developers to express complex data processing logic using a combination of
-high-level operations, promoting code reusability and readability. With
-Streams, you can perform a wide range of operations on your data, such as
-filtering elements, transforming values, aggregating results, sorting, and
-more. These operations can be seamlessly chained together to form a processing
-pipeline, where each operation processes the data and passes it on to the next
-operation. One of the key benefits of Stream is lazy evaluation. This means
-that the operations are executed only when the result is actually needed,
-optimizing resource usage and enabling efficient processing of large or
+CSV, JSON, XML and YAML files. Let's take a look at a small example: ```python
+from pystreamapi import Stream Stream.of([" ", '3', None, "2", 1, ""]) \
+.filter(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \
+.filter(lambda x: len(x) > 0) \ .map(int) \ .sorted() \ .for_each(print) #
+Output: 1 2 3 ``` And here's the equivalent code in Java: ```java Object[]
+words = { " ", '3', null, "2", 1, "" }; Arrays.stream( words ) .filter
+( Objects::nonNull ) .map( Objects::toString ) .map( String::trim ) .filter( s
+-> ! s.isEmpty() ) .map( Integer::parseInt ) .sorted() .forEach( System.out::
+println ); // Output: 1 2 3 ``` ## What is a Stream? A `Stream` is a powerful
+abstraction for processing sequences of data in a functional and declarative
+manner. It enables efficient and concise data manipulation and transformation.
+Similar to its counterparts in Java and Kotlin, a Stream represents a pipeline
+of operations that can be applied to a collection or any iterable data source.
+It allows developers to express complex data processing logic using a
+combination of high-level operations, promoting code reusability and
+readability. With Streams, you can perform a wide range of operations on your
+data, such as filtering elements, transforming values, aggregating results,
+sorting, and more. These operations can be seamlessly chained together to form
+a processing pipeline, where each operation processes the data and passes it on
+to the next operation. One of the key benefits of Stream is lazy evaluation.
+This means that the operations are executed only when the result is actually
+needed, optimizing resource usage and enabling efficient processing of large or
 infinite datasets. Furthermore, Stream supports both sequential and parallel
 execution. This allows you to leverage parallel processing capabilities when
 dealing with computationally intensive tasks or large amounts of data,
 significantly improving performance. `pystreamapi.Stream` represents a stream
 that facilitates the execution of one or more operations. Stream operations can
 be categorized as either intermediate or terminal. Terminal operations return a
 result of a specific type, while intermediate operations return the stream
@@ -118,31 +119,35 @@
 numeric) Stream.of_noneable(None) ``` If the source is `None`, you get an empty
 `Stream` --- ```python Stream.iterate(0, lambda n: n + 2) ``` Creates a Stream
 of an infinite Iterator created by iterative application of a function f to an
 initial element seed, producing a Stream consisting of seed, f(seed), f(f
 (seed)), etc. > **Note** > Do not forget to limit the stream with `.limit()` --
 - ```python Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) # Like
 Stream.of([1, 2, 3, 4]) ``` Creates a new Stream from multiple Streams. Order
-doesn't change. ## Use loaders: Load data from CSV, JSON and XML files in just
-one line PyStreamAPI offers a convenient way to load data from CSV, JSON and
-XML files. Like that you can start processing your files right away without
-having to worry about reading and parsing the files. You can import the loaders
-with: ```python from pystreamapi.loaders import csv, json, xml ``` Now you can
-use the loaders directly when creating your Stream: For CSV: ```python
-Stream.of(csv("data.csv", delimiter=";")) \ .map(lambda x: x.attr1) \ .for_each
-(print) ``` For JSON: ```python Stream.of(json("data.json")) \ .map(lambda x:
-x.attr1) \ .for_each(print) ``` You can access the attributes of the data
-structures directly like you would do with a normal object. For XML: In order
-to use the XML loader, you need to install the optional xml dependency: ```bash
-pip install streams.py[xml_loader] ``` Afterward, you can use the XML loader
-like this: ```python Stream.of(xml("data.xml")) .map(lambda x: x.attr1)
-.for_each(print) ``` The access to the attributes is using a node path syntax.
-For more details on how to use the node path syntax, please refer to the
-[documentation](https://pystreamapi.pickwicksoft.org/reference/data-loaders).
-## API Reference For a more detailed documentation view the docs on GitBook:
+doesn't change. ## Use loaders: Load data from CSV, JSON, XML and YAML files in
+just one line PyStreamAPI offers a convenient way to load data from CSV, JSON,
+XML and YAML files. Like that you can start processing your files right away
+without having to worry about reading and parsing the files. You can import the
+loaders with: ```python from pystreamapi.loaders import csv, json, xml, yaml
+``` Now you can use the loaders directly when creating your Stream: For CSV:
+```python Stream.of(csv("data.csv", delimiter=";")) \ .map(lambda x: x.attr1) \
+.for_each(print) ``` For JSON: ```python Stream.of(json("data.json")) \ .map
+(lambda x: x.attr1) \ .for_each(print) ``` You can access the attributes of the
+data structures directly like you would do with a normal object. For XML: In
+order to use the XML loader, you need to install the optional xml dependency:
+```bash pip install streams.py[xml_loader] ``` Afterward, you can use the XML
+loader like this: ```python Stream.of(xml("data.xml")) \ .map(lambda x:
+x.attr1) \ .for_each(print) ``` The access to the attributes is using a node
+path syntax. For more details on how to use the node path syntax, please refer
+to the [documentation](https://pystreamapi.pickwicksoft.org/reference/data-
+loaders). For YAML: In order to use the YAML loader, you need to install the
+optional yaml dependency: ```bash pip install streams.py[yaml_loader] ```
+Afterward, you can use the YAML loader like this: ```python Stream.of(yaml
+("data.yaml")) \ .map(lambda x: x.attr1) \ .for_each(print) ``` ## API
+Reference For a more detailed documentation view the docs on GitBook:
 [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/) ## Complex Examples
 #### Get all numbers from list of different types. Use parallelization.
 ```python Stream.parallel_of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x:
 x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len
 (x) > 0) \ .map(int) \ .sorted()\ .for_each(print) # 1 2 3 ``` #### Generate a
 Stream of 10 Fibonacci numbers ```python def fib(): a, b = 0, 1 while True:
 yield a a, b = b, a + b Stream.of(fib()) \ .limit(10) \ .for_each(print) # 0 1
```

