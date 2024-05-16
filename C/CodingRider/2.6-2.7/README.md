# Comparing `tmp/codingrider-2.6.tar.gz` & `tmp/codingrider-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codingrider-2.6.tar", last modified: Tue May 14 03:57:30 2024, max compression
+gzip compressed data, was "codingrider-2.7.tar", last modified: Thu May 16 07:04:14 2024, max compression
```

## Comparing `codingrider-2.6.tar` & `codingrider-2.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:57:30.340740 codingrider-2.6/
-drwxrwxrwx   0        0        0        0 2024-05-14 03:57:30.331437 codingrider-2.6/CodingRider/
--rw-rw-rw-   0        0        0      109 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      484 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/crc.py
--rw-rw-rw-   0        0        0    44020 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/drone.py
--rw-rw-rw-   0        0        0    73925 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     1904 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10251 2024-05-14 03:51:54.000000 codingrider-2.6/CodingRider/system.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:57:30.339231 codingrider-2.6/CodingRider/tools/
--rw-rw-rw-   0        0        0       33 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/tools/__init__.py
--rw-rw-rw-   0        0        0    31268 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/tools/parser.py
--rw-rw-rw-   0        0        0     9491 2024-05-14 03:14:00.000000 codingrider-2.6/CodingRider/tools/update.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:57:30.339735 codingrider-2.6/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      718 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 03:57:30.000000 codingrider-2.6/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-14 03:14:00.000000 codingrider-2.6/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-14 03:14:00.000000 codingrider-2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      718 2024-05-14 03:57:30.340740 codingrider-2.6/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-05-14 03:14:00.000000 codingrider-2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 03:57:30.341882 codingrider-2.6/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-05-14 03:55:16.000000 codingrider-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:04:14.180271 codingrider-2.7/
+drwxrwxrwx   0        0        0        0 2024-05-16 07:04:14.156143 codingrider-2.7/CodingRider/
+-rw-rw-rw-   0        0        0      109 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    41310 2024-05-16 06:25:01.000000 codingrider-2.7/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    61138 2024-05-16 06:58:18.000000 codingrider-2.7/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1696 2024-05-16 06:55:33.000000 codingrider-2.7/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10845 2024-05-16 06:25:19.000000 codingrider-2.7/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:04:14.177445 codingrider-2.7/CodingRider/tools/
+-rw-rw-rw-   0        0        0       48 2024-05-14 06:50:08.000000 codingrider-2.7/CodingRider/tools/__init__.py
+-rw-rw-rw-   0        0        0    29709 2024-05-14 06:50:01.000000 codingrider-2.7/CodingRider/tools/parser.py
+-rw-rw-rw-   0        0        0     9495 2024-05-14 06:53:10.000000 codingrider-2.7/CodingRider/tools/update.py
+-rw-rw-rw-   0        0        0     9515 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/update.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:04:14.179254 codingrider-2.7/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      718 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-14 03:14:00.000000 codingrider-2.7/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-14 03:14:00.000000 codingrider-2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      718 2024-05-16 07:04:14.180271 codingrider-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-14 03:14:00.000000 codingrider-2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:04:14.181277 codingrider-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-05-16 07:04:07.000000 codingrider-2.7/setup.py
```

### Comparing `codingrider-2.6/CodingRider/crc.py` & `codingrider-2.7/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.6/CodingRider/drone.py` & `codingrider-2.7/CodingRider/drone.py`

 * *Files 5% similar despite different names*

```diff
@@ -288,17 +288,14 @@
 
         # 들어오는 데이터를 저장
         self._runHandler(header, dataArray)
 
         # 콜백 이벤트 실행
         self._runEventHandler(header.dataType)
 
-        # Monitor 데이터 처리
-        self._runHandlerForMonitor(header, dataArray)
-
         # 데이터 처리 완료 확인
         self._receiver.checked()
 
         return header.dataType
 
 
 
@@ -316,73 +313,15 @@
         if (isinstance(dataType, DataType)) and (self._eventHandler.d[dataType] != None) and (self._storage.d[dataType] != None):
             return self._eventHandler.d[dataType](self._storage.d[dataType])
         else:
             return None
 
 
 
-    def _runHandlerForMonitor(self, header, dataArray):
-        
-        # Monitor 데이터 처리
-        # 수신 받은 데이터를 파싱하여 self.monitorData[] 배열에 데이터를 넣음
-        if header.dataType == DataType.Monitor:
-            
-            monitorHeaderType = MonitorHeaderType(dataArray[0])
-
-            if monitorHeaderType == MonitorHeaderType.Monitor0:
-                
-                monitor0 = Monitor0.parse(dataArray[1:1 + Monitor0.getSize()])
-
-                if monitor0.monitorDataType == MonitorDataType.F32:
-                    
-                    dataCount = (dataArray.len() - 1 - Monitor0.getSize()) / 4
-
-                    for i in range(0, dataCount):
-                        
-                        if monitor0.index + i < len(self.monitorData):
-                            
-                            index = 1 + Monitor0.getSize() + (i * 4)
-                            self.monitorData[monitor0.index + i], = unpack('<f', dataArray[index:index + 4])
-
-            elif monitorHeaderType == MonitorHeaderType.Monitor4:
-                
-                monitor4 = Monitor4.parse(dataArray[1:1 + Monitor4.getSize()])
-
-                if monitor4.monitorDataType == MonitorDataType.F32:
-                    
-                    self.systemTimeMonitorData = monitor4.systemTime
-                    
-                    dataCount = (dataArray.len() - 1 - Monitor4.getSize()) / 4
-
-                    for i in range(0, dataCount):
-                        
-                        if monitor4.index + i < len(self.monitorData):
-                            
-                            index = 1 + Monitor4.getSize() + (i * 4)
-                            self.monitorData[monitor4.index + i], = unpack('<f', dataArray[index:index + 4])
-
-            elif monitorHeaderType == MonitorHeaderType.Monitor8:
-                
-                monitor8 = Monitor8.parse(dataArray[1:1 + Monitor8.getSize()])
-
-                if monitor8.monitorDataType == MonitorDataType.F32:
-                    
-                    self.systemTimeMonitorData = monitor8.systemTime
-                    
-                    dataCount = (dataArray.len() - 1 - Monitor8.getSize()) / 4
-
-                    for i in range(0, dataCount):
-                        
-                        if monitor8.index + i < len(self.monitorData):
-                            
-                            index = 1 + Monitor8.getSize() + (i * 4)
-                            self.monitorData[monitor8.index + i], = unpack('<f', dataArray[index:index + 4])
-
-
-
+   
     def setEventHandler(self, dataType, eventHandler):
         
         if (not isinstance(dataType, DataType)):
             return
 
         self._eventHandler.d[dataType] = eventHandler
```

### Comparing `codingrider-2.6/CodingRider/protocol.py` & `codingrider-2.7/CodingRider/protocol.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,100 +28,93 @@
 
 
 # DataType Start
 
 
 class DataType(Enum):
     
