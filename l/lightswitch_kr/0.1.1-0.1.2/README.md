# Comparing `tmp/lightswitch_kr-0.1.1.tar.gz` & `tmp/lightswitch_kr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightswitch_kr-0.1.1.tar", max compression
+gzip compressed data, was "lightswitch_kr-0.1.2.tar", max compression
```

## Comparing `lightswitch_kr-0.1.1.tar` & `lightswitch_kr-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-22 07:52:34.932538 lightswitch_kr-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      452 2024-05-14 12:10:46.527767 lightswitch_kr-0.1.1/lightswitch/__init__.py
--rw-r--r--   0        0        0     3498 2024-05-08 02:36:11.635497 lightswitch_kr-0.1.1/lightswitch/custom_sseclient.py
--rw-r--r--   0        0        0     1587 2024-05-13 01:44:03.193340 lightswitch_kr-0.1.1/lightswitch/exceptions.py
--rw-r--r--   0        0        0    10500 2024-05-10 08:10:17.254557 lightswitch_kr-0.1.1/lightswitch/lightswitch.py
--rw-r--r--   0        0        0     7668 2024-05-10 07:30:44.698548 lightswitch_kr-0.1.1/lightswitch/models.py
--rw-r--r--   0        0        0     2312 2024-05-10 06:30:25.904886 lightswitch_kr-0.1.1/lightswitch/stream_manager.py
--rw-r--r--   0        0        0     1670 2024-05-13 01:09:52.189173 lightswitch_kr-0.1.1/lightswitch/utils.py
--rw-r--r--   0        0        0      901 2024-05-14 12:12:16.245672 lightswitch_kr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 07:44:45.572583 lightswitch_kr-0.1.1/README.md
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 lightswitch_kr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2024-05-16 05:15:34.401889 lightswitch_kr-0.1.2/lightswitch/__init__.py
+-rw-r--r--   0        0        0     3103 2024-05-14 07:02:02.552428 lightswitch_kr-0.1.2/lightswitch/custom_sseclient.py
+-rw-r--r--   0        0        0     1587 2024-05-13 01:44:03.193340 lightswitch_kr-0.1.2/lightswitch/exceptions.py
+-rw-r--r--   0        0        0     9768 2024-05-16 05:41:52.140479 lightswitch_kr-0.1.2/lightswitch/lightswitch.py
+-rw-r--r--   0        0        0     6308 2024-05-16 05:28:43.310887 lightswitch_kr-0.1.2/lightswitch/models.py
+-rw-r--r--   0        0        0     1906 2024-05-14 07:02:02.552428 lightswitch_kr-0.1.2/lightswitch/stream_manager.py
+-rw-r--r--   0        0        0      617 2024-05-14 07:01:59.092132 lightswitch_kr-0.1.2/lightswitch/utils.py
+-rw-r--r--   0        0        0      901 2024-05-16 05:47:31.783393 lightswitch_kr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 05:46:46.226828 lightswitch_kr-0.1.2/README.md
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 lightswitch_kr-0.1.2/PKG-INFO
```

### Comparing `lightswitch_kr-0.1.1/lightswitch/custom_sseclient.py` & `lightswitch_kr-0.1.2/lightswitch/custom_sseclient.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,36 +57,28 @@
     @classmethod
     def parse(cls, raw):
         """
         Given a possibly-multiline string representing an SSE message, parse it
         and return an Event object.
         """
         msg = cls()
-        # print("raw : ", raw)
         raw = raw.replace('\r\n', '')
-        # test = codecs.decode(raw, 'unicode_escape')
-        # print("test:", test)
         for line in raw.splitlines():
             line = line.encode('latin1').decode('utf-8')
-            # print("test : ", line)
             m = cls.sse_line_pattern.match(line)
             if m is None:
-                # Malformed line.  Discard but warn.
                 warnings.warn('Invalid SSE line: "%s"' % line, SyntaxWarning)
                 continue
 
             name = m.group('name')
             if name == '':
-                # line began with a ":", so is a comment.  Ignore
                 continue
             value = m.group('value')
 
             if name == 'data':
