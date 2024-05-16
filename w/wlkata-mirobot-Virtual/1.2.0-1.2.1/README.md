# Comparing `tmp/wlkata_mirobot_Virtual-1.2.0.tar.gz` & `tmp/wlkata_mirobot_Virtual-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkata_mirobot_Virtual-1.2.0.tar", last modified: Mon May 13 10:21:48 2024, max compression
+gzip compressed data, was "wlkata_mirobot_Virtual-1.2.1.tar", last modified: Thu May 16 08:37:39 2024, max compression
```

## Comparing `wlkata_mirobot_Virtual-1.2.0.tar` & `wlkata_mirobot_Virtual-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 10:21:48.972180 wlkata_mirobot_Virtual-1.2.0/
--rw-rw-rw-   0        0        0      110 2024-05-13 10:21:48.971182 wlkata_mirobot_Virtual-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-05-13 07:29:56.000000 wlkata_mirobot_Virtual-1.2.0/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 10:21:48.972180 wlkata_mirobot_Virtual-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      236 2024-05-13 10:21:35.000000 wlkata_mirobot_Virtual-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:21:48.966195 wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual/
--rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual/__init__.py
--rw-rw-rw-   0        0        0    15689 2024-05-13 10:21:12.000000 wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:21:48.970185 wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual.egg-info/
--rw-rw-rw-   0        0        0      110 2024-05-13 10:21:48.000000 wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-13 10:21:48.000000 wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 10:21:48.000000 wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-13 10:21:48.000000 wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 08:37:39.067685 wlkata_mirobot_Virtual-1.2.1/
+-rw-rw-rw-   0        0        0      110 2024-05-16 08:37:39.066687 wlkata_mirobot_Virtual-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-05-13 07:29:56.000000 wlkata_mirobot_Virtual-1.2.1/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 08:37:39.067685 wlkata_mirobot_Virtual-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      236 2024-05-16 08:36:20.000000 wlkata_mirobot_Virtual-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:37:39.062699 wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual/
+-rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual/__init__.py
+-rw-rw-rw-   0        0        0    16203 2024-05-16 08:36:11.000000 wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:37:39.065690 wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual.egg-info/
+-rw-rw-rw-   0        0        0      110 2024-05-16 08:37:38.000000 wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-16 08:37:39.000000 wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 08:37:38.000000 wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 08:37:38.000000 wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual.egg-info/top_level.txt
```

### Comparing `wlkata_mirobot_Virtual-1.2.0/license.txt` & `wlkata_mirobot_Virtual-1.2.1/license.txt`

 * *Files identical despite different names*

### Comparing `wlkata_mirobot_Virtual-1.2.0/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py` & `wlkata_mirobot_Virtual-1.2.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 ###### 虚拟控制器---API 示例
 ###### 
-###### Date: 2024-5-10
+###### Date: 2024-5-16
 
 import socket
 import json, os, re, socket,  inspect
 from struct import pack, unpack
-import  time,json, logging
+import  time,json, logging, threading
 
 FolderPath = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 robot_logger=logging.getLogger("Controler-Driver")
 robot_logger.setLevel(logging.DEBUG)
 
 class Virtual_WlkataMirobot():
 
     def __init__(self,server_IP='', server_port=None):
         
         self.server_IP = server_IP  
         self.server_port = server_port
         self.invalid_IP_Port_Connect()
+
         self.robot_type = 1
         self.global_state = [1,1,1]
         self.IO = [0,0,0,0,0,0,0,0]
         self.default_speed = 1000
+        ####
+        self.status_state = None
+        self.status_state2 = None
+
         ### 第七轴/滑轨
         self.angles_7 = 0
+        self.angles_7_com2 = 0
+
+        ### 接收数据线程
+        self.recv_thread_flag = True
+        receive_thread = threading.Thread(target = self.receive_data_from_server) 
+        receive_thread.start() 
+        
   
     ### 作为client 连接服务端--Start
     def invalid_IP_Port_Connect(self,):
         self.flag = False
         self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         #### 更改IP/PORT连接服务端 
         if self.server_IP == '':
@@ -43,24 +55,47 @@
             try:
                 ip_pattern = r'^((25[0-5]|2[0-4]\d|1\d{2}|[1-9]\d|\d)\.){3}(25[0-5]|2[0-4]\d|1\d{2}|[1-9]\d|\d)$'  
                 if not re.match(ip_pattern, self.server_IP):  
                     return False, 'Invalid IP address'  
                 
                 self.client_socket.connect((self.server_IP, self.server_port))
                 self.flag = True
-                print(f"Connected to {self.server_IP}:{self.server_port}")     
+                print(f"Connected to {self.server_IP}:{self.server_port}")
             
             except ValueError:
                 print(f"Please input the right ip/port")
                 return
 