-    None_                       = 0x00      # 없음
+    None_						= 0x00		# 없음
+    Ping						= 0x01		# 통신 확인
+    Ack							= 0x02		# 데이터 수신에 대한 응답
+    Error						= 0x03		# 오류
+    Request						= 0x04		# 지정한 타입의 데이터 요청
+    Information					= 0x07		# 펌웨어 및 장치 정보
+    Control						= 0x10		# 조종
+    
+    Command						= 0x11		# 명령
+    Pairing						= 0x12		# 페어링
+    ResponseRate				= 0x13		# ResponseRate
     
-    Ping                        = 0x01      # 통신 확인
-    Ack                         = 0x02      # 데이터 수신에 대한 응답
-    Error                       = 0x03      # 오류(reserve, 비트 플래그는 추후에 지정)
-    Request                     = 0x04      # 지정한 타입의 데이터 요청
-    Message                     = 0x05      # 문자열 데이터
-    Address                     = 0x06      # 장치 주소(MAC이 있는 경우 MAC) 혹은 고유번호(MAC이 없는 경우 UUID)
-    Information                 = 0x07      # 펌웨어 및 장치 정보
-    Monitor                     = 0x0F      # 디버깅용 값 배열 전송. 첫번째 바이트에 타입, 두 번째 바이트에 페이지 지정(수신 받는 데이터의 저장 경로 구분)
-    Control                     = 0x10      # 조종
-
-    Command                     = 0x11      # 명령
-    Pairing                     = 0x12      # 페어링
-    Rssi                        = 0x13      # RSSI
-    
-    Battle                      = 0x1F      # 전투
-
     # Light
-    LightManual                 = 0x20      # LED 수동 제어
-    LightMode                   = 0x21      # LED 모드
-    LightEvent                  = 0x22      # LED 이벤트
-    LightDefault                = 0x23      # LED 초기 모드
-
+    LightManual					= 0x20		# LED 수동 제어
+    LightMode					= 0x21,		# LED 모드 지정
+    LightEvent					= 0x22,		# LED 이벤트
+    
     # 센서 RAW 데이터
-    RawMotion                   = 0x30      # Motion 센서 데이터 RAW 값
-
-    # 상태, 센서
-    State                       = 0x40      # 드론의 상태(비행 모드 방위기준 배터리량)
-    Altitude                    = 0x43      # 높이, 고도
-    Motion                      = 0x44      # Motion 센서 데이터 처리한 값(IMU)
-    VisionSensor				= 0x47,		# Vision Sensor X, Y, Z
-
+    RawMotion					= 0x30		# Motion 센서 데이터 RAW 값
+    
+    # 상태,  센서
+    State						= 0x40		# 드론의 상태(비행 모드, 방위기준, 배터리량)
+    Altitude					= 0x43		# 높이, 고도
+    Motion						= 0x44		# Motion 센서 데이터 처리한 값(IMU)
+    VisionSensor				= 0x47		# Vision Sensor X, Y, Z
+    
     # 설정
-    Count                       = 0x50      # 카운트
-    Trim                        = 0x52      # 트림
-    LostConnection              = 0x54      # 연결이 끊긴 후 반응 시간 설정
-
-    # Devices
-    Buzzer                      = 0x62      # 부저 제어
-    Vibrator                    = 0x63      # 진동 제어
-    Battery					    = 0x64,		# 배터리
-
+    Count						= 0x50		# 카운트
+    Bias						= 0x51		# 엑셀, 자이로 바이어스 값
+    Trim						= 0x52		# 트림
+    LostConnection				= 0x54		# 연결이 끊긴 후 반응 시간 설정
+    
+    # Device
+    Motor						= 0x60		# 모터 제어 및 현재 제어값 확인
+    Buzzer						= 0x62		# 버저 제어
+    Battery						= 0x64		# 배터리
+    
     # Input
-    Button                      = 0x70      # 버튼 입력
-    Joystick                    = 0x71      # 조이스틱 입력
+    Button						= 0x70		# 버튼
+    Joystick					= 0x71		# 조이스틱
     
     # Information Assembled
-    InformationAssembledForController   = 0xA0      # 자주 갱신되는 데이터 모음
-    InformationAssembledForEntry        = 0xA1      # 자주 갱신되는 데이터 모음
-
-    EndOfType                           = 0xDC
+    InformationAssembledForController			= 0xA0,		# 데이터 모음
+    
+    EndOfType                   = 0xDC
 
 
 # DataType End
 
 
 
 # CommandType Start
 
 
 class CommandType(Enum):
     
-    None_                   = 0x00      # 없음
-
-    Stop                    = 0x01      # 정지
-
-    # 설정
-    ModeControlFlight       = 0x02      # 비행 제어 모드 설정
-    Headless                = 0x03      # 헤드리스 모드 선택
-    ControlSpeed            = 0x04      # 제어 속도 설정
-
-    ClearBias               = 0x05      # 자이로 바이어스 리셋(트림도 같이 초기화 됨)
-    ClearTrim               = 0x06      # 트림 초기화
-
-    FlightEvent             = 0x07      # 비행 이벤트 실행
-
-    SetDefault              = 0x08      # 기본 설정으로 초기화
-    ModeController          = 0x0A      # 조종기 동작 모드(0x10:조종, 0x80:링크)
-    Link                    = 0x0B      # 링크 제어(0:Client Mode, 1:Server Mode, 2:Pairing Start)
-
-    SetSwarm				= 0x0F		# 군집 고도제어 설정
+    None_						= 0x00		# 이벤트 없음
+    
+    Stop						= 0x01		# 정지
+    
+    ModeControlFlight			= 0x02		# 비행 제어 모드 설정
+    Headless						= 0x03		# 이스케이프 모드 설정
+    ControlSpeed				= 0x04		# 제어 속도 설정
+    
+    ClearBias					= 0x05		# 자이로/엑셀 바이어스 리셋(트림도 같이 초기화 됨)
+    ClearTrim					= 0x06		# 트림 초기화
+    
+    FlightEvent					= 0x07		# 비행 이벤트 실행
     
-    ModeTest				= 0xF0      # 테스트 모드
+    SetDefault					= 0x08		# 기본 설정으로 초기화
+    ModeController				= 0x0A		# 조종기 동작 모드(0x10:조종, 0x80:링크)
+    Link						= 0x0B		# 링크 제어(0:Client Mode, 1:Server Mode, 2:Pairing Start)
+    LoadDefaultColor			= 0x0C		# 기본 색상으로 변경
     
-    EndOfType               = 0xEC
+    Trim						= 0x0D		# 트림
+    
+    ModeTest					= 0xF0		# 테스트 락(테스트를 완료하기 전까진 사용 불가 / 27:활성화, 11:해제))
+    
+    EndOfType                   = 0xEC
 
 
 # CommandType End
 
 
 
 # Header Start
@@ -539,14 +532,40 @@
         if len(dataArray) != cls.getSize():
             return None
         
         data.address0, data.address1, data.address2, data.address3, data.address4, data.channel0 = unpack('<BBBBBB', dataArray)
         return data
 
 
