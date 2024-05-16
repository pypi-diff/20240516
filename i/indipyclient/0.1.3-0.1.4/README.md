# Comparing `tmp/indipyclient-0.1.3.tar.gz` & `tmp/indipyclient-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.1.3.tar` & `indipyclient-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.3/LICENSE
--rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.3/README.md
--rw-r--r--   0        0        0      416 2024-05-14 10:23:25.000000 indipyclient-0.1.3/indipyclient/__init__.py
--rw-r--r--   0        0        0     3520 2024-05-14 07:13:24.000000 indipyclient-0.1.3/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.3/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    22122 2024-05-14 07:04:08.000000 indipyclient-0.1.3/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.3/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.3/indipyclient/console/windows.py
--rw-r--r--   0        0        0    26738 2024-05-03 13:06:57.000000 indipyclient-0.1.3/indipyclient/events.py
--rw-r--r--   0        0        0    33660 2024-05-13 11:23:49.000000 indipyclient-0.1.3/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16279 2024-05-03 09:59:43.000000 indipyclient-0.1.3/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.3/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-05-14 10:23:12.000000 indipyclient-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.4/README.md
+-rw-r--r--   0        0        0      416 2024-05-16 10:35:07.000000 indipyclient-0.1.4/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3663 2024-05-16 10:28:14.000000 indipyclient-0.1.4/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.4/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    21226 2024-05-15 17:27:54.000000 indipyclient-0.1.4/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.4/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.4/indipyclient/console/windows.py
+-rw-r--r--   0        0        0    26848 2024-05-15 10:33:05.000000 indipyclient-0.1.4/indipyclient/events.py
+-rw-r--r--   0        0        0    32735 2024-05-15 11:40:24.000000 indipyclient-0.1.4/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16339 2024-05-15 11:03:42.000000 indipyclient-0.1.4/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.4/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-05-16 10:34:35.000000 indipyclient-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.4/PKG-INFO
```

### Comparing `indipyclient-0.1.3/LICENSE` & `indipyclient-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.3/README.md` & `indipyclient-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.3/indipyclient/__main__.py` & `indipyclient-0.1.4/indipyclient/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,28 +66,34 @@
     # On receiving an event, the client appends it into eventque
     client = ConsoleClient(indihost=args.host, indiport=args.port, eventque=eventque)
 
     # Monitors eventque and acts on the events, creates the console screens
     # and calls the send vector methods of client to transmit data
     control = ConsoleControl(client, blobfolder=blobfolder)
 
+    loglevel = 0
+
     if args.loglevel and args.logfile:
         try:
             loglevel = int(args.loglevel)
             if loglevel not in (1,2,3,4):
                 print("Error: If given, the loglevel should be 1, 2, 3 or 4")
                 return 1
             level = control.setlogging(loglevel, args.logfile)
             if level != loglevel:
                 print("Error: Failed to set logging")
                 return 1
-        except:
+        except Exception:
             print("Error: If given, the loglevel should be 1, 2, 3 or 4")
             return 1
 
+    if loglevel < 2:
+        # If logging debug not enabled, reduce traceback info
+        sys.tracebacklimit = 0
+
     try:
         asyncio.run(runclient(client, control))
     finally:
         # clear curses setup
         control.console_reset()
 
     return 0
```

### Comparing `indipyclient-0.1.3/indipyclient/console/consoleclient.py` & `indipyclient-0.1.4/indipyclient/console/consoleclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                 logger.setLevel(logging.DEBUG)
                 self.client.debug_verbosity(1)
             elif level == 1:
                 logger.setLevel(logging.INFO)
 
             fh = logging.FileHandler(logfile)
             logger.addHandler(fh)
-        except:
+        except Exception:
             return
         return level
 
 
     def color(self, state):
         "Returns curses.color_pair given a state"
         if not curses.has_colors():
@@ -160,17 +160,14 @@
         # so either shutdown has been requested or the ipyclient has stopped for some reason
         if not self.client.stopped:
             # client is still running, shut it down
             self.client.report("Shutting down client - please wait")
             self.client.shutdown()
         # Now stop console co-routines
         self.stop = True
