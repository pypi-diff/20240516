# Comparing `tmp/upstash_redis-1.0.0.tar.gz` & `tmp/upstash_redis-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-1.0.0.tar", max compression
+gzip compressed data, was "upstash_redis-1.1.0.tar", max compression
```

## Comparing `upstash_redis-1.0.0.tar` & `upstash_redis-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-12-04 10:35:25.493155 upstash_redis-1.0.0/LICENSE
--rw-r--r--   0        0        0     4441 2023-12-04 10:35:25.493155 upstash_redis-1.0.0/README.md
--rw-r--r--   0        0        0     1458 2023-12-04 10:35:25.493155 upstash_redis-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       83 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     5365 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     3790 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/client.py
--rw-r--r--   0        0        0   116670 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/commands.py
--rw-r--r--   0        0        0    37917 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/commands.pyi
--rw-r--r--   0        0        0       40 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/errors.py
--rw-r--r--   0        0        0     8625 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/format.py
--rw-r--r--   0        0        0     4649 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/http.py
--rw-r--r--   0        0        0        0 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/py.typed
--rw-r--r--   0        0        0      527 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/typing.py
--rw-r--r--   0        0        0     3715 2023-12-04 10:35:25.501155 upstash_redis-1.0.0/upstash_redis/utils.py
--rw-r--r--   0        0        0     5770 1970-01-01 00:00:00.000000 upstash_redis-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-16 08:51:18.587069 upstash_redis-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5624 2024-05-16 08:51:18.587069 upstash_redis-1.1.0/README.md
+-rw-r--r--   0        0        0     1458 2024-05-16 08:51:18.587069 upstash_redis-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       83 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     9683 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     7712 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/client.py
+-rw-r--r--   0        0        0   116698 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/commands.py
+-rw-r--r--   0        0        0    56221 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/commands.pyi
+-rw-r--r--   0        0        0       40 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/errors.py
+-rw-r--r--   0        0        0     9245 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/format.py
+-rw-r--r--   0        0        0     5486 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/http.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/py.typed
+-rw-r--r--   0        0        0      527 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/typing.py
+-rw-r--r--   0        0        0     3715 2024-05-16 08:51:18.591069 upstash_redis-1.1.0/upstash_redis/utils.py
+-rw-r--r--   0        0        0     6953 1970-01-01 00:00:00.000000 upstash_redis-1.1.0/PKG-INFO
```

### Comparing `upstash_redis-1.0.0/LICENSE` & `upstash_redis-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-1.0.0/pyproject.toml` & `upstash_redis-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upstash-redis"
-version = "1.0.0"
+version = "1.1.0"
 description = "Serverless Redis SDK from Upstash"
 license = "MIT"
 authors = ["Upstash <support@upstash.com>", "Zgîmbău Tudor <tudor.zgimbau@gmail.com>"]
 maintainers = ["Upstash <support@upstash.com>"]
 readme = "README.md"
 repository = "https://github.com/upstash/redis-python"
 keywords = ["Upstash Redis", "Serverless Redis"]
```

### Comparing `upstash_redis-1.0.0/upstash_redis/commands.py` & `upstash_redis-1.1.0/upstash_redis/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -4316,7 +4316,8 @@
     def execute(self) -> ResponseT:
         return self.client.execute(command=self.command)
 
 
 AsyncCommands = Commands
 AsyncBitFieldCommands = BitFieldCommands
 AsyncBitFieldROCommands = BitFieldROCommands
+PipelineCommands = Commands
```

### Comparing `upstash_redis-1.0.0/upstash_redis/commands.pyi` & `upstash_redis-1.1.0/upstash_redis/commands.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1014,7 +1014,491 @@
 
 class AsyncBitFieldROCommands:
     def __init__(self, client: AsyncCommands, key: str): ...
     def get(
         self, encoding: str, offset: Union[int, str]
     ) -> "AsyncBitFieldROCommands": ...
     async def execute(self) -> List: ...