-                # If we already have some data, then join to it with a newline.
-                # Else this is it.
                 if msg.data:
                     msg.data = '%s\n%s' % (msg.data, value)
                 else:
                     if '{' in value:
                         index = value.find('{')
                         msg.data = value[index:-1]
                     else:
```

### Comparing `lightswitch_kr-0.1.1/lightswitch/exceptions.py` & `lightswitch_kr-0.1.2/lightswitch/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightswitch_kr-0.1.1/lightswitch/lightswitch.py` & `lightswitch_kr-0.1.2/lightswitch/lightswitch.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 from .models import Flags, Flag, LSUser
 from .stream_manager import StreamManager, StreamEvent
-from .exceptions import StreamDataError, LSServerError, LSTypeCastError
+from .exceptions import StreamDataError, LSServerError, LSTypeCastError, LSFlagNotFoundError
 
 
 DEFAULT_API_URL = 'http://localhost:8000/api/v1/'
 DEFAULT_REALTIME_API_URL = 'http://localhost:8000/api/v1/sse/subscribe'
 JsonType = typing.Union[
     None,
     int,
@@ -28,23 +28,19 @@
     lightswitch http API와 통신하는 interface를 제공
     """
     _instance = None
     flags: typing.Optional[Flags] = None
     environment_key: typing.Optional[str] = None
 
     @classmethod
-    def get_instance(cls, **kwargs):  # 싱글톤 인스턴스를 반환
+    def get_instance(cls, **kwargs):
         if cls._instance is None:
             cls._instance = cls(**kwargs)
         return cls._instance
 
-    # 초기화할 때
-    # 1.모든 플래그를 가져와서 저장
-    # 2.sdk 키로 subscribe post 해서 userkey 받고 : api/v1/sse/subscribe
-    # 3.subscribe/userkey 로 sse 연결
     def __init__(
         self,
         api_url: typing.Optional[str] = None,
         sse_realtime_api_url: typing.Optional[str] = None,
         request_timeout_seconds: typing.Optional[int] = None,
         update_frequency_seconds:typing.Union[int, float] = 10,
         retries: typing.Optional[Retry] = None,
@@ -62,21 +58,19 @@
 
         sse_realtime_api_url = sse_realtime_api_url or DEFAULT_REALTIME_API_URL
         self.sse_realtime_api_url = sse_realtime_api_url
 
         self.request_timeout_seconds = request_timeout_seconds
         self.session.mount(self.api_url, HTTPAdapter(max_retries=retries))
 
-        # event 처리 함수
         self.handle_event = self.process_stream_event_update
 
-        # 필요 시 api_url 이외의 url 속성 할당
-        self.environment_url = f"{self.api_url}environment"
-        self.environment_flags_url = f"{self.api_url}sdk/init"  # 현재는 이 주소만 정의됨 - 현재 환경의 모든 플래그 가져오기
-        self.identity_flags_url = f"{self.api_url}identity"
+        # self.environment_url = f"{self.api_url}environment"
+        self.environment_flags_url = f"{self.api_url}sdk/init"
+        # self.identity_flags_url = f"{self.api_url}identity"
 
         self.user_key = None
         self.stream_manager = None
 
     def init(self, environment_key: str) -> None:
         self.environment_key = environment_key
         self._initialize_environment(environment_key)
@@ -87,15 +81,14 @@
         self.stream_manager = StreamManager(
             stream_url=self.sse_realtime_api_url + "/" + user_key,
             on_event=self.handle_event,
             request_timeout_seconds=self.request_timeout_seconds,
         )
         self.stream_manager.start()
 
-    # sdk 키로 subscribe post 해서 userkey 받기
     def _get_user_key(self, environment_key):
         headers = {
             'Content-Type': 'application/json',
         }
         payload = {
             'sdkKey': environment_key
         }
@@ -113,108 +106,111 @@
             f"userKey를 받아오는 데 실패했습니다. "
             f"Response status code: {response.status_code}"
         )
 
     def _initialize_environment(self, environment_key: typing.Optional[str]) -> None:
         Lightswitch.flags = self._get_all_environment_flags_from_api(environment_key)
 
-    # 새로운 SSE event를 받았을 때 EventStreamManager 스레드에 의해 호출되는 메서드
-    # SSE 응답을 매개변수로 받아 이벤트 타입에 따라 플래그 목록을 동기화
-    '''
-    response 형식은 다음과 같음
-    {
-      "userKey": "string",
-      "type": "CREATE",
-      "data": {}
-    }
-    '''
     def process_stream_event_update(self, event: StreamEvent) -> None:
         try:
             new_stream_event = json.loads(event.data)
-            print("new_stream_event : ", new_stream_event)
-            event_type = new_stream_event.get('type')  # 예를 들어 CREATE
-            print("event-type : ", event_type)
+            # print("new_stream_event : ", new_stream_event)
+            event_type = new_stream_event.get('type')
+            # print("event-type : ", event_type)
             new_flag_data = new_stream_event['data']
-            print("new_flag_data : ", new_flag_data)
+            # print("new_flag_data : ", new_flag_data)
 
             if event_type == "CREATE":
                 new_flag = Flag.flag_from_api(new_flag_data)
                 self.add_flag(new_flag)
 
             elif event_type == "UPDATE":
                 new_flag = Flag.flag_from_api(new_flag_data)
                 title = new_flag.title
                 self.update_flag(title, new_flag)
 
             elif event_type == "SWITCH":
                 self.toggle_flag(new_flag_data)
-            else:  # DELETE
+
+            else:
                 self.delete_flag(new_flag_data['title'])
 
         except json.JSONDecodeError as e:
             raise StreamDataError(
                 "new_stream_event로부터 유효한 json 데이터를 가져오는데 실패하였습니다."
             ) from e
 
     def add_flag(self, new_flag: Flag):
         if self.flags is None:
             self.flags = Flags()
-        # flags에 플래그 추가
         self.flags.add_flag(new_flag)
 
     def update_flag(self, title, new_data):
         self.flags.update_flag_value(title, new_data)
 
     def delete_flag(self, title):
         self.flags.delete_flag_by_name(title)
 
     def toggle_flag(self, new_flag):  # 플래그 활성화 상태 변경
         self.flags.toggle_flag_activation(new_flag)
 
-    # 해당 환경의 플래그 데이터 모두 가져오기
     def _get_all_environment_flags_from_api(self, environment_key) -> Flags:
         try:
             data = {
                 "sdkKey": environment_key
             }
             json_response: typing.List[typing.Mapping[str, JsonType]] = (
                 self._get_json_response(url=self.environment_flags_url, method="POST", body=data)['data']
             )
             return Flags.flags_from_api(
                 flags_data=json_response
             )
         except json.JSONDecodeError as e:
-            # logging.error(f"API 요청 중 에러 발생: {e}")
             raise LSServerError(
                 "LightSwitch 서버와 통신에 실패했습니다."
                 "응답 데이터가 유효한 JSON 타입이 아닙니다."
             ) from e
 
-    # 플래그 이름과 유저 모델 받아서 해당 유저의 플래그 변량 반환
     def get_flag(self, flag_title: str, user: LSUser, default_value: typing.Any) -> typing.Any:
-        flag = self.flags.get_flag_by_name(flag_title)
+        try:
+            flag = self.flags.get_flag_by_name(flag_title)
+        except LSFlagNotFoundError:
+            return default_value
+
         value_if_is_targeted = flag.get_user_variation_by_keyword(user)
-        if not value_if_is_targeted:  # 키워드에 해당하지 않으면
+        if value_if_is_targeted == "not targeted":
             return flag.get_user_variation_by_percentile(user)
         return value_if_is_targeted
 
     def get_boolean_flag(self, flag_title: str, user: LSUser, default_value: bool) -> bool:
-        flag = self.flags.get_flag_by_name(flag_title)
+        try:
+            flag = self.flags.get_flag_by_name(flag_title)
+        except LSFlagNotFoundError:
+            return default_value
+
         if flag.type != "BOOLEAN":
             raise LSTypeCastError(flag_title, "BOOLEAN")
         return self.get_flag(flag_title, user, default_value)
 
     def get_number_flag(self, flag_title: str, user: LSUser, default_value: int) -> int:
-        flag = self.flags.get_flag_by_name(flag_title)
+        try:
+            flag = self.flags.get_flag_by_name(flag_title)
+        except LSFlagNotFoundError:
+            return default_value
+
         if flag.type != "INTEGER":
             raise LSTypeCastError(flag_title, "INTEGER")
         return self.get_flag(flag_title, user, default_value)
 
     def get_string_flag(self, flag_title: str, user: LSUser, default_value: str) -> str:
-        flag = self.flags.get_flag_by_name(flag_title)
+        try:
+            flag = self.flags.get_flag_by_name(flag_title)
+        except LSFlagNotFoundError:
+            return default_value
+
         if flag.type != "STRING":
             raise LSTypeCastError(flag_title, "STRING")
         return self.get_flag(flag_title, user, default_value)
 
     def _get_json_response(
         self,
         url: str,
@@ -263,7 +259,8 @@
 
         # 그 외 모든 정보 초기화
         self.user_key = None
 
         # 세션 종료
         self.session.close()
 
+
```

### Comparing `lightswitch_kr-0.1.1/lightswitch/models.py` & `lightswitch_kr-0.1.2/lightswitch/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,125 +3,123 @@
 import json
 import typing
 from dataclasses import dataclass, field
 
 from .exceptions import LSFlagNotFoundError
 from .utils import get_hashed_percentage_for_object_ids
 
+
 # 데이터 모델 정의
 @dataclass
 class LSUser:
     user_id: str
     property: typing.Dict[str, str] = field(default_factory=dict)
 
     def set_property(self, key: str, value: str) -> 'LSUser':
         self.property[key] = value
         return self
 
 
 @dataclass
 class Property:
-    property_name: str  # "관리자 아이디"(식별자)
-    data: str  # 아이디 값 - ex) "3"
+    property_name: str
+    data: str
 
 
 @dataclass
 class Keyword:
     property_list: typing.List[Property]
     description: str
     value: str
 
 
 @dataclass
-class Context:  # variation과 동일
+class Context:
     value: str
     portion: int
     description: str
 
 
 @dataclass
 class Flag:
     flag_id: int
     title: str
     description: str
     type: str
-    keywords: typing.List[Keyword]  # 타겟 테스팅 조건 데이터
+    keywords: typing.List[Keyword]
     default_value: str
     default_value_portion: int
     default_value_description: str
-    variations: typing.List[Context]  # 그룹 분배 테스트 조건 데이터
+    variations: typing.List[Context]
     maintainer_id: int
     created_at: str
     updated_at: str
     delete_at: str
     active: bool
 
     def get_attribute_value(self, attribute: str):
         try:
             return getattr(self, attribute)
         except AttributeError as exc:
-            raise AttributeError(f"Attribute '{attribute}' 은 해당 플래그에 존재하지 않습니다.") from exc
+            raise AttributeError(f"Attribute '{attribute}' 은(는) 해당 플래그에 존재하지 않습니다.") from exc
 
-    # 플래그의 키워드를 확인, 해당 유저가 타겟팅되어 있으면 그에 맞는 값을 반환, 아니면 플래그 기본값
     def get_user_variation_by_keyword(self, user: LSUser) -> typing.Any:
         flag_keywords = self.keywords
-        for keyword in flag_keywords:  # keyword는 OR
+        if len(flag_keywords) == 0:
+            return "not targeted"
+        
+        for keyword in flag_keywords:
             is_targeted = True
-            for prop in keyword.get('properties', []):  # prop은 AND -> 모든 prop 조건에 해당하는지 확인
-                user_has_the_key = prop['property'] in user.property  # 유저 속성에 키워드의 키가 존재하는지 여부
+            for prop in keyword.get('properties', []):
+                user_has_the_key = prop['property'] in user.property
                 if user_has_the_key and prop['data'] == user.property[prop['property']]:
                     continue
                 else:
                     is_targeted = False
                     break
-            # prop의 모든 조건을 만족하는 경우
+
             if is_targeted:
-                value = self.convert_value(keyword.get('value'))  # 처음 만족하는 조건의 값을 반환
+                value = self.convert_value(keyword.get('value'))
                 return value
 
-
-
-    # 플래그의 context를 확인, 유저의 백분율 값을 계산하여 어디에 속하는지 확인
     def get_user_variation_by_percentile(self, user: LSUser) -> str:
-        # 유저의 백분율값을 계산(유저 식별자와 플래그 식별자 함께 사용 : 플래그마다 다른 백분율값을 갖게 하기 위함)
-        user_percentile=get_hashed_percentage_for_object_ids([f"{user.user_id}", "self.flag_id"])
-
+        user_percentile = get_hashed_percentage_for_object_ids([f"{user.user_id}", "self.flag_id"])
+        print("user percentile : ", user_percentile)
         start_percentage = 0  # 시작 percentile
         for context in sorted(self.variations, key=lambda context: context['portion']):
             limit = start_percentage + context['portion']
             if start_percentage <= user_percentile < limit:
                 value = self.convert_value(context['value'])
                 return value
 
             start_percentage = limit
 
         return self.default_value
 
-    def convert_value(self, value: str) -> typing.Any:  # 형변환 이후에 반환
+    def convert_value(self, value: str) -> typing.Any:
         """
         value를 flag 타입에 따라 적절한 데이터 타입으로 변환하여 반환합니다.
         """
         if self.type == "BOOLEAN":
             return bool(value)
         if self.type == "INTEGER":
             return int(value)
         if self.type == "JSON":
             try:
                 return json.loads(value)
-            except json.JSONDecodeError:  # 디코딩 에러 발생 시에는 그대로 반환
+            except json.JSONDecodeError:
                 return value
         if self.type == "STRING":
             return str(value)
         return value
 
-    # SSE flag_data를 기반으로 인스턴스 생성
     @classmethod
     def flag_from_api(
             cls,
-            flag_data: typing.Mapping[str, typing.Any]  # 딕셔너리 형식의 인자를 받음
+            flag_data: typing.Mapping[str, typing.Any]
     ) -> Flag:
         return Flag(
             flag_id=flag_data["flagId"],
             title=flag_data["title"],
             description=flag_data["description"],
             type=flag_data["type"],
             keywords=flag_data.get("keywords", []),
@@ -132,77 +130,69 @@
             maintainer_id=flag_data["maintainerId"],
             created_at=flag_data["createdAt"],
             updated_at=flag_data["updatedAt"],
             delete_at=flag_data["deleteAt"],
             active=flag_data["active"],
         )
 
-    # 해당 플래그의 keyword 가져오기
     def get_keywords(self) -> typing.List[Keyword]:
         return self.keywords
 
-    # 해당 플래그의 context 가져오기
     def get_contexts(self) -> typing.List[Context]:
         return self.variations
 
 
 @dataclass
 class Flags:
-    flags: typing.Dict[str, Flag] = field(default_factory=dict)  # "기능 이름" : "Flag객체" 형식으로 개별 기능을 저장
+    flags: typing.Dict[str, Flag] = field(default_factory=dict)
 
     @classmethod
     def flags_from_api(
             cls,
             flags_data: typing.Sequence[typing.Mapping[str, typing.Any]]
     ) -> Flags:
         flags = {
             flag_data["title"]: Flag.flag_from_api(flag_data)
             for flag_data in flags_data
         }
-        # Flags 인스턴스를 반환
         return cls(
             flags=flags
         )
 
     def get_all_flags(self) -> typing.List[Flag]:
-        return list(self.flags.values())  # Flag 인스턴스의 리스트 반환
+        return list(self.flags.values())
 
-    def is_feature_enabled(self, feature_name: str) -> bool:  # 플래그 활성화 여부 리턴
+    def is_feature_enabled(self, feature_name: str) -> bool:
         return self.get_flag_by_name(feature_name).active
 
-    def get_feature_value_by_name(self, feature_name: str) -> typing.Any:  # 기본값 리턴
+    def get_feature_value_by_name(self, feature_name: str) -> typing.Any:
         return self.get_flag_by_name(feature_name).default_value
 
     def get_flag_by_name(self, feature_name: str) -> Flag:
         try:
             flag = self.flags[feature_name]
         except KeyError as exc:
             raise LSFlagNotFoundError(feature_name) from exc
         return flag
 
-    # event 타입에 따라 수행할 메서드
     def add_flag(self, new_flag: Flag):
         self.flags[new_flag.title] = new_flag
-        print('flag created.')
 
     def update_flag_value(self, flag_name: str, new_value: typing.Any):
-        if flag_name in self.flags:
+        try:
             self.flags[flag_name].default_value = new_value
-            print('flag updated.')
-        else:
-            raise FeatureNotFoundError(flag_name)
+        except KeyError as exc:
+            raise LSFlagNotFoundError(flag_name) from exc
 
     def delete_flag_by_name(self, flag_name: str):
-        if flag_name in self.flags:
+        try:
             del self.flags[flag_name]
-            print('flag deleted.')
-        else:
-            raise FeatureNotFoundError(flag_name)
+        except KeyError as exc:
+            raise LSFlagNotFoundError(flag_name) from exc
 
     def toggle_flag_activation(self, new_flag: typing.Dict[str, typing.Any]):
         flag_title = new_flag["title"]
         flag_is_active = new_flag["active"]
-        if flag_title in self.flags:
+        try:
             self.flags[flag_title].active = flag_is_active
-            print("flag toggled.")
-        else:
-            raise FeatureNotFoundError(flag_title)
+        except KeyError as exc:
+            raise LSFlagNotFoundError(flag_title) from exc
```

### Comparing `lightswitch_kr-0.1.1/lightswitch/stream_manager.py` & `lightswitch_kr-0.1.2/lightswitch/stream_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,42 +21,38 @@
         *args: typing.Any,
         stream_url: str,
         on_event: Callable[[StreamEvent], None],
         request_timeout_seconds: Optional[int] = None,
         **kwargs: typing.Any
     ) -> None:
         super().__init__(*args, **kwargs)
-        # self.lightswitch = lightswitch
-        self._stop_event = threading.Event()  # threading event로 초기화(스레드의 lifecycle을 관리하기 위함)
+        self._stop_event = threading.Event()
         self.stream_url = stream_url
-        self.on_event = on_event # 이벤트 발생 시 호출될 함수
+        self.on_event = on_event
         self.request_timeout_seconds = request_timeout_seconds
 
     def run(self) -> None:
         while not self._stop_event.is_set():
             try:
                 sse_client = CustomSSEClient(self.stream_url, headers={"Accept": "application/json, text/event-stream"}, timeout=None)
 
                 for event in sse_client:
-                    # print("event 발생!", event, "여기까지 EVENT")
-                    if hasattr(event, 'event'):
-                        print(f"Event: {event.event}")
-                    if hasattr(event, 'data'):
-                        print(f"Data: {event.data}")
-                    if hasattr(event, 'type'):
-                        print(f"Type: {event.type}")
-                    if event.data.strip():  # data 내용이 있는 경우에만
-                        # print("이벤트 발생")
-                        if event.data != 'SSE connected':
-                            self.on_event(event)  # process_stream_event_update() 호출
+                    # if hasattr(event, 'event'):
+                    #     print(f"Event: {event.event}")
+                    # if hasattr(event, 'data'):
+                    #     print(f"Data: {event.data}")
+                    # if hasattr(event, 'type'):
+                    #     print(f"Type: {event.type}")
+                    if event.data.strip():
+                        if event.data != 'SSE connected':  # 수정 필요
+                            self.on_event(event)
 
             except requests.exceptions.ReadTimeout:
                 pass
             except (StreamDataError, requests.RequestException):
                 logger.exception('Error while streaming data')
 
-    # run 메서드의 루프를 종료시키고 스레드도 종료
     def stop(self) -> None:
         self._stop_event.set()
 
     def __del__(self) -> None:
-        self._stop_event.set()
+        self._stop_event.set()
```

### Comparing `lightswitch_kr-0.1.1/pyproject.toml` & `lightswitch_kr-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightswitch_kr"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple SDK for your API"
 authors = ["sumtuckyi <sumin510@naver.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [
   {include = "lightswitch"},
 ]
```

### Comparing `lightswitch_kr-0.1.1/PKG-INFO` & `lightswitch_kr-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightswitch_kr
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple SDK for your API
 License: MIT
 Author: sumtuckyi
 Author-email: sumin510@naver.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