+    def receive_data_from_server(self,):
+        while True:
+                try:
+                    ### 处理接收到的数据
+                    msg = self.client_socket.recv(1024).decode("utf-8")
+                    # print(f"接收: {msg}")
+
+                    # 正则表达式来匹配可能的JSON对象（这里简化了匹配规则，可能需要根据实际情况调整）  
+                    # pattern = r'"com1State":"(\w+)"'
+                    pattern = r'"com1State":"(\w*)","com2State":"(\w*)"'
+                    
+                    match = re.search(pattern, msg)
+                    if match:
+                        self.status_state = match.group(1)
+                        self.status_state2 = match.group(2)
+                
+                    else:
+                        self.status_state = None
+                        self.status_state2 = None
+                        print("No match found state")
+                    
+                except Exception as e:
+                    print(e)
+
     def disConnected(self):
         self.client_socket.close()
 
-
     ### 虚拟控制器测试代码--单元
     # 定义通讯协议格式  
     def build_packet(self,data_size, packet_type, message_body):  
         # 构建报头  
         header = json.dumps({  
             "data_size": data_size,  
             "type": packet_type  
@@ -89,97 +124,74 @@
             "RS485": rs485, 
             "com1Float": com1Float,
             "com2Float": com2Float,
             "IO": io  
         }  
         return json.dumps(message_body)  
 
-    def get_status_state(self):
-        try:
-            state = None
-            state2 = None
-           
-            ### 处理接收到的数据
-            msg = self.client_socket.recv(1024).decode("utf-8")
-            # print(f"接收: {msg}")
-
-            # 正则表达式来匹配可能的JSON对象（这里简化了匹配规则，可能需要根据实际情况调整）  
-            # pattern = r'"com1State":"(\w+)"'
-            pattern = r'"com1State":"(\w+)","com2State":"(\w+)"'
-            
-            match = re.search(pattern, msg)
-            if match:
-                state = match.group(1)
-                state2 = match.group(2)
-
-            else:
-                state = None
-                print("No match found state")
-
-        except Exception as e:
-            print(e)
-        return state, state2
-
     def validJog_Cartians_Speed(self, text):
         try:
             value = float(text)
             if value < -100 or value > 160:
                 print ("Value out of range")
         except ValueError:
             print()
 
-    def send_msg(self,com1_data=None, com2_data = None, wait_idle=False):
+    def send_msg(self, com1_data=None, com2_data = None, wait_idle=False):
         robot_type = self.robot_type
         state = self.global_state
         com1 = com1_data
-        com2 = com2_data ### if com2_data is not None else com1_data
+        com2 = com2_data
         rs485 = ""
         com1Float = self.angles_7 
-        com2Float = self.angles_7 
+        com2Float = self.angles_7_com2
         io = self.IO
         
         ### 消息体
         message_body = self.create_message_body(robot_type, state, com1, com2, rs485, com1Float, com2Float, io)
         ### 消息体长度
         data_size = len(message_body)
         ### 控制器类型：虚拟控制器
         packet_type = "virtual" 
         ### 构建数据包 
         packet = self.build_packet(data_size, packet_type, message_body)
-        
         self.client_socket.sendall(packet)
         time.sleep(0.5)
- 
+
         if wait_idle is None:
             wait_idle = False
         
-        if com2_data is not None:
-            self.status_state2 = None
-        
         if wait_idle:
-            self.wait_until_idle()
-    
+            if com2_data is not None:
+                self.wait_until_idle_2()
+            else:
+                self.wait_until_idle()
+
+    def wait_until_idle_2(self, refresh_rate = 0.1):
+        while self.status_state2 != "Idle" and  self.status_state != "Idle":
+            time.sleep(refresh_rate)
+            continue
+
+
     def wait_until_idle(self, refresh_rate = 0.1):
-        set_state = self.get_status_state()
-        status_state, status_state2 = set_state
-        if status_state2 is not None:
-            while status_state2 != "Idle" and  status_state != "Idle":
-                time.sleep(refresh_rate)
-                self.get_status_state()
-        else:
-            while status_state != "Idle" or status_state is None:
-                time.sleep(refresh_rate)
-                self.get_status_state()
+        while self.status_state != "Idle" or self.status_state is None:
+            time.sleep(refresh_rate)
+            continue
 
     ### G代码指令转换
     ### API函数
     ### IO输出设置
+    def set_7axis(self, com1_7axis = None, com2_7axis = None):
+            self.angles_7 = com1_7axis
+            self.angles_7_com2 = com2_7axis
+            return 1 #self.send_msg(wait_idle=True)
+
     def set_Output(self, output_id, value):
-        self.IO[output_id] = value
-        return self.send_msg()
+            self.IO[output_id] = value
+            return self.send_msg(wait_idle=True)
     
     def get_Input(self, input_id):
         try:
             msg = self.client_socket.recv(1024).decode("utf-8")
             pattern = r'"IO":\[([^\]]+)\]'
             match = re.search(pattern, msg)
             input = match.group(1)
@@ -190,26 +202,27 @@
             return None
 
     ### 机器人操作
     def home(self, has_slider=False,com1 = False, com2 = False):
         '''机械臂Homing'''
         if com1:
             if has_slider:
-                return self.home_7axis(com1 = com1)
+                self.home_7axis(com1 = com1)
+                return True
             else:
                 print("com1 home")
                 self.home_6axis(com1 = com1)
-                return 1
+                return True
         elif com2:
             if has_slider:
                 return self.home_7axis(com2 = com2)
             else:
                 print("com2 home")
                 self.home_6axis(com2 = com2)
-                return 1      
+                return True     
 
     def home_1axis(self, axis_id):
         '''单轴Homing'''
         if not isinstance(axis_id, int) or not (axis_id >= 1 and axis_id <= 7):
             return False
         msg = f'$h{axis_id}'
         return self.send_msg(msg, wait_idle=True)
@@ -217,15 +230,15 @@
     def home_6axis(self,com1 = False, com2 = False):
         '''六轴Homing'''
         msg = f'$h'
         if com1:
             self.send_msg(com1_data=msg, wait_idle=True)
         elif com2:
             self.send_msg(com2_data=msg, wait_idle=True)
-        return 1
+        return True
 
     def home_6axis_in_turn(self):
         '''六轴Homing, 各关节依次Homing'''
         msg = f'$hh'
         return self.send_msg(msg, wait_idle=True)
     
     def stop(self):
@@ -236,32 +249,33 @@
         msg = f'%'
         return self.send_msg(msg)
 
     def home_7axis(self, com1= False, com2 = False):
         '''七轴Homing(本体 + 滑台)'''
         msg = f'$h0'
         if com1:
+            print(f"home_7axis")
             self.send_msg(com1_data=msg, wait_idle=True)
         elif com2:
             self.send_msg(com2_data=msg, wait_idle=True)
-        return 1
+        return True
         
     def unlock_all_axis(self):
         '''解锁各轴锁定状态'''
         msg = 'M50'
         return self.send_msg(msg, wait_idle=True)
         
     def go_to_zero(self,com1 = False, com2 = False):
         '''回零-运动到名义上的各轴零点'''
         msg = 'M21 G90 G00 X0 Y0 Z0 A0 B0 C0 F2000'
         if com1:
             self.send_msg(com1_data=msg, wait_idle=True)
         elif com2:
             self.send_msg(com2_data=msg, wait_idle=True)
-        return 1
+        return True
 
     def set_speed(self, speed):
         '''设置转速'''
         # 转换为整数
         speed = int(speed)
         # 检查数值范围是否合法
         if speed <= 0 or speed > 6000:
@@ -320,15 +334,15 @@
             m3 = "G01"
 
         instruction = f"{m1} {m2} {m3} "
         
         msg = self.generate_args_string(instruction, pairings)
         return msg
 
-    def set_joint_angle(self, joint_angles=None, com1_P=None, com2_P = None,speed=None, is_relative=False, is_com2 = False, wait_ok=None):
+    def set_joint_angle(self, joint_angles=None, com1_P=None, com2_P = None,speed=None, is_relative=False, is_com2 = False, ):
         '''
         设置机械臂关节的角度
         joint_angles 目标关节角度字典, key是关节的ID号, value是角度(单位°)
             举例: {1:45.0, 2:-30.0}
         '''
         if joint_angles is not None:
             for joint_i in range(1, 8):
@@ -342,17 +356,17 @@
             joint_angles = {1:com2_P[0],2:com2_P[1],3:com2_P[2],4:com2_P[3],5:com2_P[4],6:com2_P[5]}
             is_com2 = True
         else :
             for joint_i in range(1, 7):
                 joint_angles[joint_i] = None
 
         return self.go_to_axis(x=joint_angles[1], y=joint_angles[2], z=joint_angles[3], a=joint_angles[4], \
-            b=joint_angles[5], c=joint_angles[6], is_relative=is_relative, speed=speed, is_com2 = is_com2, wait_ok=wait_ok)
+            b=joint_angles[5], c=joint_angles[6], is_relative=is_relative, speed=speed, is_com2 = is_com2,)
 
