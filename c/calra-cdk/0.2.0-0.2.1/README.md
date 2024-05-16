# Comparing `tmp/calra_cdk-0.2.0-py3-none-any.whl.zip` & `tmp/calra_cdk-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10903 bytes, number of entries: 8
+Zip file size: 10866 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       45 b- defN 24-May-14 00:29 calra_cdk/__init__.py
--rw-r--r--  2.0 unx    10929 b- defN 24-May-14 00:29 calra_cdk/ast_helper.py
--rw-r--r--  2.0 unx    14626 b- defN 24-May-14 00:29 calra_cdk/resource_builder.py
--rw-r--r--  2.0 unx     1087 b- defN 24-May-14 00:32 calra_cdk-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5693 b- defN 24-May-14 00:32 calra_cdk-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 00:32 calra_cdk-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-14 00:32 calra_cdk-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      640 b- defN 24-May-14 00:32 calra_cdk-0.2.0.dist-info/RECORD
-8 files, 33122 bytes uncompressed, 9789 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx    10875 b- defN 24-May-14 18:24 calra_cdk/ast_helper.py
+-rw-r--r--  2.0 unx    14595 b- defN 24-May-14 18:24 calra_cdk/resource_builder.py
+-rw-r--r--  2.0 unx     1087 b- defN 24-May-14 18:25 calra_cdk-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5731 b- defN 24-May-14 18:25 calra_cdk-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 18:25 calra_cdk-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-14 18:25 calra_cdk-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      640 b- defN 24-May-14 18:25 calra_cdk-0.2.1.dist-info/RECORD
+8 files, 33075 bytes uncompressed, 9752 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: calra_cdk/ast_helper.py
 Comment: 
 
 Filename: calra_cdk/resource_builder.py
 Comment: 
 
-Filename: calra_cdk-0.2.0.dist-info/LICENSE
+Filename: calra_cdk-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: calra_cdk-0.2.0.dist-info/METADATA
+Filename: calra_cdk-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: calra_cdk-0.2.0.dist-info/WHEEL
+Filename: calra_cdk-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: calra_cdk-0.2.0.dist-info/top_level.txt
+Filename: calra_cdk-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: calra_cdk-0.2.0.dist-info/RECORD
+Filename: calra_cdk-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## calra_cdk/ast_helper.py

```diff
@@ -3,15 +3,15 @@
 
 class Method:
     ALLOWED_METHODS = {'PUT', 'POST', 'GET', 'DELETE', 'ANY'}
 
     def __init__(self, path_to_file:str, file: str, handler: str, method: str, decorators: dict):
         '''One http method is always associated with a file:handler entrypoint in a one-to-one relationship and each handler has decorators in a one-to-many relationship'''
         if method not in self.ALLOWED_METHODS:
-            raise ValueError(f'Invalid method: {method}. Allowed methods are {', '.join(self.ALLOWED_METHODS)}')
+            raise ValueError(f"Invalid method: {method}. Allowed methods are {', '.join(self.ALLOWED_METHODS)}")
         self.method = method
         self.file = file.replace(os.sep, '/')
         self.path_to_file = path_to_file.replace(os.sep, '/')
         self.handler = handler
         self.decorators = decorators
 
     def __str__(self):
@@ -69,15 +69,14 @@
     def __str__(self):
         methods_str = ' '
         for method in self.get_methods():
             methods_str = '(' + str(method.__str__()) + ') '
             #methods_str = methods_str + '(' + method.get_method() + ' at ' + method.get_logical_id() + ') '
         return self.get_path() + methods_str 
     
-    #Validar GET PUT UPDATE DELETE? QUE NO SE REPITA?
     def add_method(self, method: Method) -> bool:
         '''Aggregate Method to present Resource's endpoint'''
         if method not in self.methods:
             self.methods.append(method)
             return True
         else:
             return False
```

## calra_cdk/resource_builder.py