-        while (not self.updatescreenstopped) and (not self.getinputstopped):
-            await asyncio.sleep(0)
-
 
     def console_reset(self):
         "Resets console, called in finally clause at program shutdown"
         curses.nocbreak()
         self.stdscr.keypad(False)
         curses.curs_set(1)
         curses.echo()
@@ -273,20 +270,17 @@
                 # so its not a delete property
                 if isinstance(self.screen, windows.ChooseVectorScreen):
                     self.screen.update(event)
                     continue
                 if isinstance(self.screen, windows.VectorScreen) and (self.screen.vectorname == event.vectorname):
                     # The event refers to this vector
                     self.screen.update(event)
-        except asyncio.CancelledError:
-            self.shutdown()
-            raise
         except Exception:
             logger.exception("Exception report from ConsoleControl.updatescreen")
-            self.shutdown()
+            raise
         finally:
             self.updatescreenstopped = True
 
 
     async def getinput(self):
         try:
             while not self.stop:
@@ -443,20 +437,17 @@
                         self.screen.show()
                         continue
                     if result == "Vectors":
                         self.screen = windows.ChooseVectorScreen(self.stdscr, self, self.screen.devicename, group=self.screen.vector.group)
                         self.screen.show()
                         continue
 
-        except asyncio.CancelledError:
-            self.shutdown()
-            raise
         except Exception:
             logger.exception("Exception report from ConsoleControl.getinput")
-            self.shutdown()
+            raise
         finally:
             self.getinputstopped = True
 
 
     def send_enableBLOB(self):
         "Sends Also to enable blobs for all devices"
         if not self.blobenabled:
@@ -474,23 +465,8 @@
             if device.enable:
                 self.client.send_enableBLOB('Never', devicename)
 
 
     async def asyncrun(self):
         """Gathers tasks to be run simultaneously"""
         self.stop = False
-        t1 = asyncio.create_task(self.updatescreen())
-        t2 = asyncio.create_task(self.getinput())
-        t3 = asyncio.create_task(self._checkshutdown())
-        try:
-            await asyncio.gather(t1, t2, t3)
-        except Exception:
-            # one task has raised an exception, shutdown and wait for the
-            # remaining task to shutdown
-            logger.exception("Exception report from  ConsoleControl.asyncrun coroutine")
-            self.stop = True
-            while not t1.done():
-                await asyncio.sleep(0)
-            while not t2.done():
-                await asyncio.sleep(0)
-            while not t3.done():
-                await asyncio.sleep(0)
+        await asyncio.gather(self.updatescreen(), self.getinput(), self._checkshutdown())
```

### Comparing `indipyclient-0.1.3/indipyclient/console/widgets.py` & `indipyclient-0.1.4/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.3/indipyclient/console/windows.py` & `indipyclient-0.1.4/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.3/indipyclient/events.py` & `indipyclient-0.1.4/indipyclient/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     remainder = remainder[:6]
                 remainder = int(remainder)
                 timestamp = datetime.fromisoformat(timestamp_string)
                 timestamp = timestamp.replace(microsecond=remainder, tzinfo=timezone.utc)
             else:
                 timestamp = datetime.fromisoformat(timestamp_string)
                 timestamp = timestamp.replace(tzinfo=timezone.utc)
-        except:
+        except Exception:
             timestamp = None
     else:
         timestamp = datetime.now(tz=timezone.utc)
     return timestamp
 
 
 class VectorTimeOut:
@@ -160,15 +160,15 @@
             raise ParseException("defSwitchVector has invalid rule")
         try:
             timeout = root.get("timeout")
             if not timeout:
                 self.timeout = 0.0
             else:
                 self.timeout = float(timeout)
-        except:
+        except Exception:
             self.timeout = 0.0
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defSwitch":
                 membername = member.get("name")
@@ -221,15 +221,15 @@
             raise ParseException
         try:
             timeout = root.get("timeout")
             if not timeout:
                 self.timeout = 0.0
             else:
                 self.timeout = float(timeout)
-        except:
+        except Exception:
             self.timeout = 0.0
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defText":
                 membername = member.get("name")
