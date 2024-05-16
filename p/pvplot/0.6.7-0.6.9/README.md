# Comparing `tmp/pvplot-0.6.7.tar.gz` & `tmp/pvplot-0.6.9.tar.gz`

## Comparing `pvplot-0.6.7.tar` & `pvplot-0.6.9.tar`

### file list

```diff
@@ -1,35 +1,50 @@
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pvplot-0.6.7/tmp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvplot-0.6.7/cad_epics/__init__.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 pvplot-0.6.7/cad_epics/epics.py
--rw-r--r--   0        0        0    34350 2020-02-02 00:00:00.000000 pvplot-0.6.7/fallback/__main__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteaccess/.__init__.py.swp
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteaccess/__init__.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteaccess/liteCNS.py
--rw-r--r--   0        0        0    25797 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteaccess/liteaccess.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/__init__.py
--rw-r--r--   0        0        0    40241 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/liteserver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/__init__.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/helpers.py
--rw-r--r--   0        0        0    33552 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/i2c.py
--rw-r--r--   0        0        0    31584 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/i2c_312.py
--rw-r--r--   0        0        0    32249 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/i2c_320.py
--rw-r--r--   0        0        0    33494 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/i2c_322.py
--rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/i2c_TLV493D.py
--rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteCNSserver.py
--rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteGQ.py
--rwxr-xr-x   0        0        0     7867 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteLabjack.py
--rw-r--r--   0        0        0    21330 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteMCUFEC.py
--rwxr-xr-x   0        0        0     7921 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/litePeakSimulator.py
--rwxr-xr-x   0        0        0    10272 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteScaler.py
--rwxr-xr-x   0        0        0     4691 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteUSBCam.py
--rwxr-xr-x   0        0        0     4895 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteUvcCam.py
--rwxr-xr-x   0        0        0    11306 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteVGM.py
--rwxr-xr-x   0        0        0     2612 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/liteWLM.py
--rwxr-xr-x   0        0        0    16342 2020-02-02 00:00:00.000000 pvplot-0.6.7/ln/liteserver/device/senstation.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pvplot-0.6.7/pvplot/__init__.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 pvplot-0.6.7/pvplot/__main__.py
--rw-r--r--   0        0        0    34699 2020-02-02 00:00:00.000000 pvplot-0.6.7/pvplot/pvplot.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pvplot-0.6.7/LICENSE
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 pvplot-0.6.7/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pvplot-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pvplot-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pvplot-0.6.9/tmp.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/__main__.py
+-rw-r--r--   0        0        0    34917 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/pvplot.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/apstrim/__init__.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/apstrim/__main__.py
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/apstrim/apstrim.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/apstrim/liteCNS.py
+-rw-r--r--   0        0        0     7500 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/apstrim/pubEPICS.py
+-rw-r--r--   0        0        0    14585 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/apstrim/scan.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 pvplot-0.6.9/apwork/apstrim/view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvplot-0.6.9/cad_epics/__init__.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 pvplot-0.6.9/cad_epics/epics.py
+-rw-r--r--   0        0        0    34350 2020-02-02 00:00:00.000000 pvplot-0.6.9/fallback/__main__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pvplot-0.6.9/liteaccess/.__init__.py.swp
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pvplot-0.6.9/liteaccess/__init__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pvplot-0.6.9/liteaccess/liteCNS.py
+-rw-r--r--   0        0        0    26178 2020-02-02 00:00:00.000000 pvplot-0.6.9/liteaccess/liteaccess.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/__init__.py
+-rw-r--r--   0        0        0    39354 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/liteserver.py
+-rw-r--r--   0        0        0    40274 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/liteserver_unlist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/__init__.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/helpers.py
+-rw-r--r--   0        0        0    41548 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/i2c.py
+-rw-r--r--   0        0        0    31584 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/i2c_312.py
+-rw-r--r--   0        0        0    32249 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/i2c_320.py
+-rw-r--r--   0        0        0    33494 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/i2c_322.py
+-rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/i2c_TLV493D.py
+-rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteCNSserver.py
+-rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteGQ.py
+-rwxr-xr-x   0        0        0     7867 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteLabjack.py
+-rw-r--r--   0        0        0    22629 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteMCUFEC.py
+-rwxr-xr-x   0        0        0     8152 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/litePeakSimulator.py
+-rwxr-xr-x   0        0        0    10296 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteScaler.py
+-rwxr-xr-x   0        0        0     4691 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteUSBCam.py
+-rwxr-xr-x   0        0        0     4895 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteUvcCam.py
+-rwxr-xr-x   0        0        0    11306 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteVGM.py
+-rwxr-xr-x   0        0        0     2612 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/liteWLM.py
+-rwxr-xr-x   0        0        0    17199 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/senstation.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 pvplot-0.6.9/ln/liteserver/device/test/test_dht11.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pvplot-0.6.9/pvplot/__init__.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 pvplot-0.6.9/pvplot/__main__.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 pvplot-0.6.9/pvplot/apstrimAccess.py
+-rw-r--r--   0        0        0    36488 2020-02-02 00:00:00.000000 pvplot-0.6.9/pvplot/pvp.py
+-rw-r--r--   0        0        0    37023 2020-02-02 00:00:00.000000 pvplot-0.6.9/pvplot/pvp1.py
+-rw-r--r--   0        0        0    38854 2020-02-02 00:00:00.000000 pvplot-0.6.9/pvplot/pvplot.py
+-rw-r--r--   0        0        0    34739 2020-02-02 00:00:00.000000 pvplot-0.6.9/pvplot/pvpopld.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pvplot-0.6.9/LICENSE
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 pvplot-0.6.9/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pvplot-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pvplot-0.6.9/PKG-INFO
```

### Comparing `pvplot-0.6.7/tmp.py` & `pvplot-0.6.9/tmp.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/cad_epics/epics.py` & `pvplot-0.6.9/cad_epics/epics.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/fallback/__main__.py` & `pvplot-0.6.9/fallback/__main__.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteaccess/.__init__.py.swp` & `pvplot-0.6.9/liteaccess/.__init__.py.swp`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteaccess/liteCNS.py` & `pvplot-0.6.9/liteaccess/liteCNS.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteaccess/liteaccess.py` & `pvplot-0.6.9/liteaccess/liteaccess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Module for accessing multiple Process Variables, served by a liteServer.
 """
-__version__ = '3.1.3 2023-09-09'# error handling in case of wrong naming.
+__version__ = '3.2.1 2024-02-27'# prevent locking with receive_dictio_lock, proper handling of Timeout in recvfrom
 
 import sys, time, socket
 from os import getpid
 import getpass
 from timeit import default_timer as _timer
 import threading
-recvLock = threading.Lock()
+#recvLock = threading.Lock()
 receive_dictio_lock = threading.Lock()
 
 # object encoding
 #import ubjson
 #encoderDump = ubjson.dumpb
 #encoderLoad = ubjson.loadb
 #import msgpack as encoder
@@ -124,15 +124,15 @@
         _printe(f'Could not resolve host name {h}')
         sys.exit(1)
     return h,p
 
 retransmitInProgress = None
 def _recvUdp(sock, socketSize):
     """Receive the chopped UDP data"""
-    port = sock.getsockname()[1]
+    sockAddr,port = sock.getsockname()
     #print(f'>_recvUdp {port} locked: {recvLock.locked()}')
     #with recvLock:
     global retransmitInProgress
     chunks = {sock:{}}
     tryMore = 5# Max number of allowed lost packets
     ts = _timer()
     ignoreEOD = 3
@@ -150,18 +150,18 @@
             buf, addr = sock.recvfrom(socketSize)
             ReceiverStatistics["records"] += 1
             ReceiverStatistics["bytes"] += len(buf)
             ReceiverStatistics["time"] = time.time()
             
         #else:#except Exception as e:
         except socket.timeout as e:
-            msg = f'Timeout in recvfrom port {port}'
-            _printi(msg)
+            msg = f'Timeout in recvfrom {sockAddr,port}'
+            #_printi(msg)
             # Don not return, raise exception, otherwise the pypet will not recover
-            raise
+            raise TimeoutError(msg)
         if buf is None:
             raise RuntimeError(msg)
         size = len(buf) - PrefixLength
         offset = int.from_bytes(buf[:PrefixLength],'big')# python3
         
         #DNP_printi(f'chunk received at port {port}: {offset,size}')
 
@@ -273,14 +273,17 @@
     devParList = list(dpd.items())
     dictio = {'cmd':(cmd,devParList)}
     #_printv('sending cmd: '+str(dictio))
     _send_dictio(dictio, sock, hostPort)
 
 def _receive_dictio(sock, hostPort:tuple):
   """Receive and decode message from associated socket"""
+  if receive_dictio_lock.locked():
+      #print('receive_dictio locked')
+      return {}
   with receive_dictio_lock:
     # _printv('\n>receive_dictio')
     if UDP:
         data, addr = _recvUdp(sock, socketSize)
         # acknowledge the receiving
         if Access.dbgDrop_Ack > 0:
             Access.dbgDrop_Ack -= 1
@@ -312,15 +315,15 @@
     # allow exception here, it will be caught in execute_cmd
     if len(data) == 0:
         _printw(f'empty reply for: {LastDictio}')
         return {}
     try:
         decoded = encoderLoad(data)
     except Exception as e:
-        _printw(f'exception in ubjson.load Data[{len(data)}]: {e}')
+        _printw(f'exception in encoder.load Data[{len(data)}]: {e}')
         #print(str(data)[:150])
         #raise ValueError('in _receive_dictio: '+msg)
         return {}
     #for key,val in decoded.items():
     #    print(f'received from {key}: {val.keys()}')
 
     if not isinstance(decoded,dict):
@@ -399,16 +402,16 @@
     def receivingThread(self):
         _printi(f'>receiving thread started for {self.hostPort}') 
         while not self.event.is_set():
             try:
                 _printv(f'>subscription receive_dict {self.socket}')
                 try:
                     dictio = _receive_dictio(self.socket, self.hostPort)
-                except Exception as e:
-                    _printe(f'Exception in subscription thread: {e}')
+                except TimeoutError as e:
+                    _printw(f'Timeout in subscription thread: {e}')
                     continue
             #except socket.timeout as e:
             #except RuntimeError as e:
             except Exception as e:
                 msg = f'in subscription thread socket {self.name}: '+str(e)
                 _printw(msg)
                 raise
@@ -531,15 +534,16 @@
         _printv(f'<Channel {hostPort,devParDict}: {self.sock}')
 
     def _transaction(self, cmd, value=None):
         # normal transaction: send command, receive response
         if Channel.Perf: ts = _timer()
         #print(f'channel send to {self.sock}: {self.devParDict}, {cmd,value}')
         _send_cmd(cmd, self.devParDict, self.sock, self.hostPort, value)
-        r = True if cmd == 'set' else _receive_dictio(self.sock, self.hostPort)            
+        #r = True if cmd == 'set' else _receive_dictio(self.sock, self.hostPort)
+        r = _receive_dictio(self.sock, self.hostPort)
         if not UDP:
             self.sock.close()
         if Channel.Perf: print('transaction time: %.5f'%(_timer()-ts))
         #print(f'reply from channel {self.name}: {r}')
         return r
     
 class PVs(object): #inheritance from object is needed in python2 for properties to work
@@ -553,34 +557,39 @@
         self.channelMap = {}
         if isinstance(ldoPars[0], str):
             _printe('Device,parameter should be a list or tuple')
             return
             sys.exit(1)
         for ldoPar in ldoPars:
             ldo = ldoPar[0]
-            pars = ldoPar[1] if len(ldoPar) > 1 else ''
+            if len(ldoPar) == 1:
+                pars = '*'
+            else:
+                if isinstance(ldoPar[1],str):
+                    ldoPar = list(ldoPar)
+                    ldoPar[1] = [ldoPar[1]]
+                pars = ldoPar[1:]
             try:    ldo = ldo.split(NSDelimiter)
             except: pass
             ldo = tuple(ldo)
-            if isinstance(pars,str): pars = [pars]
+            #if isinstance(pars,str): pars = [[pars]]
             # ldo is in form: (hostName,devName)
             ldoHost = _hostPort(ldo)
             cnsNameDev = NSDelimiter.join(ldo)
             if ldoHost not in self.channelMap:
-                self.channelMap[ldoHost] = {cnsNameDev:[pars]}
-                # _printv(f'created self.channelMap[{ldoHost,self.channelMap[ldoHost]}')
+                self.channelMap[ldoHost] = {cnsNameDev:pars}
+                #_printv(f'created self.channelMap[{ldoHost,self.channelMap[ldoHost]}')
             else:
-                try:
-                    # _printv(f'appending old cnsNameDev {ldoHost,cnsNameDev} with {pars[0]}')
+                if False:#try:
+                    _printv(f'try to append old cnsNameDev {ldoHost,cnsNameDev} with {pars[0]}')
                     self.channelMap[ldoHost][cnsNameDev][0].append(pars[0])
-                except:
-                    # _printv(f'creating new cnsNameDev {ldoHost,cnsNameDev} with {pars[0]}')
-                    self.channelMap[ldoHost][cnsNameDev] = [pars]
-                #print(('updated self.channelMap[%s]='%ldoHost\
-                #+ str(self.channelMap[ldoHost]))
+                else:#except:
+                    _printv(f'creating new cnsNameDev {ldoHost,cnsNameDev} with {pars[0]}')
+                    self.channelMap[ldoHost][cnsNameDev] = pars
+                print(f'updated self.channelMap[{ldoHost}: {self.channelMap[ldoHost]}')
         channelList = list(self.channelMap.items())
         _printv(f',,,,,,,,,,,,,,,,,,,channelList constructed: {channelList}')
         self.channels = [Channel(*i) for i in channelList]
         return
 
     def info(self):
         for channel in self.channels:
```

### Comparing `pvplot-0.6.7/ln/liteserver/liteserver.py` & `pvplot-0.6.9/ln/liteserver/liteserver_unlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 LA.Access.get((bpc,('yMin','yMax')))
 {('192.168.1.132:dev1', 'yMin'): {'value': 101.017, 'timestamp': 1679343794.4135463}, ('192.168.1.132:dev1', 'yMax'): {'value': 219.963, 'timestamp': 1679343794.4135463}}
 # subscribe to parameter y:
 LA.Access.subscribe(LA.testCallback,(bpc,'y'))
 Received in last 10.0s: {'records': 1240, 'acks': 10, 'bytes': 80005600.0, 'retrans': 7}
 LA.Access.unsubscribe()
 """
