# Comparing `tmp/Serializer_Deserializer-1.4.tar.gz` & `tmp/Serializer_Deserializer-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Serializer_Deserializer-1.4.tar", last modified: Mon Apr 22 15:01:10 2024, max compression
+gzip compressed data, was "Serializer_Deserializer-1.5.tar", last modified: Thu May 16 11:44:05 2024, max compression
```

## Comparing `Serializer_Deserializer-1.4.tar` & `Serializer_Deserializer-1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 15:01:10.634974 Serializer_Deserializer-1.4/
--rw-rw-rw-   0        0        0      167 2024-04-22 15:01:10.635965 Serializer_Deserializer-1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 15:01:10.625964 Serializer_Deserializer-1.4/SerializerDeserializerModels/
--rw-rw-rw-   0        0        0     2638 2024-04-22 15:00:50.000000 Serializer_Deserializer-1.4/SerializerDeserializerModels/SerializerDeserializerModels.py
--rw-rw-rw-   0        0        0        0 2024-04-22 14:17:22.000000 Serializer_Deserializer-1.4/SerializerDeserializerModels/__init__.py
--rw-rw-rw-   0        0        0     2140 2024-04-22 14:14:00.000000 Serializer_Deserializer-1.4/SerializerDeserializerModels/models.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:01:10.633972 Serializer_Deserializer-1.4/Serializer_Deserializer.egg-info/
--rw-rw-rw-   0        0        0      167 2024-04-22 15:01:10.000000 Serializer_Deserializer-1.4/Serializer_Deserializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-22 15:01:10.000000 Serializer_Deserializer-1.4/Serializer_Deserializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 15:01:10.000000 Serializer_Deserializer-1.4/Serializer_Deserializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 14:27:54.000000 Serializer_Deserializer-1.4/Serializer_Deserializer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2024-04-22 15:01:10.000000 Serializer_Deserializer-1.4/Serializer_Deserializer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 15:01:10.637000 Serializer_Deserializer-1.4/setup.cfg
--rw-rw-rw-   0        0        0      291 2024-04-22 15:01:02.000000 Serializer_Deserializer-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:44:05.897154 Serializer_Deserializer-1.5/
+-rw-rw-rw-   0        0        0      167 2024-05-16 11:44:05.898155 Serializer_Deserializer-1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 11:44:05.893154 Serializer_Deserializer-1.5/SerializerDeserializerModels/
+-rw-rw-rw-   0        0        0     2639 2024-05-02 10:13:27.000000 Serializer_Deserializer-1.5/SerializerDeserializerModels/SerializerDeserializerModels.py
+-rw-rw-rw-   0        0        0        0 2024-04-22 14:17:22.000000 Serializer_Deserializer-1.5/SerializerDeserializerModels/__init__.py
+-rw-rw-rw-   0        0        0     2189 2024-05-16 11:41:52.000000 Serializer_Deserializer-1.5/SerializerDeserializerModels/models.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:44:05.897154 Serializer_Deserializer-1.5/Serializer_Deserializer.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-05-16 11:44:05.000000 Serializer_Deserializer-1.5/Serializer_Deserializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-16 11:44:05.000000 Serializer_Deserializer-1.5/Serializer_Deserializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:44:05.000000 Serializer_Deserializer-1.5/Serializer_Deserializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 14:27:54.000000 Serializer_Deserializer-1.5/Serializer_Deserializer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       29 2024-05-16 11:44:05.000000 Serializer_Deserializer-1.5/Serializer_Deserializer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:44:05.898155 Serializer_Deserializer-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      291 2024-05-16 11:43:31.000000 Serializer_Deserializer-1.5/setup.py
```

### Comparing `Serializer_Deserializer-1.4/SerializerDeserializerModels/SerializerDeserializerModels.py` & `Serializer_Deserializer-1.5/SerializerDeserializerModels/SerializerDeserializerModels.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             'EMAIL': user.email,
             'AGE': user.age,
         }
 
     @staticmethod
     def json_to_user(user_dict):
         user = User(name=user_dict.get('NAME', None), id=user_dict.get('ID', None),
-                    email=user_dict.get('NAME', None),age=user_dict.get('AGE', None),
+                    email=user_dict.get('EMAIL', None),age=user_dict.get('AGE', None),
                     password=user_dict.get('PASSWORD_HASH', None))
         return user
 
     @staticmethod
     def message_to_json(message):
         return {
             'ID': message.id,
```

### Comparing `Serializer_Deserializer-1.4/SerializerDeserializerModels/models.py` & `Serializer_Deserializer-1.5/SerializerDeserializerModels/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 class User(Base):
     __tablename__ = 'user'
     id = Column(Integer, primary_key=True)
     name = Column(String, unique=True)
     email = Column(String)
     age = Column(Integer)
     password = Column(String, nullable=False)
+    avatar = Column(String, nullable=False)
     UniqueConstraint('name')
 
 
 class Message(Base):
     __tablename__ = 'message'
     id = Column(Integer, primary_key=True)
     from_user = Column(Integer, ForeignKey('user.id', ondelete='CASCADE'),nullable=False)
@@ -30,14 +31,16 @@
 
 class Query(Base):
     __tablename__ = 'query'
     id = Column(Integer, primary_key=True)
     from_user = Column(Integer, ForeignKey('user.id', ondelete='CASCADE'), nullable=False)
     to_user = Column(Integer, ForeignKey('user.id', ondelete='CASCADE'), nullable=False)
 
+
+
 class Friend(Base):
     __tablename__ = 'friend'
     id = Column(Integer, primary_key=True)
     user1 = Column(Integer, ForeignKey('user.id', ondelete='CASCADE'), nullable=False)
     user2 = Column(Integer, ForeignKey('user.id', ondelete='CASCADE'), nullable=False)
```