-    def go_to_axis(self, x=None, y=None, z=None, a=None, b=None, c=None, speed=None, is_relative=False, is_com2 = False, wait_ok=True):
+    def go_to_axis(self, x=None, y=None, z=None, a=None, b=None, c=None, speed=None, is_relative=False, is_com2 = False, ):
         '''设置关节角度/位置'''
         instruction = 'M21 G90'  # X{x} Y{y} Z{z} A{a} B{b} C{c} F{speed}
         if is_relative:
             instruction = 'M21 G91'
         if not speed:
             speed = self.default_speed
         if speed:
@@ -363,15 +377,15 @@
         if is_com2:
             self.send_msg(com2_data=msg, wait_idle=True)
         else:
             self.send_msg(com1_data=msg, wait_idle=True)
 
         return True
 
-    def set_tool_pose(self, x=None, y=None, z=None, roll=None, pitch=None, yaw=None, com1_P = None, com2_P = None,mode='p2p', speed=None, is_relative=False, is_com2 = False, wait_ok=True):
+    def set_tool_pose(self, x=None, y=None, z=None, roll=None, pitch=None, yaw=None, com1_P = None, com2_P = None,mode='p2p', speed=None, is_relative=False, is_com2 = False):
         '''设置工具位姿'''
 
         if com1_P is not None:
             x = com1_P[6]
             y = com1_P[7]
             z = com1_P[8]
             roll = com1_P[9]