-__version__ = '3.1.0 2023-07-30'# use CBOR encoder
+__version__ = '3.2.0 2024-02-12'#
 #TODO: WARN.LS and ERROR.LS messages should be published in server:status
 
 import sys, time, math, traceback
 timer = time.perf_counter
 import threading
 publish_Lock = threading.Lock()
 ackCount_Lock = threading.Lock()
@@ -535,14 +535,15 @@
             devs = list(Server.DevDict)
             return devs
         else:   raise ValueError('expect cmd,args')
         
     returnedDict = {}
         
     for devParPropVal in args:
+        printv(f'devParPropVal: {devParPropVal}')
         try:
             cnsDevName,sParPropVals = devParPropVal
         except Exception as e:
             msg = 'ERR.LS in _replyData for '+str(cmdArgs)
             printi(msg)
             raise TypeError(msg) from e
```

### Comparing `pvplot-0.6.7/ln/liteserver/device/helpers.py` & `pvplot-0.6.9/ln/liteserver/device/helpers.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/i2c.py` & `pvplot-0.6.9/ln/liteserver/device/i2c_322.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """`````````````````````````````Access to I2C bus``````````````````````````
 For installation: https://www.instructables.com/Raspberry-Pi-I2C-Python/
 I2C speed: https://www.raspberrypi-spy.co.uk/2018/02/change-raspberry-pi-i2c-bus-speed/
 """
-__version__ = 'v3.2.2 2023-09-22'# HMC5883: swapped axxes y and z, added samples for HMC an MMC
+__version__ = 'v3.2.2 2023-09-22'# 
 print(f'i2c: {__version__}')
 #TODO: display errors and warnings in device status
 #TODO: the DevClassMap should be incorporated into I2C class
 
 import sys, time
 timer = time.perf_counter
 import struct
@@ -239,19 +239,19 @@
         return xzy[0],xzy[2],xzy[1]
         
     def read(self, timestamp):
         pv = {'X':[], 'Y':[], 'Z':[], 'M':[], 't':[]}
         ts = time.time()
         samples = self.devLDOs[self.name+'_samples'].value[0]
         for sample in range(samples):
+            print(f'samples: {sample}')
             try:    xyz = list(self.read_xyz(timestamp))
             except Exception:# as e:
                 printw(f'Exception in read_xyz: {e}')
                 return
-            pv['t'].append(round(time.time() - ts,6))
             ovf = -4096# Hardware indication of the overflow
             g = self.fsr/self.dataRange[1]
             gc = self.gainCorrection if self.correct else (1.,1.,1.)
             for i in (X,Y,Z):
                 v = xyz[i]
                 xyz[i] = 10. if v == ovf else round(v*g*gc[i],6)
             printv(f'xyz {self.name}: {xyz}')
@@ -412,15 +412,15 @@
         self.set_bandwidth()
 
         printv(f'Sensor MMC5983MA created: {n, self.addr}')
 
     def read(self, timestamp):
         pv = {'X':[], 'Y':[], 'Z':[], 'M':[], 't':[]}
         da = self.name
-
+        
         ts = time.time()
         samples = self.devLDOs[self.name+'_samples'].value[0]
         for sample in range(samples):
             #print(f'sample {sample}')
             if I2C_MMC5983MA.cm_freq == 0:
                 # ask to measure field
                 I2C.write_i2c_byte(self.addr, 0x09,0x1)
@@ -449,15 +449,15 @@
                 pv[axis].append(round(v,6))
                 m2 += v**2
             # calculate magnitude
             pv['M'].append(round(float(np.sqrt(m2)),6))
             printv(f"xyzm {self.name}: {pv['X'],pv['Y'],pv['Z'],pv['M']}")
 
         # update PVs
-        rtime = round(time.time()-ts,6)
+        rtime = round(time.time()-ts,6)        
         self.devLDOs[self.name+'_readout'].set_valueAndTimestamp(rtime, timestamp)
         for suffix,value in pv.items():
             self.devLDOs[self.name+'_'+suffix].set_valueAndTimestamp(value, timestamp)
 
         # force the temperature update once per 10s
         tm = time.time()
         if tm - self.lastSlowUpdate > 10.:
```

### Comparing `pvplot-0.6.7/ln/liteserver/device/i2c_312.py` & `pvplot-0.6.9/ln/liteserver/device/i2c_312.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/i2c_320.py` & `pvplot-0.6.9/ln/liteserver/device/i2c_320.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/i2c_322.py` & `pvplot-0.6.9/ln/liteserver/device/i2c_TLV493D.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,175 @@
 """`````````````````````````````Access to I2C bus``````````````````````````
 For installation: https://www.instructables.com/Raspberry-Pi-I2C-Python/
 I2C speed: https://www.raspberrypi-spy.co.uk/2018/02/change-raspberry-pi-i2c-bus-speed/
 """
-__version__ = 'v3.2.2 2023-09-22'# 
-print(f'i2c: {__version__}')
+__version__ = 'v3.1.1 2023-08-29'# Added TLV
 #TODO: display errors and warnings in device status
-#TODO: the DevClassMap should be incorporated into I2C class
 
-import sys, time
-timer = time.perf_counter
+import time
 import struct
-from functools import partial
 import numpy as np
 import ctypes
 c_uint16 = ctypes.c_uint16
 c_uint8 = ctypes.c_uint8
 
 #import smbus as I2CSMBus
 from smbus2 import SMBus as I2CSMBus
 
 from liteserver.liteserver import LDO
 
+"""def _print(msg, mgr=None):
+    print(msg)
+    if mgr: mgr.set_status(msg)
+def printi(msg, mgr=None):    _print(f'inf_i2c: {msg}', mgr)
+def printw(msg, mgr=None):    _print(f'WARNING_i2c: {msg}', mgr)
+def printe(msg, mgr=None):    _print(f'ERROR_i2c: {msg}', mgr)
+"""
 def printi(msg): print(f'inf_i2c: {msg}')
 def printw(msg): print(f'WARNING_i2c: {msg}')
 def printe(msg): print(f'ERROR_i2c: {msg}')
 def printv(msg):
     if I2C.verbosity>0: print(f'i2cDbg{I2C.verbosity}: {msg}')
 def printvv(msg):
     if I2C.verbosity>1: print(f'i2cDbg{I2C.verbosity}: {msg}')
-def tosigned12(n:int):
-    n = n & 0xfff
-    return (n ^ 0x800) - 0x800
 
 X,Y,Z = 0,1,2
 
 class I2C():
     """Static class with I2C access methods."""
-    verbosity = 0# 1: Show log messages, 2: show even more.
-    DeviceClassMap = {}# Map of device classes: {addr: DeviceClass,,,,}
-    # filled by add_deviceClasses()
-    DeviceMap = {}# Map of existing devices: {(muxCh,addr): DeviceClass,...}
-    LDOMap = {}# Map of Process Variables of I2C devices, filled by init()
-    # filled by init()
+    verbosity = 0# 1: Show log messages, 2: show even more. 
+    DeviceName = {# map of supported devices: {address:deviceName,...}
+    0x0d:'QMC5883',
+    0x30:'MMC5983MA',
+    0x1e:'HMC5883',
+    0x48:'ADS1115',
+    0x49:'ADS1015',
+    0x5E:'TLV493D',
+    
+    }
+    DeviceMap = {}# 
+
     muxAddr = 0x77# address of the multiplexer on I2C bus
     busMask = 0xFF# bit-mask of enabled sub-busses
     I2CBus = 1 # Rpi I2C bus is 1
-    CurrentMuxCh = None
+    CurrentMuxCh = 0
     # Note: pigpio wrappers for accessing I2C have overhead ~0.5ms/transaction
     SMBus = I2CSMBus(I2CBus)
 
     def write_i2cMux(value):
         if I2C.muxAddr is None:
             return
         try:
-            printv(f'write_i2cMux: {value}')
+            printvv(f'write_i2cMux: {value}')
             I2C.SMBus.write_byte_data(I2C.muxAddr, 0, value)
             if value == 0:
                 printi('Mux is Reset (set to 0).')
         except Exception as e:
             printw((f'There is no I2C mux at {I2C.muxAddr}: {e},\n'
             ' Only directly visible devices will be served'))
             I2C.muxAddr = None
     def enable_i2cMuxChannel(ch:int):
-        #print(f'enable_i2c mux {ch}, current: {I2C.CurrentMuxCh}')
         if ch == 0:
             I2C.write_i2cMux(0)
         elif ch != I2C.CurrentMuxCh:
             I2C.write_i2cMux(1<<(ch-1))
         I2C.CurrentMuxCh = ch
     def read_i2c_byte(addr:tuple, reg:int):
-        #print(f'read_i2c_byte: {addr, reg}')
         I2C.enable_i2cMuxChannel(addr[0])
         return I2C.SMBus.read_byte_data(addr[1], reg)
     def read_i2c_word(addr:tuple, reg:int):
-        #print(f'read_i2c_word: {addr, reg}')
         I2C.enable_i2cMuxChannel(addr[0])
         return I2C.SMBus.read_word_data(addr[1], reg)
     def write_i2c_byte(addr:tuple, reg:int, value:int):
-        #print(f'write_i2c_byte: {addr,reg,value}')
         I2C.enable_i2cMuxChannel(addr[0])
         I2C.SMBus.write_byte_data(addr[1], reg, value)
     def write_i2c_word(addr:tuple, reg, value):
-        #print(f'write_i2c_word: {addr,reg,value}')
         I2C.enable_i2cMuxChannel(addr[0])
         I2C.SMBus.write_word_data(addr[1], reg, value)
     def read_i2c_data(addr:tuple, reg:int, count=None):
-        #print(f'read_i2c_data: {addr, reg, count}')
         I2C.enable_i2cMuxChannel(addr[0])
         if count is None:
             return I2C.SMBus.read_block_data(addr[1], reg)
         else:
             return I2C.SMBus.read_i2c_block_data(addr[1], reg, count)
 