@@ -280,15 +280,15 @@
             raise ParseException
         try:
             timeout = root.get("timeout")
             if not timeout:
                 self.timeout = 0.0
             else:
                 self.timeout = float(timeout)
-        except:
+        except Exception:
             self.timeout = 0.0
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and
         # value being a tuple of (label, format, min, max, step)
         self.memberlabels = {}
         for member in root:
             if member.tag == "defNumber":
@@ -413,15 +413,15 @@
             raise ParseException("Invalid perm given in defBLOBVector")
         try:
             timeout = root.get("timeout")
             if not self.timeout:
                 self.timeout = 0.0
             else:
                 self.timeout = float(timeout)
-        except:
+        except Exception:
             self.timeout = 0.0
         # create a dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defBLOB":
                 membername = member.get("name")
                 if not membername:
@@ -487,15 +487,15 @@
 
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         try:
             timeout = root.get("timeout")
             if not timeout is None:
                 self.timeout = float(timeout)
-        except:
+        except Exception:
             # dont update
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneSwitch":
                 membername = member.get("name")
                 if not membername:
@@ -524,15 +524,15 @@
 
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         try:
             timeout = root.get("timeout")
             if not timeout is None:
                 self.timeout = float(timeout)
-        except:
+        except Exception:
             # dont update
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneText":
                 membername = member.get("name")
                 if not membername:
@@ -558,15 +558,15 @@
 
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         try:
             timeout = root.get("timeout")
             if not timeout is None:
                 self.timeout = float(timeout)
-        except:
+        except Exception:
             # dont update
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneNumber":
                 membername = member.get("name")
                 if not membername:
@@ -631,15 +631,15 @@
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         self.eventtype = "SetBLOB"
         try:
             timeout = root.get("timeout")
             if not timeout is None:
                 self.timeout = float(timeout)
-        except:
+        except Exception:
             # dont update
             pass
         # create a dictionary of member name to value
         # and dictionary sizeformat
         # with key member name and value being a tuple of size, format
         self.sizeformat = {}
         for member in root:
@@ -648,24 +648,24 @@
                 if not membername:
                     raise ParseException("Missing name in oneBLOB")
                 membersize = member.get("size")
                 if not membersize:
                     raise ParseException("Missing size in oneBLOB")
                 try:
                     memberize = int(membersize)
-                except:
+                except Exception:
                     raise ParseException("Invalid size in oneBLOB")
                 memberformat = member.get("format")
                 if not memberformat:
                     raise ParseException("Missing format in oneBLOB")
                 if not member.text:
                     raise ParseException("Missing value in oneBLOB")
                 try:
                     self.data[membername] = standard_b64decode(member.text.encode('ascii'))