+class ResponseRate(ISerializable) :
+    
+    def __init__(self):
+        self.responseRate = 0
+        
+    @classmethod
+    def getSize(cls):
+        return 1
+
+
+    def toArray(self):
+        return pack('<B', self.responseRate)
+
+
+    @classmethod
+    def parse(cls, dataArray):
+        data = ResponseRate()
+        
+        if len(dataArray) != cls.getSize():
+            return None
+        
+        data.responseRate, = unpack('<B', dataArray)
+
+        return data
+
+
 
 class Rssi(ISerializable):
 
     def __init__(self):
         self.rssi       = 0
 
 
@@ -572,15 +591,15 @@
 
 
 
 class Command(ISerializable):
 
     def __init__(self):
         self.commandType    = CommandType.None_
-        self.option         = 0
+        self.option         = ModeControlFlight.None_
 
 
     @classmethod
     def getSize(cls):
         return 2
 
 
@@ -707,174 +726,14 @@
 
         return data
 
 
 # Common End
 
 
-
-# Monitor Start
-
-
-class MonitorHeaderType(Enum):
-    
-    Monitor0            = 0x00
-    Monitor4            = 0x01
-    Monitor8            = 0x02
-
-    EndOfType           = 0x03
-
-
-
-class MonitorDataType(Enum):
-    
-    U8          = 0x00,
-    S8          = 0x01,
-    U16         = 0x02,
-    S16         = 0x03,
-    U32         = 0x04,
-    S32         = 0x05,
-    U64         = 0x06,
-    S64         = 0x07,
-    F32         = 0x08,
-    F64         = 0x09,
-
-    EndOfType   = 0x0A
-
-
-
-class MonitorType(ISerializable):
-
-    def __init__(self):
-        self.monitorHeaderType    = MonitorHeaderType.Monitor8
-
-
-    @classmethod
-    def getSize(cls):
-        return 1
-
-
-    def toArray(self):
-        return pack('<B', self.monitorHeaderType.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = MonitorType()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.monitorHeaderType, = unpack('<B', dataArray)
-
-        data.monitorHeaderType  = MonitorHeaderType(data.monitorHeaderType)
-
-        return data
-
-
-
-class Monitor0(ISerializable):
-
-    def __init__(self):
-        self.monitorDataType        = MonitorDataType.F32
-        self.index                  = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 2
-
-
-    def toArray(self):
-        return pack('<BB', self.monitorDataType.value, self.index)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = Monitor0()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.monitorDataType, data.index = unpack('<BB', dataArray)
-
-        data.monitorDataType  = MonitorDataType(data.monitorDataType)
-
-        return data
-
-
-
-class Monitor4(ISerializable):
-
-    def __init__(self):
-        self.systemTime             = 0
-        self.monitorDataType        = MonitorDataType.F32
-        self.index                  = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 6
-
-
-    def toArray(self):
-        return pack('<IBB', self.systemTime, self.monitorDataType.value, self.index)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = Monitor4()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.systemTime, data.monitorDataType, data.index = unpack('<IBB', dataArray)
-
-        data.monitorDataType  = MonitorDataType(data.monitorDataType)
-
-        return data
-
-
-
-class Monitor8(ISerializable):
-    
-    def __init__(self):
-        self.systemTime             = 0
-        self.monitorDataType        = MonitorDataType.F32
-        self.index                  = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 10
-
-
-    def toArray(self):
-        return pack('<QBB', self.systemTime, self.monitorDataType.value, self.index)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = Monitor8()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.systemTime, data.monitorDataType, data.index = unpack('<QBB', dataArray)
-
-        data.monitorDataType  = MonitorDataType(data.monitorDataType)
-
-        return data
-
-
-
-# Monitor End
-
-
-
 # Control Start
 
 
 class ControlQuad8(ISerializable):
 
     def __init__(self):
         self.roll       = 0
@@ -1526,428 +1385,29 @@
 
         return data
 
 
 # Light End
 
 
-
-# Display Start
-
-
-class DisplayPixel(Enum):
-    
-    Black               = 0x00
-    White               = 0x01
-    Inverse             = 0x02
-    Outline             = 0x03
-
-
-
-class DisplayFont(Enum):
-    
-    LiberationMono5x8   = 0x00
-    LiberationMono10x16 = 0x01
-
-
-
-class DisplayAlign(Enum):
-    
-    Left                = 0x00
-    Center              = 0x01
-    Right               = 0x02
-
-
-
-class DisplayLine(Enum):
-    
-    Solid               = 0x00
-    Dotted              = 0x01
-    Dashed              = 0x02
-
-
-
-class DisplayClearAll(ISerializable):
-
-    def __init__(self):
-        self.pixel       = DisplayPixel.White
-
-
-    @classmethod
-    def getSize(cls):
-        return 1
-
-
-    def toArray(self):
-        return pack('<B', self.pixel.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayClearAll()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.pixel, = unpack('<B', dataArray)
-        data.pixel  = DisplayPixel(data.pixel)
-        
-        return data
-
-
-
-class DisplayClear(ISerializable):
-
-    def __init__(self):
-        self.x           = 0
-        self.y           = 0
-        self.width       = 0
-        self.height      = 0
-        self.pixel       = DisplayPixel.White
-
-
-    @classmethod
-    def getSize(cls):
-        return 9
-
-
-    def toArray(self):
-        return pack('<hhhhB', self.x, self.y, self.width, self.height, self.pixel.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayClear()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.width, data.height, data.pixel = unpack('<hhhhB', dataArray)
-
-        data.pixel = DisplayPixel(data.pixel)
-        
-        return data
-
-
-
-class DisplayInvert(ISerializable):
-
-    def __init__(self):
-        self.x           = 0
-        self.y           = 0
-        self.width       = 0
-        self.height      = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 8
-
-
-    def toArray(self):
-        return pack('<hhhh', self.x, self.y, self.width, self.height)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayInvert()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.width, data.height = unpack('<hhhh', dataArray)
-        
-        return data
-
-
-
-class DisplayDrawPoint(ISerializable):
-
-    def __init__(self):
-        self.x           = 0
-        self.y           = 0
-        self.pixel       = DisplayPixel.White
-
-
-    @classmethod
-    def getSize(cls):
-        return 5
-
-
-    def toArray(self):
-        return pack('<hhB', self.x, self.y, self.pixel.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawPoint()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.pixel = unpack('<hhB', dataArray)
-
-        data.pixel = DisplayPixel(data.pixel)
-        
-        return data
-
-
-
-class DisplayDrawLine(ISerializable):
-
-    def __init__(self):
-        self.x1          = 0
-        self.y1          = 0
-        self.x2          = 0
-        self.y2          = 0
-        self.pixel       = DisplayPixel.White
-        self.line        = DisplayLine.Solid
-
-
-    @classmethod
-    def getSize(cls):
-        return 10
-
-
-    def toArray(self):
-        return pack('<hhhhBB', self.x1, self.y1, self.x2, self.y2, self.pixel.value, self.line.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawLine()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x1, data.y1, data.x2, data.y2, data.pixel, data.line = unpack('<hhhhBB', dataArray)
-
-        data.pixel  = DisplayPixel(data.pixel)
-        data.line   = DisplayLine(data.line)
-        
-        return data
-
-
-
-class DisplayDrawRect(ISerializable):
-
-    def __init__(self):
-        self.x          = 0
-        self.y          = 0
-        self.width      = 0
-        self.height     = 0
-        self.pixel      = DisplayPixel.White
-        self.flagFill   = True
-        self.line       = DisplayLine.Solid
-
-
-    @classmethod
-    def getSize(cls):
-        return 11
-
-
-    def toArray(self):
-        return pack('<hhhhB?B', self.x, self.y, self.width, self.height, self.pixel.value, self.flagFill, self.line.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawRect()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.width, data.height, data.pixel, data.flagFill, data.line = unpack('<hhhhB?B', dataArray)
-
-        data.pixel  = DisplayPixel(data.pixel)
-        data.line   = DisplayLine(data.line)
-        
-        return data
-
-
-
-class DisplayDrawCircle(ISerializable):
-
-    def __init__(self):
-        self.x          = 0
-        self.y          = 0
-        self.radius     = 0
-        self.pixel      = DisplayPixel.White
-        self.flagFill   = True
-
-
-    @classmethod
-    def getSize(cls):
-        return 8
-
-
-    def toArray(self):
-        return pack('<hhhB?', self.x, self.y, self.radius, self.pixel.value, self.flagFill)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawCircle()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-
-        data.x, data.y, data.radius, data.pixel, data.flagFill = unpack('<hhhB?', dataArray)
-
-        data.pixel = DisplayPixel(data.pixel)
-        
-        return data
-
-
-
-class DisplayDrawString(ISerializable):
-
-    def __init__(self):
-        self.x          = 0
-        self.y          = 0
-        self.font       = DisplayFont.LiberationMono5x8
-        self.pixel      = DisplayPixel.White
-        self.message    = ""
-
-
-    @classmethod
-    def getSize(cls):
-        return 6
-
-
-    def getSizeTotal(self):
-        return self.getSize() + len(self.message)
-
-
-    def toArray(self):
-        dataArray = bytearray()
-        dataArray.extend(pack('<hhBB', self.x, self.y, self.font.value, self.pixel.value))
-        dataArray.extend(self.message.encode('ascii', 'ignore'))
-        return dataArray
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawString()
-        
-        if len(dataArray) <= cls.getSize():
-            return None
-
-        data.x, data.y, data.font, data.pixel = unpack('<hhBB', dataArray[0:cls.getSize()])
-
-        data.font       = DisplayFont(data.font)
-        data.pixel      = DisplayPixel(data.pixel)
-        data.message    = dataArray[cls.getSize():len(dataArray)].decode()
-        
-        return data
-
-
-
-class DisplayDrawStringAlign(ISerializable):
-
-    def __init__(self):
-        
-        self.x_start    = 0
-        self.x_end      = 0
-        self.y          = 0
-        self.align      = DisplayAlign.Center
-        self.font       = DisplayFont.LiberationMono5x8
-        self.pixel      = DisplayPixel.White
-        self.message    = ""
-
-
-    @classmethod
-    def getSize(cls):
-        return 9
-
-
-
-    def getSizeTotal(self):
-        return self.getSize() + len(self.message)
-
-
-
-    def toArray(self):
-        dataArray = bytearray()
-        dataArray.extend(pack('<hhhBBB', self.x_start, self.x_end, self.y, self.align.value, self.font.value, self.pixel.value))
-        dataArray.extend(self.message.encode('ascii', 'ignore'))
-        return dataArray
-    
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayDrawStringAlign()
-        
-        if len(dataArray) <= cls.getSize():
-            return None
-
-        data.x_start, data.x_end, data.y, data.align, data.font, data.pixel, data.message = unpack('<hhhBBBs', dataArray[0:cls.getSize()])
-        data.align = DisplayAlign(data.align)
-        data.font = DisplayFont(data.font)
-        data.pixel = DisplayPixel(data.pixel)
-        data.message = dataArray[cls.getSize():len(dataArray)].decode()
-        
-        return data
-
-
-
-class DisplayImage(ISerializable):
-
-    def __init__(self):
-        self.x          = 0
-        self.y          = 0
-        self.width      = 0
-        self.height     = 0
-        self.image      = bytearray()
-
-
-    @classmethod
-    def getSize(cls):
-        return 8
-
-
-    def toArray(self):
-        dataArray = bytearray()
-        dataArray.extend(pack('<hhhh', self.x, self.y, self.width, self.height))
-        dataArray.extend(self.image)
-        return dataArray
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = DisplayImage()
-        
-        if len(dataArray) <= cls.getSize():
-            return None
-
-        data.x, data.y, data.width, data.height = unpack('<hhhh', dataArray)
-        data.image = dataArray[cls.getSize():(len(dataArray) - cls.getSize())]
-        
-        return data
-
-
-# Display End
-
-
-
 # Buzzer Start
 
 
 class BuzzerMode(Enum):
 
-    Stop                = 0     # 정지(Mode에서의 Stop은 통신에서 받았을 때 Buzzer를 끄는 용도로 사용, set으로만 호출)
+    Stop                = 0    # 정지(Mode에서의 Stop은 통신에서 받았을 때 Buzzer를 끄는 용도로 사용, set으로만 호출)
 
-    Mute                = 1     # 묵음 즉시 적용
-    MuteReserve         = 2     # 묵음 예약
+    MuteInstantly       = 1    # 묵음 즉시 적용
+    MuteContinually     = 2    # 묵음 예약
 
-    Scale               = 3     # 음계 즉시 적용
-    ScaleReserve        = 4     # 음계 예약
+    ScaleInstantly      = 3    # 음계 즉시 적용
+    ScaleContinually    = 4    # 음계 예약
 
-    Hz                  = 5     # 주파수 즉시 적용
-    HzReserve           = 6     # 주파수 예약
+    HzInstantly         = 5    # 주파수 즉시 적용
+    HzContinually       = 6    # 주파수 예약
 
     EndOfType           = 7
 
 
 
 class BuzzerScale(Enum):
 
@@ -1964,14 +1424,48 @@
     EndOfType   = 0x60
 
     Mute        = 0xEE  # 묵음
     Fin         = 0xFF  # 악보의 끝
 
 
 
+
+
+class BuzzerMelody(Enum):
+    
+    DoMiSol     = 0x00		# 도미솔
+    SolMiDo     = 0x01		# 솔미도
+    LaLa        = 0x02		# 라라
+    SiRaSiRa    = 0x03		# 시라시라
+    
+    Warning1    = 0x04		# 경고 1
+    Warning2    = 0x05		# 경고 2
+    Warning3    = 0x06		# 경고 3
+    Warning4    = 0x07		# 경고 4
+    
+    Du          = 0x08		# Trim -
+    DuDu        = 0x09		# Trim - End
+    DiDic       = 0x0A		# Trim Center
+    DiDic2      = 0x0B		# Trim Center 2
+    Di          = 0x0C		# Trim +
+    DiDi        = 0x0D		# Trim + End
+    
+    BuzzSound1   = 0x0E
+    BuzzSound2   = 0x0F
+    BuzzSound3   = 0x10
+    BuzzSound4   = 0x11
+    
+    Button       = 0x12
+    Shot         = 0x13
+    
+    EndOfType    = 0x14
+
+
+
+
 class Buzzer(ISerializable):
 
     def __init__(self):
         self.mode       = BuzzerMode.Stop
         self.value      = 0
         self.time       = 0
 
@@ -2054,31 +1548,30 @@
 
 
 # Button Start
 
 
 class ButtonFlagController(Enum):
 
-    None_               = 0x0000
-    
-    FrontLeftTop        = 0x0001
-    FrontLeftBottom     = 0x0002
-    FrontRightTop       = 0x0004
-    FrontRightBottom    = 0x0008
-    
-    TopLeft             = 0x0010
-    TopRight            = 0x0020    # POWER ON/OFF
-    
-    MidUp               = 0x0040
-    MidLeft             = 0x0080
-    MidRight            = 0x0100
-    MidDown             = 0x0200
-    
-    BottomLeft          = 0x0400
-    BottomRight         = 0x0800
+    None_   			= 0x0000
+                
+    # 버튼
+    FrontLeft			= 0x0001
+    FrontRight			= 0x0002
+
+    MidUpLeft			= 0x0004
+    MidUpRight			= 0x0008
+
+    MidUp				= 0x0010
+    MidLeft				= 0x0020
+    MidRight			= 0x0040
+    MidDown				= 0x0080
+
+    BottomLeft			= 0x0100
+    BottomRight			= 0x0200
 
 
 
 class ButtonFlagDrone(Enum):
 
     None_               = 0x0000
     
@@ -2133,15 +1626,15 @@
 
 
 # Joystick Start
 
 
 class JoystickDirection(Enum):
 
-    None_   = 0         # 정의하지 않은 영역(무시함)
+    None_   = 0x00      # 정의하지 않은 영역(무시함)
 
     VT      = 0x10      #   위(세로)
     VM      = 0x20      # 중앙(세로)
     VB      = 0x40      # 아래(세로)
 
     HL      = 0x01      #   왼쪽(가로)
     HM      = 0x02      #   중앙(가로)
@@ -2267,42 +1760,14 @@
         
         data.accelX, data.accelY, data.accelZ, data.gyroRoll, data.gyroPitch, data.gyroYaw = unpack('<hhhhhh', dataArray)
         
         return data
 
 
 
-class RawFlow(ISerializable):
-
-    def __init__(self):
-        self.x     = 0
-        self.y     = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 8
-
-
-    def toArray(self):
-        return pack('<ff', self.x, self.y)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = RawFlow()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.x, data.y = unpack('<ff', dataArray)
-        
-        return data
-
-
 # Sensor Raw End
 
 
 
 # Information Start
 
 
@@ -2541,39 +2006,39 @@
 # Information End
 
 
 
 # Sensor Start
 
 
-class Vector(ISerializable):
-
+class VisionSensor(ISerializable):
+    
     def __init__(self):
         self.x      = 0
         self.y      = 0
         self.z      = 0
 
 
     @classmethod
     def getSize(cls):
-        return 6
+        return 12
 
 
     def toArray(self):
-        return pack('<hhh', self.x, self.y, self.z)
+        return pack('<fff', self.x, self.y, self.z)
 
 
     @classmethod
     def parse(cls, dataArray):
-        data = Vector()
+        data = VisionSensor()
         
         if len(dataArray) != cls.getSize():
             return None
         
-        data.x, data.y, data.z = unpack('<hhh', dataArray)
+        data.x, data.y, data.z = unpack('<fff', dataArray)
         
         return data
 
 
 
 class Count(ISerializable):
```

### Comparing `codingrider-2.6/CodingRider/receiver.py` & `codingrider-2.7/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.6/CodingRider/storage.py` & `codingrider-2.7/CodingRider/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,30 +44,27 @@
 
     def __init__(self):
         self.d = dict.fromkeys(list(DataType))
 
         self.d[DataType.Ping]               = Ping.parse
         self.d[DataType.Ack]                = Ack.parse
         self.d[DataType.Error]              = Error.parse
-        self.d[DataType.Message]            = Message.parse
-        self.d[DataType.Address]            = Address.parse
         self.d[DataType.Information]        = Information.parse
-
+        self.d[DataType.VisionSensor]       = VisionSensor.parse
         self.d[DataType.Pairing]            = Pairing.parse
-        self.d[DataType.Rssi]               = Rssi.parse
 
         self.d[DataType.RawMotion]          = RawMotion.parse
 
         self.d[DataType.State]              = State.parse
+    
         self.d[DataType.Altitude]           = Altitude.parse
         self.d[DataType.Motion]             = Motion.parse
 
         self.d[DataType.Count]              = Count.parse
         self.d[DataType.Trim]               = Trim.parse
 
         self.d[DataType.Button]             = Button.parse
         self.d[DataType.Joystick]           = Joystick.parse
 
         self.d[DataType.InformationAssembledForController]  = InformationAssembledForController.parse
-        self.d[DataType.InformationAssembledForEntry]       = InformationAssembledForEntry.parse
```

### Comparing `codingrider-2.6/CodingRider/tools/parser.py` & `codingrider-2.7/CodingRider/tools/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
-from e_drone.drone import *
-from e_drone.tools.update import Updater
+from CodingRider.drone import *
+from CodingRider.tools.update import Updater
 
 import colorama
 from colorama import Fore, Back, Style
 
 # Parser Start
 
 
@@ -30,165 +30,144 @@
             print("Count:{0} ".format(self.count) , end='')
 
             for arg in self.arguments:
                 print("/ {0} ".format(arg), end='')
 
             print("")
 
-            # >python -m e_drone upgrade
-            # >python -m e_drone update
+            # >python -m CodingRider upgrade
+            # >python -m CodingRider update
             if      (self.arguments[0] == "upgrade") or (self.arguments[0] == "update"):
                 updater = Updater()
                 updater.update()
                 return
 
-            # >python -m e_drone request State 10 0.2
+            # >python -m CodingRider request State 10 0.2
             elif    ((self.count == 4) and 
                     (self.arguments[0] == "request") and
                     (self.arguments[1] == "state")):         # time interval
                 #print("* State - Ready     Blue    Red     Black   Black   None_             1830   1631   2230      76      ")    
                 print ("         |ModeSystem   |ModeFlight |ModeControlFlight |ModeMovement |Headless |ControlSpeed |SensorOrientation |Battery |")
                 self.request(DeviceType.Drone, DataType.State, int(self.arguments[2]), float(self.arguments[3]))
                 return
 
-            # >python -m e_drone request Motion 10 0.2
+            # >python -m CodingRider request Motion 10 0.2
             elif    ((self.count == 4) and 
                     (self.arguments[0] == "request") and
                     (self.arguments[1] == "motion")):         # time interval
                 #print("* Motion      -38      64     -32     457     -40    -400      16       0   20500")    
                 print ("         |Accel                  |Gyro                   |Angle                  |")
                 print ("         |      X|      Y|      Z|   Roll|  Pitch|    Yaw|   Roll|  Pitch|    Yaw|")
                 self.request(DeviceType.Drone, DataType.Motion, int(self.arguments[2]), float(self.arguments[3]))
                 return
 
-            # >python -m e_drone request CardRaw 10 0.2
-            elif    ((self.count == 4) and 
-                    (self.arguments[0] == "request") and
-                    (self.arguments[1] == "cardraw")):         # time interval
-                #print("* CardRaw   335  503  766  692  309  395 100  39  96  40   9  17 303  61  39 344  77  15   Magenta         Red")
-                print ("          |Front Raw     |Rear Raw      |Front RGB  |Rear RGB   |Front HSVL      |Rear HSVL       |Front Color  |Rear Color   |")
-                print ("          |   R    G    B|   R    G    B|  R   G   B|  R   G   B|  H   S   V   L|  H   S   V   L|             |             |")
-                self.request(DeviceType.Drone, DataType.CardRaw, int(self.arguments[2]), float(self.arguments[3]))
-                return
-
-            # >python -m e_drone request CardRange 10 0.2
-            elif    ((self.count == 4) and 
-                    (self.arguments[0] == "request") and
-                    (self.arguments[1] == "cardrange")):         # time interval
-                #print("* CardRange       200  2000   200  2000   200  2000   200     0   200     0   200     0")
-                print ("               |Front                              |Rear                               |")
-                print ("               |Red        |Green      |Blue       |Red        |Green      |Blue       |")
-                print ("               |  Min|  Max|  Min|  Max|  Min|  Max|  Min|  Max|  Min|  Max|  Min|  Max|")
-                self.request(DeviceType.Drone, DataType.CardRange, int(self.arguments[2]), float(self.arguments[3]))
-                return
-
             # 이륙
             #                   0
-            # python -m e_drone Takeoff
+            # python -m CodingRider Takeoff
             elif    ((self.count == 1) and 
                     (self.arguments[0] == "takeoff")):
                 print (Fore.YELLOW + "takeoff" + Style.RESET_ALL)
                 self.command(CommandType.FlightEvent, FlightEvent.TakeOff.value)
                 return
 
             # 착륙
             #                   0
-            # python -m e_drone Landing
+            # python -m CodingRider Landing
             elif    ((self.count == 1) and 
                     (self.arguments[0] == "landing")):
                 print (Fore.YELLOW + "landing" + Style.RESET_ALL)
                 self.command(CommandType.FlightEvent, FlightEvent.Landing.value)
                 return
 
             # 정지
             #                   0
-            # python -m e_drone Stop
+            # python -m CodingRider Stop
             elif    ((self.count == 1) and 
                     (self.arguments[0] == "stop")):
                 print (Fore.YELLOW + "stop" + Style.RESET_ALL)
                 self.command(CommandType.FlightEvent, FlightEvent.Stop.value)
                 return
 
             # 조종
             #                   0        1      2       3     4          5
-            # python -m e_drone control [roll] [pitch] [yaw] [throttle] [time(ms)]
+            # python -m CodingRider control [roll] [pitch] [yaw] [throttle] [time(ms)]
             # 지정한 시간이 종료되면 입력값을 모두 0으로 변경하고 멈춤
-            # >python -m e_drone control 40 0 3
+            # >python -m CodingRider control 40 0 3
             elif    ((self.count == 6) and 
                     (self.arguments[0] == "control")):
                 print (Fore.YELLOW + "control" + Style.RESET_ALL)
                 self.control(int(self.arguments[1]), int(self.arguments[2]), int(self.arguments[3]), int(self.arguments[4]), int(self.arguments[5]))
                 return
 
             # 이동(전체)
             #                   0         1   2   3   4          5         6
-            # python -m e_drone position [x] [y] [z] [velocity] [heading] [rotational velocity]
+            # python -m CodingRider position [x] [y] [z] [velocity] [heading] [rotational velocity]
             elif    ((self.count == 7) and 
                     (self.arguments[0] == "position")):
                 print (Fore.YELLOW + "position" + Style.RESET_ALL)
                 self.controlPosition(float(self.arguments[1]), float(self.arguments[2]), float(self.arguments[3]), float(self.arguments[4]), float(self.arguments[5]), float(self.arguments[6]))
                 return
 
             # 이동(위치)
             #                   0         1   2   3   4
-            # python -m e_drone position [x] [y] [z] [velocity]
+            # python -m CodingRider position [x] [y] [z] [velocity]
             elif    ((self.count == 5) and 
                     (self.arguments[0] == "position")):
                 print (Fore.YELLOW + "position" + Style.RESET_ALL)
                 self.controlPosition(float(self.arguments[1]), float(self.arguments[2]), float(self.arguments[3]), float(self.arguments[4]), 0, 0)
                 return
 
             # 이동(헤딩)
             #                   0        1         2
-            # python -m e_drone heading [heading] [rotational velocity]
+            # python -m CodingRider heading [heading] [rotational velocity]
             elif    ((self.count == 3) and 
                     (self.arguments[0] == "heading")):
                 print (Fore.YELLOW + "heading" + Style.RESET_ALL)
                 self.controlPosition(0, 0, 0, 0, float(self.arguments[1]), float(self.arguments[2]))
                 return
 
             # 버저
             #                   1       2    3
-            # python -m e_drone buzzer [hz] [time(ms)]
-            # >python -m e_drone buzzer 400 2000
+            # python -m CodingRider buzzer [hz] [time(ms)]
+            # >python -m CodingRider buzzer 400 2000
             elif    ((self.count == 3) and 
                     (self.arguments[0] == "buzzer")):
                 print (Fore.WHITE + "Buzz Sound: " + Fore.YELLOW + "{0}".format(int(self.arguments[1])) + Fore.WHITE + "Hz, " + Fore.CYAN + "{0}".format(int(self.arguments[2])) + Fore.WHITE + "ms" + Style.RESET_ALL)
                 self.buzzer(DeviceType.Controller, int(self.arguments[1]), int(self.arguments[2]))
                 return
 
             # 진동
             #                   1         2          3           4
-            # python -m e_drone vibrator [on(ms)] [off(ms)] [total(ms)]
-            # >python -m e_drone vibrator 500 500 2000
+            # python -m CodingRider vibrator [on(ms)] [off(ms)] [total(ms)]
+            # >python -m CodingRider vibrator 500 500 2000
             elif    ((self.count == 4) and 
                     (self.arguments[0] == "vibrator")):
                 print (Fore.WHITE + "Vibrator: on " + Fore.YELLOW + "{0}".format(int(self.arguments[1])) + Fore.WHITE + "ms, off " + Fore.CYAN + "{0}".format(int(self.arguments[2])) + Fore.WHITE + "ms, total " + Fore.CYAN + "{0}".format(int(self.arguments[3])) + Fore.WHITE + "ms" + Style.RESET_ALL)
                 self.vibrator(DeviceType.Controller, int(self.arguments[1]), int(self.arguments[2]), int(self.arguments[3]))
                 return
 
 
-            # >python -m e_drone light body flicker 100 50 50 10
-            # >python -m e_drone light body flickerdouble 100 50 50 10
-            # >python -m e_drone light body dimming 3 50 50 10
-            # >python -m e_drone light body sunrise 5 50 50 10
-            # >python -m e_drone light body sunset 5 50 50 10
-            # >python -m e_drone light body rainbow 8 50 50 10
-            # >python -m e_drone light body rainbow2 8 50 50 10
+            # >python -m CodingRider light body flicker 100 50 50 10
+            # >python -m CodingRider light body flickerdouble 100 50 50 10
+            # >python -m CodingRider light body dimming 3 50 50 10
+            # >python -m CodingRider light body sunrise 5 50 50 10
+            # >python -m CodingRider light body sunset 5 50 50 10
+            # >python -m CodingRider light body rainbow 8 50 50 10
+            # >python -m CodingRider light body rainbow2 8 50 50 10
             elif    ((self.count == 7) and 
                     (self.arguments[0] == "light")):
                 print (Fore.WHITE + "Light: " + Fore.YELLOW + "{0}, {1}, {2}, ({3}, {4}, {5})".format(self.arguments[1], self.arguments[2], int(self.arguments[3]), int(self.arguments[4]), int(self.arguments[5]), int(self.arguments[6])) + Style.RESET_ALL)
                 self.lightModeRgb(self.arguments[1], self.arguments[2], int(self.arguments[3]), int(self.arguments[4]), int(self.arguments[5]), int(self.arguments[6]))
                 return
 
-            # >python -m e_drone light front hold 100
-            # >python -m e_drone light head hold 100
-            # >python -m e_drone light tail hold 100
-            # >python -m e_drone light left hold 100
-            # >python -m e_drone light right hold 100
+            # >python -m CodingRider light front hold 100
+            # >python -m CodingRider light head hold 100
+            # >python -m CodingRider light tail hold 100
+            # >python -m CodingRider light left hold 100
+            # >python -m CodingRider light right hold 100
             elif    ((self.count == 4) and 
                     (self.arguments[0] == "light")):
                 print (Fore.WHITE + "Light: " + Fore.YELLOW + "{0}, {1}, {2}".format(self.arguments[1], self.arguments[2], int(self.arguments[3])) + Style.RESET_ALL)
                 self.lightModeSingle(self.arguments[1], self.arguments[2], int(self.arguments[3]))
                 return
 
         # 아무것도 실행되지 않은 경우
@@ -202,16 +181,14 @@
         if drone.open() == False:
             print(Fore.RED + "* Error : Unable to open serial port." + Style.RESET_ALL)
             sys.exit(1)
         
         # 이벤트 핸들링 함수 등록
         drone.setEventHandler(DataType.State, self.eventState)
         drone.setEventHandler(DataType.Motion, self.eventMotion)
-        drone.setEventHandler(DataType.CardRaw, self.eventCardRaw)
-        drone.setEventHandler(DataType.CardRange, self.eventCardRange)
 
         # 데이터 요청
         for i in range(repeat):
             drone.sendRequest(deviceType, dataType)
             sleep(interval)
 
 
@@ -410,80 +387,80 @@
     def help(self):
 
         print("")
         print(Fore.YELLOW + "* Command List " + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Firmware Upgrade" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "upgrade" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "upgrade" + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Request Data" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "request " + Fore.WHITE + "[" + Fore.YELLOW + "data type" + Fore.WHITE + "] [" + Fore.GREEN + "number of times" + Fore.WHITE + "] [" + Fore.YELLOW + "time interval(sec)" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "request " + Fore.YELLOW + "state " + Fore.GREEN + "10 " + Fore.YELLOW + "0.2" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "request " + Fore.YELLOW + "motion " + Fore.GREEN + "10 " + Fore.YELLOW + "0.2" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "request " + Fore.WHITE + "[" + Fore.YELLOW + "data type" + Fore.WHITE + "] [" + Fore.GREEN + "number of times" + Fore.WHITE + "] [" + Fore.YELLOW + "time interval(sec)" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "request " + Fore.YELLOW + "state " + Fore.GREEN + "10 " + Fore.YELLOW + "0.2" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "request " + Fore.YELLOW + "motion " + Fore.GREEN + "10 " + Fore.YELLOW + "0.2" + Style.RESET_ALL)
         ## 카드 코딩과 관련된 내용이 최신 버전인지 알 수 없는 관계로 일단 보류(2021.1.4)
-        ##print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "request " + Fore.YELLOW + "RawCard " + Fore.GREEN + "10 " + Fore.YELLOW + "0.2" + Style.RESET_ALL)
-        ##print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "request " + Fore.YELLOW + "RawCardRange " + Fore.GREEN + "10 " + Fore.YELLOW + "0.2" + Style.RESET_ALL)
+        ##print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "request " + Fore.YELLOW + "RawCard " + Fore.GREEN + "10 " + Fore.YELLOW + "0.2" + Style.RESET_ALL)
+        ##print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "request " + Fore.YELLOW + "RawCardRange " + Fore.GREEN + "10 " + Fore.YELLOW + "0.2" + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - FlightEvent" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.WHITE + "[" + Fore.YELLOW + "FlightEvent" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.YELLOW + "takeoff" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.YELLOW + "landing" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.YELLOW + "stop" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.WHITE + "[" + Fore.YELLOW + "FlightEvent" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.YELLOW + "takeoff" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.YELLOW + "landing" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.YELLOW + "stop" + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Control" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "control " + Fore.WHITE + "[" + Fore.RED + "roll" + Fore.WHITE + "] [" + Fore.GREEN + "pitch" + Fore.WHITE + "] [" + Fore.BLUE + "yaw" + Fore.WHITE + "] [" + Fore.MAGENTA + "throttle" + Fore.WHITE + "] [" + Fore.YELLOW + "time(ms)" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "control " + Fore.RED + "0 " + Fore.GREEN + "30 " + Fore.BLUE + "0 " + Fore.MAGENTA + "0 " + Fore.YELLOW + "5000 " + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "control " + Fore.WHITE + "[" + Fore.RED + "roll" + Fore.WHITE + "] [" + Fore.GREEN + "pitch" + Fore.WHITE + "] [" + Fore.BLUE + "yaw" + Fore.WHITE + "] [" + Fore.MAGENTA + "throttle" + Fore.WHITE + "] [" + Fore.YELLOW + "time(ms)" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "control " + Fore.RED + "0 " + Fore.GREEN + "30 " + Fore.BLUE + "0 " + Fore.MAGENTA + "0 " + Fore.YELLOW + "5000 " + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Control - Position, Heading" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "position " + Fore.WHITE + "[" + Fore.RED + "x(meter)" + Fore.WHITE + "] [" + Fore.GREEN + "y(meter)" + Fore.WHITE + "] [" + Fore.BLUE + "z(meter)" + Fore.WHITE + "] [" + Fore.YELLOW + "speed(m/sec)" + Fore.WHITE + "] [" + Fore.MAGENTA + "heading(degree)" + Fore.WHITE + "] [" + Fore.YELLOW + "rotational velocity(deg/sec)" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "position " + Fore.RED + "5 " + Fore.GREEN + "0 " + Fore.BLUE + "0 "  + Fore.YELLOW + "2 " + Fore.MAGENTA + "90 " + Fore.YELLOW + "45 "+ Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "position " + Fore.WHITE + "[" + Fore.RED + "x(meter)" + Fore.WHITE + "] [" + Fore.GREEN + "y(meter)" + Fore.WHITE + "] [" + Fore.BLUE + "z(meter)" + Fore.WHITE + "] [" + Fore.YELLOW + "speed(m/sec)" + Fore.WHITE + "] [" + Fore.MAGENTA + "heading(degree)" + Fore.WHITE + "] [" + Fore.YELLOW + "rotational velocity(deg/sec)" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "position " + Fore.RED + "5 " + Fore.GREEN + "0 " + Fore.BLUE + "0 "  + Fore.YELLOW + "2 " + Fore.MAGENTA + "90 " + Fore.YELLOW + "45 "+ Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Control - Position" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "position " + Fore.WHITE + "[" + Fore.RED + "x(meter)" + Fore.WHITE + "] [" + Fore.GREEN + "y(meter)" + Fore.WHITE + "] [" + Fore.BLUE + "z(meter)" + Fore.WHITE + "] [" + Fore.YELLOW + "speed(m/sec)" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "position " + Fore.RED + "5 " + Fore.GREEN + "0 " + Fore.BLUE + "0 "  + Fore.YELLOW + "2 " + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "position " + Fore.WHITE + "[" + Fore.RED + "x(meter)" + Fore.WHITE + "] [" + Fore.GREEN + "y(meter)" + Fore.WHITE + "] [" + Fore.BLUE + "z(meter)" + Fore.WHITE + "] [" + Fore.YELLOW + "speed(m/sec)" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "position " + Fore.RED + "5 " + Fore.GREEN + "0 " + Fore.BLUE + "0 "  + Fore.YELLOW + "2 " + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Control - Heading" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "heading " + Fore.WHITE + "[" + Fore.MAGENTA + "heading(degree)" + Fore.WHITE + "] [" + Fore.YELLOW + "rotational velocity(deg/sec)" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "heading " + Fore.MAGENTA + "90 " + Fore.YELLOW + "45" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "heading " + Fore.WHITE + "[" + Fore.MAGENTA + "heading(degree)" + Fore.WHITE + "] [" + Fore.YELLOW + "rotational velocity(deg/sec)" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "heading " + Fore.MAGENTA + "90 " + Fore.YELLOW + "45" + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Buzzer" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "buzzer " + Fore.WHITE + "[" + Fore.YELLOW + "hz" + Fore.WHITE + "] [" + Fore.GREEN + "time(ms)" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "buzzer " + Fore.YELLOW + "400 " + Fore.GREEN + "2000" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "buzzer " + Fore.WHITE + "[" + Fore.YELLOW + "hz" + Fore.WHITE + "] [" + Fore.GREEN + "time(ms)" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "buzzer " + Fore.YELLOW + "400 " + Fore.GREEN + "2000" + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Vibrator" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "vibrator " + Fore.WHITE + "[" + Fore.YELLOW + "on(ms)" + Fore.WHITE + "] [" + Fore.GREEN + "off(ms)" + Fore.WHITE + "] [" + Fore.YELLOW + "total(ms)" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "vibrator " + Fore.YELLOW + "500 " + Fore.GREEN + "500 " + Fore.YELLOW + "2000" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "vibrator " + Fore.WHITE + "[" + Fore.YELLOW + "on(ms)" + Fore.WHITE + "] [" + Fore.GREEN + "off(ms)" + Fore.WHITE + "] [" + Fore.YELLOW + "total(ms)" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "vibrator " + Fore.YELLOW + "500 " + Fore.GREEN + "500 " + Fore.YELLOW + "2000" + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Light single" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.WHITE + "[" + Fore.MAGENTA + "part" + Fore.WHITE + "] [" + Fore.CYAN + "mode" + Fore.WHITE + "] [" + Fore.YELLOW + "interval" + Fore.WHITE + "]" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "rear " + Fore.CYAN + "hold " + Fore.YELLOW + "100" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "a " + Fore.CYAN + "hold " + Fore.YELLOW + "100" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "b " + Fore.CYAN + "hold " + Fore.YELLOW + "100" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.WHITE + "[" + Fore.MAGENTA + "part" + Fore.WHITE + "] [" + Fore.CYAN + "mode" + Fore.WHITE + "] [" + Fore.YELLOW + "interval" + Fore.WHITE + "]" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "rear " + Fore.CYAN + "hold " + Fore.YELLOW + "100" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "a " + Fore.CYAN + "hold " + Fore.YELLOW + "100" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "b " + Fore.CYAN + "hold " + Fore.YELLOW + "100" + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Light RGB" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.WHITE + "[" + Fore.MAGENTA + "part" + Fore.WHITE + "] [" + Fore.CYAN + "mode" + Fore.WHITE + "] [" + Fore.YELLOW + "interval" + Fore.WHITE + "] [" + Fore.RED + "R" + Fore.WHITE + "] [" + Fore.GREEN + "G" + Fore.WHITE + "] [" + Fore.BLUE + "B" + Fore.WHITE + "] " + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "hold " + Fore.YELLOW + "100 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "flicker " + Fore.YELLOW + "100 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "flickerdouble " + Fore.YELLOW + "100 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "dimming " + Fore.YELLOW + "3 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "sunrise " + Fore.YELLOW + "5 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "sunset " + Fore.YELLOW + "5 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "rainbow " + Fore.YELLOW + "8 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
-        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m e_drone " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "rainbow2 " + Fore.YELLOW + "8 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.WHITE + "[" + Fore.MAGENTA + "part" + Fore.WHITE + "] [" + Fore.CYAN + "mode" + Fore.WHITE + "] [" + Fore.YELLOW + "interval" + Fore.WHITE + "] [" + Fore.RED + "R" + Fore.WHITE + "] [" + Fore.GREEN + "G" + Fore.WHITE + "] [" + Fore.BLUE + "B" + Fore.WHITE + "] " + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "hold " + Fore.YELLOW + "100 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "flicker " + Fore.YELLOW + "100 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "flickerdouble " + Fore.YELLOW + "100 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "dimming " + Fore.YELLOW + "3 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "sunrise " + Fore.YELLOW + "5 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "sunset " + Fore.YELLOW + "5 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "rainbow " + Fore.YELLOW + "8 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
+        print(Fore.GREEN + "   > " + Fore.WHITE + "python -m CodingRider " + Fore.CYAN + "light " + Fore.MAGENTA + "body " + Fore.CYAN + "rainbow2 " + Fore.YELLOW + "8 " + Fore.RED + "50 " + Fore.GREEN + "50 " + Fore.BLUE + "10" + Style.RESET_ALL)
         print("")
 
 
     def eventState(self, state):
 
         print(  "* State   " +
                 Fore.YELLOW + "{0:12}  ".format(state.modeSystem.name) +
```

### Comparing `codingrider-2.6/CodingRider/tools/update.py` & `codingrider-2.7/CodingRider/tools/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import abc
 import sys
 from struct import *
 from enum import Enum
 from urllib.request import urlopen
 from time import sleep
 
-from e_drone.drone import *
+from CodingRider.drone import *
 
 
 # Firmware Start
 
 
 class FirmwareHeader():
```

### Comparing `codingrider-2.6/CodingRider.egg-info/PKG-INFO` & `codingrider-2.7/CodingRider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.6
+Version: 2.7
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
```

### Comparing `codingrider-2.6/PKG-INFO` & `codingrider-2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.6
+Version: 2.7
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
```

### Comparing `codingrider-2.6/setup.py` & `codingrider-2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "2.6",
+    version = "2.7",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
```