@@ -387,23 +401,23 @@
             roll= com2_P[9]
             pitch= com2_P[10]
             yaw= com2_P[11]
             is_com2 = True
 
         if mode == "p2p":
             # 点控模式 Point To Point
-            self.p2p_interpolation(x=x, y=y, z=z, a=roll, b=pitch, c=yaw, speed=speed, is_relative=is_relative, is_com2 = is_com2, wait_ok=wait_ok)
+            self.p2p_interpolation(x=x, y=y, z=z, a=roll, b=pitch, c=yaw, speed=speed, is_relative=is_relative, is_com2 = is_com2,)
         elif mode == "linear":
             # 直线插补 Linera Interpolation
-            self.linear_interpolation(x=x, y=y, z=z, a=roll, b=pitch, c=yaw, speed=speed,is_relative=is_relative, is_com2 = is_com2, wait_ok=wait_ok)
+            self.linear_interpolation(x=x, y=y, z=z, a=roll, b=pitch, c=yaw, speed=speed,is_relative=is_relative, is_com2 = is_com2,)
         else:
             # 默认是点到点
-            self.p2p_interpolation(x=x, y=y, z=z, a=roll, b=pitch, c=yaw, speed=speed, is_com2 = is_com2, wait_ok=wait_ok)
+            self.p2p_interpolation(x=x, y=y, z=z, a=roll, b=pitch, c=yaw, speed=speed, is_com2 = is_com2, wait_idle=wait_idle)
 
-    def p2p_interpolation(self, x=None, y=None, z=None, a=None, b=None, c=None, speed=None, is_relative=False, is_com2 = False, wait_ok=None):
+    def p2p_interpolation(self, x=None, y=None, z=None, a=None, b=None, c=None, speed=None, is_relative=False, is_com2 = False):
         '''点到点插补'''
         instruction = 'M20 G90 G0'  # X{x} Y{y} Z{z} A{a} B{b} C{c} F{speed}
         if is_relative:
             instruction = 'M20 G91 G0'
 
         if not speed:
             speed = self.default_speed
@@ -414,19 +428,19 @@
         msg = self.generate_args_string(instruction, pairings)
         if is_com2:
             self.send_msg(com2_data=msg, wait_idle=True)
         else:
             self.send_msg(com1_data=msg, wait_idle=True)
         return True
     
-    def linear_interpolation(self,P1,speed=None, is_relative=False, is_com2 = False, wait_ok=None):
+    def linear_interpolation(self,P1,speed=None, is_relative=False, is_com2 = False, wait_idle=None):
         self.linear_interpolation_o( x=P1[6], y=P1[7], z=P1[8], a=P1[9], b=P1[10], c=P1[11],
-                            speed=speed,is_relative=is_relative,is_com2 = is_com2, wait_ok=wait_ok)
+                            speed=speed,is_relative=is_relative,is_com2 = is_com2)
     
-    def linear_interpolation_o(self, x=None, y=None, z=None, a=None, b=None, c=None, speed=None, is_relative=False, is_com2 = False, wait_ok=None):
+    def linear_interpolation_o(self, x=None, y=None, z=None, a=None, b=None, c=None, speed=None, is_relative=False, is_com2 = False):
         '''直线插补'''
         instruction = 'M20 G90 G1'  # X{x} Y{y} Z{z} A{a} B{b} C{c} F{speed}
         if is_relative:
             instruction = 'M20 G91 G1'
         if not speed:
             speed = self.default_speed
         if speed:
```