-                except:
+                except Exception:
                     raise ParseException("Unable to decode oneBLOB contents")
                 self.sizeformat[membername] = (membersize, memberformat)
             else:
                 raise ParseException("Invalid child tag of setBLOBVector")
         self.vector = device[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
```

### Comparing `indipyclient-0.1.3/indipyclient/ipyclient.py` & `indipyclient-0.1.4/indipyclient/ipyclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-import os, sys, collections, threading, asyncio, pathlib, time, traceback, copy
+import os, sys, collections, threading, asyncio, pathlib, time, copy
 
 from time import sleep
 
 from datetime import datetime, timezone
 
 from base64 import standard_b64encode
 
@@ -179,15 +179,15 @@
             try:
                 self.readerque.put_nowait(root)
             except asyncio.QueueFull:
                 # The queue is full, something may be wrong
                 # discard this data and continue
                 pass
         except Exception :
-            logger.exception("Error in IPyClient.report method")
+            logger.exception("Exception report from IPyClient.report method")
 
 
     def enabledlen(self):
         "Returns the number of enabled devices"
         return sum(map(lambda x:1 if x.enable else 0, self.data.values()))
 
 
@@ -215,20 +215,20 @@
                     self.clear()
                     self.report(f"Connected to {self.indihost}:{self.indiport}")
                     t1 = asyncio.create_task(self._run_tx(writer))
                     t2 = asyncio.create_task(self._run_rx(reader))
                     t3 = asyncio.create_task(self._check_alive(writer))
                     await asyncio.gather(t1, t2, t3)
                 except ConnectionRefusedError:
-                    self.report(f"Error: Connection refused on {self.indihost}:{self.indiport}")
-                except ConnectionResetError:
-                    self.report("Error: Connection Lost")
+                    self.report(f"Connection refused on {self.indihost}:{self.indiport}")
+                except ConnectionError:
+                    self.report("Connection Lost")
                 except Exception:
                     logger.exception("Connection Error")
-                    self.report("Error: Connection failed")
+                    self.report("Connection failed")
                 self._clear_connection()
                 # connection has failed, ensure all tasks are done
                 if t1:
                     while not t1.done():
                         await asyncio.sleep(0)
                 if t2:
                     while not t2.done():
@@ -245,15 +245,16 @@
                 count = 0
                 while not self._stop:
                     await asyncio.sleep(0.5)
                     count += 1
                     if count >= 10:
                         break
         except Exception:
-            logger.exception("Error in IPyClient._comms method")
+            logger.exception("Exception report from IPyClient._comms method")
+            raise
         finally:
             self.shutdown()
 
 
     def _clear_connection(self):
         "On a connection closing down, clears devices"
         self.connected = False
@@ -283,16 +284,17 @@
                        self._clear_connection()
                        if not self._stop:
                            self.report("Error: Connection timed out")
             if self.connected and self._stop:
                 writer.close()
                 await writer.wait_closed()
                 self._clear_connection()
-        except KeyboardInterrupt:
-            self.shutdown()
+        except Exception:
+            logger.exception("Error in IPyClient._check_alive method")
+            raise
         finally:
             self.connected = False
 
 
     def _logtx(self, txdata):
         "log tx data with level debug, and detail depends on self._verbose"
 
@@ -348,16 +350,17 @@
                 if (self.tx_timer is None) and (txdata.tag != "enableBLOB"):
                     self.tx_timer = time.time()
                 self.idle_timer = time.time()
                 if logger.isEnabledFor(logging.DEBUG):
                     self._logtx(txdata)
             # stop writing data, so clear writerque
             self.writerque.clear()
-        except KeyboardInterrupt:
-            self.shutdown()
+        except Exception:
+            logger.exception("Exception report from IPyClient._run_tx method")
+            raise
 
     def _logrx(self, rxdata):
         "log rx data to file"
         startlog = "RX:: "
         if self._verbose == 3:
             binarydata = ET.tostring(rxdata)
             logger.debug(startlog + binarydata.decode())
@@ -395,26 +398,17 @@
                         continue
                     # rxdata is now in readerque
                     break
                 if logger.isEnabledFor(logging.DEBUG):
                     self._logrx(rxdata)
                 if (not self.connected) or self._stop:
                     break
-        except RuntimeError:
-            # catches StopAsyncIteration and stops this coroutine
-            pass
-        except StopAsyncIteration:
-            # catches StopAsyncIteration and stops this coroutine
-            pass
-        except KeyboardInterrupt:
-            self.shutdown()
         except Exception:
-            logger.exception("Error in _run_rx")
-            self.shutdown()
-
+            logger.exception("Exception report from IPyClient._run_rx method")
+            raise
 
 
     async def _datasource(self, reader):
         "get received data, parse it, and yield it as xml.etree.ElementTree object"
         data_in = self._datainput(reader)
         message = b''
         messagetagnumber = None
@@ -464,33 +458,29 @@
                 # To reach this point, the message is in progress, with a messagetagnumber set
                 # keep adding the received data to message, until an endtag is reached
                 message += data
                 if message.endswith(_ENDTAGS[messagetagnumber]):
                     # the message is complete, handle message here
                     try:
                         root = ET.fromstring(message.decode("us-ascii"))
-                    except KeyboardInterrupt:
-                        self.shutdown()
-                        break
                     except ET.ParseError as e:
                         message = b''
                         messagetagnumber = None
                         continue
                     # xml datablock done, yield it up
                     yield root
                     # and start again, waiting for a new message
                     message = b''
                     messagetagnumber = None
-        except KeyboardInterrupt:
-            self.shutdown()
-        except asyncio.CancelledError:
-            self.shutdown()
+        except Exception:
+            logger.exception("Exception report from IPyClient._datasource method")
             raise
 
 
+
     async def _datainput(self, reader):
         "Generator producing binary string of data from the port"
         binarydata = b""
         try:
             while self.connected and (not self._stop):
                 await asyncio.sleep(0)
                 try:
@@ -509,18 +499,16 @@
                     binarydata = binarydata + data
                     yield binarydata
                     binarydata = b""
                 else:
                     # data has content but no > found
                     binarydata += data
                     # could put a max value here to stop this increasing indefinetly
-        except KeyboardInterrupt:
-            self.shutdown()
-        except asyncio.CancelledError:
-            self.shutdown()
+        except Exception:
+            logger.exception("Exception report from IPyClient._datainput method")
             raise
 
 
     async def _rxhandler(self):
         """Populates the events using data from self.readerque"""
         try:
             while not self._stop:
@@ -560,18 +548,18 @@
                     self.report(str(pe))
                     continue
                 finally:
                     self.readerque.task_done()
                 # and to get here, continue has not been called
                 # and an event has been created, call the user event handling function
                 await self.rxevent(event)
-        except asyncio.CancelledError:
-            raise
+
         except Exception:
-            logger.exception("Error in IPyClient._rxhandler method")
+            logger.exception("Exception report from IPyClient._rxhandler method")
+            raise
         finally:
             self.shutdown()
 
 
     def snapshot(self):
         """Take a snapshot of the devices and returns a dictionary of device
            names to objects which are restricted copies of the current state of devices and
@@ -605,16 +593,18 @@
                 propertyvector.send_newSwitchVector(timestamp, members)
             elif propertyvector.vectortype == "TextVector":
                 propertyvector.send_newTextVector(timestamp, members)
             elif propertyvector.vectortype == "NumberVector":
                 propertyvector.send_newNumberVector(timestamp, members)
             elif propertyvector.vectortype == "BLOBVector":
                 propertyvector.send_newBLOBVector(timestamp, members)
-        except KeyboardInterrupt:
-            self.shutdown()
+        except Exception:
+            logger.exception("Exception report from IPyClient.send_newVector method")
+            raise
+
 
     def set_vector_timeouts(self, timeout_enable=None, timeout_min=None, timeout_max=None):
         """Whenever you send updated values, a timer is started and if a timeout occurs
            before the server responds, a VectorTimeOut event will be created, which you
            could choose to ignore, or take action such as setting an Alert flag.
            The INDI protocol allows the server to suggest a timeout for each vector. This
            method allows you to set minimum and maximum timeouts which restricts the
@@ -664,18 +654,17 @@
                         # then send a getProperties, every five seconds, when count is zero
                         if not count:
                             self.send_getProperties()
                             self.report("getProperties sent")
                         count += 1
                         if count >= 10:
                             count = 0
-        except asyncio.CancelledError:
-             raise
         except Exception:
             logger.exception("Exception report from IPyClient._timeout_monitor method")
+            raise
         finally:
             self.shutdown()
 
 
     def send_getProperties(self, devicename=None, vectorname=None):
         """Sends a getProperties request. On startup the IPyClient object
            will automatically send getProperties, so typically you will
@@ -712,30 +701,15 @@
            event is an object with attributes according to the data received."""
         pass
 
 
     async def asyncrun(self):
         "Await this method to run the client."
         self._stop = False
-        t1 = asyncio.create_task(self._comms())
-        t2 = asyncio.create_task(self._rxhandler())
-        t3 = asyncio.create_task(self._timeout_monitor())
-        try:
-            await asyncio.gather(t1, t2, t3)
-        except Exception:
-            # one task has raised an exception, wait for the
-            # remaining tasks to stop
-            self._stop = True
-            logger.exception("Exception report from IPyClient.asyncrun coroutine")
-            while not t1.done():
-                await asyncio.sleep(0)
-            while not t2.done():
-                await asyncio.sleep(0)
-            while not t3.done():
-                await asyncio.sleep(0)
+        await asyncio.gather(self._comms(), self._rxhandler(), self._timeout_monitor())
         self.stopped = True
 
 
 class Device(collections.UserDict):
 
     "Each device is a mapping of vector name to vector object."
 
@@ -805,18 +779,16 @@
                 return events.defBLOBVector(root, self, self._client)
             elif root.tag == "setBLOBVector":
                 return events.setBLOBVector(root, self, self._client)
             else:
                 raise ParseException("Unrecognised tag received")
         except ParseException:
             raise
-        except KeyboardInterrupt:
-            raise
         except Exception:
-            logger.exception("Error in IPyClient.rxvector method")
+            logger.exception("Exception report from IPyClient.rxvector method")
             raise ParseException("Error while attempting to parse received data")
 
 
     def _snapshot(self):
         "Creates snapshot of this device and its vectors"
         snapdevice = Device(self.devicename)
         for vectorname, vector in self.data:
```

### Comparing `indipyclient-0.1.3/indipyclient/propertymembers.py` & `indipyclient-0.1.4/indipyclient/propertymembers.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             parts.append("0")
         assert len(parts) == 3
         # a part could be empty string, ie if 2:5: is given
         numbers = list(float(x) if x else 0.0 for x in parts)
         floatvalue = numbers[0] + (numbers[1]/60) + (numbers[2]/3600)
         if negative:
             floatvalue = -1 * floatvalue
-    except:
+    except Exception:
         raise TypeError("Unable to parse number value")
     return floatvalue
 
 
 class Member():
 
     """This class is the parent of further member classes.
@@ -298,15 +298,15 @@
                         integerminutes = 0
                         degrees = degrees + 1
                 valstring = f"{'-' if negative else ''}{degrees}:{integerminutes:02d}:{seconds:0{fn-4}.{fn-7}f}"
                 if w:
                     return valstring.rjust(int(w), ' ')
                 return valstring
 
-        except:
+        except Exception:
             raise TypeError("Unable to parse number value")
 
         # no other options accepted
         raise TypeError("Unable to process number format")
 
 
 class NumberMember(ParentNumberMember):
@@ -327,15 +327,15 @@
             raise ParseException("Number step value must be given as a string")
         self.step = step
         if not isinstance(membervalue, str):
             raise ParseException("Number value must be given as a string")
         try:
             # test a float can be created from this membervalue
             self._floatvalue = getfloat(membervalue)
-        except:
+        except Exception:
             raise ParseException("Cannot parse number received.")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
@@ -346,15 +346,15 @@
             raise ParseException("Number value must be given as a string")
         if not value:
             raise ParseException("No number value given")
         try:
             # test a float can be created from this membervalue
             # and save the float
             self._floatvalue = getfloat(value)
-        except:
+        except Exception:
             raise ParseException("Cannot parse number received")
         self._membervalue = value
 
 
     def getfloatvalue(self):
         """The INDI spec allows a number of different number formats, this method returns
            this members value as a float."""
@@ -416,15 +416,15 @@
         xmldata.set("size", str(newsize))
         # the value set in the xmldata object should be a bytes object
         if isinstance(newvalue, bytes):
             xmldata.text = newvalue
         elif isinstance(newvalue, pathlib.Path):
             try:
                 xmldata.text = newvalue.read_bytes()
-            except:
+            except Exception:
                 raise ParseException("Unable to read the given file")
         elif hasattr(newvalue, "seek") and hasattr(newvalue, "read") and callable(newvalue.read):
             # a file-like object
             # set seek(0) so is read from start of file
             newvalue.seek(0)
             bytescontent = newvalue.read()
             newvalue.close()
@@ -434,15 +434,15 @@
                 raise ParseException("The read BLOB value is empty")
             xmldata.text = bytescontent
         else:
             # could be a path to a file
             try:
                 with open(newvalue, "rb") as fp:
                     bytescontent = fp.read()
-            except:
+            except Exception:
                 raise ParseException("Unable to read the given file")
             if bytescontent == b"":
                 raise ParseException("The read BLOB value is empty")
             xmldata.text = bytescontent
         return xmldata
```

### Comparing `indipyclient-0.1.3/indipyclient/propertyvectors.py` & `indipyclient-0.1.4/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.3/pyproject.toml` & `indipyclient-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.1.3"
+version = "0.1.4"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.1.3/PKG-INFO` & `indipyclient-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