+
+class PipelineCommands:
+    def bitcount(
+        self, key: str, start: Optional[int] = None, end: Optional[int] = None
+    ) -> PipelineCommands: ...
+    def bitfield(self, key: str) -> PipelineCommands: ...
+    def bitfield_ro(self, key: str) -> PipelineCommands: ...
+    def bitop(
+        self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *keys: str
+    ) -> PipelineCommands: ...
+    def bitpos(
+        self,
+        key: str,
+        bit: Literal[0, 1],
+        start: Optional[int] = None,
+        end: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def getbit(self, key: str, offset: int) -> PipelineCommands: ...
+    def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> PipelineCommands: ...
+    def ping(self, message: Optional[str] = None) -> PipelineCommands: ...
+    def echo(self, message: str) -> PipelineCommands: ...
+    def copy(self, source: str, destination: str, replace: bool = False) -> PipelineCommands: ...
+    def delete(self, *keys: str) -> PipelineCommands: ...
+    def exists(self, *keys: str) -> PipelineCommands: ...
+    def expire(
+        self,
+        key: str,
+        seconds: Union[int, datetime.timedelta],
+        nx: bool = False,
+        xx: bool = False,
+        gt: bool = False,
+        lt: bool = False,
+    ) -> PipelineCommands: ...
+    def expireat(
+        self,
+        key: str,
+        unix_time_seconds: Union[int, datetime.datetime],
+        nx: bool = False,
+        xx: bool = False,
+        gt: bool = False,
+        lt: bool = False,
+    ) -> PipelineCommands: ...
+    def keys(self, pattern: str) -> PipelineCommands: ...
+    def persist(self, key: str) -> PipelineCommands: ...
+    def pexpire(
+        self,
+        key: str,
+        milliseconds: Union[int, datetime.timedelta],
+        nx: bool = False,
+        xx: bool = False,
+        gt: bool = False,
+        lt: bool = False,
+    ) -> PipelineCommands: ...
+    def pexpireat(
+        self,
+        key: str,
+        unix_time_milliseconds: Union[int, datetime.datetime],
+        nx: bool = False,
+        xx: bool = False,
+        gt: bool = False,
+        lt: bool = False,
+    ) -> PipelineCommands: ...
+    def pttl(self, key: str) -> PipelineCommands: ...
+    def randomkey(self) -> PipelineCommands: ...
+    def rename(self, key: str, newkey: str) -> PipelineCommands: ...
+    def renamenx(self, key: str, newkey: str) -> PipelineCommands: ...
+    def scan(
+        self,
+        cursor: int,
+        match: Optional[str] = None,
+        count: Optional[int] = None,
+        type: Optional[str] = None,
+    ) -> PipelineCommands: ...
+    def touch(self, *keys: str) -> PipelineCommands: ...
+    def ttl(self, key: str) -> PipelineCommands: ...
+    def type(self, key: str) -> PipelineCommands: ...
+    def unlink(self, *keys: str) -> PipelineCommands: ...
+    def geoadd(
+        self,
+        key: str,
+        *members: Tuple[float, float, str],
+        nx: bool = False,
+        xx: bool = False,
+        ch: bool = False,
+    ) -> PipelineCommands: ...
+    def geodist(
+        self,
+        key: str,
+        member1: str,
+        member2: str,
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+    ) -> PipelineCommands: ...
+    def geohash(self, key: str, *members: str) -> PipelineCommands: ...
+    def geopos(
+        self, key: str, *members: str
+    ) -> PipelineCommands: ...
+    def georadius(
+        self,
+        key: str,
+        longitude: float,
+        latitude: float,
+        radius: float,
+        unit: Literal["M", "KM", "FT", "MI"],
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Optional[int] = None,
+        any: bool = False,
+        order: Optional[Literal["ASC", "DESC"]] = None,
+        store: Optional[str] = None,
+        storedist: Optional[str] = None,
+    ) -> PipelineCommands: ...
+    def georadius_ro(
+        self,
+        key: str,
+        longitude: float,
+        latitude: float,
+        radius: float,
+        unit: Literal["M", "KM", "FT", "MI"],
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Optional[int] = None,
+        any: bool = False,
+        order: Optional[Literal["ASC", "DESC"]] = None,
+    ) -> PipelineCommands: ...
+    def georadiusbymember(
+        self,
+        key: str,
+        member: str,
+        radius: float,
+        unit: Literal["M", "KM", "FT", "MI"],
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Optional[int] = None,
+        any: bool = False,
+        order: Optional[Literal["ASC", "DESC"]] = None,
+        store: Optional[str] = None,
+        storedist: Optional[str] = None,
+    ) -> PipelineCommands: ...
+    def georadiusbymember_ro(
+        self,
+        key: str,
+        member: str,
+        radius: float,
+        unit: Literal["M", "KM", "FT", "MI"],
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Optional[int] = None,
+        any: bool = False,
+        order: Optional[Literal["ASC", "DESC"]] = None,
+    ) -> PipelineCommands: ...
+    def geosearch(
+        self,
+        key: str,
+        unit: Literal["M", "KM", "FT", "MI"],
+        member: Optional[str] = None,
+        longitude: Optional[float] = None,
+        latitude: Optional[float] = None,
+        radius: Optional[float] = None,
+        width: Optional[float] = None,
+        height: Optional[float] = None,
+        order: Optional[Literal["ASC", "DESC"]] = None,
+        count: Optional[int] = None,
+        any: bool = False,
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+    ) -> PipelineCommands: ...
+    def geosearchstore(
+        self,
+        destination: str,
+        source: str,
+        member: Optional[str] = None,
+        longitude: Optional[float] = None,
+        latitude: Optional[float] = None,
+        unit: Literal["M", "KM", "FT", "MI"] = "M",
+        radius: Optional[float] = None,
+        width: Optional[float] = None,
+        height: Optional[float] = None,
+        order: Optional[Literal["ASC", "DESC"]] = None,
+        count: Optional[int] = None,
+        any: bool = False,
+        storedist: bool = False,
+    ) -> PipelineCommands: ...
+    def hdel(self, key: str, *fields: str) -> PipelineCommands: ...
+    def hexists(self, key: str, field: str) -> PipelineCommands: ...
+    def hget(self, key: str, field: str) -> PipelineCommands: ...
+    def hgetall(self, key: str) -> PipelineCommands: ...
+    def hincrby(self, key: str, field: str, increment: int) -> PipelineCommands: ...
+    def hincrbyfloat(self, key: str, field: str, increment: float) -> PipelineCommands: ...
+    def hkeys(self, key: str) -> PipelineCommands: ...
+    def hlen(self, key: str) -> PipelineCommands: ...
+    def hmget(self, key: str, *fields: str) -> PipelineCommands: ...
+    def hmset(self, key: str, values: Mapping[str, ValueT]) -> PipelineCommands: ...
+    def hrandfield(
+        self, key: str, count: Optional[int] = None, withvalues: bool = False
+    ) -> PipelineCommands: ...
+    def hscan(
+        self,
+        key: str,
+        cursor: int,
+        match: Optional[str] = None,
+        count: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def hset(
+        self,
+        key: str,
+        field: Optional[str] = None,
+        value: Optional[str] = None,
+        values: Optional[Mapping[str, ValueT]] = None,
+    ) -> PipelineCommands: ...
+    def hsetnx(self, key: str, field: str, value: ValueT) -> PipelineCommands: ...
+    def hstrlen(self, key: str, field: str) -> PipelineCommands: ...
+    def hvals(self, key: str) -> PipelineCommands: ...
+    def pfadd(self, key: str, *elements: ValueT) -> PipelineCommands: ...
+    def pfcount(self, *keys: str) -> PipelineCommands: ...
+    def pfmerge(self, destkey: str, *sourcekeys: str) -> PipelineCommands: ...
+    def lindex(self, key: str, index: int) -> PipelineCommands: ...
+    def linsert(
+        self,
+        key: str,
+        where: Literal["BEFORE", "AFTER"],
+        pivot: ValueT,
+        element: str,
+    ) -> PipelineCommands: ...
+    def llen(self, key: str) -> PipelineCommands: ...
+    def lmove(
+        self,
+        source: str,
+        destination: str,
+        wherefrom: Literal["LEFT", "RIGHT"] = "LEFT",
+        whereto: Literal["LEFT", "RIGHT"] = "RIGHT",
+    ) -> PipelineCommands: ...
+    def lpop(
+        self, key: str, count: Optional[int] = None
+    ) -> PipelineCommands: ...
+    def lpos(
+        self,
+        key: str,
+        element: ValueT,
+        rank: Optional[int] = None,
+        count: Optional[int] = None,
+        maxlen: Optional[int] = None,
+    ) -> Union[(Optional[int]), List[int]]: ...
+    def lpush(self, key: str, *elements: ValueT) -> PipelineCommands: ...
+    def lpushx(self, key: str, *elements: ValueT) -> PipelineCommands: ...
+    def lrange(self, key: str, start: int, stop: int) -> PipelineCommands: ...
+    def lrem(self, key: str, count: int, element: ValueT) -> PipelineCommands: ...
+    def lset(self, key: str, index: int, element: ValueT) -> PipelineCommands: ...
+    def ltrim(self, key: str, start: int, stop: int) -> PipelineCommands: ...
+    def rpop(
+        self, key: str, count: Optional[int] = None
+    ) -> PipelineCommands: ...
+    def rpoplpush(self, source: str, destination: str) -> PipelineCommands: ...
+    def rpush(self, key: str, *elements: ValueT) -> PipelineCommands: ...
+    def rpushx(self, key: str, *elements: ValueT) -> PipelineCommands: ...
+    def publish(self, channel: str, message: ValueT) -> PipelineCommands: ...
+    def eval(
+        self,
+        script: str,
+        keys: Optional[List[str]] = None,
+        args: Optional[List[str]] = None,
+    ) -> PipelineCommands: ...
+    def evalsha(
+        self,
+        sha1: str,
+        keys: Optional[List[str]] = None,
+        args: Optional[List[str]] = None,
+    ) -> PipelineCommands: ...
+    def dbsize(self) -> PipelineCommands: ...
+    def flushall(
+        self, flush_type: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> PipelineCommands: ...
+    def flushdb(
+        self, flush_type: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> PipelineCommands: ...
+    def time(self) -> PipelineCommands: ...
+    def sadd(self, key: str, *members: ValueT) -> PipelineCommands: ...
+    def scard(self, key: str) -> PipelineCommands: ...
+    def sdiff(self, *keys: str) -> PipelineCommands: ...
+    def sdiffstore(self, destination: str, *keys: str) -> PipelineCommands: ...
+    def sinter(self, *keys: str) -> PipelineCommands: ...
+    def sinterstore(self, destination: str, *keys: str) -> PipelineCommands: ...
+    def sismember(self, key: str, member: ValueT) -> PipelineCommands: ...
+    def smismember(self, key: str, *members: ValueT) -> PipelineCommands: ...
+    def smembers(self, key: str) -> PipelineCommands: ...
+    def smove(self, source: str, destination: str, member: ValueT) -> PipelineCommands: ...
+    def spop(
+        self, key: str, count: Optional[int] = None
+    ) -> PipelineCommands: ...
+    def srandmember(
+        self, key: str, count: Optional[int] = None
+    ) -> PipelineCommands: ...
+    def srem(self, key: str, *members: ValueT) -> PipelineCommands: ...
+    def sscan(
+        self,
+        key: str,
+        cursor: int = 0,
+        match: Optional[str] = None,
+        count: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def sunion(self, *keys: str) -> PipelineCommands: ...
+    def sunionstore(self, destination: str, *keys: str) -> PipelineCommands: ...
+    def zadd(
+        self,
+        key: str,
+        scores: Dict[str, float],
+        nx: bool = False,
+        xx: bool = False,
+        gt: bool = False,
+        lt: bool = False,
+        ch: bool = False,
+        incr: bool = False,
+    ) -> PipelineCommands: ...
+    def zcard(self, key: str) -> PipelineCommands: ...
+    def zcount(self, key: str, min: FloatMinMaxT, max: FloatMinMaxT) -> PipelineCommands: ...
+    def zdiff(
+        self, keys: List[str], withscores: bool = False
+    ) -> PipelineCommands: ...
+    def zdiffstore(self, destination: str, keys: List[str]) -> PipelineCommands: ...
+    def zincrby(self, key: str, increment: float, member: str) -> PipelineCommands: ...
+    def zinter(
+        self,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
+        aggregate: Optional[Literal["SUM", "MIN", "MAX"]] = None,
+        withscores: bool = False,
+    ) -> PipelineCommands: ...
+    def zinterstore(
+        self,
+        destination: str,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
+        aggregate: Optional[Literal["SUM", "MIN", "MAX"]] = None,
+    ) -> PipelineCommands: ...
+    def zlexcount(self, key: str, min: str, max: str) -> PipelineCommands: ...
+    def zmscore(self, key: str, members: List[str]) -> PipelineCommands: ...
+    def zpopmax(
+        self, key: str, count: Optional[int] = None
+    ) -> PipelineCommands: ...
+    def zpopmin(
+        self, key: str, count: Optional[int] = None
+    ) -> PipelineCommands: ...
+    def zrandmember(
+        self, key: str, count: Optional[int] = None, withscores: bool = False
+    ) -> PipelineCommands: ...
+    def zrange(
+        self,
+        key: str,
+        start: FloatMinMaxT,
+        stop: FloatMinMaxT,
+        sortby: Optional[Literal["BYSCORE", "BYLEX"]] = None,
+        rev: bool = False,
+        offset: Optional[int] = None,
+        count: Optional[int] = None,
+        withscores: bool = False,
+    ) -> PipelineCommands: ...
+    def zrangebylex(
+        self,
+        key: str,
+        min: str,
+        max: str,
+        offset: Optional[int] = None,
+        count: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def zrangebyscore(
+        self,
+        key: str,
+        min: FloatMinMaxT,
+        max: FloatMinMaxT,
+        withscores: bool = False,
+        offset: Optional[int] = None,
+        count: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def zrangestore(
+        self,
+        dst: str,
+        src: str,
+        min: FloatMinMaxT,
+        max: FloatMinMaxT,
+        sortby: Optional[Literal["BYSCORE", "BYLEX"]] = None,
+        rev: bool = False,
+        offset: Optional[int] = None,
+        count: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def zrank(self, key: str, member: str) -> PipelineCommands: ...
+    def zrem(self, key: str, *members: str) -> PipelineCommands: ...
+    def zremrangebylex(self, key: str, min: str, max: str) -> PipelineCommands: ...
+    def zremrangebyrank(self, key: str, start: int, stop: int) -> PipelineCommands: ...
+    def zremrangebyscore(
+        self, key: str, min: FloatMinMaxT, max: FloatMinMaxT
+    ) -> PipelineCommands: ...
+    def zrevrange(
+        self, key: str, start: int, stop: int, withscores: bool = False
+    ) -> PipelineCommands: ...
+    def zrevrangebylex(
+        self,
+        key: str,
+        max: str,
+        min: str,
+        offset: Optional[int] = None,
+        count: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def zrevrangebyscore(
+        self,
+        key: str,
+        max: FloatMinMaxT,
+        min: FloatMinMaxT,
+        withscores: bool = False,
+        offset: Optional[int] = None,
+        count: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def zrevrank(self, key: str, member: str) -> PipelineCommands: ...
+    def zscan(
+        self,
+        key: str,
+        cursor: int,
+        match: Optional[str] = None,
+        count: Optional[int] = None,
+    ) -> PipelineCommands: ...
+    def zscore(self, key: str, member: str) -> PipelineCommands: ...
+    def zunion(
+        self,
+        keys: List[str],
+        weights: Optional[List[float]] = None,
+        aggregate: Optional[Literal["SUM", "MIN", "MAX"]] = None,
+        withscores: bool = False,
+    ) -> PipelineCommands: ...
+    def zunionstore(
+        self,
+        destination: str,
+        keys: List[str],
+        weights: Optional[List[float]] = None,
+        aggregate: Optional[Literal["SUM", "MIN", "MAX"]] = None,
+    ) -> PipelineCommands: ...
+    def append(self, key: str, value: str) -> PipelineCommands: ...
+    def decr(self, key: str) -> PipelineCommands: ...
+    def decrby(self, key: str, decrement: int) -> PipelineCommands: ...
+    def get(self, key: str) -> PipelineCommands: ...
+    def getdel(self, key: str) -> PipelineCommands: ...
+    def getex(
+        self,
+        key: str,
+        ex: Optional[int] = None,
+        px: Optional[int] = None,
+        exat: Optional[int] = None,
+        pxat: Optional[int] = None,
+        persist: Optional[bool] = None,
+    ) -> PipelineCommands: ...
+    def getrange(self, key: str, start: int, end: int) -> PipelineCommands: ...
+    def getset(self, key: str, value: ValueT) -> PipelineCommands: ...
+    def incr(self, key: str) -> PipelineCommands: ...
+    def incrby(self, key: str, increment: int) -> PipelineCommands: ...
+    def incrbyfloat(self, key: str, increment: float) -> PipelineCommands: ...
+    def mget(self, *keys: str) -> PipelineCommands: ...
+    def mset(self, values: Mapping[str, ValueT]) -> PipelineCommands: ...
+    def msetnx(self, values: Mapping[str, ValueT]) -> PipelineCommands: ...
+    def psetex(self, key: str, milliseconds: int, value: str) -> PipelineCommands: ...
+    def set(
+        self,
+        key: str,
+        value: ValueT,
+        nx: bool = False,
+        xx: bool = False,
+        get: bool = False,
+        ex: Optional[int] = None,
+        px: Optional[int] = None,
+        exat: Optional[int] = None,
+        pxat: Optional[int] = None,
+        keepttl: bool = False,
+    ) -> PipelineCommands: ...
+    def setex(self, key: str, seconds: int, value: ValueT) -> PipelineCommands: ...
+    def setnx(self, key: str, value: ValueT) -> PipelineCommands: ...
+    def setrange(self, key: str, offset: int, value: str) -> PipelineCommands: ...
+    def strlen(self, key: str) -> PipelineCommands: ...
+    def substr(self, key: str, start: int, end: int) -> PipelineCommands: ...
+    def script_exists(self, *sha1: str) -> PipelineCommands: ...
+    def script_flush(
+        self, flush_type: Optional[Literal["ASYNC", "SYNC"]] = None
+    ) -> PipelineCommands: ...
+    def script_load(self, script: str) -> PipelineCommands: ...
```

### Comparing `upstash_redis-1.0.0/upstash_redis/format.py` & `upstash_redis-1.1.0/upstash_redis/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Callable, Dict, List, Literal, Optional, Tuple, Union
 
 from upstash_redis.utils import GeoSearchResult
+from upstash_redis.typing import RESTResultT
 
 
 def list_to_dict(raw: List, command=None) -> Dict:
     """
     Convert a list that contains ungrouped pairs as consecutive elements (usually field-value or similar) into a dict.
     """
 
@@ -324,7 +325,27 @@
     "MSET": ok_to_bool,
     "MSETNX": to_bool,
     "HMSET": ok_to_bool,
     "LSET": ok_to_bool,
     "SCRIPT FLUSH": ok_to_bool,
     "SCRIPT EXISTS": list_to_bool_list,
 }
+
+def cast_response(command: List[str], response: RESTResultT):
+    """
+    Given a command and its response, casts the response using the `FORMATTERS`
+    map
+
+    :param command: Used to determine the formatting to apply
+    :param response: Response to format 
+    """
+
+    # get main command
+    main_command = command[0]
+    if len(command) > 1 and main_command == "SCRIPT":
+        main_command = f"{main_command} {command[1]}"
+
+    # format response
+    if main_command in FORMATTERS:
+        return FORMATTERS[main_command](response, command)
+    
+    return response
```

### Comparing `upstash_redis-1.0.0/upstash_redis/http.py` & `upstash_redis-1.1.0/upstash_redis/http.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import time
 from asyncio import sleep
 from base64 import b64decode
 from json import dumps
 from platform import python_version
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional, Union
 
 from aiohttp import ClientSession
 from requests import Session
 
 from upstash_redis import __version__
 from upstash_redis.errors import UpstashError
 from upstash_redis.typing import RESTResultT
@@ -44,37 +44,29 @@
     session: ClientSession,
     url: str,
     headers: Dict[str, str],
     encoding: Optional[Literal["base64"]],
     retries: int,
     retry_interval: float,
     command: List,
-) -> RESTResultT:
+    from_pipeline: bool = False
+) -> Union[RESTResultT, List[RESTResultT]]:
     """
     Execute the given command over the REST API.
 
     :param encoding: the encoding that can be used by the REST API to parse the response before sending it
     :param retries: how many times an HTTP request will be retried if it fails
     :param retry_interval: how many seconds will be waited between each retry
     :param allow_telemetry: whether anonymous telemetry can be collected
     """
 
     # Serialize the command; more specifically, write string-incompatible types as JSON strings.
-    command = [
-        element
-        if (
-            isinstance(element, str)
-            or isinstance(element, int)
-            or isinstance(element, float)
-        )
-        else dumps(element)
-        for element in command
-    ]
+    command = _format_command(command, from_pipeline=from_pipeline)
 
-    response: Optional[Dict[str, Any]] = None
+    response: Optional[Union[Dict, List[Dict]]] = None
     last_error: Optional[Exception] = None
 
     for attempts_left in range(max(0, retries), -1, -1):
         try:
             async with session.post(url, headers=headers, json=command) as r:
                 response = await r.json()
                 break  # Break the loop as soon as we receive a proper response
@@ -86,44 +78,34 @@
 
     if response is None:
         assert last_error is not None
 
         # Exhausted all retries, but no response is received
         raise last_error
 
-    if response.get("error"):
-        raise UpstashError(response["error"])
-
-    result = response["result"]
-
-    if encoding == "base64":
-        return decode(result)
-
-    return result
+    if not from_pipeline:
+        return format_response(response, encoding) # type: ignore[arg-type]
+    else:
+        return [
+            format_response(sub_response, encoding)
+            for sub_response in response
+        ]
 
 
 def sync_execute(
     session: Session,
     url: str,
     headers: Dict[str, str],
     encoding: Optional[Literal["base64"]],
     retries: int,
     retry_interval: float,
     command: List[Any],
-) -> RESTResultT:
-    command = [
-        element
-        if (
-            isinstance(element, str)
-            or isinstance(element, int)
-            or isinstance(element, float)
-        )
-        else dumps(element)
-        for element in command
-    ]
+    from_pipeline: bool = False
+) -> Union[RESTResultT, List[RESTResultT]]:
+    command = _format_command(command, from_pipeline=from_pipeline)
 
     response: Optional[Dict[str, Any]] = None
     last_error: Optional[Exception] = None
 
     for attempts_left in range(max(0, retries), -1, -1):
         try:
             response = session.post(url, headers=headers, json=command).json()
@@ -136,17 +118,34 @@
 
     if response is None:
         assert last_error is not None
 
         # Exhausted all retries, but no response is received
         raise last_error
 
+    if not from_pipeline:
+        return format_response(response, encoding)
+    else:
+        return [
+            format_response(sub_response, encoding) # type: ignore[arg-type]
+            for sub_response in response
+        ]
+
+def format_response(
+        response: Dict[str, Any],
+        encoding: Optional[Literal["base64"]]
+) -> RESTResultT:
+    """
+    Raise exception if the response is an error
+
+    Otherwise, decode if an encoding was used
+    """
     if response.get("error"):
         raise UpstashError(response["error"])
-
+    
     result = response["result"]
 
     if encoding == "base64":
         return decode(result)
 
     return result
 
@@ -164,7 +163,28 @@
         return [
             # Decode recursively.
             decode(element)
             for element in raw
         ]
     else:
         raise UpstashError(f"Error decoding data for result type {str(type(raw))}")
+
+
+def _format_command(command: List[Any], from_pipeline: bool = False):
+    """
+    Format command
+
+    If not from_pipeline, treat the command as a single command. Otherwise,
+    treat it as a list of commands
+    """
+    if from_pipeline:
+        return [
+            _format_command(command=pipeline_command, from_pipeline=False)
+            for pipeline_command in command
+        ]
+    
+    return [
+        element
+        if isinstance(element, (str, int, float))
+        else dumps(element)
+        for element in command
+    ]
```

### Comparing `upstash_redis-1.0.0/upstash_redis/typing.py` & `upstash_redis-1.1.0/upstash_redis/typing.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-1.0.0/upstash_redis/utils.py` & `upstash_redis-1.1.0/upstash_redis/utils.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-1.0.0/PKG-INFO` & `upstash_redis-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 1.0.0
+Version: 1.1.0
 Summary: Serverless Redis SDK from Upstash
 Home-page: https://github.com/upstash/redis-python
 License: MIT
 Keywords: Upstash Redis,Serverless Redis
 Author: Upstash
 Author-email: support@upstash.com
 Maintainer: Upstash
@@ -29,14 +29,19 @@
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/upstash/redis-python
 Description-Content-Type: text/markdown
 
 # Upstash Redis Python SDK
 
+> [!NOTE]  
+> **This project is in GA Stage.**
+>
+> The Upstash Professional Support fully covers this project. It receives regular updates, and bug fixes. The Upstash team is committed to maintaining and improving its functionality.
+
 upstash-redis is a connectionless, HTTP-based Redis client for Python, designed to be used in serverless and serverful environments such as:
 - AWS Lambda
 - Vercel Serverless
 - Google Cloud Functions
 - and other environments where HTTP is preferred over TCP.
 
 Inspired by other Redis clients like [@upstash/redis](https://github.com/upstash/upstash-redis) and [redis-py](https://github.com/redis/redis-py),
@@ -144,14 +149,62 @@
 If you want to run a command that hasn't been implemented, you can use the `execute` function of your client instance
 and pass the command as a `list`.
 
 ```python
 redis.execute(command=["XLEN", "test_stream"])
 ```
 
+### Pipelines & Transactions
+
+If you want to submit commands in batches to reduce the number of roundtrips, you can utilize pipelining or
+transactions. The difference between pipelines and transactions is that transactions are atomic: no other
+command is executed during that transaction. In pipelines there is no such guarantee.
+
+To use a pipeline, simply call the `pipeline` method:
+
+```python
+pipeline = redis.pipeline()
+
+pipeline.set("foo", 1)
+pipeline.incr("foo")
+pipeline.get("foo")
+
+result = pipeline.exec()
+
+print(result)
+# prints [True, 2, '2']
+```
+
+For transaction, use `mutli`:
+
+```python
+pipeline = redis.multi()
+
+pipeline.set("foo", 1)
+pipeline.incr("foo")
+pipeline.get("foo")
+
+result = pipeline.exec()
+
+print(result)
+# prints [True, 2, '2']
+```
+
+You can also chain the commands:
+
+```python
+pipeline = redis.pipeline()
+
+pipeline.set("foo", 1).incr("foo").get("foo")
+result = pipeline.exec()
+
+print(result)
+# prints [True, 2, '2']
+```
+
 # Encoding
 Although Redis can store invalid JSON data, there might be problems with the deserialization.
 To avoid this, the Upstash REST proxy is capable of encoding the data as base64 on the server and then sending it to the client to be
 decoded. 
 
 For very large data, this can add a few milliseconds in latency. So, if you're sure that your data is valid JSON, you can set
 `rest_encoding` to `None`.
@@ -170,7 +223,8 @@
 ## Running tests
 To run all the tests, make sure the poetry virtual environment activated with all 
 the necessary dependencies. Set the `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` environment variables and run:
 
 ```bash
 poetry run pytest
 ```
+
```