```diff
@@ -169,38 +169,38 @@
     
     def get_common_environment(self, value: str):
         return self.common_environments[value]
     
     def get_custom_layer(self, value: str) -> lambda_.LayerVersion | _lambda_python.PythonLayerVersion:
         if self.custom_layers.get(value):
             return self.custom_layers[value]
-        else: raise KeyError(name=f'Value {value} not previously declared as custom layer')
+        else: raise KeyError(f"Value {value} not previously declared as custom layer")
 
     def get_custom_roles(self):
         return self.custom_roles
     
     def get_custom_role(self, value: str) -> iam.Role:
         if self.custom_roles.get(value):
             return self.custom_roles[value]
-        else: raise KeyError(name=f'Value {value} not previously declared as custom role')
+        else: raise KeyError(f"Value {value} not previously declared as custom role")
     
     def get_custom_security_group(self, value: str) -> ec2.SecurityGroup:
         if self.custom_security_groups.get(value):
             return self.custom_security_groups[value]
-        else: raise KeyError(name=f'Value {value} not previously declared as custom security group')
+        else: raise KeyError(f"Value {value} not previously declared as custom security group")
     
     def get_custom_environment(self, value: str) -> str:
         if self.custom_environments.get(value):
             return self.custom_environments[value]
-        else: raise KeyError(name=f'Value {value} not previously declared as custom environment')
+        else: raise KeyError(f"Value {value} not previously declared as custom environment")
     
     def get_custom_runtime(self, value: str) -> lambda_.Runtime: 
         if self.custom_runtimes.get(value):
             return self.custom_runtimes[value]
-        else: raise KeyError(name=f'Value {value} not previously declared as custom runtime')
+        else: raise KeyError(f"Value {value} not previously declared as custom runtime")
     
     def get_custom_vpc(self, value: str) -> tuple:
         #TODO
         return self.custom_vpcs[value]
 
     def build(self, construct, api_resource: apigateway.IResource, lambda_path:str, print_tree: bool = False):
         '''
@@ -241,15 +241,15 @@
             elif key == 'layer':
                 if type(value) == list:
                     for v in value:
                         options[key].append(self.get_custom_layer(v))
                 else:
                     options[key].append(self.get_custom_layer(value))
             elif key == 'role':
-                options[key].append(self.get_custom_role(value))
+                options[key] = self.get_custom_role(value)
             elif key == 'security_group':
                 if type(value) == list:
                     for v in value:
                         options[key].append(self.get_custom_environment(v))
                 else:
                     options[key].append(self.get_custom_security_group(value))
             elif key == 'environment':
```

## Comparing `calra_cdk-0.2.0.dist-info/LICENSE` & `calra_cdk-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `calra_cdk-0.2.0.dist-info/METADATA` & `calra_cdk-0.2.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calra-cdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: CDK Ast Lambda Rest Api - CDK Package
 Author-email: Mateo Marcos <calra.github+mateo@gmail.com>, Emanuel Arguinarena <calra.github+emanuel@gmail.com>, Lucas Picchi <calra.github+lucas@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 CDK Ast Lambda Rest-API (Calra)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,15 @@
 
 ### Installation
 
 `calra_cdk` is available from PyPI as `calra-cdk`:
 
     pip install calra-cdk
 
-Installation of [calra-lambda](https://example.com) is also required as a dependency for your lambda functions, since it provides the definition of decorators used within this module.
+Installation of [calra-lambda](https://pypi.org/project/calra-lambda/) is also required as a dependency for your lambda functions, since it provides the definition of decorators used within this module.
 You can as well rely on the [calra-example](https://https://github.com/cdk-ast-lambda-rest-api/calra-example) repository to get started.
 
 ### Example
 
 ```python
     import calra_cdk
     or
@@ -93,15 +93,15 @@
     builder.add_custom_environment("URL-PREFIX", "calra-cdk-") #Lambda Function should have decorator @environment("URL-PREFIX")
 ```
 
 ### Building
 
 Assuming you have already instantiated a Builder, configured it and ready to deploy your stack, then simply define the directory of your Lambda Functions and build!
 
-Note: For a Lambda Function to be recognised and built, it has to have a decorator specifying the HTTP method it responds to. Again, the [calra-example](https://https://github.com/cdk-ast-lambda-rest-api/calra-example) repository will provide a firm example of a builder setting and lambda proper annotation with decorators using the [calra-lambda](https://example.com) module.
+Note: For a Lambda Function to be recognised and built, it has to have a decorator specifying the HTTP method it responds to. Again, the [calra-example](https://https://github.com/cdk-ast-lambda-rest-api/calra-example) repository will provide a firm example of a builder setting and lambda proper annotation with decorators using the [calra-lambda](https://pypi.org/project/calra-lambda/) module.
 
 ```python
 [...] # Imports
 
 class CalraExampleStack(Stack):
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
```

