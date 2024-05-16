# Comparing `tmp/simple_archive-0.1.0.tar.gz` & `tmp/simple_archive-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_archive-0.1.0.tar", last modified: Wed May 15 12:18:31 2024, max compression
+gzip compressed data, was "simple_archive-0.2.0.tar", last modified: Thu May 16 08:21:38 2024, max compression
```

## Comparing `simple_archive-0.1.0.tar` & `simple_archive-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-03-09 07:53:34.249724 simple_archive-0.1.0/LICENSE
--rw-r--r--   0        0        0      678 2023-03-17 13:48:04.038671 simple_archive-0.1.0/README.md
--rw-r--r--   0        0        0      783 2024-05-15 12:18:31.004655 simple_archive-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      148 2024-05-15 09:27:14.920671 simple_archive-0.1.0/simple_archive/__init__.py
--rw-r--r--   0        0        0      598 2024-05-15 10:51:30.260991 simple_archive-0.1.0/simple_archive/cli.py
--rw-r--r--   0        0        0     6683 2024-05-15 10:53:32.174332 simple_archive-0.1.0/simple_archive/simple_archive.py
--rw-r--r--   0        0        0     2594 2024-05-15 11:00:48.011027 simple_archive-0.1.0/simple_archive/use_cases.py
--rw-r--r--   0        0        0    14693 2024-05-15 11:08:00.877721 simple_archive-0.1.0/tests/requirements-testing.lock
--rw-r--r--   0        0        0      121 2024-05-15 09:22:48.450654 simple_archive-0.1.0/tests/test_dublin_core.py
--rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 simple_archive-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-16 08:21:22.545306 simple_archive-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2292 2024-05-16 08:21:22.545306 simple_archive-0.2.0/README.md
+-rw-r--r--   0        0        0      769 2024-05-16 08:21:38.345406 simple_archive-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      148 2024-05-16 08:21:22.545306 simple_archive-0.2.0/simple_archive/__init__.py
+-rw-r--r--   0        0        0      598 2024-05-16 08:21:22.545306 simple_archive-0.2.0/simple_archive/cli.py
+-rw-r--r--   0        0        0     6968 2024-05-16 08:21:22.545306 simple_archive-0.2.0/simple_archive/simple_archive.py
+-rw-r--r--   0        0        0     2594 2024-05-16 08:21:22.545306 simple_archive-0.2.0/simple_archive/use_cases.py
+-rw-r--r--   0        0        0    18267 2024-05-16 08:21:22.545306 simple_archive-0.2.0/tests/requirements-testing.lock
+-rw-r--r--   0        0        0      121 2024-05-16 08:21:22.545306 simple_archive-0.2.0/tests/test_dublin_core.py
+-rw-r--r--   0        0        0      362 2024-05-16 08:21:22.545306 simple_archive-0.2.0/tests/test_simple_archive.py
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 simple_archive-0.2.0/PKG-INFO
```

### Comparing `simple_archive-0.1.0/LICENSE` & `simple_archive-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_archive-0.1.0/pyproject.toml` & `simple_archive-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "simple-archive"
-version = "0.1.0"
+version = "0.2.0"
 description = "CLI and library for working with Simple Archive Format"
 authors = [
     { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 readme = "README.md"
-requires-python = ">=3.8.1"
+requires-python = ">=3.9"
 dependencies = [
     "typer<1.0.0,>=0.7.0",
-    "pydantic<2.0.0,>=1.10.6",
+    "pydantic>=2",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 safar = "simple_archive.cli:app"
```

### Comparing `simple_archive-0.1.0/simple_archive/cli.py` & `simple_archive-0.2.0/simple_archive/cli.py`

 * *Files identical despite different names*

### Comparing `simple_archive-0.1.0/simple_archive/simple_archive.py` & `simple_archive-0.2.0/simple_archive/simple_archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Model for Simple Archive."""
 
 import csv
 import logging
 import shutil
 from datetime import date
 from pathlib import Path
-from typing import List, Optional
+from typing import Any, Optional
 from xml.etree.ElementTree import Element, ElementTree, SubElement
 from zipfile import ZIP_DEFLATED, ZipFile
 
 import pydantic
 
 DEFAULT_ENCODING = "utf-8"
 
@@ -31,15 +31,15 @@
     qualifier: Optional[str] = None
     language: Optional[str] = None
 
 
 class DublinCore(pydantic.BaseModel):
     """Dublin Core model."""
 
-    elements: List[DublinCoreElement]
+    elements: list[DublinCoreElement]
 
 
 def build_xml(dc: DublinCore) -> ElementTree:
     """Build an ElementTree from a DublinCore model.
 
     Args:
         dc (DublinCore): the model to build from
@@ -89,36 +89,41 @@
         elem.text = text
     return elem
 
 
 class Item(pydantic.BaseModel):
     """Simple Archive Item model."""
 
-    files: List[Path]
+    files: list[Path]
     dc: DublinCore
 
-    @pydantic.validator("files", pre=True)
+    @pydantic.field_validator("files", mode="before")
     @classmethod
-    def split_str(cls, v):  # noqa: ANN206, D102, ANN001
+    def split_str(cls, v: Any) -> Any:  # noqa: D102
         return v.split("||") if isinstance(v, str) else v
 
-    @pydantic.root_validator(pre=True)
+    @pydantic.model_validator(mode="before")
     @classmethod
-    def collect_dc_fields(cls, values):  # noqa: ANN206, D102, ANN001
-        new_values = {}
+    def collect_dc_fields(cls, values: Any) -> dict:  # noqa: D102
+        new_values: dict[str, dict[str, list[dict[str, str]]]] = {}
         for field, value in values.items():
             if field.startswith("dc."):
                 if "dc" not in new_values:
                     new_values["dc"] = {}
                 if "elements" not in new_values["dc"]:
                     new_values["dc"]["elements"] = []
-                subfields = field.split(".")
+                subfields: list[str] = field.split(".")
                 element = {"value": value}
                 for sub_field, key in zip(
-                    subfields[1:], ("element", "qualifier", "language"), strict=False
+                    subfields[1:],
+                    (
+                        "element",
+                        "qualifier",
+                        "language",
+                    ),  # strict=False TODO: use this when Python 3.9 is dropped, see https://github.com/spraakbanken/simple-archive/issuse/5
                 ):
                     element[key] = sub_field  # noqa: PERF403
                 new_values["dc"]["elements"].append(element)
                 # new_values["dc"][field[3:]] = value
             else:
                 new_values[field] = value
         return new_values
```

### Comparing `simple_archive-0.1.0/simple_archive/use_cases.py` & `simple_archive-0.2.0/simple_archive/use_cases.py`

 * *Files identical despite different names*

### Comparing `simple_archive-0.1.0/tests/requirements-testing.lock` & `simple_archive-0.2.0/tests/requirements-testing.lock`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 # This file is @generated by PDM.
 # Please do not edit it manually.
 
-bump-my-version==0.10.0 \
-    --hash=sha256:a18d5442c8eca1b26e07ae4b76de545b9737c09deed32d043b11ec3f93842af7 \
-    --hash=sha256:f696d25ba652077b6f0e5755f775aa05425f425ce91ca2ef1c7e6f3d989fabd2
+annotated-types==0.6.0 \
+    --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
+    --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
+bracex==2.4 \
+    --hash=sha256:a27eaf1df42cf561fed58b7a8f3fdf129d1ea16a81e1fadd1d17989bc6384beb \
+    --hash=sha256:efdc71eff95eaff5e0f8cfebe7d01adf2c8637c8c92edaf63ef348c241a82418
+bump-my-version==0.21.0 \
+    --hash=sha256:a614d8176b5ac0e644239c9a8a246b696d316f68406fd78b8486a9e13fc93266 \
+    --hash=sha256:c3f1a31e32345679b517cbba99a0875457ee45d7ba6189fcd2a74d3ddae41515
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 colorama==0.4.6; sys_platform == "win32" or platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 coverage==7.5.1 \
-    --hash=sha256:0646599e9b139988b63704d704af8e8df7fa4cbc4a1f33df69d97f36cb0a38de \
-    --hash=sha256:0cdcbc320b14c3e5877ee79e649677cb7d89ef588852e9583e6b24c2e5072661 \
     --hash=sha256:0d0a0f5e06881ecedfe6f3dd2f56dcb057b6dbeb3327fd32d4b12854df36bf26 \
-    --hash=sha256:1434e088b41594baa71188a17533083eabf5609e8e72f16ce8c186001e6b8c41 \
     --hash=sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d \
     --hash=sha256:1cc0fe9b0b3a8364093c53b0b4c0c2dd4bb23acbec4c9240b5f284095ccf7981 \
     --hash=sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2 \
     --hash=sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34 \
     --hash=sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f \
     --hash=sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a \
     --hash=sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35 \
     --hash=sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223 \
     --hash=sha256:4cc37def103a2725bc672f84bd939a6fe4522310503207aae4d56351644682f1 \
     --hash=sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746 \
-    --hash=sha256:5037f8fcc2a95b1f0e80585bd9d1ec31068a9bcb157d9750a172836e98bc7a90 \
     --hash=sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c \
     --hash=sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca \
-    --hash=sha256:57e0204b5b745594e5bc14b9b50006da722827f0b8c776949f1135677e88d0b8 \
     --hash=sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596 \
-    --hash=sha256:5c3721c2c9e4c4953a41a26c14f4cef64330392a6d2d675c8b1db3b645e31f0e \
     --hash=sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd \
     --hash=sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e \
     --hash=sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3 \
     --hash=sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e \
     --hash=sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312 \
     --hash=sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7 \
     --hash=sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572 \
     --hash=sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428 \
     --hash=sha256:79afb6197e2f7f60c4824dd4b2d4c2ec5801ceb6ba9ce5d2c3080e5660d51a4f \
     --hash=sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07 \
     --hash=sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e \
-    --hash=sha256:8fe7502616b67b234482c3ce276ff26f39ffe88adca2acf0261df4b8454668b4 \
     --hash=sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136 \
     --hash=sha256:9735317685ba6ec7e3754798c8871c2f49aa5e687cc794a0b1d284b2389d1bd5 \
     --hash=sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8 \
-    --hash=sha256:9e78295f4144f9dacfed4f92935fbe1780021247c2fabf73a819b17f0ccfff8d \
     --hash=sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228 \
     --hash=sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206 \
     --hash=sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa \
     --hash=sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e \
     --hash=sha256:c3e757949f268364b96ca894b4c342b41dc6f8f8b66c37878aacef5930db61be \
-    --hash=sha256:ca498687ca46a62ae590253fba634a1fe9836bc56f626852fb2720f334c9e4e5 \
     --hash=sha256:d1d0d98d95dd18fe29dc66808e1accf59f037d5716f86a501fc0256455219668 \
     --hash=sha256:d21918e9ef11edf36764b93101e2ae8cc82aa5efdc7c5a4e9c6c35a48496d601 \
     --hash=sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057 \
     --hash=sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146 \
     --hash=sha256:dde0070c40ea8bb3641e811c1cfbf18e265d024deff6de52c5950677a8fb1e0f \
     --hash=sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8 \
-    --hash=sha256:e2213def81a50519d7cc56ed643c9e93e0247f5bbe0d1247d15fa520814a7cd7 \
     --hash=sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987 \
     --hash=sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19 \
     --hash=sha256:fc0b4d8bfeabd25ea75e94632f5b6e047eef8adaed0c2161ada1e922e7f7cece
 exceptiongroup==1.2.1; python_version < "3.11" \
     --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
     --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
 iniconfig==2.0.0 \
@@ -72,90 +68,137 @@
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
     --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
 mypy==1.10.0 \
-    --hash=sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061 \
     --hash=sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99 \
     --hash=sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de \
     --hash=sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a \
     --hash=sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9 \
     --hash=sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec \
     --hash=sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1 \
     --hash=sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131 \
-    --hash=sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f \
     --hash=sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821 \
     --hash=sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5 \
     --hash=sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee \
     --hash=sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e \
     --hash=sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746 \
     --hash=sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2 \
-    --hash=sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0 \
     --hash=sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b \
     --hash=sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53 \
     --hash=sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30 \
     --hash=sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda \
     --hash=sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051 \
     --hash=sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2 \
     --hash=sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7 \
     --hash=sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee \
-    --hash=sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727 \
-    --hash=sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976 \
-    --hash=sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4
+    --hash=sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
 packaging==24.0 \
     --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
     --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
 pluggy==1.5.0 \
     --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
     --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
-pydantic==1.10.15 \
-    --hash=sha256:0d142fa1b8f2f0ae11ddd5e3e317dcac060b951d605fda26ca9b234b92214986 \
-    --hash=sha256:22ed12ee588b1df028a2aa5d66f07bf8f8b4c8579c2e96d5a9c1f96b77f3bb55 \
-    --hash=sha256:2746189100c646682eff0bce95efa7d2e203420d8e1c613dc0c6b4c1d9c1fde4 \
-    --hash=sha256:28e552a060ba2740d0d2aabe35162652c1459a0b9069fe0db7f4ee0e18e74d58 \
-    --hash=sha256:3287e1614393119c67bd4404f46e33ae3be3ed4cd10360b48d0a4459f420c6a3 \
-    --hash=sha256:3350f527bb04138f8aff932dc828f154847fbdc7a1a44c240fbfff1b57f49a12 \
-    --hash=sha256:394f08750bd8eaad714718812e7fab615f873b3cdd0b9d84e76e51ef3b50b6b7 \
-    --hash=sha256:4e316e54b5775d1eb59187f9290aeb38acf620e10f7fd2f776d97bb788199e53 \
-    --hash=sha256:50f1666a9940d3d68683c9d96e39640f709d7a72ff8702987dab1761036206bb \
-    --hash=sha256:51d405b42f1b86703555797270e4970a9f9bd7953f3990142e69d1037f9d9e51 \
-    --hash=sha256:584f2d4c98ffec420e02305cf675857bae03c9d617fcfdc34946b1160213a948 \
-    --hash=sha256:5e09c19df304b8123938dc3c53d3d3be6ec74b9d7d0d80f4f4b5432ae16c2022 \
-    --hash=sha256:676ed48f2c5bbad835f1a8ed8a6d44c1cd5a21121116d2ac40bd1cd3619746ed \
-    --hash=sha256:67f1a1fb467d3f49e1708a3f632b11c69fccb4e748a325d5a491ddc7b5d22383 \
-    --hash=sha256:6a51a1dd4aa7b3f1317f65493a182d3cff708385327c1c82c81e4a9d6d65b2e4 \
-    --hash=sha256:6bd7030c9abc80134087d8b6e7aa957e43d35714daa116aced57269a445b8f7b \
-    --hash=sha256:75279d3cac98186b6ebc2597b06bcbc7244744f6b0b44a23e4ef01e5683cc0d2 \
-    --hash=sha256:7ac9237cd62947db00a0d16acf2f3e00d1ae9d3bd602b9c415f93e7a9fc10528 \
-    --hash=sha256:82790d4753ee5d00739d6cb5cf56bceb186d9d6ce134aca3ba7befb1eedbc2c8 \
-    --hash=sha256:92229f73400b80c13afcd050687f4d7e88de9234d74b27e6728aa689abcf58cc \
-    --hash=sha256:a980a77c52723b0dc56640ced396b73a024d4b74f02bcb2d21dbbac1debbe9d0 \
-    --hash=sha256:bbc6989fad0c030bd70a0b6f626f98a862224bc2b1e36bfc531ea2facc0a340c \
-    --hash=sha256:be51dd2c8596b25fe43c0a4a59c2bee4f18d88efb8031188f9e7ddc6b469cf44 \
-    --hash=sha256:c365ad9c394f9eeffcb30a82f4246c0006417f03a7c0f8315d6211f25f7cb654 \
-    --hash=sha256:c3d5731a120752248844676bf92f25a12f6e45425e63ce22e0849297a093b5b0 \
-    --hash=sha256:ca832e124eda231a60a041da4f013e3ff24949d94a01154b137fc2f2a43c3ffb \
-    --hash=sha256:d207d5b87f6cbefbdb1198154292faee8017d7495a54ae58db06762004500d00 \
-    --hash=sha256:d3b5c4cbd0c9cb61bbbb19ce335e1f8ab87a811f6d589ed52b0254cf585d709c \
-    --hash=sha256:d573082c6ef99336f2cb5b667b781d2f776d4af311574fb53d908517ba523c22 \
-    --hash=sha256:e49db944fad339b2ccb80128ffd3f8af076f9f287197a480bf1e4ca053a866f0
+prompt-toolkit==3.0.36 \
+    --hash=sha256:3e163f254bef5a03b146397d7c1963bd3e2812f0964bb9a24e6ec761fd28db63 \
+    --hash=sha256:aa64ad242a462c5ff0363a7b9cfe696c20d55d9fc60c11fd8e632d064804d305
+pydantic==2.7.1 \
+    --hash=sha256:e029badca45266732a9a79898a15ae2e8b14840b1eabbb25844be28f0b33f3d5 \
+    --hash=sha256:e9dbb5eada8abe4d9ae5f46b9939aead650cd2b68f249bb3a8139dbe125803cc
+pydantic-core==2.18.2 \
+    --hash=sha256:0098300eebb1c837271d3d1a2cd2911e7c11b396eac9661655ee524a7f10587b \
+    --hash=sha256:042473b6280246b1dbf530559246f6842b56119c2926d1e52b631bdc46075f2a \
+    --hash=sha256:05b7133a6e6aeb8df37d6f413f7705a37ab4031597f64ab56384c94d98fa0e90 \
+    --hash=sha256:0680b1f1f11fda801397de52c36ce38ef1c1dc841a0927a94f226dea29c3ae3d \
+    --hash=sha256:0d69b4c2f6bb3e130dba60d34c0845ba31b69babdd3f78f7c0c8fae5021a253e \
+    --hash=sha256:1404c69d6a676245199767ba4f633cce5f4ad4181f9d0ccb0577e1f66cf4c46d \
+    --hash=sha256:182245ff6b0039e82b6bb585ed55a64d7c81c560715d1bad0cbad6dfa07b4027 \
+    --hash=sha256:1a388a77e629b9ec814c1b1e6b3b595fe521d2cdc625fcca26fbc2d44c816804 \
+    --hash=sha256:20aca1e2298c56ececfd8ed159ae4dde2df0781988c97ef77d5c16ff4bd5b400 \
+    --hash=sha256:219da3f096d50a157f33645a1cf31c0ad1fe829a92181dd1311022f986e5fbe3 \
+    --hash=sha256:22057013c8c1e272eb8d0eebc796701167d8377441ec894a8fed1af64a0bf399 \
+    --hash=sha256:223ee893d77a310a0391dca6df00f70bbc2f36a71a895cecd9a0e762dc37b349 \
+    --hash=sha256:224c421235f6102e8737032483f43c1a8cfb1d2f45740c44166219599358c2cd \
+    --hash=sha256:2334ce8c673ee93a1d6a65bd90327588387ba073c17e61bf19b4fd97d688d63c \
+    --hash=sha256:269322dcc3d8bdb69f054681edff86276b2ff972447863cf34c8b860f5188e2e \
+    --hash=sha256:2728b01246a3bba6de144f9e3115b532ee44bd6cf39795194fb75491824a1413 \
+    --hash=sha256:2b8ed04b3582771764538f7ee7001b02e1170223cf9b75dff0bc698fadb00cf3 \
+    --hash=sha256:2e29d20810dfc3043ee13ac7d9e25105799817683348823f305ab3f349b9386e \
+    --hash=sha256:36789b70d613fbac0a25bb07ab3d9dba4d2e38af609c020cf4d888d165ee0bf3 \
+    --hash=sha256:3a6515ebc6e69d85502b4951d89131ca4e036078ea35533bb76327f8424531ce \
+    --hash=sha256:3f9a801e7c8f1ef8718da265bba008fa121243dfe37c1cea17840b0944dfd72c \
+    --hash=sha256:43f0f463cf89ace478de71a318b1b4f05ebc456a9b9300d027b4b57c1a2064fb \
+    --hash=sha256:4456f2dca97c425231d7315737d45239b2b51a50dc2b6f0c2bb181fce6207664 \
+    --hash=sha256:470b94480bb5ee929f5acba6995251ada5e059a5ef3e0dfc63cca287283ebfa6 \
+    --hash=sha256:4b4356d3538c3649337df4074e81b85f0616b79731fe22dd11b99499b2ebbdf3 \
+    --hash=sha256:553ef617b6836fc7e4df130bb851e32fe357ce36336d897fd6646d6058d980af \
+    --hash=sha256:6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043 \
+    --hash=sha256:6e5c584d357c4e2baf0ff7baf44f4994be121e16a2c88918a5817331fc7599d7 \
+    --hash=sha256:75250dbc5290e3f1a0f4618db35e51a165186f9034eff158f3d490b3fed9f8a0 \
+    --hash=sha256:75f7e9488238e920ab6204399ded280dc4c307d034f3924cd7f90a38b1829563 \
+    --hash=sha256:7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72 \
+    --hash=sha256:800d60565aec896f25bc3cfa56d2277d52d5182af08162f7954f938c06dc4ee3 \
+    --hash=sha256:886eec03591b7cf058467a70a87733b35f44707bd86cf64a615584fd72488b7c \
+    --hash=sha256:8b172601454f2d7701121bbec3425dd71efcb787a027edf49724c9cefc14c038 \
+    --hash=sha256:95b9d5e72481d3780ba3442eac863eae92ae43a5f3adb5b4d0a1de89d42bb250 \
+    --hash=sha256:98758d627ff397e752bc339272c14c98199c613f922d4a384ddc07526c86a2ec \
+    --hash=sha256:997abc4df705d1295a42f95b4eec4950a37ad8ae46d913caeee117b6b198811c \
+    --hash=sha256:9b5155ff768083cb1d62f3e143b49a8a3432e6789a3abee8acd005c3c7af1c74 \
+    --hash=sha256:9e08e867b306f525802df7cd16c44ff5ebbe747ff0ca6cf3fde7f36c05a59a81 \
+    --hash=sha256:a1874c6dd4113308bd0eb568418e6114b252afe44319ead2b4081e9b9521fe75 \
+    --hash=sha256:a8309f67285bdfe65c372ea3722b7a5642680f3dba538566340a9d36e920b5f0 \
+    --hash=sha256:ae0a8a797a5e56c053610fa7be147993fe50960fa43609ff2a9552b0e07013e8 \
+    --hash=sha256:b14d82cdb934e99dda6d9d60dc84a24379820176cc4a0d123f88df319ae9c150 \
+    --hash=sha256:b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438 \
+    --hash=sha256:b3ef08e20ec49e02d5c6717a91bb5af9b20f1805583cb0adfe9ba2c6b505b5ae \
+    --hash=sha256:b89ed9eb7d616ef5714e5590e6cf7f23b02d0d539767d33561e3675d6f9e3857 \
+    --hash=sha256:c4fcf5cd9c4b655ad666ca332b9a081112cd7a58a8b5a6ca7a3104bc950f2038 \
+    --hash=sha256:c6fdc8627910eed0c01aed6a390a252fe3ea6d472ee70fdde56273f198938374 \
+    --hash=sha256:c9bd70772c720142be1020eac55f8143a34ec9f82d75a8e7a07852023e46617f \
+    --hash=sha256:ca7b0c1f1c983e064caa85f3792dd2fe3526b3505378874afa84baf662e12241 \
+    --hash=sha256:cbca948f2d14b09d20268cda7b0367723d79063f26c4ffc523af9042cad95592 \
+    --hash=sha256:cc1cfd88a64e012b74e94cd00bbe0f9c6df57049c97f02bb07d39e9c852e19a4 \
+    --hash=sha256:ccdd111c03bfd3666bd2472b674c6899550e09e9f298954cfc896ab92b5b0e6d \
+    --hash=sha256:cfeecd1ac6cc1fb2692c3d5110781c965aabd4ec5d32799773ca7b1456ac636b \
+    --hash=sha256:d7d904828195733c183d20a54230c0df0eb46ec746ea1a666730787353e87182 \
+    --hash=sha256:d9319e499827271b09b4e411905b24a426b8fb69464dfa1696258f53a3334641 \
+    --hash=sha256:e18609ceaa6eed63753037fc06ebb16041d17d28199ae5aba0052c51449650a9 \
+    --hash=sha256:e1b395e58b10b73b07b7cf740d728dd4ff9365ac46c18751bf8b3d8cca8f625a \
+    --hash=sha256:e23ec367a948b6d812301afc1b13f8094ab7b2c280af66ef450efc357d2ae543 \
+    --hash=sha256:e25add29b8f3b233ae90ccef2d902d0ae0432eb0d45370fe315d1a5cf231004b \
+    --hash=sha256:e6dac87ddb34aaec85f873d737e9d06a3555a1cc1a8e0c44b7f8d5daeb89d86f \
+    --hash=sha256:ef26c9e94a8c04a1b2924149a9cb081836913818e55681722d7f29af88fe7b38 \
+    --hash=sha256:eff2de745698eb46eeb51193a9f41d67d834d50e424aef27df2fcdee1b153845 \
+    --hash=sha256:f0a21cbaa69900cbe1a2e7cad2aa74ac3cf21b10c3efb0fa0b80305274c0e8a2 \
+    --hash=sha256:f459a5ce8434614dfd39bbebf1041952ae01da6bed9855008cb33b875cb024c0 \
+    --hash=sha256:f93a8a2e3938ff656a7c1bc57193b1319960ac015b6e87d76c76bf14fe0244b4 \
+    --hash=sha256:fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
+pydantic-settings==2.2.1 \
+    --hash=sha256:00b9f6a5e95553590434c0fa01ead0b216c3e10bc54ae02e37f359948643c5ed \
+    --hash=sha256:0235391d26db4d2190cb9b31051c4b46882d28a51533f97440867f012d4da091
 pygments==2.18.0 \
     --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
     --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
 pytest==8.2.0 \
     --hash=sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233 \
     --hash=sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f
 pytest-cov==5.0.0 \
     --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
     --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
+python-dotenv==1.0.1 \
+    --hash=sha256:e324ee90a023d808f1959c46bcbc04446a10ced277783dc6ee09987c37ec10ca \
+    --hash=sha256:f7b63ef50f1b690dddf550d03497b66d609393b40b564ed0d674909a68ebf16a
+questionary==2.0.1 \
+    --hash=sha256:8ab9a01d0b91b68444dff7f6652c1e754105533f083cbe27597c8110ecc230a2 \
+    --hash=sha256:bcce898bf3dbb446ff62830c86c5c6fb9a22a54146f0f5597d3da43b10d8fc8b
 rich==13.7.1 \
     --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
     --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
 rich-click==1.8.2 \
     --hash=sha256:8e29bdede858b59aa2859a1ab1c4ccbd39ed7ed5870262dae756fba6b5dc72e8 \
     --hash=sha256:b57856f304e4fe0394b82d7ce0784450758f8c8b4e201ccc4320501cc201806b
 ruff==0.4.4 \
@@ -187,7 +230,13 @@
     --hash=sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c
 typer==0.12.3 \
     --hash=sha256:070d7ca53f785acbccba8e7d28b08dcd88f79f1fbda035ade0aecec71ca5c914 \
     --hash=sha256:49e73131481d804288ef62598d97a1ceef3058905aa536a1134f90891ba35482
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+wcmatch==8.5.2 \
+    --hash=sha256:17d3ad3758f9d0b5b4dedc770b65420d4dac62e680229c287bf24c9db856a478 \
+    --hash=sha256:a70222b86dea82fb382dd87b73278c10756c138bd6f8f714e2183128887b9eb2
+wcwidth==0.2.13 \
+    --hash=sha256:3da69048e4540d84af32131829ff948f1e022c1c6bdb8d6102117aac784f6859 \
+    --hash=sha256:72ea0c06399eb286d978fdedb6923a9eb47e1c486ce63e9b4e64fc18303972b5
```