+    def create_DeviceMap(mask=0xff):
+        """Returns map of devices, present on I2C. 
+        It detects devices on connected to multiplexed sub-busses.
+        """
+        devMap = {}
+        def scan(subbus:int):
+            # scan I2CBus with current setting of the mux
+            printv(f'scanning sub-bus {subbus}')
+            r = {}
+            for devAddr in range(128):
+                try:
+                    h = I2C.read_i2c_byte((subbus,devAddr),0)
+                    if devAddr < 0x70:# if it is not a multiplexer
+                        devName = I2C.DeviceName.get(devAddr, 'Unknown')
+                        r[(subbus,devAddr)] = devName
+                        printv(f'Detected {devName}@{subbus,devAddr}')
+                except OSError:
+                    pass
+                except Exception as e:
+                    printe(f'in create_DeviceMap: {devAddr,e}')
+            return r
+        for ch in range(8):
+            chmask = 1<<ch
+            if mask&chmask == 0:
+                continue
+            devMap.update(scan(ch+1))
+        return devMap
+
+    def _scanI2C(busMask = 0xFF):
+        for busAddr,devName in I2C.DeviceMap.items():
+            printv(f'Registering {busAddr,devName}')
+            if devName == 'Unknown':
+                continue
+            self.i2cBusaddrDev[busAddr] = DevClassMap[devName](busAddr)
+            pars.update(self.i2cBusaddrDev[busAddr].pPV)
+
+    #```````````````I2C Initialization``````````````````````````````````````````
+    def __init__(self, mask=0xFF, muxAddr=0x77):
+        """Detects devices on I2C multiplexed sub-buses and enables them.
+        The mask is 8-bit mask of sub-busses to be enabled.
+        """  
+        I2C.busMask = mask
+        I2C.muxAddr = muxAddr
+        printi(f'i2c.version: {__version__}, verbosity: {I2C.verbosity}')
+        printi(f'I2CSMBus opened: using smbus package, busMask={I2C.busMask}')
+        """Scan multiplexed I2C sub-busses"""
+        if I2C.busMask:
+            printi(f'muxAddr: {type(I2C.muxAddr), I2C.muxAddr}')
+            I2C.DeviceMap = I2C.create_DeviceMap(I2C.busMask)
+        else:
+            I2C.DeviceMap = {}
+            try:    I2C.write_i2cMux(0)# reset the mux
+            except: pass
+        I2C.CurrentMuxCh = 0
+        printi(f'I2C devices detected: {I2C.DeviceMap}')
+
 class I2CDev():
     """Base class for I2C devices"""
     def __init__(self, addr:tuple, sensorType:str, model):
         # addr is (mux channel, address on mux channel) 
         #self.name = self.__class__.__name__+'_'+'.'.join([str(i) for i in addr])
-        self.name = f'I2C{addr[0]}'
+        self.name = f'I2C{addr[0]}'       
         self.addr = addr
