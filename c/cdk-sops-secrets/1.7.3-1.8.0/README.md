# Comparing `tmp/cdk-sops-secrets-1.7.3.tar.gz` & `tmp/cdk-sops-secrets-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.7.3.tar", last modified: Fri May  3 06:08:24 2024, max compression
+gzip compressed data, was "cdk-sops-secrets-1.8.0.tar", last modified: Thu May 16 13:57:35 2024, max compression
```

## Comparing `cdk-sops-secrets-1.7.3.tar` & `cdk-sops-secrets-1.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:08:24.516737 cdk-sops-secrets-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-03 06:08:24.516737 cdk-sops-secrets-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:08:24.516737 cdk-sops-secrets-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:08:24.504737 cdk-sops-secrets-1.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:08:24.504737 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)    76606 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:08:24.504737 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  8963935 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.7.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:08:14.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:08:24.504737 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-03 06:08:24.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-03 06:08:24.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:08:24.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-03 06:08:24.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 06:08:24.000000 cdk-sops-secrets-1.7.3/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:35.228165 cdk-sops-secrets-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-05-16 13:57:35.228165 cdk-sops-secrets-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:57:35.228165 cdk-sops-secrets-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:35.216165 cdk-sops-secrets-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:35.216165 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    84982 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:35.220165 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  8966558 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.8.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:57:25.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:35.220165 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-05-16 13:57:35.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-16 13:57:35.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:57:35.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 13:57:35.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 13:57:35.000000 cdk-sops-secrets-1.8.0/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.7.3/LICENSE` & `cdk-sops-secrets-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.7.3/PKG-INFO` & `cdk-sops-secrets-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.7.3
+Version: 1.8.0
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -189,14 +189,47 @@
 {
   "context": {
     "sops_sync_provider_asset_path": "some/path/asset.zip"
   }
 }
 ```
 
+### I want to upload the sops file myself and only want to reference it
+
+That's possible since version 1.8.0. You can reference the file in S3 like:
+
+```python
+new SopsSecret(stack, 'SopsSecret', {
+  sopsS3Bucket: 'testbucket',
+  sopsS3Key: 'secret.json',
+  sopsFileFormat: 'json',
+  // ...
+});
+```
+
+Passing those values as CloudFormation parameters should also be possible:
+
+```python
+
+const sopsS3BucketParam = new CfnParameter(this, "s3BucketName", {
+  type: "String",
+  description: "The name of the Amazon S3 bucket where your sopsFile was uploaded."});
+
+const sopsS3KeyParam = new CfnParameter(this, "s3KeyName", {
+  type: "String",
+  description: "The name of the key of the sopsFile inside the Amazon S3 bucket."});
+
+new SopsSecret(stack, 'SopsSecret', {
+  sopsS3Bucket: sopsS3BucketParam.valueAsString,
+  sopsS3Key: sopsS3KeyParam.valueAsString,
+  sopsFileFormat: 'json',
+  // ...
+});
+```
+
 ## Motivation
 
 I have created this project to solve a recurring problem of syncing Mozilla/sops secrets into AWS SecretsManager in a convenient, secure way.
 
 Other than that, or perhaps more importantly, my goal was to learn new things:
 
 * Write a Golang lambda
```

### Comparing `cdk-sops-secrets-1.7.3/README.md` & `cdk-sops-secrets-1.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -166,14 +166,47 @@
 {
   "context": {
     "sops_sync_provider_asset_path": "some/path/asset.zip"
   }
 }
 ```
 
+### I want to upload the sops file myself and only want to reference it
+
+That's possible since version 1.8.0. You can reference the file in S3 like:
+
+```python
+new SopsSecret(stack, 'SopsSecret', {
+  sopsS3Bucket: 'testbucket',
+  sopsS3Key: 'secret.json',
+  sopsFileFormat: 'json',
+  // ...
+});
+```
+
+Passing those values as CloudFormation parameters should also be possible:
+
+```python
+
+const sopsS3BucketParam = new CfnParameter(this, "s3BucketName", {
+  type: "String",
+  description: "The name of the Amazon S3 bucket where your sopsFile was uploaded."});
+
+const sopsS3KeyParam = new CfnParameter(this, "s3KeyName", {
+  type: "String",
+  description: "The name of the key of the sopsFile inside the Amazon S3 bucket."});
+
+new SopsSecret(stack, 'SopsSecret', {
+  sopsS3Bucket: sopsS3BucketParam.valueAsString,
+  sopsS3Key: sopsS3KeyParam.valueAsString,
+  sopsFileFormat: 'json',
+  // ...
+});
+```
+
 ## Motivation
 
 I have created this project to solve a recurring problem of syncing Mozilla/sops secrets into AWS SecretsManager in a convenient, secure way.
 
 Other than that, or perhaps more importantly, my goal was to learn new things:
 
 * Write a Golang lambda
```