-        self.model = model
-        self.lastSlowUpdate = 0.
-        self.devLDOs = {
-            self.name+'_sensor': LDO('R','Sensor model and type',
-              f'{model} {sensorType}'),
-            self.name+'_readout': LDO('R','Readout time', 0., units='s'),
+        self.pPV = {
+            self.name+'_sensor': LDO('R','Sensor_type model',
+              f'{sensorType},{model}')
         }
 
     def read(self, timestamp):
         print(f'I2CDev.read() not implemented for {self.name}')
         return
 
     def calibration(self, option:str):
-        printw(f'Calibration is not implemented for {self.name, self.model}')
+        print(f'I2CDev.calibrate() is not implemented for {self.name}')
 
 #```````````````````HMC5883 compass````````````````````````````````````````````
 class HMC5883_bits_ConfigRegA(ctypes.LittleEndianStructure):
     _fields_ = [
         ("MS", c_uint8, 2),# Measurement Configuration Bits.
         ("DO", c_uint8, 3),# Data Output Rate.
         ("MA", c_uint8, 2),]# Moving average. 0=1, 1=2, 2=4, 3=8.
@@ -149,14 +202,15 @@
         try:
             devId = I2C.read_i2c_data(self.addr, 0x0a, 3)
         except:
             printe(f'There is no device with address {self.addr}')
             sys.exit()
         if devId != [0x48, 0x34, 0x33]:
             raise RuntimeError(f'Chip is not HMC5883L: {[hex(i) for i in devId]}')
+        printi(f'Sensor detected: {self.name,self.addr}')
 
         # Initialize HMC5883
         self.configRegA = HMC5883_ConfigRegA()
         self.configRegA.b.DO = 4# Data rate 4: 15 Hz, 5:30, 6:75
         self.configRegA.b.MA = 3# Average window, 3: 8 samples
         self.configRegA.b.MS = 0# Normal Measurements
         I2C.write_i2c_byte(self.addr, self.configRegA.addr, self.configRegA.B)
@@ -173,104 +227,89 @@
 
         gain = (1370, 1090, 820, 660, 440, 390, 330, 230) #Lsb/Gauss
         lvFSR = [str(round(self.dataRange[1]/g,3)) for g in gain]
         # field strength of the excitation strap on X,Y,Z axes
         self.testField = (1.16, 1.16, 1.08)
         self.gainCorrection = [1., 1., 1.]
         self.correct = False
-        self.xzySumCount = 0
-        self.xzySum = np.zeros(3)
+        self.xyzSumCount = 0
+        self.xyzSum = np.zeros(3)
 
-        n = self.name
-        self.devLDOs.update({
-            n+'_FSR': LDO('WE','Full scale range is [-FSR:+FSR]',
+        self.pPV.update({
+            self.name+'_FSR': LDO('WE','Full scale range is [-FSR:+FSR]',
                 [lvFSR[self.configRegB.b.FSR]], legalValues=lvFSR, units='G',
                 setter=self.set_FSR),
-            n+'_samples': LDO('RWE','Number of samples', [1]),
-            n+'_t': LDO('R','Time axis for samples', [0.], units='s'),
-            n+'_X': LDO('R','X-axis field', 0., units='G'),
-            n+'_Y': LDO('R','Y-axis field', 0., units='G'),
-            n+'_Z': LDO('R','Z-axis field', 0., units='G'),
-            n+'_M': LDO('R','Magnitude', 0., units='G'),
+            self.name+'_X': LDO('R','X-axis field', 0., units='G'),
+            self.name+'_Y': LDO('R','Y-axis field', 0., units='G'),
+            self.name+'_Z': LDO('R','Z-axis field', 0., units='G'),
+            self.name+'_M': LDO('R','Magnitude', 0., units='G'),
         })
         printv(f'CRA: {hex(I2C.read_i2c_byte(self.addr, self.configRegA.addr))}')
-        printv(f'Sensor HMC5883 detected: {self.name,self.addr}')
+        printi(f'Created {self.name}')
 
     def _set_FSR(self, idx:int):
         self.configRegB.b.FSR = idx
         #print(f'>configRegB: {self.configRegB.addr, self.configRegB.B}')
         I2C.write_i2c_byte(self.addr, self.configRegB.addr, self.configRegB.B)
         r = I2C.read_i2c_byte(self.addr, self.configRegB.addr)
         printi(f'configRegB: {hex(r)}')
 
     def set_FSR(self):
         #print(f'>set_FSR')
-        pv = self.devLDOs[self.name+'_FSR']
+        pv = self.pPV[self.name+'_FSR']
         fsrTxt = pv.value[0]
-        printv(f'fsr: {fsrTxt, type(fsrTxt)}, lv: {pv.legalValues}')
+        print(f'fsr: {fsrTxt, type(fsrTxt)}, lv: {pv.legalValues}')
         self.fsr = float(fsrTxt)
         idx = pv.legalValues.index(fsrTxt)
         self._set_FSR(idx)
 
-    def read_xyz(self, timestamp):
-        ts = timer()
+    def read_xyz(self):
         if I2C_HMC5883.mode == 1:   # Single measurement
             I2C.write_i2c_byte(self.addr, self.modeReg.addr, I2C_HMC5883.mode)
+            ts = time.time()
             while I2C.read_i2c_byte(self.addr, 0x9) & 1 == 0:
-                if timer() - ts > 0.010:# should last ~1ms
-                    printw(f'Timeout reading {self.name, self.addr}')
+                if time.time() - ts > 0.010:# should last ~1ms
+                    printw(f'Timeout reading {self.name}')
                     return
         try:
             r = I2C.read_i2c_data(self.addr, 0x00, 10)
         except Exception as e:
-            printw(f'reading_xyz {self.name,self.addr}: {e}')
+            printw(f'reading {self.name}: {e}')
             return
-        printv(f'read {self.name}: {[hex(i) for i in r]}')
-        xzy = struct.unpack('>3h', bytearray(r[3:9]))
+        printvv(f'read {self.name}: {[hex(i) for i in r]}')
+        xyz = struct.unpack('>3h', bytearray(r[3:9]))
         if r[0] & 1:# Internal field is excited, collect statistics
-            printv(f'xzy.max: {max(xzy)}, {self.xzySumCount}')
-            if max(xzy) < self.dataRange[1]*0.8 and self.xzySumCount != None:
-                printv(f'self.xzySumCount {self.xzySumCount}, {self.xzySum}')
-                self.xzySumCount += 1
-                self.xzySum += xzy
+            printv(f'xyz.max: {max(xyz)}, {self.xyzSumCount}')
+            if max(xyz) < self.dataRange[1]*0.8 and self.xyzSumCount != None:
+                printv(f'self.xyzSumCount {self.xyzSumCount}, {self.xyzSum}')
+                self.xyzSumCount += 1
+                self.xyzSum += xyz
             else:
-                self.xzySumCount = None
-                self.xzySum = np.zeros(3)
+                self.xyzSumCount = None
+                self.xyzSum = np.zeros(3)
                 printe(f'Correction processing failed for {self.name}')
-        return xzy[0],xzy[2],xzy[1]
+        return xyz
         
     def read(self, timestamp):
-        pv = {'X':[], 'Y':[], 'Z':[], 'M':[], 't':[]}
-        ts = time.time()
-        samples = self.devLDOs[self.name+'_samples'].value[0]
-        for sample in range(samples):
-            print(f'samples: {sample}')
-            try:    xyz = list(self.read_xyz(timestamp))
-            except Exception:# as e:
-                printw(f'Exception in read_xyz: {e}')
-                return
-            ovf = -4096# Hardware indication of the overflow
-            g = self.fsr/self.dataRange[1]
-            gc = self.gainCorrection if self.correct else (1.,1.,1.)
-            for i in (X,Y,Z):
-                v = xyz[i]
-                xyz[i] = 10. if v == ovf else round(v*g*gc[i],6)
-            printv(f'xyz {self.name}: {xyz}')
-            m2 = 0.
-            for axis,value in zip('XYZ',xyz):
-                pv[axis].append(round(value,6))
-                m2 += value**2
-            # calculate magnitude
-            magn = round(float(np.sqrt(m2)),6) if max(xyz) < 10. else 3*10.
-            pv['M'].append(magn)
-            printv(f"xyzm {self.name}: {pv['X'][-1],pv['Y'][-1],pv['Z'][-1],pv['M'][-1]}")
-        rtime = round(time.time()-ts,6)
-        self.devLDOs[self.name+'_readout'].set_valueAndTimestamp(rtime, timestamp)
-        for suffix,value in pv.items():
-            self.devLDOs[self.name+'_'+suffix].set_valueAndTimestamp(value, timestamp)
+        try:    xyz = list(self.read_xyz())
+        except: return
+        ovf = -4096# Hardware indication of the overflow
+        g = self.fsr/self.dataRange[1]
+        gc = self.gainCorrection if self.correct else (1.,1.,1.)
+        for i in (X,Y,Z):
+            v = xyz[i]
+            xyz[i] = 10. if v == ovf else round(v*g*gc[i],6)
+        x,y,z = xyz
+        m = 10. if max(x,y,z) == 10. else round(float(np.sqrt(x**2 + y**2 + z**2)),6)
+        printv(f'xyzm {self.name}: {x,y,z,m}')
+        da = self.name
+        self.pPV[da+'_X'].set_valueAndTimestamp(x, timestamp)
+        self.pPV[da+'_Y'].set_valueAndTimestamp(y, timestamp)
+        self.pPV[da+'_Z'].set_valueAndTimestamp(z, timestamp)
+        self.pPV[da+'_M'].set_valueAndTimestamp(m, timestamp)
 
     def calibration(self, calibMode:str):
         if calibMode == 'Off':
             printi(f'Calibration is disabled for {self.name}')
             self.correct = False
         elif calibMode == 'SelfTest':
             self.xyzSumCount = 0.
@@ -310,240 +349,131 @@
         ("FSR", c_uint8, 2), #Full scale range, 0:2G, 1:8G
         ("OSR", c_uint8, 2),]#Over sample ratio, 512,256,128,64
 class QMC5883_ConfigRegA(ctypes.Union):
     _fields_ = [("b", QMC5883_bits_ConfigRegA),
                ("B", c_uint8),]
     addr = 0x9
 class I2C_QMC5883(I2CDev):
-    #TODO: add samples as in MMC5983MA
     mode = 1# Measurement mode 1:continuous
     def __init__(self, devAddr):
         super().__init__(devAddr, 'Magnetometer', 'QMC5883L')
         try:    devId = I2C.read_i2c_byte(self.addr, 0x0d)
         except:
             printe(f'There is no device with address {self.addr}')
             sys.exit()
         if devId != 0xff:
             raise RuntimeError(f'Chip is not QMC5883L: {devId}')
+        printi(f'Sensor detected: {self.name}')
 
         # Initialize QMC5883
         self.configRegA = QMC5883_ConfigRegA()
         self.configRegA.b.MODE = I2C_QMC5883.mode
         self.configRegA.b.DO = 0# 10Hz. No effect.
         self.configRegA.b.FSR = 0# 2G
         self.configRegA.b.OSR = 0# OverSampling = 256. Less noise
         I2C.write_i2c_byte(self.addr, self.configRegA.addr, self.configRegA.B)
 
         lvFSR = ('2.', '8.')
-        self.devLDOs.update({
+        self.pPV.update({
         self.name+'_FSR': LDO('WE','Full scale range is [-FSR:+FSR]',
             lvFSR[self.configRegA.b.FSR], legalValues=lvFSR, units='G',
             setter=self.set_FSR),
         self.name+'_X': LDO('R','X-axis field', 0., units='G'),
         self.name+'_Y': LDO('R','Y-axis field', 0., units='G'),
         self.name+'_Z': LDO('R','Z-axis field', 0., units='G'),
         self.name+'_M': LDO('R','Magnitude', 0., units='G'),
         self.name+'_T': LDO('R','Relative temperature', 0., units='C'),
         })
-        printv(f'Sensor QMC5883 created: {self.name, self.addr}')
+        printi(f'Created {self.name}')
 
     def set_FSR(self):
-        pv = self.devLDOs[self.name+'_FSR']
+        pv = self.pPV[self.name+'_FSR']
         self.fsr = pv.value[0]
         idx = pv.legalValues.index(str(self.fsr))
         self.configRegA.b.FSR = idx
         #print(f'fsr: {self.fsr,idx}')
         #print(f'configRegA: {self.configRegA.addr, self.configRegA.B}')
         I2C.write_i2c_byte(self.addr, self.configRegA.addr, self.configRegA.B)
 
     def read(self, timestamp):
-        ts = timer()
         pv = {'X':0., 'Y':0., 'Z':0., 'M':0.,'T':0.}
         # note: reading more than 6 bytes may give wrong result when cable is long
         try:
             r = I2C.read_i2c_data(self.addr, 0x00, 6)
         except Exception as e:
-            printw(f'reading {self.name,self.addr}: {e}')
+            printw(f'reading {self.name}: {e}')
             return
-        rtime = round(timer()-ts,6)
-        self.devLDOs[self.name+'_readout'].set_valueAndTimestamp(rtime, timestamp)
         #printv(f'conf,status: {hex(r[0x9]), hex(r[0x6])}')
         printvv(f'read {self.name}: {[hex(i) for i in r]}')
         g = self.fsr/32768.
         xyz = struct.unpack('<3h', bytearray(r[:6]))
         pv['X'],pv['Y'],pv['Z'] = [round(g*i,6) for i in xyz]
         pv['M'] = round(float(np.sqrt(pv['X']**2 + pv['Y']**2 +pv['Z']**2)), 6)
         r = I2C.read_i2c_data(self.addr, 0x07, 2)
         pv['T'] = round(struct.unpack('<h', bytearray(r))[0]/100. + 30.,2)
         printv(f"xyzm {self.name}: {pv['X'],pv['Y'],pv['Z'],pv['M'],pv['T']}")
         for suffix,value in pv.items():
-            self.devLDOs[self.name+'_'+suffix].set_valueAndTimestamp(value, timestamp)
+            self.pPV[self.name+'_'+suffix].set_valueAndTimestamp(value, timestamp)
 
 #```````````````````MMC5983MA compass```````````````````````````````````````````
-MMC5983_bandwidth = {'100':0, '200':1, '400':2, '800':3}# Bandwidth of the decimation filter in Hz, it controls the duration of each measurement
 class I2C_MMC5983MA(I2CDev):
-    cm_freq = 0x0# Continuous mode off
-    FSR = 8.# Full scale range in Gauss
+    cm_freq = 0x0# Continuous mode, frequency=1Hz
+    FSR = 8# Full scale range in Gauss
     def __init__(self, devAddr):
         super().__init__(devAddr, 'Magnetometer', 'MMC5983MA')
         devID = I2C.read_i2c_byte(self.addr, 0x2f)
         sensStatus = I2C.read_i2c_byte(self.addr, 0x8)
         printv(f'sensStatus: {sensStatus}')
         if sensStatus&0x10 == 0:
             raise RuntimeError('Chip could not read its memory')
         if devID != 0x30:
             raise RuntimeError(f'MMC5983 has wrong address: {devID}')
         printv(f'MMC5983MA ID: {devID}')
-
-        n = self.name
-        self.devLDOs.update({
-        n+'_bandwidth': LDO('RWE','bandwidth', ['100'], units='Hz',
-            legalValues=('100','200','400','800'), setter=self.set_bandwidth),
-        n+'_samples': LDO('RWE','Number of samples', [1]),
-        n+'_t': LDO('R','Time axis for samples', [0.], units='s'),
-        n+'_X': LDO('R','X-axis field', [0.], units='G'),
-        n+'_Y': LDO('R','Y-axis field', [0.], units='G'),
-        n+'_Z': LDO('R','Z-axis field', [0.], units='G'),
-        n+'_M': LDO('R','Magnitude', [0.], units='G'),
-        n+'_T': LDO('R','Sensor temperature', 0., units='C'),
-        })
+        printi(f'Sensor detected: {self.name}')
         I2C.write_i2c_byte(self.addr, 0x9, 0x0)
+        I2C.write_i2c_byte(self.addr, 0xa, 0x3)
         I2C.write_i2c_byte(self.addr, 0xb, I2C_MMC5983MA.cm_freq)
         I2C.write_i2c_byte(self.addr, 0xc, 0x0)
-        self.set_bandwidth()
 
-        printv(f'Sensor MMC5983MA created: {n, self.addr}')
+        self.pPV.update({
+        self.name+'_X': LDO('R','X-axis field', 0., units='G'),
+        self.name+'_Y': LDO('R','Y-axis field', 0., units='G'),
+        self.name+'_Z': LDO('R','Z-axis field', 0., units='G'),
+        self.name+'_M': LDO('R','Magnitude', 0., units='G'),
+        self.name+'_T': LDO('R','Sensor temperature', 0., units='C'),
+        })
+        printi(f'Created {self.name}')
 
     def read(self, timestamp):
-        pv = {'X':[], 'Y':[], 'Z':[], 'M':[], 't':[]}
+        pv = {'X':0., 'Y':0., 'Z':0., 'M':0.,'T':0.}
         da = self.name
-        
-        ts = time.time()
-        samples = self.devLDOs[self.name+'_samples'].value[0]
-        for sample in range(samples):
-            #print(f'sample {sample}')
-            if I2C_MMC5983MA.cm_freq == 0:
-                # ask to measure field
-                I2C.write_i2c_byte(self.addr, 0x09,0x1)
-            # wait for measurement to complete
-            for ntry in range(3):
-                time.sleep(self.integrationTime)
-                status = I2C.read_i2c_byte(self.addr, 0x8)
-                if status&0x1:
-                    break
-            printv(f'MStatus = {hex(status)}')
-            try:
-                r = I2C.read_i2c_data(self.addr, 0x00, 7)
-            except Exception as e:
-                printw(f'reading {self.name}: {e}')
-                return
-            printv(f'regs: {[hex(i) for i in r]}')
-            # decode 18-bit values xyz18
-            xyz17_2 = [i for i in struct.unpack('>3H', bytearray(r[:6]))]
-            xyzOut2 = ((r[6]>>6)&3, (r[6]>>4)&3,(r[6]>>2)&3)
-            xyz18 = [((xyz17_2[i])<<2) + xyzOut2[i] for i in range(3)]
-            printv(f'xyz18: {[hex(i) for i in xyz18]}')
-            pv['t'].append(round(time.time() - ts,6))
-            m2 = 0.
-            for axis,value in zip('XYZ',xyz18):
-                v = (value/0x20000-1.)*I2C_MMC5983MA.FSR
-                pv[axis].append(round(v,6))
-                m2 += v**2
-            # calculate magnitude
-            pv['M'].append(round(float(np.sqrt(m2)),6))
-            printv(f"xyzm {self.name}: {pv['X'],pv['Y'],pv['Z'],pv['M']}")
-
-        # update PVs
-        rtime = round(time.time()-ts,6)        
-        self.devLDOs[self.name+'_readout'].set_valueAndTimestamp(rtime, timestamp)
-        for suffix,value in pv.items():
-            self.devLDOs[self.name+'_'+suffix].set_valueAndTimestamp(value, timestamp)
-
-        # force the temperature update once per 10s
-        tm = time.time()
-        if tm - self.lastSlowUpdate > 10.:
-            self.lastSlowUpdate = tm
-            # ask to measure temperature
+        if I2C_MMC5983MA.cm_freq == 0:
             I2C.write_i2c_byte(self.addr, 0x09,0x2)
-            # wait for measurement to complete
-            for ntry in range(3):
-                
-                status = I2C.read_i2c_byte(self.addr, 0x8)
-                if status&0x2:
-                    break
-            temp = I2C.read_i2c_byte(self.addr, 0x7)
-            printv(f'TStatus = {hex(status)}, temp: {temp}')
-            temp = round(-75. + temp*0.8,2)
-            self.devLDOs[self.name+'_T'].set_valueAndTimestamp(temp, timestamp)
-
-    def set_bandwidth(self):
-        v = self.devLDOs[self.name+'_bandwidth'].value[0]
-        I2C.write_i2c_byte(self.addr, 0xa, MMC5983_bandwidth[v])
-        self.integrationTime = 1./float(v)
-        print(f'>set_bandwidth {v}, integration time:{self.integrationTime}')
-
-#```````````````````TLV493D magnetometer```````````````````````````````````````
-class I2C_TLV493D(I2CDev):
-    UDataMax = 2048# Max unsigned readout value
-    LSB = 0.98# Gauss per Low Significant Bit = 0.98
-    LinearRange = (-1300.0, +1300.0)# Gauss
-    LSBT = 1.1# Celsius Degree per LSB for temperature reading
-    MaxRate = 1./3300# Fast update rate is automatic, 3.3 KHz
-    def __init__(self, devAddr):
-        printv(f'I2C_TLV493D {devAddr}')
-        super().__init__(devAddr, 'Magnetometer', 'TLV493D')
-        self.devLDOs.update({# Add LDOs
-            self.name+'_X': LDO('R','X-axis field', 0., units='G'),
-            self.name+'_Y': LDO('R','Y-axis field', 0., units='G'),
-            self.name+'_Z': LDO('R','Z-axis field', 0., units='G'),
-            self.name+'_M': LDO('R','Magnitude', 0., units='G'),
-            self.name+'_T': LDO('R','Temperature', 0., units='C'),
-        })
-        regs = I2C.read_i2c_data(self.addr, 0x0, 7)
-        printv(f'regs: {[hex(i) for i in regs]}')
-
-        # Set device to Low-power mode, all other modes can hangup ADC and cause I2C bus locks.
-        I2C.write_i2c_byte(self.addr, 1, 0x1)# Low-power mode
-        #ISSUE#I2C.write_i2c_byte(self.addr, 1, 0x7)# Master Controlled Mode
-        printv(f'Sensor TLV493D created: {self.name, self.addr}')
+            time.sleep(0.01)
+        t = I2C.read_i2c_byte(self.addr, 0x7)
+        #printv(f't: {hex(t)}')
+        pv['T']= round(-75. + t*0.8,2)
+        if I2C_MMC5983MA.cm_freq == 0:
+            I2C.write_i2c_byte(self.addr, 0x09,0x1)
+            time.sleep(0.01)
+        v = I2C.read_i2c_byte(self.addr, 0x8)
+        try:
+            r = I2C.read_i2c_data(self.addr, 0x00, 7)
+        except Exception as e:
+            printw(f'reading {self.name}: {e}')
+            return
+        #TODO: extract 18-bit precision from r[7]
+        #printv(f'r: {[hex(i) for i in r]}')
+        pv['X'],pv['Y'],pv['Z'] = [round((i/0x8000-1.)*I2C_MMC5983MA.FSR,6)\
+            for i in struct.unpack('>3H', bytearray(r[:6]))]
+        pv['M'] = round(float(np.sqrt(pv['X']**2 + pv['Y']**2 +pv['Z']**2)), 6)
+        printv(f"xyzmt {self.name}: {pv['X'],pv['Y'],pv['Z'],pv['M'],pv['T']}")
+        for suffix,value in pv.items():
+            self.pPV[self.name+'_'+suffix].set_valueAndTimestamp(value, timestamp)
 
-    def read(self, timestamp):
-        # For low power mode we might need to turn Low Power On, wait for DP bit, readout, then set Low Power Off
-        m1 = self.UDataMax
-        m2 = m1*2
-        ts = timer()
-        # The waiting for conversion does not improve anything
-        #while timer()-ts < 0.09:
-        r = I2C.read_i2c_data(self.addr, 0x0, 7)
-        #    if (r[5])&0x10:# Conversion completed
-        #        break
-        #printv(f'r5: {hex(r[5]), round(timer()-ts,6)}')
-        rtime = round(timer()-ts,6)
-        self.devLDOs[self.name+'_readout'].set_valueAndTimestamp(rtime, timestamp)
-        printv(f'read: {[hex(i) for i in r]}, {rtime}')
-        x = tosigned12((r[0]<<4) + ((r[4]>>4)&0xF))
-        y = tosigned12((r[1]<<4) + (r[4]&0xF))
-        z = tosigned12((r[2]<<4) + (r[5]&0xF))
-        printv(f'xyz: {x,y,z}')
-        m = round(float(np.sqrt(x**2 + y**2 + z**2)), 6)
-
-        # update parameters
-        for suffix,v in zip('XYZM', (x,y,z,m)):
-            v*= self.LSB
-            self.devLDOs[self.name+'_'+suffix].set_valueAndTimestamp(v, timestamp)
-        # force the temperature update once per 10s
-        tm = time.time()
-        if tm - self.lastSlowUpdate > 10.:
-            self.lastSlowUpdate = tm
-            t7_0 = r[6]#I2C.read_i2c_byte(self.addr, 6)
-            t11_8 = r[3]#I2C.read_i2c_byte(self.addr, 3)
-            tbits = ((t11_8&0xF0)<<4) + t7_0
-            t = (tbits - 340.)*self.LSBT + 25.
-            printv(f'(tempTLV: {hex(t7_0), hex(t11_8), hex(tbits), t}')
-            self.devLDOs[self.name+'_T'].set_valueAndTimestamp(t, timestamp)
 
 #```````````````````ADS1115, ADS1015```````````````````````````````````````````
 # 4-channel 16/12 bit ADC.
 # Sampling time of 4 channels = 14ms.
 class ADS1115_bits_ConfigReg(ctypes.LittleEndianStructure):
     _fields_ = [
         ("MODE", c_uint16, 1),
@@ -565,29 +495,29 @@
         self.config = ADS1115_ConfigReg()
         self.config.W = I2C.read_i2c_word(self.addr, 1)
         self.config.b.MODE = ADS1115_SingleShot
         I2C.write_i2c_word(self.addr, 1, self.config.W )
         lvFSR = ('6.144', '4.096', '2.048', '1.024', '0.512' , '0.256')
         lvDR = {'ADS1115': ('8',     '16',   '32',   '64',  '128',  '250',  '475',  '860'),
                 'ADS1015': ('128',  '250',  '490',  '920', '1600', '2400', '3300', '300')}
-        self.devLDOs.update({
+        self.pPV.update({
         self.name+'_rlength': LDO('RWE', 'Record length, ', 1),
         self.name+'_tAxis': LDO('R', 'Time axis for samples', [0.], units='s'),
         self.name+'_nCh': LDO('RWE', 'Number of active ADC channels. Select 1 for faster performance.',
             '4', legalValues=['4','1']),
         self.name+'_diff': LDO('RWE', 'Differential mode, Ch0=AIN0-AIN1, Ch1=AIN2-AIN3', 'Single-ended', legalValues=['Single-ended','Diff']),
         self.name+'_Ch0': LDO('R', 'ADC channel 0', [0.], units='V'),
         self.name+'_Ch1': LDO('R', 'ADC channel 1', [0.], units='V'),
         self.name+'_Ch2': LDO('R', 'ADC channel 2', [0.], units='V'),
         self.name+'_Ch3': LDO('R', 'ADC channel 3', [0.], units='V'),
         self.name+'_FSR': LDO('RWE', 'FSR, Full scale range is [-FSR:+FSR]',
-            [lvFSR[self.config.b.FSR]], legalValues=lvFSR, units='V',
+            lvFSR[self.config.b.FSR], legalValues=lvFSR, units='V',
             setter=partial(self.set_pv,'FSR')),
         self.name+'_DR': LDO('RWE', 'Data rate',
-            [lvDR[model][self.config.b.DR]], units='SPS',
+            lvDR[model][self.config.b.DR], units='SPS',
             legalValues=lvDR[model], setter=partial(self.set_pv, 'DR')),
         })
         '''The following parts are handled internally
         self.name+'_MODE': LDO('RWE', 'Device operating mode', self.config.b.MODE,
             opLimits=(0,1), setter=partial(self.set_pv, 'MODE')),
         self.name+'_MUX': LDO('RWE', 'Input multiplexer config', self.config.b.MUX,
             opLimits=(0,7), setter=partial(self.set_pv,'MUX')),
@@ -603,153 +533,88 @@
         self.name+'_COMP_POL': LDO('RWE', 'Comparator polarity, active high',
             self.config.b.COMP_POL,
             opLimits=(0,1), setter=partial(self.set_pv, 'COMP_POL')),
         self.name+'_COMP_MODE': LDO('RWE', 'Window comparator',
             self.config.b.COMP_MODE,
             opLimits=(0,1), setter=partial(self.set_pv, 'COMP_MODE')),
         '''
-        printi(f'Sensor {model} created {self.name, self.addr}')
+        printi(f'Created  {model}_{self.name}')
 
     def read(self, timestamp):
         def wait_conversion():
-            tswc = timer()
+            tswc = time.time()
             if self.config.b.MODE == 1:# in Single-shot mode: wait when OS bit = 1
                 while True:
                     self.config.W = I2C.read_i2c_word(self.addr, 1)
                     if self.config.b.OS == 1:
                         break
-                    if timer() - tswc > .2:
+                    if time.time() - tswc > .2:
                         raise TimeoutError('Timeout in I2C_ADS1115')
             else:
                 # in continuous mode the OS is always 1, wait approximately one conversion period. 
-                sleepTime = max(0, 1./(self.devLDOs[self.name+'_DR'].value[0])\
+                sleepTime = max(0, 1./(self.pPV[self.name+'_DR'].value[0])\
                  - 0.0013)# 1.3ms is correction for transaction time
                 time.sleep(sleepTime)
             v = I2C.read_i2c_word(self.addr, 0)
             v = int(((v&0xff)<<8) + ((v>>8)&0xff))# swap bytes
             if v & 0x8000:  v = v - 0x10000
-            v = v/0x10000*float(self.devLDOs[da+'_FSR'].value[0])*2.
+            v = v/0x10000*self.pPV[da+'_FSR'].value[0]*2.
             return v
 
         self.config.W = I2C.read_i2c_word(self.addr, 1)
         da = self.name
-        nCh = int(self.devLDOs[da+'_nCh'].value[0])
-        if self.devLDOs[da+'_diff'].value[0].startswith('Diff'):
+        nCh = self.pPV[da+'_nCh'].value[0]
+        if self.pPV[da+'_diff'].value[0].startswith('Diff'):
             listCmd = [(0,'_Ch0'), (3,'_Ch1')]
         else:
             listCmd = [(4,'_Ch0'), (5,'_Ch1'), (6,'_Ch2'), (7,'_Ch3')]
         # set mux for first item of the list
         self.config.b.MUX = listCmd[0][0]
         self.config.b.MODE = 0 if nCh == 1 else ADS1115_SingleShot
         I2C.write_i2c_word(self.addr, 1, self.config.W )
 
         # init the sample data
-        nSamples = self.devLDOs[self.name+'_rlength'].value[0]
-        self.devLDOs[da+'_tAxis'].value = [0.]*nSamples
+        nSamples = self.pPV[self.name+'_rlength'].value[0]
+        self.pPV[da+'_tAxis'].value = [0.]*nSamples
         for mux,ch in listCmd[:nCh]:
-            self.devLDOs[da+ch].value = [0.]*nSamples
-        t0 = timer()
+            self.pPV[da+ch].value = [0.]*nSamples
+        t0 = time.time()
+        #ts = timer(), #tt = []
 
         # collect samples
         for sample in range(nSamples):
             for mux,ch in listCmd[:nCh]:
                 if nCh > 1:
                     self.config.b.MUX = mux
                     I2C.write_i2c_word(self.addr, 1, self.config.W)
                 #tt.append(round(timer()-ts,6))
                 v = wait_conversion()
-                self.devLDOs[da+ch].value[sample] = v
-            self.devLDOs[da+'_tAxis'].value[sample] = round(timer() - t0,6)
-        rtime = round(timer()-t0,6)
-        self.devLDOs[self.name+'_readout'].set_valueAndTimestamp(rtime, timestamp)
+                self.pPV[da+ch].value[sample] = v
+            self.pPV[da+'_tAxis'].value[sample] = round(time.time() - t0,6)
 
-        # invalidate timestamps to schedule LDOs for publishing
+        # invalidate timestamps to schedule PVs for publishing
         for mux,ch in listCmd[:nCh]:
-            self.devLDOs[da+ch].timestamp = timestamp
-        self.devLDOs[da+'_tAxis'].timestamp = timestamp
+            self.pPV[da+ch].timestamp = timestamp
+        self.pPV[da+'_tAxis'].timestamp = timestamp
         #tt.append(round(timer()-ts,6))
         #print(f'read time: {tt}')
 
     def set_pv(self, field):
-        pv = self.devLDOs[self.name+'_'+field]        
-        printv(f'>ADS1115.set_config {pv.name} = {pv.value[0]}')
+        pv = self.pPV[self.name+'_'+field]        
+        #print(f'>set_config {pv.name} = {pv.value[0]}')
         self.config.W = I2C.read_i2c_word(self.addr, 1)
-        printv(f'current: {hex(self.config.W)}')
-        printv(f'ADS1115.legalValues: {pv.legalValues}')
+        #print(f'current: {hex(self.config.W)}')
         try:    v = pv.legalValues.index(pv.value[0])
-        except Exception as e:
-            printv(f'exception in ADS1115.set_pv: {e}')
-            v = pv.value[0]
-        printv(f'set v: {v}')
+        except: v = pv.value[0]
         setattr(self.config.b, field, v)
-        printv(f'new: {hex(self.config.W)}')
+        #print(f'new: {hex(self.config.W)}')
         I2C.write_i2c_word(self.addr, 1, self.config.W)
 
 class I2C_ADS1015(I2C_ADS1115):
     def __init__(self, devAddr):
         printv(f'>I2C_ADS1015')
         super().__init__(devAddr, 'ADS1015')
 
-# Predefined device classes
-BuiltinDeviceMap = {
-    0x48:   I2C_ADS1115,
-    0x49:   I2C_ADS1015,
-    0x30:   I2C_MMC5983MA,
-    0x1e:   I2C_HMC5883,
-    0x0d:   I2C_QMC5883,
-    0x5e:   I2C_TLV493D,
+DevClassMap = {'MMC5983MA':I2C_MMC5983MA,
+    'ADS1115':I2C_ADS1115, 'ADS1015':I2C_ADS1015,
+    'HMC5883':I2C_HMC5883, 'QMC5883':I2C_QMC5883
 }
-I2C.DeviceClassMap = BuiltinDeviceMap
-
-def add_deviceClass(addr:int, devclass):
-    """To add or replace item in deviceClassMap by user-defined I2C device. 
-Should be called pior to scan()"""
-    i2c.DeviceClassMap[addr] = devclass
-
-def init(muxAddr:int, mask:int):
-    """Scan multiplexed I2C bus and fill i2c.DeviceMap and initialize the I2C 
-    for further use.
-    muxAddr: address of the I2C multiplexer.
-    mask: bitmask of enabled multiplexer channels
-    """
-    I2C.muxAddr = muxAddr
-    I2C.busMask = mask
-    I2C.CurrentMuxCh = 0
-    printi(f'i2c.version: {__version__}, verbosity: {I2C.verbosity}')
-    printi(f'I2CSMBus opened: using smbus package, busMask={I2C.busMask}')
-    if I2C.busMask == 0:
-        I2C.DeviceMap = {}
-        I2C.write_i2cMux(0)# reset the mux
-        if I2C.muxAddr == None:
-            sys.exit(1)
-        printi('Mux reset')
-        
-    devMap = {}
-    def scan(subbus:int):
-        printv(f'scanning sub-bus {subbus}')
-        r = {}
-        for devAddr in range(128):
-            try:
-                h = I2C.read_i2c_byte((subbus,devAddr),0)
-                if devAddr < 0x70:# if it is not a multiplexer
-                    devClass = I2C.DeviceClassMap.get(devAddr, 'Unknown')
-                    devInstance = devClass((subbus,devAddr))
-                    r[(subbus,devAddr)] = devInstance
-                    printv(f'Detected {devInstance.name}@{subbus,devAddr}')
-            except OSError:
-                pass# timeout
-            #except Exception as e:
-            #    printe(f'during scan: {devAddr,e}')
-        return r
-    for ch in range(8):
-        chmask = 1<<ch
-        if mask&chmask == 0:
-            continue
-        devMap.update(scan(ch+1))
-    printi(f'I2C devices detected: {[(dclass.name, addr, type(dclass).__name__)  for addr,dclass in devMap.items()]}')
-    I2C.DeviceMap = devMap
-    I2C.CurrentMuxCh = None
-
-    # Fill I2C.LDOMap
-    for devInstance in I2C.DeviceMap.values():
-        I2C.LDOMap.update(devInstance.devLDOs)
-    printv(f'I2C parameters added: {I2C.LDOMap.keys()}')
```

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteCNSserver.py` & `pvplot-0.6.9/ln/liteserver/device/liteCNSserver.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteGQ.py` & `pvplot-0.6.9/ln/liteserver/device/liteGQ.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteLabjack.py` & `pvplot-0.6.9/ln/liteserver/device/liteLabjack.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteMCUFEC.py` & `pvplot-0.6.9/ln/liteserver/device/liteMCUFEC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 """LiteServer for MCUFEC devices"""
-__version__ = '3.1.0 2023-08-23'# from .. import liteserver
+__version__ = '3.2.4 2024-02-27'# --stop option, handle payload=OK during set()
  
 import sys, time, threading
 timer = time.perf_counter
 import numpy as np
 import serial
 import json
 from functools import partial
 
 from .. import liteserver
 
+PV_ADCS = False# Do not host multi-dimensional parameter 'adcs'
+
 #get_data_lock = threading.Lock()
 ExecLock = threading.Lock()
 LDO = liteserver.LDO
 Device = liteserver.Device
 SerDev = None
 SerObjectEvent = threading.Event()# informs that new SerObject was detected 
 Event = threading.Event()
@@ -143,49 +145,62 @@
 
         thread = threading.Thread(target=self.seriaListener, daemon = True)
         thread.start()
         if not Event.wait(.2):
             printe('Listener did not start')
             sys.exit(1)
 
-        #if pargs.stop:
-        reply = self.execute_command('set fec stop')
-        time.sleep(.5)
+        if pargs.stop:
+            printi(f'Disable ADC trigger')
+            write_serdev('set adc_trig disable')
+            time.sleep(.5)
 
         #TODO check if it stopped, exit if not
         # parameters, retrieved from device
         pars = self.adopt_PVs()
         if pars is None:
             printe('Could not extract parameters from device.')
             sys.exit(1)
         self._pars.update(pars)
 
         # derived parameters
-        self._pars.update({'adcs':   LDO('R','Multi-dimensional array of all ADC channels',
-          [], ptype='numpy.ndarray')})
-        print(f"nadcs: {self._pars['nADC'].value[0]}")
+        if PV_ADCS:
+            self._pars.update({'adcs':   LDO('R','Multi-dimensional array of all ADC channels',
+            [], ptype='numpy.ndarray')})
+        nADCs = self._pars['nADC'].value[0]
+        print(f"nadcs: {nADCs}")
+        adcmask = '1'*nADCs if pargs.adcmask=='*' else pargs.adcmask[:nADCs]
         for i in range(self._pars['nADC'].value[0]):
+            try:
+                if adcmask[i] == '0':
+                    continue
+            except:
+                continue
             print(f'creating ADC{i+1}')
             self._pars.update({f'adc{i+1}':LDO('R','ADC channel',
-              [], ptype='numpy.ndarray')})
+              #[], ptype='numpy.ndarray')})
+              [0.], ptype='numpy.ndarray')})
 
-        self._pars.update({'xscale': LDO('R','Scale, converting samples to time',
-            1., units='ms', ptype='numpy.ndarray')})
-        nADCs = self._pars['nADC'].value[0]
+        #self._pars.update({'xscale': LDO('R','Scale, converting samples to time',
+        #    1., units='ms', ptype='numpy.ndarray')})
+        self._pars.update({'xaxis': LDO('R','X axis of ADC arrays',
+            [0.], units='ms')})
         self._pars.update({'peak2peak': LDO('R','Peak-to-Peak amplitudes of ADC channels',
           [0.]*nADCs, units='V')}),
         self._pars.update({'mean': LDO('R','Average of all samples of ADC channels',
           [0.]*nADCs, units='V')}),
         self._pars.update({'gain': LDO('R','Conversion of ADC counts to Volts, if 0 then it will be returned in ADC counts',
-          [1., 1., 2./2450, 2./2450, 2./690, 2./700], units='V')})
+          #[1., 1., 2./2450, 2./2450, 2./690, 2./700],units='V')})
+          [3.3/4096]*nADCs, units='V')})
         self._pars.update({'offset': LDO('R','ADC offset',
-          [0, 0, 168, 168, 1792, 1785])})
+          #[0, 0, 168, 168, 1792, 1785])})
+          [0.]*nADCs)})
         super().__init__(name, self._pars)
 
-        self.update_xscale()
+        self.update_xaxis()
         self.initialized = True
         printi('Initialization finished')
         time.sleep(.1)
 
     #``````````````Overridables````````````````````````````````````````````````        
     def start(self):
         printi('>start')
@@ -233,41 +248,49 @@
                 printe(f'data[{len(payload)}] shape is wrong, channels: {hdrNCh}, width: {samplesPerChannel}')
                 resync()
                 return
             if not self.initialized:
                 printv('ADC data ignored since parameters are not created yet')
                 return
             printv(f'ADC array[{arr.shape}] accepted')
-            pv_ADCs = self.PV['adcs']
-            # update multidimensional parameter adcs
-            pv_ADCs.set_valueAndTimestamp(arr, timestamp)
+            if PV_ADCS:
+                # update multidimensional parameter adcs
+                pv_ADCs = self.PV['adcs']
+                pv_ADCs.set_valueAndTimestamp(arr, timestamp)
 
             # update waveforms, peak2peaks and means of individual ADC channels
             peak2peak = []
             mean = []
-            for i,a in enumerate(arr):
-                printvv(f'setting adc{i+1} to {a}')
+            for i, rawArray in enumerate(arr):
+                self.adcLen = len(rawArray)
+                #printvv(f'setting adc{i+1} to {rawArray}')
+                gain = self.PV['gain'].value[i]
+                offset = self.PV['offset'].value[i]                
+                scaledArray = np.array(rawArray)*gain + offset
                 try:
-                    self._pars['adc'+str(i+1)].set_valueAndTimestamp(a, timestamp)
+                    self._pars['adc'+str(i+1)].set_valueAndTimestamp(scaledArray, timestamp)
                 except KeyError:
                     #printw(f'ADC {i+1} not required')
                     continue
-                gain = self.PV['gain'].value[i]
-                offset = self.PV['offset'].value[i]
-                b = np.convolve(a, SmoothingKernel, 'valid')
-                peak2peak.append(round((b.max() - b.min())*gain,5))
-                mean.append(round((a.mean()-offset)*gain,5))
+                smoothedArray = np.convolve(scaledArray, SmoothingKernel, 'valid')
+                peak2peak.append(round((smoothedArray.max() - smoothedArray.min())*gain,5))
+                #mean.append(round((a.mean()-offset)*gain,5))
+                mean.append(round(scaledArray.mean(),5))
             self._pars['peak2peak'].set_valueAndTimestamp(peak2peak, timestamp)
             self._pars['mean'].set_valueAndTimestamp(mean, timestamp)
 
         elif hdrID == b'<':# JSON formatted reply
             #printv('updating pv_reply')
             self._pars['reply'].set_valueAndTimestamp([payload.decode()],
               timestamp)
             if not payload.startswith(b'{'):
+                if payload == b'OK':
+                    # normal reply to set()
+                    SerObjectEvent.set()
+                    return
                 printi(f'msg: {payload}')
                 if payload.startswith(b'ERR'):
                     self._pv_reply = payload.decode()
                     SerObjectEvent.set()
                 return
             try:
                 self._pv_reply = json.loads(payload)
@@ -463,64 +486,72 @@
             printi(f'creating {pv}={v}, {features}, units:{units}, opLimits:{opLimits}, lv:{legalValues}')
             pars.update({pv:LDO(features, pvinfo['desc'], v, units,
               opLimits, legalValues, ptype=ptype,
               setter=partial(self.set_pv, pv),
               getter=partial(self.get_pv, pv))})
         return pars
 
-    def update_xscale(self):
-        self.PV['xscale'].set_valueAndTimestamp(\
-          [1000./self.PV['adc_srate'].value[0]], time.time())
-        #printi(f'xcale: {pv_xscale.value[0]}')
+    def update_xaxis(self):
+        try:
+            adcLen = self.adcLen
+        except:
+            printw('Could not set xaxis: ADCs not yet aquired')
+            return
+        step = 1000./self.PV['adc_srate'].value[0]
+        self.PV['xaxis'].set_valueAndTimestamp(\
+          np.arange(adcLen)*step, time.time())
+        #printi(f'xcale: {pv_xaxis.value[0]}')
 
     def interpret_reply(self, reply):
         if reply is None:
             return
         printv(f'interpret: {reply}')
         for pvname, value in reply.items():
             pv = self._pars[pvname]
             ts = time.time()
             try:
                 pv.value[0] = reply[pvname]
                 pv.timestamp = ts
             except Exception as e:
                 printe(f'Unexpected reply: {e}')
             if pvname == 'adc_srate':
-                self.update_xscale()
+                self.update_xaxis()
 
     def set_pv(self, pvname):
         pv = self.PV[pvname]
         cmd = f'set {pvname} {pv.value[0]}'
-        printi(f'>set {cmd}')
+        printv(f'>set {cmd}')
         self.execute_command(cmd)
 
     def get_pv(self, pvname):
         cmd = f'get {pvname}'
-        printi(f'>get {cmd}')#, prev: {pv.value}')
+        printv(f'>get {cmd}')#, prev: {pv.value}')
         self.execute_command(cmd)
 #,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
 #``````````````````Main function``````````````````````````````````````````````
 if __name__ == "__main__":
     # parse arguments
     import argparse
     parser = argparse.ArgumentParser(description=__doc__
         ,formatter_class=argparse.ArgumentDefaultsHelpFormatter
         ,epilog=f'LiteMCUFEC version {__version__}, liteserver {liteserver.__version__}')
+    parser.add_argument('-a', '--adcmask', default='*',
+      help='Mask of enabled ADCs, e.g. 01010101 enables ADC 2,4,6,8')
     parser.add_argument('-b', '--baudrate', type=int, default=7372800,# 10000000,
       help='Baud rate for serial communications')
     parser.add_argument('-d', '--debug',  action='store_true',
       help='Debug session using pdb')
     defaultIP = liteserver.ip_address('')
     parser.add_argument('-i','--interface', default = defaultIP, help=\
     'Network interface. Default is the interface, which connected to internet.')
     n = 1100# to fit LiteMCUFEC volume into one chunk
     parser.add_argument('-p','--port', type=int, default=9700, help=\
     'Serving IP port.')
     parser.add_argument('-s','--stop', action='store_true', help=\
-    'Stop device')
+    'Disable ADC_trigger')
     parser.add_argument('-v','--verbose', nargs='*', help='Show more log messages.')
     parser.add_argument('tty', nargs='?', default='/dev/ttyACM0', help=\
       'Device for serial communication')
     pargs = parser.parse_args()
     printi(f"Receive data from {pargs.tty}.")
     if pargs.debug:
         breakpoint()
```

### Comparing `pvplot-0.6.7/ln/liteserver/device/litePeakSimulator.py` & `pvplot-0.6.9/ln/liteserver/device/litePeakSimulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 """liteserver, simulating peaks"""
-__version__ = '3.2.1 2023-09-21'# update timestamps for pv['x'] 
+__version__ = '3.2.1 2024-02-27'# xStatic added
 
 import sys, time, threading
 timer = time.perf_counter
 import numpy as np
 
 from .. import liteserver
 LDO = liteserver.LDO
 Device = liteserver.Device
+xScale = 0.1
 
 #````````````````````````````Helper functions`````````````````````````````````
 def gaussian(x, sigma):
     """Function, representing gaussian peak shape"""
     try: r = np.exp(-0.5*(x/sigma)**2) 
     except: r = np.zeros(len(x))
     return r
@@ -39,29 +40,32 @@
     v = func_sum_of_peaks(x, *par)
     return v + noise
 #````````````````````````````Lite Data Objects````````````````````````````````
 class Dev(Device):
     """ Derived from liteserver.Device.
     Note: All class members, which are not process variables should 
     be prefixed with _"""
+    xVals = None
     def __init__(self, name, no_float32=False):
+        Dev.xVals = np.arange(pargs.nPoints)
         pars = {
           'frequency':  LDO('RWE','Update frequency of all counters',
             pargs.frequency, units='Hz', opLimits=(0.001,1001.)),
           'nPoints':    LDO('RWE','Number of points in the waveform'
           ,pargs.nPoints, setter=self.set_peaks),
           'background': LDO('RWE','3 Coefficients for quadratic background'
           , pargs.background, setter=self.set_peaks),
           'noise':      LDO('RWE','Nose level'
           ,pargs.noise, setter=self.set_peaks),
           'peakPars':   LDO('RWE','Peak parameters'
           ,pargs.peaks, setter=self.set_peaks),
           'swing':      LDO('RWE','Horizontal peak oscillations',
                       				pargs.swing, units='%'),
-          'x':          LDO('R','X-values',np.arange(pargs.nPoints)),
+          'xStatic':    LDO('R','Static X-values',Dev.xVals*xScale),
+          'x':          LDO('R','Dynamic X-values',Dev.xVals*xScale),
           'y':          LDO('R','Y-Values',np.zeros(pargs.nPoints)),
           'yMin':       LDO('R','',0.),
           'yMax':       LDO('R','',0.),
           'rps':        LDO('R','Cycles per second',0.,units='Hz'),
           'cycle':      LDO('R','Cycle number',0),
         }
         super().__init__(name, pars)
@@ -70,24 +74,25 @@
 
         thread = threading.Thread(target=self._state_machine)
         thread.daemon = False
         thread.start()
 
     def update_peaks(self):
         pars = self.PV['background'].value + self.PV['peakPars'].value
-        return peaks(self.PV['x'].value, *pars, noiseLevel=self.PV['noise'].value[0])
+        return peaks(Dev.xVals, *pars, noiseLevel=self.PV['noise'].value[0])
 
     def set_peaks(self):
         n = self.PV['nPoints'].value[0]
+        Dev.xVals = np.arange(n)
         pp = generate_pars(n)
         self.PV['background'].value = pp[:3]
         self.PV['peakPars'].value = pp[3:]
         pars={i.name:(type(i.value[0]),i.value) for i in (self.PV['nPoints']
         ,self.PV['background'], self.PV['peakPars'], self.PV['noise'])}
-        self.PV['x'].value = np.arange(n)
+        self.PV['x'].value = Dev.xVals*xScale
         self.PV['y'].value = self.update_peaks()
         #print(f'y:{self.PV['y'].value}')
 
     def swing_peaks(self):
         n = self.PV['nPoints'].value[0]
         deviation = np.sin(self.PV['cycle'].value/10*np.pi)*self.PV['swing'].value[0]/100*n
         for i in range(0,len(self.PV['peakPars'].value),3):
@@ -116,14 +121,15 @@
                 self.PV['rps'].value = (self.PV['cycle'].value - prevCycle)/dt
                 self.PV['rps'].timestamp = timestamp
                 prevCycle = self.PV['cycle'].value
             self.PV['cycle'].value += 1
 
             if self.PV['swing'].value[0] != 0.:
                 self.swing_peaks()
+            self.PV['x'].value += 0.001*(self.PV['cycle'].value)
             self.PV['y'].value = self.update_peaks().round(3)
             self.PV['yMin'].value = float(self.PV['y'].value.min())
             self.PV['yMax'].value = float(self.PV['y'].value.max())
             # invalidate timestamps for changing variables, otherwise the
             # publish() will ignore them
             for i in [self.PV['cycle'], self.PV['x'], self.PV['y'],
               self.PV['yMin'], self.PV['yMax']]:
@@ -180,10 +186,10 @@
     liteserver.Server.Dbg = 0 if pargs.verbose is None else len(pargs.verbose)+1
     devices = [Dev('dev1', no_float32=pargs.doubles)]
 
     server = liteserver.Server(devices, interface=pargs.interface,
         port=pargs.port)
 
     print('`'*79)
-    print(f"To monitor, use: pvplot -s.01 -a'L:{server.host};{pargs.port}:dev1' 'x,y'")
+    print(f"To monitor, use: python -m pvplot -s.01 -a'L:{server.host};{pargs.port}:dev1:' 'x,y'")
     print(','*79)
     server.loop()
```

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteScaler.py` & `pvplot-0.6.9/ln/liteserver/device/liteScaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,12 +214,11 @@
       Scaler('dev'+str(i+1), bigImage=pargs.bigImage)\
       for i in range(pargs.scalers)]
 
     server = liteserver.Server(devices, interface=pargs.interface,
         port=pargs.port)
 
     print('`'*79)
-    print((f"To monitor, use: pvplot -a'L:{server.host};{pargs.port}:dev1' "\
-"'counters'"))
+    print((f"To monitor, use: python3 -m pvplot -a'L:{server.host};{pargs.port}:dev1:' 'publishingSpeed udpSpeed'"))
     print(','*79)
 
     server.loop()
```

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteUSBCam.py` & `pvplot-0.6.9/ln/liteserver/device/liteUSBCam.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteUvcCam.py` & `pvplot-0.6.9/ln/liteserver/device/liteUvcCam.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteVGM.py` & `pvplot-0.6.9/ln/liteserver/device/liteVGM.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/liteWLM.py` & `pvplot-0.6.9/ln/liteserver/device/liteWLM.py`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/ln/liteserver/device/senstation.py` & `pvplot-0.6.9/ln/liteserver/device/senstation.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 Supported:
   - Two hardware PWMs 1Hz-300 MHz, GPIO 12,13.
   - Temperature sensors DS18B20 (0.5'C resolution), GPIO 4.
   - Digital IOs (GPIO 19,20).
   - Pulse Counter (GPIO 26).
   - Spark detector (GPIO 26).
   - Buzzer (GPIO 13).
-  - RGB LED indicator (GPIO 16,6,5).
+  - RGB LED indicator (GPIO 22,27,17).
   - I2C devices: ADS1x15, MMC5983MA, HMC5883, QMC5983.
   - I2C mutiplexers TCA9548, PCA9546.
   - OmegaBus serial sensors
 """
-__version__ = '3.2.1 2023-09-04'# An LDO added: 'period'.
+__version__ = '3.2.5 2024-05-02'# DHT disabled by default
 
 #TODO: take care of microsecond ticks in callback
 
 print(f'senstation {__version__}')
 
 import sys, time, threading, glob, struct
 timer = time.perf_counter
@@ -31,22 +31,23 @@
 GPIO = {
     'Temp0': 4,
     'PWM0': 12,# 'PWM1':13,
     'Buzz': 13,
     'DI0':  19,
     'DI1':  20,
     'Counter0': 26,
-    'RGB':  [16,6,5],
+    'RGB':  [22,27,17],
     'DO3':  25,
     'DO4':  24,
-    'DHT':  21,
+    'DHT':  23,
 }
 EventGPIO = {'Counter0':0.} # event-generated GPIOs, store the time when it was last published
 #CallbackMinimalPublishPeiod = 0.01
 MaxPWMRange = 1000000 # for hardware PWM0 and PWM1
+Seldom_update_period = 60.# update period for slow-changing parameters like temperature and humidity
 
 #`````````````````````````````Helper methods```````````````````````````````````
 from . import helpers
 def printi(msg):  helpers.printi(msg)
 def printe(msg):
     helpers.printe(msg)
     if MgrInstance is not None: MgrInstance.set_status('ERROR: '+msg)
@@ -89,15 +90,14 @@
     print(f'OneWire_folder: {OneWire_folder}')
     if OneWire_folder is None:
         print('WARNING: Thermometer sensor is not connected')
         def measure_temperature(): return None
     else:
         device_file = OneWire_folder + '/w1_slave'
         print(f'Thermometer driver is: {device_file}')
-         
         def read_temperature():
             f = open(device_file, 'r')
             lines = f.readlines()
             f.close()
             return lines
         #read_temperature()
 
@@ -138,28 +138,27 @@
 
 
 #````````````````````````````liteserver methods````````````````````````````````
 class SensStation(Device):
     """ Derived from liteserver.Device.
     Note: All class members, which are not process variables should 
     be prefixed with _"""
+
     def __init__(self,name):
         ldos = {}
 
         # Add I2C devices
         if pargs.muxAddr:
             from liteserver.device import i2c
             self.I2C = i2c.I2C
             self.I2C.verbosity = pargs.verbose
             i2c.init(pargs.muxAddr, pargs.muxMask)
             ldos.update(self.I2C.LDOMap)
 
         ldos.update({
-          'Calibration': LDO('RWE', 'Calibrate attached sensors.', ['Off'],
-            legalValues=['On','Off','Periodic','SelfTest'], setter=self.set_calib),
           'boardTemp':  LDO('R','Temperature of the Raspberry Pi', 0., units='C'),
           'cycle':      LDO('R', 'Cycle number', 0),
           'cyclePeriod':LDO('RWE', 'Cycle period', pargs.update, units='s'),
           'period':     LDO('R', 'Measured period', pargs.update, units='s'),
           'PWM0_Freq':  LDO('RWE', f'Frequency of PWM at GPIO {GPIO["PWM0"]}',
             10, units='Hz', setter=partial(self.set_PWM_frequency, 'PWM0'),
             opLimits=[0,125000000]),
@@ -182,21 +181,39 @@
             '0', legalValues=['0','1'], setter=partial(self.set_DO, 'DO4')),
           'Buzz':       LDO('RWE', f'Buzzer at GPIO {GPIO["Buzz"]}, activates when the Counter0 changes',
             '0', legalValues=['0','1'], setter=self.set_Buzz),
           'BuzzDuration': LDO('RWE', f'Buzz duration', 5., units='s'),
         })
         if pargs.oneWire:
             ldos['Temp0'] = LDO('R','Temperature of the DS18B20 sensor', 0.,
-                units='C'),
+                units='C')
         if 'OmegaBus' in pargs.serial:
             ldos['OmegaBus'] = LDO('R','OmegaBus reading', 0., units='V')
-        
+
+        if pargs.dht is not None:
+            from pigpio_dht import DHT11, DHT22
+            try:
+                dhtModel,dhtPin = pargs.dht.split('.')
+                pin = int(dhtPin)
+            except:
+                printw('Wrong option value for --dht')
+            try:
+                pargs.dht = DHT11(pin) if dhtModel == '11' else\
+                DHT22(pin)
+            except Exception as e:
+                printw(f'Could not initialize a DHT sensor: {e}')
+            if pargs.dht is not None:
+                ldos['Temperature'] = LDO('R',
+                'Temperature, provided by the DHT sensor', 0., units='C')
+                ldos['Humidity'] = LDO('R',
+                'Humidity, provided by the DHT sensor', 0.)
+
         super().__init__(name,ldos)
 
-        # connect callback function to a GPIO pulse edge 
+        # connect callback function to a GPIO pulse edge
         for eventParName in EventGPIO:
             PiGPIO.callback(GPIO[eventParName], pigpio.RISING_EDGE, callback)
         self.start()
 
     #``````````````Overridables```````````````````````````````````````````````
     def start(self):
         printi('Senstation started')
@@ -230,23 +247,14 @@
 
     def gpiov(self, parName):
         v = self.PV[parName].value[0]
         key = parName.split('_')[0]
         gpio = GPIO[key]
         printv(f'gpiov {gpio,v}')
         return gpio,v
-        
-    def set_calib(self):
-        v = self.PV['Calibration'].value[0]
-        for i2cDev in self.I2C.DeviceMap.values():
-            try:
-                i2cDev.calibration(v)
-            except Exception as e:
-                printw(f'Exception in calib: {i2cDev.name}: {e}')
-                continue
 
     def set_PWM_frequency(self, pwm):
         parName = pwm + '_Freq'
         gpio, v = self.gpiov(parName)
         #r = PiGPIO.hardware_PWM(gpio, int(v))
         dutyCycle = int(MaxPWMRange*self.PV[pwm+'_Duty'].value[0])
         r = PiGPIO.hardware_PWM(gpio, int(v), dutyCycle)
@@ -280,15 +288,15 @@
             PiGPIO.write(GPIO['RGB'][i], v&1)
             v = v >> 1
 
     def _threadRun(self):
         printi('threadRun started')
         timestamp = time.time()
         prevcurtime = timestamp
-        periodic_update = timestamp
+        last_seldom_update = timestamp
         self.prevCPUTempTime = 0.
         while not Device.EventExit.is_set():
             if self.PV['run'].value[0][:4] == 'Stop':
                 break
             curtime = time.time()
             period = round(curtime - prevcurtime,6)
             prevcurtime = curtime
@@ -308,46 +316,53 @@
             if self.PV['RGBControl'].value[0] == 'RGBCycle':
                 self.PV['RGB'].set_valueAndTimestamp(\
                     [self.PV['cycle'].value[0] & 0x7], timestamp)
                 self.set_RGB()
             self.publish()# publish all fresh parameters
 
             # do a less frequent tasks in a thread
-            dt = timestamp - periodic_update
-            if dt > 10.:
-                periodic_update = timestamp
+            dt = timestamp - last_seldom_update
+            if dt > Seldom_update_period:
+                last_seldom_update = timestamp
                 thread = threading.Thread(target=self.seldomThread)
                 thread.start()
         printi('threadRun stopped')
         self.stop()
 
     def seldomThread(self):
         #print(f'>seldomThread: {timestamp}')
-        #ts = timer()
-        ctime = time.time()
         try:
-            if ctime - self.prevCPUTempTime > 60.:
-                self.prevCPUTempTime = ctime
-                with open(r"/sys/class/thermal/thermal_zone0/temp") as f:
-                    r = f.readline()
-                    temperature = float(r.rstrip()) / 1000.
-                    self.PV['boardTemp'].set_valueAndTimestamp([temperature])
+            with open(r"/sys/class/thermal/thermal_zone0/temp") as f:
+                r = f.readline()
+                temperature = float(r.rstrip()) / 1000.
+                self.PV['boardTemp'].set_valueAndTimestamp([temperature])
         except Exception as e:
             printw(f'Could not read CPU temperature `{r}`: {e}')
         temp = measure_temperature()# 0.9s spent here
         #print(f'Temp0 time: {round(timer()-ts,6)}')
         if temp is not None:
             self.PV['Temp0'].set_valueAndTimestamp([temp])
         if 'OmegaBus' in pargs.serial:
             OmegaBus.write(b'$1RD\r\n')
             r = OmegaBus.read(100)
             #print(f'OmegaBus read: {r}')
             if len(r) != 0:
                 self.PV['OmegaBus'].set_valueAndTimestamp([float(r.decode()[2:])/1000.])
         #print(f'<seldomThread time: {round(timer()-ts,6)}')
+        if pargs.dht is not None:
+            try:
+                result = pargs.dht.read()
+                #print(f'dht: {result}')
+                if result['valid']:
+                    self.PV['Temperature'].set_valueAndTimestamp([result['temp_c']])
+                    self.PV['Humidity'].set_valueAndTimestamp([result['humidity']])
+                else:
+                    printw('DHT invalid')
+            except Exception as e:
+                printw(f'in dht.read: {e}')
 
     def set_status(self, msg):
         self.PV['status'].set_valueAndTimestamp(msg)
 
 def callback(gpio, level, tick):
     #print(f'callback: {gpio, level, tick}')
     timestamp = time.time()
@@ -372,39 +387,40 @@
 #``````````````````Main````````````````````````````````````````````````````````
 if __name__ == "__main__":
     # parse arguments
     import argparse
     parser = argparse.ArgumentParser(description=__doc__
     ,formatter_class=argparse.ArgumentDefaultsHelpFormatter
     ,epilog=f'senstation: {__version__}')
+    parser.add_argument('-H','--dht', nargs = '?', help=\
+    ('Type and pin of the connected DHT sensor (humidity and temperature sensor), '
+    ' for example: "-H11.23", if just "-H" then no DHT will be supported.'))
     parser.add_argument('-i','--interface', default = '', help=\
     'Network interface. Default is the interface, which connected to internet')
     n = 12000# to fit liteScaler volume into one chunk
     #parser.add_argument('-I','--I2C', help=\
     #('Comma separated list of I2C device_address, e.g. MMC5983MA_48,'
     #'ADS1115_72, ADS1015_72, HMC5883_30, QMC5883_13')),
     parser.add_argument('-m','--muxMask', default='11111111', help=\
     ('Mask of enabled channels of I2C multiplexer (if it is present).'
     'If 0 then all channels will be enabled but not processed'))
     parser.add_argument('-M','--muxAddr', type=int, default=0x77, help=\
-    'I2C address of the multiplexer') 
+    'I2C address of the multiplexer')
     parser.add_argument('-p','--port', type=int, default=9700, help=\
     'Serving port, default: 9700')
     parser.add_argument('-s','--serial', default = '', help=\
     'Comma separated list of serial devices to support, e.g.:OmegaBus')
     parser.add_argument('-1','--oneWire', action='store_true', help=\
     'Support OneWire device, DS18B20')
     parser.add_argument('-u','--update', type=float, default=1.0, help=\
     'Updating period')
-    parser.add_argument('-v','--verbose', nargs='*', help=\
-        'Show more log messages, (-vv: show even more).')
+    parser.add_argument('-v', '--verbose', action='count', default=0, help=\
+      'Show more log messages (-vv: show even more).')
     pargs = parser.parse_args()
-    pargs.verbose = 0 if pargs.verbose is None else len(pargs.verbose)+1
     pargs.muxMask = int(pargs.muxMask,2)
-
     liteserver.Server.Dbg = pargs.verbose
     init_gpio()
 
     if pargs.serial != '':
         import serial
         init_serial()
```

### Comparing `pvplot-0.6.7/pvplot/__main__.py` & `pvplot-0.6.9/pvplot/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ,epilog=(f'pvplot: {pvplot.__version__}'))
     parser.add_argument('-a', '--prefix', default='', help=\
       "Prefix, which will be added to all data objects, e.g: 'L:localhost:dev1:'")
     #TODO:parser.add_argument('-H', '--histogram', help=\
     #  'Plot the space-separated parameters as histograms')
     parser.add_argument('-s', '--sleepTime', type=float, default=0.1,
       help='sleep time between data delivery [s]')
-    parser.add_argument('-v', '--verbose', nargs='*', help=\
+    parser.add_argument('-v', '--verbose', action='count', default=0, help=\
       'Show more log messages (-vv: show even more).')
     parser.add_argument('-x', '--xscale', help=\
      'Parameter, which provides dynamic scale for X-axis')
     parser.add_argument('-X', '--xrange', help=\
      'Fixed range of X axis, e.g: -x10:20')
     parser.add_argument('-y', '--yscale', help=\
      'Parameter, which provides dynamic scale for Y-axis')
```

### Comparing `pvplot-0.6.7/pvplot/pvplot.py` & `pvplot-0.6.9/pvplot/pvpopld.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,45 +384,46 @@
         if ts:
             if ts == self.lastTimeUpdated:
                 #print(f'curve {self.name} did not change {round(ts,3)}')
                 if time2plot:
                     self.plot(ts)
                 return
         self.lastTimeUpdated = ts
-        printv(f'update_plot: {curvePars}')# data:{yd}')
+        #printv(f'update_plot: {curvePars}, data:{yd}')
         #print(f'update {self.name, round(ts,3), round(self.lastTimePlotted,3)}')
         try:    
             l = len(yd)
             if l == 1: yd = yd[0]
         except: 
             l = 1
 
         # Evaluate X and Y arrays
         if l > 1:
-            # the plot is array plot
+            #printv('Array plot')
             self.data[Y] = np.array(yd)
             if len(curvePars) > 1:
                 # use last item as horizontal axis
                 self.data[X],*_ = get_pv(curvePars[-1][0])
             else:
                 # scaled sample number
                 self.data[X] = np.arange(len(yd))*PVPlot.scaleUnits[X][Scale]
             self.dataPtr = len(yd)
             self.plot(ts)
             return
         else:
             # the plot is scrolling or correlation plot
             ptr = self.dataPtr
             if ptr >= PVPlot.maxPoints:
-                # do not extent the data buffer, roll it over insted
+                # do not extent the data buffer, roll it over instead
                 self.data[X] = np.roll(self.data[X],-1)
                 self.data[Y] = np.roll(self.data[Y],-1)
                 ptr -= 1
             self.data[Y][ptr] = yd
-            if len(curvePars) > 1: 
+            if len(curvePars) > 1:
+                #print('Correlation Plot') 
                 printv(f'correlation plot: {curvePars[1][0]}')
                 try:
                     v,*_ = get_pv(curvePars[1][0])
                     try:    v = v[0]
                     except: pass 
                     self.data[X][ptr] = v
                 except Exception as e:
```

### Comparing `pvplot-0.6.7/LICENSE` & `pvplot-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/README.md` & `pvplot-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pvplot-0.6.7/pyproject.toml` & `pvplot-0.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pvplot"
-version = "0.6.7"
+version = "0.6.9"
 authors = [
   { name="Andrei Sukhanov", email="cyxandr@gmail.com" },
 ]
 description = "Plotting tool for EPICS PVs, ADO and LITE parameters"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pvplot-0.6.7/PKG-INFO` & `pvplot-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pvplot
-Version: 0.6.7
+Version: 0.6.9
 Summary: Plotting tool for EPICS PVs, ADO and LITE parameters
 Project-URL: Homepage, https://github.com/ASukhanov/pvplot
 Project-URL: Bug Tracker, https://github.com/ASukhanov/pvplot/issues
 Author-email: Andrei Sukhanov <cyxandr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