### Comparing `cdk-sops-secrets-1.7.3/setup.py` & `cdk-sops-secrets-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.7.3",
+    "version": "1.8.0",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<markus.siebert@deutschebahn.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.7.3.jsii.tgz"
+            "cdk-sops-secrets@1.8.0.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-sops-secrets-1.7.3/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.8.0/src/cdk_sops_secrets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,14 +167,47 @@
 {
   "context": {
     "sops_sync_provider_asset_path": "some/path/asset.zip"
   }
 }
 ```
 
+### I want to upload the sops file myself and only want to reference it
+
+That's possible since version 1.8.0. You can reference the file in S3 like:
+
+```python
+new SopsSecret(stack, 'SopsSecret', {
+  sopsS3Bucket: 'testbucket',
+  sopsS3Key: 'secret.json',
+  sopsFileFormat: 'json',
+  // ...
+});
+```
+
+Passing those values as CloudFormation parameters should also be possible:
+
+```python
+
+const sopsS3BucketParam = new CfnParameter(this, "s3BucketName", {
+  type: "String",
+  description: "The name of the Amazon S3 bucket where your sopsFile was uploaded."});
+
+const sopsS3KeyParam = new CfnParameter(this, "s3KeyName", {
+  type: "String",
+  description: "The name of the key of the sopsFile inside the Amazon S3 bucket."});
+
+new SopsSecret(stack, 'SopsSecret', {
+  sopsS3Bucket: sopsS3BucketParam.valueAsString,
+  sopsS3Key: sopsS3KeyParam.valueAsString,
+  sopsFileFormat: 'json',
+  // ...
+});
+```
+
 ## Motivation
 
 I have created this project to solve a recurring problem of syncing Mozilla/sops secrets into AWS SecretsManager in a convenient, secure way.
 
 Other than that, or perhaps more importantly, my goal was to learn new things:
 
 * Write a Golang lambda
@@ -240,40 +273,44 @@
         *,
         description: typing.Optional[builtins.str] = None,
         encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
         generate_secret_string: typing.Optional[typing.Union[_aws_cdk_aws_secretsmanager_ceddda9d.SecretStringGenerator, typing.Dict[builtins.str, typing.Any]]] = None,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
         replica_regions: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_secretsmanager_ceddda9d.ReplicaRegion, typing.Dict[builtins.str, typing.Any]]]] = None,
         secret_name: typing.Optional[builtins.str] = None,
-        sops_file_path: builtins.str,
         convert_to_json: typing.Optional[builtins.bool] = None,
         flatten: typing.Optional[builtins.bool] = None,
         sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
         sops_file_format: typing.Optional[builtins.str] = None,
+        sops_file_path: typing.Optional[builtins.str] = None,
         sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
         sops_provider: typing.Optional["SopsSyncProvider"] = None,
+        sops_s3_bucket: typing.Optional[builtins.str] = None,
+        sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional["UploadType"] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param description: An optional, human-friendly description of the secret. Default: - No description.
         :param encryption_key: The customer-managed encryption key to use for encrypting the secret value. Default: - A default KMS key for the account and region is used.
         :param generate_secret_string: Configuration for how to generate a secret value. Default: - 32 characters with upper-case letters, lower-case letters, punctuation and numbers (at least one from each category), per the default values of ``SecretStringGenerator``.
         :param removal_policy: Policy to apply when the secret is removed from this stack. Default: - Not set.
         :param replica_regions: A list of regions where to replicate this secret. Default: - Secret is not replicated
         :param secret_name: A name for the secret. Note that deleting secrets from SecretsManager does not happen immediately, but after a 7 to 30 days blackout period. During that period, it is not possible to create another secret that shares the same name. Default: - A name is generated by CloudFormation.
-        :param sops_file_path: (experimental) The filepath to the sops file.
         :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
         :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
         :param sops_age_key: (experimental) The age key that should be used for encryption.
         :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: (experimental) The filepath to the sops file.
         :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
         :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
         :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
         :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__641b47276285e7c457eb639fea01f8b2e2f54dd58d3bc6f9e184404914516a11)
@@ -282,21 +319,23 @@
         props = SopsSecretProps(
             description=description,
             encryption_key=encryption_key,
             generate_secret_string=generate_secret_string,
             removal_policy=removal_policy,
             replica_regions=replica_regions,
             secret_name=secret_name,
-            sops_file_path=sops_file_path,
             convert_to_json=convert_to_json,
             flatten=flatten,
             sops_age_key=sops_age_key,
             sops_file_format=sops_file_format,
+            sops_file_path=sops_file_path,
             sops_kms_key=sops_kms_key,
             sops_provider=sops_provider,
+            sops_s3_bucket=sops_s3_bucket,
+            sops_s3_key=sops_s3_key,
             stringify_values=stringify_values,
             upload_type=upload_type,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="addRotationSchedule")
@@ -554,53 +593,59 @@
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
-        sops_file_path: builtins.str,
         convert_to_json: typing.Optional[builtins.bool] = None,
         flatten: typing.Optional[builtins.bool] = None,
         sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
         sops_file_format: typing.Optional[builtins.str] = None,
+        sops_file_path: typing.Optional[builtins.str] = None,
         sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
         sops_provider: typing.Optional["SopsSyncProvider"] = None,
+        sops_s3_bucket: typing.Optional[builtins.str] = None,
+        sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional["UploadType"] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param secret: (experimental) The secret that will be populated with the encrypted sops file content.
-        :param sops_file_path: (experimental) The filepath to the sops file.
         :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
         :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
         :param sops_age_key: (experimental) The age key that should be used for encryption.
         :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: (experimental) The filepath to the sops file.
         :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
         :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
         :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
         :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6b3134de7215a676a4feb3291975d227477d2dc9d5914405b8ab165ac30d7bad)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = SopsSyncProps(
             secret=secret,
-            sops_file_path=sops_file_path,
             convert_to_json=convert_to_json,
             flatten=flatten,
             sops_age_key=sops_age_key,
             sops_file_format=sops_file_format,
+            sops_file_path=sops_file_path,
             sops_kms_key=sops_kms_key,
             sops_provider=sops_provider,
+            sops_s3_bucket=sops_s3_bucket,
+            sops_s3_key=sops_s3_key,
             stringify_values=stringify_values,
             upload_type=upload_type,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
@@ -618,23 +663,14 @@
         '''(experimental) Was the structure flattened?
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "flatten"))
 
     @builtins.property
-    @jsii.member(jsii_name="sopsFileFormat")
-    def sops_file_format(self) -> builtins.str:
-        '''(experimental) The format of the input file.
-
-        :stability: experimental
-        '''
-        return typing.cast(builtins.str, jsii.get(self, "sopsFileFormat"))
-
-    @builtins.property
     @jsii.member(jsii_name="stringifiedValues")
     def stringified_values(self) -> builtins.bool:
         '''(experimental) Were the values stringified?
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "stringifiedValues"))
@@ -649,95 +685,97 @@
         return typing.cast(builtins.str, jsii.get(self, "versionId"))
 
 
 @jsii.data_type(
     jsii_type="cdk-sops-secrets.SopsSyncOptions",
     jsii_struct_bases=[],
     name_mapping={
-        "sops_file_path": "sopsFilePath",
         "convert_to_json": "convertToJSON",
         "flatten": "flatten",
         "sops_age_key": "sopsAgeKey",
         "sops_file_format": "sopsFileFormat",
+        "sops_file_path": "sopsFilePath",
         "sops_kms_key": "sopsKmsKey",
         "sops_provider": "sopsProvider",
+        "sops_s3_bucket": "sopsS3Bucket",
+        "sops_s3_key": "sopsS3Key",
         "stringify_values": "stringifyValues",
         "upload_type": "uploadType",
     },
 )
 class SopsSyncOptions:
     def __init__(
         self,
         *,
-        sops_file_path: builtins.str,
         convert_to_json: typing.Optional[builtins.bool] = None,
         flatten: typing.Optional[builtins.bool] = None,
         sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
         sops_file_format: typing.Optional[builtins.str] = None,
+        sops_file_path: typing.Optional[builtins.str] = None,
         sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
         sops_provider: typing.Optional["SopsSyncProvider"] = None,
+        sops_s3_bucket: typing.Optional[builtins.str] = None,
+        sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional["UploadType"] = None,
     ) -> None:
         '''(experimental) Configuration options for the SopsSync.
 
-        :param sops_file_path: (experimental) The filepath to the sops file.
         :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
         :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
         :param sops_age_key: (experimental) The age key that should be used for encryption.
         :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: (experimental) The filepath to the sops file.
         :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
         :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
         :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
         :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c2e7f5d5a68ee1675b645864f7bab39e30d7c7922956c69686578f4d6fb05723)
-            check_type(argname="argument sops_file_path", value=sops_file_path, expected_type=type_hints["sops_file_path"])
             check_type(argname="argument convert_to_json", value=convert_to_json, expected_type=type_hints["convert_to_json"])
             check_type(argname="argument flatten", value=flatten, expected_type=type_hints["flatten"])
             check_type(argname="argument sops_age_key", value=sops_age_key, expected_type=type_hints["sops_age_key"])
             check_type(argname="argument sops_file_format", value=sops_file_format, expected_type=type_hints["sops_file_format"])
+            check_type(argname="argument sops_file_path", value=sops_file_path, expected_type=type_hints["sops_file_path"])
             check_type(argname="argument sops_kms_key", value=sops_kms_key, expected_type=type_hints["sops_kms_key"])
             check_type(argname="argument sops_provider", value=sops_provider, expected_type=type_hints["sops_provider"])
+            check_type(argname="argument sops_s3_bucket", value=sops_s3_bucket, expected_type=type_hints["sops_s3_bucket"])
+            check_type(argname="argument sops_s3_key", value=sops_s3_key, expected_type=type_hints["sops_s3_key"])
             check_type(argname="argument stringify_values", value=stringify_values, expected_type=type_hints["stringify_values"])
             check_type(argname="argument upload_type", value=upload_type, expected_type=type_hints["upload_type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "sops_file_path": sops_file_path,
-        }
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if convert_to_json is not None:
             self._values["convert_to_json"] = convert_to_json
         if flatten is not None:
             self._values["flatten"] = flatten
         if sops_age_key is not None:
             self._values["sops_age_key"] = sops_age_key
         if sops_file_format is not None:
             self._values["sops_file_format"] = sops_file_format
+        if sops_file_path is not None:
+            self._values["sops_file_path"] = sops_file_path
         if sops_kms_key is not None:
             self._values["sops_kms_key"] = sops_kms_key
         if sops_provider is not None:
             self._values["sops_provider"] = sops_provider
+        if sops_s3_bucket is not None:
+            self._values["sops_s3_bucket"] = sops_s3_bucket
+        if sops_s3_key is not None:
+            self._values["sops_s3_key"] = sops_s3_key
         if stringify_values is not None:
             self._values["stringify_values"] = stringify_values
         if upload_type is not None:
             self._values["upload_type"] = upload_type
 
     @builtins.property
-    def sops_file_path(self) -> builtins.str:
-        '''(experimental) The filepath to the sops file.
-
-        :stability: experimental
-        '''
-        result = self._values.get("sops_file_path")
-        assert result is not None, "Required property 'sops_file_path' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
     def convert_to_json(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Should the encrypted sops value should be converted to JSON?
 
         Only JSON can be handled by cloud formations dynamic references.
 
         :default: true
 
@@ -778,14 +816,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("sops_file_format")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def sops_file_path(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The filepath to the sops file.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_file_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def sops_kms_key(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]]:
         '''(experimental) The kmsKey used to encrypt the sops file.
 
         Encrypt permissions
         will be granted to the custom resource provider.
@@ -808,14 +855,32 @@
 
         :stability: experimental
         '''
         result = self._values.get("sops_provider")
         return typing.cast(typing.Optional["SopsSyncProvider"], result)
 
     @builtins.property
+    def sops_s3_bucket(self) -> typing.Optional[builtins.str]:
+        '''(experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_s3_bucket")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def sops_s3_key(self) -> typing.Optional[builtins.str]:
+        '''(experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_s3_key")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def stringify_values(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Shall all values be flattened?
 
         This is usefull for dynamic references, as there
         are lookup errors for certain float types
 
         :stability: experimental
@@ -846,100 +911,103 @@
         )
 
 
 @jsii.data_type(
     jsii_type="cdk-sops-secrets.SopsSyncProps",
     jsii_struct_bases=[SopsSyncOptions],
     name_mapping={
-        "sops_file_path": "sopsFilePath",
         "convert_to_json": "convertToJSON",
         "flatten": "flatten",
         "sops_age_key": "sopsAgeKey",
         "sops_file_format": "sopsFileFormat",
+        "sops_file_path": "sopsFilePath",
         "sops_kms_key": "sopsKmsKey",
         "sops_provider": "sopsProvider",
+        "sops_s3_bucket": "sopsS3Bucket",
+        "sops_s3_key": "sopsS3Key",
         "stringify_values": "stringifyValues",
         "upload_type": "uploadType",
         "secret": "secret",
     },
 )
 class SopsSyncProps(SopsSyncOptions):
     def __init__(
         self,
         *,
-        sops_file_path: builtins.str,
         convert_to_json: typing.Optional[builtins.bool] = None,
         flatten: typing.Optional[builtins.bool] = None,
         sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
         sops_file_format: typing.Optional[builtins.str] = None,
+        sops_file_path: typing.Optional[builtins.str] = None,
         sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
         sops_provider: typing.Optional["SopsSyncProvider"] = None,
+        sops_s3_bucket: typing.Optional[builtins.str] = None,
+        sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional["UploadType"] = None,
         secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
     ) -> None:
         '''(experimental) The configuration options extended by the target Secret.
 
-        :param sops_file_path: (experimental) The filepath to the sops file.
         :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
         :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
         :param sops_age_key: (experimental) The age key that should be used for encryption.
         :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: (experimental) The filepath to the sops file.
         :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
         :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
         :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
         :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
         :param secret: (experimental) The secret that will be populated with the encrypted sops file content.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3baaf21b8ae44e7f4d83d5677857cc4141222b3d41237073b75dca6d425c2c34)
-            check_type(argname="argument sops_file_path", value=sops_file_path, expected_type=type_hints["sops_file_path"])
             check_type(argname="argument convert_to_json", value=convert_to_json, expected_type=type_hints["convert_to_json"])
             check_type(argname="argument flatten", value=flatten, expected_type=type_hints["flatten"])
             check_type(argname="argument sops_age_key", value=sops_age_key, expected_type=type_hints["sops_age_key"])
             check_type(argname="argument sops_file_format", value=sops_file_format, expected_type=type_hints["sops_file_format"])
+            check_type(argname="argument sops_file_path", value=sops_file_path, expected_type=type_hints["sops_file_path"])
             check_type(argname="argument sops_kms_key", value=sops_kms_key, expected_type=type_hints["sops_kms_key"])
             check_type(argname="argument sops_provider", value=sops_provider, expected_type=type_hints["sops_provider"])
+            check_type(argname="argument sops_s3_bucket", value=sops_s3_bucket, expected_type=type_hints["sops_s3_bucket"])
+            check_type(argname="argument sops_s3_key", value=sops_s3_key, expected_type=type_hints["sops_s3_key"])
             check_type(argname="argument stringify_values", value=stringify_values, expected_type=type_hints["stringify_values"])
             check_type(argname="argument upload_type", value=upload_type, expected_type=type_hints["upload_type"])
             check_type(argname="argument secret", value=secret, expected_type=type_hints["secret"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "sops_file_path": sops_file_path,
             "secret": secret,
         }
         if convert_to_json is not None:
             self._values["convert_to_json"] = convert_to_json
         if flatten is not None:
             self._values["flatten"] = flatten
         if sops_age_key is not None:
             self._values["sops_age_key"] = sops_age_key
         if sops_file_format is not None:
             self._values["sops_file_format"] = sops_file_format
+        if sops_file_path is not None:
+            self._values["sops_file_path"] = sops_file_path
         if sops_kms_key is not None:
             self._values["sops_kms_key"] = sops_kms_key
         if sops_provider is not None:
             self._values["sops_provider"] = sops_provider
+        if sops_s3_bucket is not None:
+            self._values["sops_s3_bucket"] = sops_s3_bucket
+        if sops_s3_key is not None:
+            self._values["sops_s3_key"] = sops_s3_key
         if stringify_values is not None:
             self._values["stringify_values"] = stringify_values
         if upload_type is not None:
             self._values["upload_type"] = upload_type
 
     @builtins.property
-    def sops_file_path(self) -> builtins.str:
-        '''(experimental) The filepath to the sops file.
-
-        :stability: experimental
-        '''
-        result = self._values.get("sops_file_path")
-        assert result is not None, "Required property 'sops_file_path' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
     def convert_to_json(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Should the encrypted sops value should be converted to JSON?
 
         Only JSON can be handled by cloud formations dynamic references.
 
         :default: true
 
@@ -980,14 +1048,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("sops_file_format")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def sops_file_path(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The filepath to the sops file.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_file_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def sops_kms_key(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]]:
         '''(experimental) The kmsKey used to encrypt the sops file.
 
         Encrypt permissions
         will be granted to the custom resource provider.
@@ -1010,14 +1087,32 @@
 
         :stability: experimental
         '''
         result = self._values.get("sops_provider")
         return typing.cast(typing.Optional["SopsSyncProvider"], result)
 
     @builtins.property
+    def sops_s3_bucket(self) -> typing.Optional[builtins.str]:
+        '''(experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_s3_bucket")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def sops_s3_key(self) -> typing.Optional[builtins.str]:
+        '''(experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_s3_key")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def stringify_values(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Shall all values be flattened?
 
         This is usefull for dynamic references, as there
         are lookup errors for certain float types
 
         :stability: experimental
@@ -1124,21 +1219,23 @@
     name_mapping={
         "description": "description",
         "encryption_key": "encryptionKey",
         "generate_secret_string": "generateSecretString",
         "removal_policy": "removalPolicy",
         "replica_regions": "replicaRegions",
         "secret_name": "secretName",
-        "sops_file_path": "sopsFilePath",
         "convert_to_json": "convertToJSON",
         "flatten": "flatten",
         "sops_age_key": "sopsAgeKey",
         "sops_file_format": "sopsFileFormat",
+        "sops_file_path": "sopsFilePath",
         "sops_kms_key": "sopsKmsKey",
         "sops_provider": "sopsProvider",
+        "sops_s3_bucket": "sopsS3Bucket",
+        "sops_s3_key": "sopsS3Key",
         "stringify_values": "stringifyValues",
         "upload_type": "uploadType",
     },
 )
 class SopsSecretProps(
     _aws_cdk_aws_secretsmanager_ceddda9d.SecretProps,
     SopsSyncOptions,
@@ -1148,39 +1245,43 @@
         *,
         description: typing.Optional[builtins.str] = None,
         encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
         generate_secret_string: typing.Optional[typing.Union[_aws_cdk_aws_secretsmanager_ceddda9d.SecretStringGenerator, typing.Dict[builtins.str, typing.Any]]] = None,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
         replica_regions: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_secretsmanager_ceddda9d.ReplicaRegion, typing.Dict[builtins.str, typing.Any]]]] = None,
         secret_name: typing.Optional[builtins.str] = None,
-        sops_file_path: builtins.str,
         convert_to_json: typing.Optional[builtins.bool] = None,
         flatten: typing.Optional[builtins.bool] = None,
         sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
         sops_file_format: typing.Optional[builtins.str] = None,
+        sops_file_path: typing.Optional[builtins.str] = None,
         sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
         sops_provider: typing.Optional[SopsSyncProvider] = None,
+        sops_s3_bucket: typing.Optional[builtins.str] = None,
+        sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional[UploadType] = None,
     ) -> None:
         '''(experimental) The configuration options of the SopsSecret.
 
         :param description: An optional, human-friendly description of the secret. Default: - No description.
         :param encryption_key: The customer-managed encryption key to use for encrypting the secret value. Default: - A default KMS key for the account and region is used.
         :param generate_secret_string: Configuration for how to generate a secret value. Default: - 32 characters with upper-case letters, lower-case letters, punctuation and numbers (at least one from each category), per the default values of ``SecretStringGenerator``.
         :param removal_policy: Policy to apply when the secret is removed from this stack. Default: - Not set.
         :param replica_regions: A list of regions where to replicate this secret. Default: - Secret is not replicated
         :param secret_name: A name for the secret. Note that deleting secrets from SecretsManager does not happen immediately, but after a 7 to 30 days blackout period. During that period, it is not possible to create another secret that shares the same name. Default: - A name is generated by CloudFormation.
-        :param sops_file_path: (experimental) The filepath to the sops file.
         :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
         :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
         :param sops_age_key: (experimental) The age key that should be used for encryption.
         :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: (experimental) The filepath to the sops file.
         :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
         :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
         :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
         :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
 
         :stability: experimental
         '''
         if isinstance(generate_secret_string, dict):
             generate_secret_string = _aws_cdk_aws_secretsmanager_ceddda9d.SecretStringGenerator(**generate_secret_string)
@@ -1188,26 +1289,26 @@
             type_hints = typing.get_type_hints(_typecheckingstub__6b5ff836a3767bbc726a1167e9f5e789f0fad2dcaf72b41a245494f0a121a8a3)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
             check_type(argname="argument generate_secret_string", value=generate_secret_string, expected_type=type_hints["generate_secret_string"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
             check_type(argname="argument replica_regions", value=replica_regions, expected_type=type_hints["replica_regions"])
             check_type(argname="argument secret_name", value=secret_name, expected_type=type_hints["secret_name"])
-            check_type(argname="argument sops_file_path", value=sops_file_path, expected_type=type_hints["sops_file_path"])
             check_type(argname="argument convert_to_json", value=convert_to_json, expected_type=type_hints["convert_to_json"])
             check_type(argname="argument flatten", value=flatten, expected_type=type_hints["flatten"])
             check_type(argname="argument sops_age_key", value=sops_age_key, expected_type=type_hints["sops_age_key"])
             check_type(argname="argument sops_file_format", value=sops_file_format, expected_type=type_hints["sops_file_format"])
+            check_type(argname="argument sops_file_path", value=sops_file_path, expected_type=type_hints["sops_file_path"])
             check_type(argname="argument sops_kms_key", value=sops_kms_key, expected_type=type_hints["sops_kms_key"])
             check_type(argname="argument sops_provider", value=sops_provider, expected_type=type_hints["sops_provider"])
+            check_type(argname="argument sops_s3_bucket", value=sops_s3_bucket, expected_type=type_hints["sops_s3_bucket"])
+            check_type(argname="argument sops_s3_key", value=sops_s3_key, expected_type=type_hints["sops_s3_key"])
             check_type(argname="argument stringify_values", value=stringify_values, expected_type=type_hints["stringify_values"])
             check_type(argname="argument upload_type", value=upload_type, expected_type=type_hints["upload_type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "sops_file_path": sops_file_path,
-        }
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
         if generate_secret_string is not None:
             self._values["generate_secret_string"] = generate_secret_string
         if removal_policy is not None:
@@ -1220,18 +1321,24 @@
             self._values["convert_to_json"] = convert_to_json
         if flatten is not None:
             self._values["flatten"] = flatten
         if sops_age_key is not None:
             self._values["sops_age_key"] = sops_age_key
         if sops_file_format is not None:
             self._values["sops_file_format"] = sops_file_format
+        if sops_file_path is not None:
+            self._values["sops_file_path"] = sops_file_path
         if sops_kms_key is not None:
             self._values["sops_kms_key"] = sops_kms_key
         if sops_provider is not None:
             self._values["sops_provider"] = sops_provider
+        if sops_s3_bucket is not None:
+            self._values["sops_s3_bucket"] = sops_s3_bucket
+        if sops_s3_key is not None:
+            self._values["sops_s3_key"] = sops_s3_key
         if stringify_values is not None:
             self._values["stringify_values"] = stringify_values
         if upload_type is not None:
             self._values["upload_type"] = upload_type
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
@@ -1294,24 +1401,14 @@
 
         :default: - A name is generated by CloudFormation.
         '''
         result = self._values.get("secret_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def sops_file_path(self) -> builtins.str:
-        '''(experimental) The filepath to the sops file.
-
-        :stability: experimental
-        '''
-        result = self._values.get("sops_file_path")
-        assert result is not None, "Required property 'sops_file_path' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
     def convert_to_json(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Should the encrypted sops value should be converted to JSON?
 
         Only JSON can be handled by cloud formations dynamic references.
 
         :default: true
 
@@ -1352,14 +1449,23 @@
 
         :stability: experimental
         '''
         result = self._values.get("sops_file_format")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def sops_file_path(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The filepath to the sops file.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_file_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def sops_kms_key(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]]:
         '''(experimental) The kmsKey used to encrypt the sops file.
 
         Encrypt permissions
         will be granted to the custom resource provider.
@@ -1382,14 +1488,32 @@
 
         :stability: experimental
         '''
         result = self._values.get("sops_provider")
         return typing.cast(typing.Optional[SopsSyncProvider], result)
 
     @builtins.property
+    def sops_s3_bucket(self) -> typing.Optional[builtins.str]:
+        '''(experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_s3_bucket")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def sops_s3_key(self) -> typing.Optional[builtins.str]:
+        '''(experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+
+        :stability: experimental
+        '''
+        result = self._values.get("sops_s3_key")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def stringify_values(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Shall all values be flattened?
 
         This is usefull for dynamic references, as there
         are lookup errors for certain float types
 
         :stability: experimental
@@ -1438,21 +1562,23 @@
     *,
     description: typing.Optional[builtins.str] = None,
     encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
     generate_secret_string: typing.Optional[typing.Union[_aws_cdk_aws_secretsmanager_ceddda9d.SecretStringGenerator, typing.Dict[builtins.str, typing.Any]]] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
     replica_regions: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_secretsmanager_ceddda9d.ReplicaRegion, typing.Dict[builtins.str, typing.Any]]]] = None,
     secret_name: typing.Optional[builtins.str] = None,
-    sops_file_path: builtins.str,
     convert_to_json: typing.Optional[builtins.bool] = None,
     flatten: typing.Optional[builtins.bool] = None,
     sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
     sops_file_format: typing.Optional[builtins.str] = None,
+    sops_file_path: typing.Optional[builtins.str] = None,
     sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
     sops_provider: typing.Optional[SopsSyncProvider] = None,
+    sops_s3_bucket: typing.Optional[builtins.str] = None,
+    sops_s3_key: typing.Optional[builtins.str] = None,
     stringify_values: typing.Optional[builtins.bool] = None,
     upload_type: typing.Optional[UploadType] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__bd08508625195135b318d9657d717ca369ecceb1cc51cd6b3fa8c66c489c3dad(
@@ -1503,51 +1629,57 @@
     pass
 
 def _typecheckingstub__6b3134de7215a676a4feb3291975d227477d2dc9d5914405b8ab165ac30d7bad(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
-    sops_file_path: builtins.str,
     convert_to_json: typing.Optional[builtins.bool] = None,
     flatten: typing.Optional[builtins.bool] = None,
     sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
     sops_file_format: typing.Optional[builtins.str] = None,
+    sops_file_path: typing.Optional[builtins.str] = None,
     sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
     sops_provider: typing.Optional[SopsSyncProvider] = None,
+    sops_s3_bucket: typing.Optional[builtins.str] = None,
+    sops_s3_key: typing.Optional[builtins.str] = None,
     stringify_values: typing.Optional[builtins.bool] = None,
     upload_type: typing.Optional[UploadType] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__c2e7f5d5a68ee1675b645864f7bab39e30d7c7922956c69686578f4d6fb05723(
     *,
-    sops_file_path: builtins.str,
     convert_to_json: typing.Optional[builtins.bool] = None,
     flatten: typing.Optional[builtins.bool] = None,
     sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
     sops_file_format: typing.Optional[builtins.str] = None,
+    sops_file_path: typing.Optional[builtins.str] = None,
     sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
     sops_provider: typing.Optional[SopsSyncProvider] = None,
+    sops_s3_bucket: typing.Optional[builtins.str] = None,
+    sops_s3_key: typing.Optional[builtins.str] = None,
     stringify_values: typing.Optional[builtins.bool] = None,
     upload_type: typing.Optional[UploadType] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__3baaf21b8ae44e7f4d83d5677857cc4141222b3d41237073b75dca6d425c2c34(
     *,
-    sops_file_path: builtins.str,
     convert_to_json: typing.Optional[builtins.bool] = None,
     flatten: typing.Optional[builtins.bool] = None,
     sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
     sops_file_format: typing.Optional[builtins.str] = None,
+    sops_file_path: typing.Optional[builtins.str] = None,
     sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
     sops_provider: typing.Optional[SopsSyncProvider] = None,
+    sops_s3_bucket: typing.Optional[builtins.str] = None,
+    sops_s3_key: typing.Optional[builtins.str] = None,
     stringify_values: typing.Optional[builtins.bool] = None,
     upload_type: typing.Optional[UploadType] = None,
     secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -1568,19 +1700,21 @@
     *,
     description: typing.Optional[builtins.str] = None,
     encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
     generate_secret_string: typing.Optional[typing.Union[_aws_cdk_aws_secretsmanager_ceddda9d.SecretStringGenerator, typing.Dict[builtins.str, typing.Any]]] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
     replica_regions: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_secretsmanager_ceddda9d.ReplicaRegion, typing.Dict[builtins.str, typing.Any]]]] = None,
     secret_name: typing.Optional[builtins.str] = None,
-    sops_file_path: builtins.str,
     convert_to_json: typing.Optional[builtins.bool] = None,
     flatten: typing.Optional[builtins.bool] = None,
     sops_age_key: typing.Optional[_aws_cdk_ceddda9d.SecretValue] = None,
     sops_file_format: typing.Optional[builtins.str] = None,
+    sops_file_path: typing.Optional[builtins.str] = None,
     sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
     sops_provider: typing.Optional[SopsSyncProvider] = None,
+    sops_s3_bucket: typing.Optional[builtins.str] = None,
+    sops_s3_key: typing.Optional[builtins.str] = None,
     stringify_values: typing.Optional[builtins.bool] = None,
     upload_type: typing.Optional[UploadType] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-sops-secrets-1.7.3/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.8.0/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.7.3
+Version: 1.8.0
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -189,14 +189,47 @@
 {
   "context": {
     "sops_sync_provider_asset_path": "some/path/asset.zip"
   }
 }
 ```
 
+### I want to upload the sops file myself and only want to reference it
+
+That's possible since version 1.8.0. You can reference the file in S3 like:
+
+```python
+new SopsSecret(stack, 'SopsSecret', {
+  sopsS3Bucket: 'testbucket',
+  sopsS3Key: 'secret.json',
+  sopsFileFormat: 'json',
+  // ...
+});
+```
+
+Passing those values as CloudFormation parameters should also be possible:
+
+```python
+
+const sopsS3BucketParam = new CfnParameter(this, "s3BucketName", {
+  type: "String",
+  description: "The name of the Amazon S3 bucket where your sopsFile was uploaded."});
+
+const sopsS3KeyParam = new CfnParameter(this, "s3KeyName", {
+  type: "String",
+  description: "The name of the key of the sopsFile inside the Amazon S3 bucket."});
+
+new SopsSecret(stack, 'SopsSecret', {
+  sopsS3Bucket: sopsS3BucketParam.valueAsString,
+  sopsS3Key: sopsS3KeyParam.valueAsString,
+  sopsFileFormat: 'json',
+  // ...
+});
+```
+
 ## Motivation
 
 I have created this project to solve a recurring problem of syncing Mozilla/sops secrets into AWS SecretsManager in a convenient, secure way.
 
 Other than that, or perhaps more importantly, my goal was to learn new things:
 
 * Write a Golang lambda
```

