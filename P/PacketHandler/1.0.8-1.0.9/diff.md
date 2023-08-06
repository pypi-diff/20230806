# Comparing `tmp/PacketHandler-1.0.8.tar.gz` & `tmp/PacketHandler-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PacketHandler-1.0.8.tar", last modified: Tue Jan  4 12:48:51 2022, max compression
+gzip compressed data, was "PacketHandler-1.0.9.tar", last modified: Sun Aug  6 14:46:39 2023, max compression
```

## Comparing `PacketHandler-1.0.8.tar` & `PacketHandler-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-01-04 12:48:51.124575 PacketHandler-1.0.8/
--rw-rw-rw-   0        0        0    35825 2020-11-27 19:30:41.000000 PacketHandler-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2736 2022-01-04 12:48:51.124076 PacketHandler-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-01-04 12:48:51.105573 PacketHandler-1.0.8/PacketHandler/
--rw-rw-rw-   0        0        0    16154 2022-01-04 12:48:37.000000 PacketHandler-1.0.8/PacketHandler/Packet.py
-drwxrwxrwx   0        0        0        0 2022-01-04 12:48:51.123075 PacketHandler-1.0.8/PacketHandler.egg-info/
--rw-rw-rw-   0        0        0     2736 2022-01-04 12:48:50.000000 PacketHandler-1.0.8/PacketHandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2022-01-04 12:48:50.000000 PacketHandler-1.0.8/PacketHandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-04 12:48:50.000000 PacketHandler-1.0.8/PacketHandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-01-04 12:48:50.000000 PacketHandler-1.0.8/PacketHandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-04 12:48:51.124575 PacketHandler-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      941 2022-01-04 10:08:31.000000 PacketHandler-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 14:46:39.307689 PacketHandler-1.0.9/
+-rw-rw-rw-   0        0        0    35825 2020-11-27 19:30:41.000000 PacketHandler-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3309 2023-08-06 14:46:39.306689 PacketHandler-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-06 14:46:39.296686 PacketHandler-1.0.9/PacketHandler/
+-rw-rw-rw-   0        0        0     4738 2023-08-06 14:38:35.000000 PacketHandler-1.0.9/PacketHandler/ExampleUsage.py
+-rw-rw-rw-   0        0        0    17903 2023-08-06 14:14:07.000000 PacketHandler-1.0.9/PacketHandler/Packet.py
+drwxrwxrwx   0        0        0        0 2023-08-06 14:46:39.305693 PacketHandler-1.0.9/PacketHandler.egg-info/
+-rw-rw-rw-   0        0        0     3309 2023-08-06 14:46:39.000000 PacketHandler-1.0.9/PacketHandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-08-06 14:46:39.000000 PacketHandler-1.0.9/PacketHandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 14:46:39.000000 PacketHandler-1.0.9/PacketHandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-06 14:46:39.000000 PacketHandler-1.0.9/PacketHandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 14:46:39.307689 PacketHandler-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-08-06 14:44:37.000000 PacketHandler-1.0.9/setup.py
```

### Comparing `PacketHandler-1.0.8/LICENSE.txt` & `PacketHandler-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PacketHandler-1.0.8/PKG-INFO` & `PacketHandler-1.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 Metadata-Version: 2.1
 Name: PacketHandler
-Version: 1.0.8
-Summary: Store data as packet. Serialize, Deserialize and Send, Recv, Encrypt, it.
+Version: 1.0.9
+Summary: Store data as packet. Send, Recv, Encrypt and Compress it. You will be able to manage **socket communication** easily and comprehensibly using this Python package.
 Home-page: https://github.com/emrecpp/PacketHandler
+Download-URL: https://pypi.org/project/PacketHandler/
 Author: Emre Demircan
 Author-email: emrecpp1@gmail.com
 License: GPL
-Download-URL: https://pypi.org/project/PacketHandler/
 Keywords: Packet,socket,Handler,PacketHandler,Packet Handler,send,recv,serialize,serialization,deserialize,deserialization,compress,encrypt
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python Packet Handler
-Store data as packet. Send, Recv, Encrypt it.
+Store data as packet. Send, Recv, Encrypt and Compress it.
+
+You will be able to manage **socket communication** easily and comprehensibly using this Python package.
+With version 1.0.9 or later, you can use the "**addListener**" function to direct incoming opcodes to the desired function upon receipt.
+
+Please refer to the [**Example Usage**](ExampleUsage.py) file for details and run it for demonstration.
+
+**These packages are also available for C# and C++ programming languages:**
 
-For C#: https://github.com/emrecpp/DataPacket-CSharp
+C#: https://github.com/emrecpp/DataPacket-CSharp
 
-For C++: https://github.com/emrecpp/DataPacket-CPP
+C++: https://github.com/emrecpp/DataPacket-CPP
+## Installation
+You can install **PacketHandler** using pip:
 
-Take a Look! [Test](https://github.com/emrecpp/PacketHandler/blob/main/Test.py)
+```
+pip install PacketHandler
+```
 
-# Example Usage
+# Usage ([**Detailed Usage**](ExampleUsage.py))
 
 ```
 from Packet import Packet, ref
 import sys, socket, select, time
 
 class opcodes:
     LOGIN=100
@@ -47,15 +57,15 @@
 while True:
     if PaketListen.Recv(socketServer):
         PaketListen.Print("RECEIVED PACKET (YOUR TITLE)!")
         if PacketListen.GetOpcode() == opcodes.LOGIN:
             UserName, Password, RememberMe, Data, Fruits = ref(str), ref(str), ref(bool), ref(bytearray), ref(list)
             PacketListen >> UserName >> Password >> RememberMe >> Data >> Fruits
             UserName, Password, RememberMe, Data, Fruits = str(UserName), str(Password), RememberMe.obj, bytearray(Data.obj), ", ".join(Fruits.obj)  # We have to cast ref object to (int, str, bool, bytearray ...)
-            # Note: Can't use bool(RememberMe), this returns True everytime!!!
+            # Note: Can't use bool(RememberMe), this returns True everytime. Use .obj always !!!
 
             print(f"Username: {UserName}\nPassword: {Password}\nRememberMe: {'Yes' if RememberMe else 'No'}\nData: {str(Data)}\nFruits: {Fruits}")
     else:
         return # Connection Lost
 
 ```
 
@@ -66,18 +76,15 @@
 Password: 123
 RememberMe: Yes
 Data: bytearray(b'\x07\x10BYTES\xff')
 Fruits: Apple, Banana, Orange
 
 
 *** RECEIVED PACKET (YOUR TITLE)! *** (67)
-00000000: 00 64 04 06 00 00 00 00 00 04 45 6D 72 65 00 00   .d........Emre..
-00000010: 00 03 31 32 33 01 00 00 00 08 07 10 42 59 54 45   ..123.......BYTE
-00000020: 53 FF 00 00 00 1D 5B 22 41 70 70 6C 65 22 2C 20   S.ÿ.........[.".A.p.p.l.e.".,..
+00000000: 00 64 02 06 00 00 04 00 00 00 45 6D 72 65 03 00   .d........Emre..
+00000010: 00 00 31 32 33 01 08 00 00 00 07 10 42 59 54 45   ..123.......BYTE
+00000020: 53 FF 1D 00 00 00 5B 22 41 70 70 6C 65 22 2C 20   S.Ã¿.........[.".A.p.p.l.e.".,..
 00000030: 22 42 61 6E 61 6E 61 22 2C 20 22 4F 72 61 6E 67   "Banana",."Orang
 00000040: 65 22 5D                                           e"]
 
 ```
 
-
-
-
```

### Comparing `PacketHandler-1.0.8/PacketHandler/Packet.py` & `PacketHandler-1.0.9/PacketHandler/Packet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,219 @@
 # -*- coding: utf-8 -*-
 """ Store data as packet. Encrypt, Compress, Send-Recv(Serialize, Deserialize) it.."""
-''' | Notes |
-  
-    1) If LittleEndian is enabled, this variable must have the same value when sending and recving packets.
-         Example:
-             On Send:
-                 PktForSend = Packet(Opcode=10, LittleEndian=True)
-                 PktForSend.Send(sock)
-             On Recv:
-                 PktForRecv = Packet(LittleEndian=True) # if don't set Little Endian to true, defaultly false this will cause error
-                 PktForRecv.Recv()                
-'''
+
 
 # https://www.github.com/emrecpp
 
-version = "1.0.8"
+version = "1.0.9"
 __author__ = "Emre Demircan (emrecpp1@gmail.com)"
-__date__ = "2022-01-04"
+__date__ = "2023-08-06"
 __github__ = "emrecpp"
 
 import sys, time, json, socket, struct
 from functools import singledispatch
 from datetime import datetime
 from enum import IntEnum
+import core.helpers as helper
+from core.DataEnums import OnSendRecv, EListener
 
+class PacketManager(object):
+    #_m_send, _m_recv = [], []
+    _m_recv:list[EListener] = []
+    @staticmethod
+    def addListener(listener:EListener):
+        PacketManager._m_recv.append(listener)
+        '''if onType == OnSendRecv.SEND:
+            PacketManager._m_send.append(onType)
+        elif onType == OnSendRecv.RECV:
+            PacketManager._m_recv.append(onType)'''
+
+    @staticmethod
+    def getListenerByOpcode(opcode:int):
+        for listener in PacketManager._m_recv:
+            if listener.opcode == opcode:
+                return listener
+        return None
+    @staticmethod
+    def removeListener(listener:EListener):
+        if not listener: return
+        if listener in PacketManager._m_recv:
+            PacketManager._m_recv.remove(listener)
+    @staticmethod
+    def removeListenerByOpcode(opcode:int):
+        PacketManager.removeListener(PacketManager.getListenerByOpcode(opcode=opcode))
 
 class Packet(object):
     storage = bytearray()
 
     # First 2 bytes : Opcodes [ 0 - (256*256-1) ]
-    INDEX_OF_FLAG           = 2  # 3. byte: Flags (is Packet LittleEndian? Encrypted? Compressed?)
-    INDEX_OF_COUNT_ELEMENTS = 3  # 4. byte: Count of Total Data types
+    __INDEX_OF_FLAG           = 2  # 3. byte: Flags (is Packet LittleEndian? Encrypted? Compressed?)
+    __INDEX_OF_COUNT_ELEMENTS = 3  # 4. byte: Count of Total Data types
     # Todo: 5. byte: empty for now
     # Todo: 6. byte: empty for now
 
-    _rpos, _wpos = 6, 6
-    _bLittleEndian, _bEncrypt, _bCompress, _bPrintErrorLog = False, False, False, False
+    _rpos = _wpos = 6
+    _m_Encrypt = _m_Compress = _m_PrintErrorLog = False
 
     Last_SendTime = None  # datetime will stored when Packet Sent
     Last_RecvTime = None  # datetime will stored when Packet Received
 
     class Flags(IntEnum):
         Encrypted    = 1
         LittleEndian = 2
         Compressed   = 4
 
     # Maximum a Variable data Size = "\xFF\xFF\xFF\xFF" (4.294.967.295 bytes (4GB))
-    def __init__(self, Opcode=0, LittleEndian=False, Encrypt=False, Compress=False, PrintErrorLog=False):
-        super(Packet, self).__init__()
+    def __init__(self, Opcode:int=0, LittleEndian:bool=False, Encrypt:bool=False, Compress:bool=False, PrintErrorLog:bool=False):
+        super().__init__()
         self.storage = bytearray()
-        self.storage.extend(struct.pack(">H", Opcode))  # Hard-coded Big Endian
-        self.storage.extend(b'\0\0\0\0')
-        self._rpos, self._wpos, self.littleEndian = 6, 6, LittleEndian
-        self._bEncrypt, self._bCompress, self._bPrintErrorLog = Encrypt, Compress, PrintErrorLog
+        self._initNew(newOpcode=Opcode) # init first 6 bytes (
+        self._rpos = self._wpos = 6
+        self._m_Encrypt, self._m_Compress, self._m_PrintErrorLog = Encrypt, Compress, PrintErrorLog
+        self.littleEndian = LittleEndian
         self.overload_append = singledispatch(self.append)
         self.overload_append.register(int, self.append_int)
         self.overload_append.register(str, self.append_str)
         self.overload_append.register(bytearray, self.append_bytearray)
         self.overload_append.register(list, self.append_list)
+        self.overload_append.register(dict, self.append_dict)
         self.overload_append.register(bool, self.append_bool)
+        self.overload_append.register(bytes, self.append_bytes)
 
     @property
-    def littleEndian(self):
-        return self._bLittleEndian
+    def littleEndian(self) -> bool:
+        return self.storage[self.__INDEX_OF_FLAG] & self.Flags.LittleEndian
 
     @littleEndian.setter
     def littleEndian(self, value):
-        self._bLittleEndian = value
         if value:
-            self.storage[self.INDEX_OF_FLAG] |= self.Flags.LittleEndian
+            self.storage[self.__INDEX_OF_FLAG] |= self.Flags.LittleEndian
         else:
-            self.storage[self.INDEX_OF_FLAG] &= ~self.Flags.LittleEndian
+            self.storage[self.__INDEX_OF_FLAG] &= ~self.Flags.LittleEndian
 
     def append(self, buffer):
-        return TypeError("Packet: append Unknown Data Type")
+        raise TypeError("Append Unknown Data Type")
+
+    def _initNew(self, newOpcode=None) -> None:
+        result_opcode = 0
+        if newOpcode:
+            result_opcode = newOpcode
+        elif self.size() > 0 and self.GetOpcode() != 0:
+            result_opcode = self.GetOpcode()
+        self.storage.clear()
+        del self.storage
+        self.storage = bytearray(struct.pack(">H", result_opcode))  # Hard-coded Big Endian
+
+        self.storage.extend(b'\0\0\0\0')
+        self._rpos = self._wpos  = 6
 
     def clear(self) -> None:
-        if self.size() > 0 and self.GetOpcode() != 0:
-            Opcode = self.GetOpcode()
-            self.storage.clear()
-            del self.storage
-            self.storage = bytearray(struct.pack(">H", Opcode))  # Hard-coded Big Endian
-            self.storage.extend(b'\0\0\0\0')
-        else:
-            self.storage.clear()
-            self.storage.extend(b'\0\0\0\0\0\0')
-        self._rpos = 6
-        self._wpos = 6
+        self._initNew()
 
-    def Encrypt(self) -> None:
+    def Encrypt(self, seed:int = 0x123) -> None:
         for i in range(2 + 4, self.size()):  # Skip opcode (first 2 bytes) and reserved 4 bytes
             data = self.storage[i]
-            encVal = 0x123 + i * 4
+            encVal = seed + i * 4
             encVal ^= 0xFF
 
             self.storage[i] = (data + encVal) & 0xFF
-        self.storage[self.INDEX_OF_FLAG] |= self.Flags.Encrypted
+        self.storage[self.__INDEX_OF_FLAG] |= self.Flags.Encrypted
 
-    def Decrypt(self) -> None:
+    def Decrypt(self, seed:int = 0x123) -> None:
         for i in range(2 + 4, self.size()):  # Skip opcode (first 2 bytes) and reserved 4 bytes
             data = self.storage[i]
-            encVal = 0x123 + i * 4
+            encVal = seed + i * 4
             encVal ^= 0xFF
 
             self.storage[i] = (data - encVal) & 0xFF
 
-        self.storage[self.INDEX_OF_FLAG] &= ~self.Flags.Encrypted
+        self.storage[self.__INDEX_OF_FLAG] &= ~self.Flags.Encrypted
 
     def Compress(self) -> None:
-        if (self.storage[self.INDEX_OF_FLAG] & self.Flags.Compressed) == self.Flags.Compressed:
+        if (self.storage[self.__INDEX_OF_FLAG] & self.Flags.Compressed) == self.Flags.Compressed:
             return  # if Already Compressed
         import bz2
         self.storage[2 + 4:] = bz2.compress(self.storage[2 + 4:])
-        self.storage[self.INDEX_OF_FLAG] |= self.Flags.Compressed
+        self.storage[self.__INDEX_OF_FLAG] |= self.Flags.Compressed
 
     def DeCompress(self) -> None:
-        if (self.storage[self.INDEX_OF_FLAG] & self.Flags.Compressed) != self.Flags.Compressed:
+        if (self.storage[self.__INDEX_OF_FLAG] & self.Flags.Compressed) != self.Flags.Compressed:
             return  # if Already DeCompressed / Not Compressed
         import bz2
         self.storage[2 + 4:] = bz2.decompress(self.storage[2 + 4:])
-        self.storage[self.INDEX_OF_FLAG] &= ~self.Flags.Compressed
+        self.storage[self.__INDEX_OF_FLAG] &= ~self.Flags.Compressed
 
-    def append_int(self, buffer) -> None:
+    def append_int(self, buffer:int) -> None:
         bf = struct.pack("<I" if self.littleEndian else ">I", buffer)
         self.storage.extend(bf)
         self._wpos += len(bf)
 
-    def append_str(self, buffer) -> None:
+    def append_str(self, buffer:str) -> None:
         bytesBuffer = bytes(buffer, "utf-8")
         bf = struct.pack("%ds" % (len(bytesBuffer)), bytesBuffer)
         self.storage.extend(struct.pack("<I" if self.littleEndian else ">I", len(bf)))
         self.storage.extend(bf)
         self._wpos += len(bf)
 
-    def append_bytearray(self, buffer) -> None:
+    def append_bytearray(self, buffer:bytearray) -> None:
         self.storage.extend(struct.pack("<I" if self.littleEndian else ">I", len(buffer)))
         self.storage.extend(buffer)
         self._wpos += len(buffer)
 
-    def append_list(self, buffer) -> None:
+    def append_list(self, buffer:list) -> None:
         self << json.dumps(buffer)
+    def append_dict(self, buffer:dict):
+        self << json.dumps(buffer, ensure_ascii=False, indent=None)
 
-    def append_bool(self, buffer) -> None:
+    def append_bool(self, buffer:bool) -> None:
         self.storage.extend(b'\x01' if buffer else b'\x00')
         self._wpos += 1
 
+    def append_bytes(self, buffer:bytes) -> None:
+        self << bytearray(buffer)
+
+
+
+
     def __len__(self) -> int:
         return self.size()
 
     def size(self) -> int:
         return len(self.storage)
 
     def GetOpcode(self) -> int:
-        return 0 if len(self.storage) < 2 else (
-        struct.unpack("<H" if self.littleEndian else ">H", self.storage[0:2])[0])
+        return 0 if len(self.storage) < 2 else (struct.unpack(">H", self.storage[0:2])[0]) # hard coded big endian
 
     def GetItemsCount(self) -> int:  # [ 0 - 255 ]
-        return int(self.storage[self.INDEX_OF_COUNT_ELEMENTS]) if self.INDEX_OF_COUNT_ELEMENTS < self.size() else 0
+        return int(self.storage[self.__INDEX_OF_COUNT_ELEMENTS]) if self.__INDEX_OF_COUNT_ELEMENTS < self.size() else 0
 
     def __lshift__(self, value):
         self.overload_append(value)
-        COUNT_ELEMENTS = self.storage[self.INDEX_OF_COUNT_ELEMENTS]
+        COUNT_ELEMENTS = self.storage[self.__INDEX_OF_COUNT_ELEMENTS]
         if COUNT_ELEMENTS + 1 <= 255:
-            self.storage[self.INDEX_OF_COUNT_ELEMENTS] += 1
+            self.storage[self.__INDEX_OF_COUNT_ELEMENTS] += 1
         return self
 
     def __rshift__(self, value):
         if value.obj == int:
             Sonuc = self.read_int()
         elif value.obj == str:
             Sonuc = self.read_str()
         elif value.obj == bytearray:
             Sonuc = self.read_bytearray()
+        elif value.obj == bytes:
+            Sonuc = self.read_bytes()
         elif value.obj == list:
             Sonuc = self.read_list()
+        elif value.obj == dict:
+            Sonuc = self.read_dict()
         elif value.obj == bool:
             Sonuc = self.read_bool()
         else:
-            return self
+            raise TypeError("Read Unknown Data Type")
 
         value.obj = Sonuc
         return self
 
     def readLength(self) -> int:  # Reserved Data Size, in 4 bytes
         return self.read_int()
 
@@ -205,19 +237,27 @@
     def read_bytearray(self) -> bytearray:
         ReadLength = self.readLength()
         if ReadLength == None:
             return bytearray()
         data = bytearray(self.storage[self._rpos:self._rpos + ReadLength])
         self._rpos += ReadLength
         return data
+    def read_bytes(self) -> bytes:
+        BYTES = ref(bytearray)
+        self >> BYTES
+        return bytes(BYTES.obj)
 
     def read_list(self) -> list:
         STR = ref(str)
         self >> STR
         return json.loads(str(STR))
+    def read_dict(self) -> list:
+        STR = ref(str)
+        self >> STR
+        return json.loads(str(STR))
 
     def read_bool(self) -> bool:
         bool = True if self.storage[self._rpos] == 1 else False
         self._rpos += 1
         return bool
 
     # waitRecv = if you have a Recv function in thread, then you sent packet will received from this thread received function. So creating new socket, sending and receiving data from new socket. So Thread Recv function can't access this data.
@@ -226,15 +266,15 @@
         :param s: Send socket
         :param waitRecv: bool
         """
         try:
             if self.size() == 0:
                 return False
             if hasattr(s, "_closed") and s._closed:
-                if self._bPrintErrorLog: print("Packet Handler | Connection is already closed!")
+                if self._m_PrintErrorLog: print("Packet Handler | Connection is already closed!")
                 return False
 
             TargetSocket = s
 
             if waitRecv:
                 SocketCreatedNew = False
                 if type(waitRecv) == socket.socket:  # if Socket created we will not close it and we can use it multiple times.
@@ -245,20 +285,20 @@
 
                     SocketCreatedNew = True
                     newSocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                     # newSocket.connect(s.getsockname())
                     newSocket.connect(s.getpeername())  # Be sure; Server can listen more than 1 socket.
                     TargetSocket = newSocket
 
-            if self._bCompress and (self.storage[self.INDEX_OF_FLAG] & self.Flags.Compressed) == 0: self.Compress()
-            if self._bEncrypt and (self.storage[self.INDEX_OF_FLAG] & self.Flags.Encrypted) == 0: self.Encrypt()
+            if self._m_Compress and (self.storage[self.__INDEX_OF_FLAG] & self.Flags.Compressed) == 0: self.Compress()
+            if self._m_Encrypt and (self.storage[self.__INDEX_OF_FLAG] & self.Flags.Encrypted) == 0: self.Encrypt()
 
             numberOfBytes = self.size()
 
-            msgLength = struct.pack("<I" if self.littleEndian else ">I", self.size())
+            msgLength = struct.pack(">I", self.size()) # Hard-coded Big Endian
             TargetSocket.send(msgLength)  # Sending Packet Size before all data
 
             totalBytesSent = 0
             while totalBytesSent < numberOfBytes:
                 totalBytesSent += TargetSocket.send(self.storage[totalBytesSent:])
             self.Last_SendTime = datetime.now()
             if waitRecv:
@@ -269,62 +309,68 @@
 
                 return self
 
             return True
         except (ConnectionError, ConnectionAbortedError, ConnectionRefusedError, ConnectionResetError):
             return False
         except OSError:
-            if self._bPrintErrorLog: print("Packet Handler | Send Failed probably Connection Closed.")
+            if self._m_PrintErrorLog: print("Packet Handler | Send Failed probably Connection Closed.")
             return False
         except Exception as ERR:
-            if self._bPrintErrorLog: self.PrintErr("Packet Send Err: %s    " % str(ERR))
+            if self._m_PrintErrorLog: helper.PrintErr("Packet Send Err: %s    " % str(ERR))
             return False
 
     def Recv(self, s, clear=True) -> bool:
         """
         :param s: Socket to wait Recv
         :param clear: Clear Packet before Receiving data
         """
         try:
             if clear:
                 self.clear()
             packetSize = s.recv(4)
             if not packetSize:  # Connection Closed
                 return False
-            packetSize = struct.unpack("<I" if self.littleEndian else ">I", packetSize)[0]
+            packetSize = struct.unpack(">I", packetSize)[0] # Hard-coded Big Endian
 
             self.storage.clear()
             totalBytesReceived = 0
 
             while totalBytesReceived < packetSize:
                 ReceivedBytes = s.recv(packetSize - totalBytesReceived)
 
                 if not ReceivedBytes:
-                    if self._bPrintErrorLog: print("Packet Handler | Connection closed while receiving")
+                    if self._m_PrintErrorLog: print("Packet Handler | Connection closed while receiving")
                     return False
                 self.storage.extend(ReceivedBytes)
                 totalBytesReceived += len(ReceivedBytes)
 
             self.Last_RecvTime = datetime.now()
-            if (self.storage[self.INDEX_OF_FLAG] & self.Flags.Encrypted) == self.Flags.Encrypted: self.Decrypt()
-            if (self.storage[self.INDEX_OF_FLAG] & self.Flags.Compressed) == self.Flags.Compressed: self.DeCompress()
+            if (self.storage[self.__INDEX_OF_FLAG] & self.Flags.Encrypted) == self.Flags.Encrypted: self.Decrypt()
+            if (self.storage[self.__INDEX_OF_FLAG] & self.Flags.Compressed) == self.Flags.Compressed: self.DeCompress()
             self._wpos = self.size()
             if self._rpos == 0 and self.size() > 0:
                 self._rpos = 6  # Skip Opcode
+            listener_if_exists = PacketManager.getListenerByOpcode(self.GetOpcode())
+            if listener_if_exists:
+                args = listener_if_exists.callback_arguments if listener_if_exists.callback_arguments else ()
+
+                if listener_if_exists.first_argument_packet:
+                    args = (self,) + args
+                    helper.CallFunc((listener_if_exists.callback, *args))
+                else:
+                    helper.CallFunc((listener_if_exists.callback, args))
             return True
         except (ConnectionError, ConnectionAbortedError, ConnectionRefusedError, ConnectionResetError):
             return False
         except Exception as ERR:
-            if self._bPrintErrorLog: self.PrintErr("Packet Recv Err: %s    " % str(ERR))
+            if self._m_PrintErrorLog: helper.PrintErr("Packet Recv Err: %s    " % str(ERR))
             return False
 
-    def PrintErr(self, ERR) -> None:
-        exc_type, exc_obj, exc_tb = sys.exc_info();
-        fname = exc_tb.tb_frame.f_code.co_filename
-        print(ERR, exc_type, fname, exc_tb.tb_lineno)
+    
 
     def Print(self, Title="", maxPerLine=16, utf_8=True, Flag=1 | 2 | 4) -> str:  # 1 Address, 2 Hex Bytes, 4 ASCII
         """
         :param maxPerLine: How many bytes will show on per line
         :param utf_8: Decode ASCII to Utf-8
         :param Flag: 1 Address, 2 Hex Bytes, 4 ASCII
         :return: printing and returning print string
@@ -375,15 +421,15 @@
                                 line += chr(byte)
                             else:
                                 line += '.'
                 Total += line + "\n"
             print(Total)
             return Total
         except Exception as err:
-            self.PrintErr("Print Error: %s    " % err)
+            helper.PrintErr("Print Error: %s    " % err)
             return ""
 
 
 class ref():  # We don't have Pointers in Python :(
     obj = None
     def __init__(self, obj): self.obj = obj
     def __get__(self, instance, owner): return self.obj
@@ -391,7 +437,11 @@
     def __eq__(self, other): return other == self.obj
     def __setattr__(self, key, value): self.__dict__[key] = value
     def __getattr__(self, item): return self.obj
     def __str__(self):  # print("Data: %s" % (data_str))
         return str(self.obj)
     def __int__(self):  # print("Data: %d" % (data_int))
         return self.obj
+
+
+class EListener(EListener): # for access only packet.py file
+    pass
```

### Comparing `PacketHandler-1.0.8/PacketHandler.egg-info/PKG-INFO` & `PacketHandler-1.0.9/PacketHandler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 Metadata-Version: 2.1
 Name: PacketHandler
-Version: 1.0.8
-Summary: Store data as packet. Serialize, Deserialize and Send, Recv, Encrypt, it.
+Version: 1.0.9
+Summary: Store data as packet. Send, Recv, Encrypt and Compress it. You will be able to manage **socket communication** easily and comprehensibly using this Python package.
 Home-page: https://github.com/emrecpp/PacketHandler
+Download-URL: https://pypi.org/project/PacketHandler/
 Author: Emre Demircan
 Author-email: emrecpp1@gmail.com
 License: GPL
-Download-URL: https://pypi.org/project/PacketHandler/
 Keywords: Packet,socket,Handler,PacketHandler,Packet Handler,send,recv,serialize,serialization,deserialize,deserialization,compress,encrypt
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Python Packet Handler
-Store data as packet. Send, Recv, Encrypt it.
+Store data as packet. Send, Recv, Encrypt and Compress it.
+
+You will be able to manage **socket communication** easily and comprehensibly using this Python package.
+With version 1.0.9 or later, you can use the "**addListener**" function to direct incoming opcodes to the desired function upon receipt.
+
+Please refer to the [**Example Usage**](ExampleUsage.py) file for details and run it for demonstration.
+
+**These packages are also available for C# and C++ programming languages:**
 
-For C#: https://github.com/emrecpp/DataPacket-CSharp
+C#: https://github.com/emrecpp/DataPacket-CSharp
 
-For C++: https://github.com/emrecpp/DataPacket-CPP
+C++: https://github.com/emrecpp/DataPacket-CPP
+## Installation
+You can install **PacketHandler** using pip:
 
-Take a Look! [Test](https://github.com/emrecpp/PacketHandler/blob/main/Test.py)
+```
+pip install PacketHandler
+```
 
-# Example Usage
+# Usage ([**Detailed Usage**](ExampleUsage.py))
 
 ```
 from Packet import Packet, ref
 import sys, socket, select, time
 
 class opcodes:
     LOGIN=100
@@ -47,15 +57,15 @@
 while True:
     if PaketListen.Recv(socketServer):
         PaketListen.Print("RECEIVED PACKET (YOUR TITLE)!")
         if PacketListen.GetOpcode() == opcodes.LOGIN:
             UserName, Password, RememberMe, Data, Fruits = ref(str), ref(str), ref(bool), ref(bytearray), ref(list)
             PacketListen >> UserName >> Password >> RememberMe >> Data >> Fruits
             UserName, Password, RememberMe, Data, Fruits = str(UserName), str(Password), RememberMe.obj, bytearray(Data.obj), ", ".join(Fruits.obj)  # We have to cast ref object to (int, str, bool, bytearray ...)
-            # Note: Can't use bool(RememberMe), this returns True everytime!!!
+            # Note: Can't use bool(RememberMe), this returns True everytime. Use .obj always !!!
 
             print(f"Username: {UserName}\nPassword: {Password}\nRememberMe: {'Yes' if RememberMe else 'No'}\nData: {str(Data)}\nFruits: {Fruits}")
     else:
         return # Connection Lost
 
 ```
 
@@ -66,18 +76,15 @@
 Password: 123
 RememberMe: Yes
 Data: bytearray(b'\x07\x10BYTES\xff')
 Fruits: Apple, Banana, Orange
 
 
 *** RECEIVED PACKET (YOUR TITLE)! *** (67)
-00000000: 00 64 04 06 00 00 00 00 00 04 45 6D 72 65 00 00   .d........Emre..
-00000010: 00 03 31 32 33 01 00 00 00 08 07 10 42 59 54 45   ..123.......BYTE
-00000020: 53 FF 00 00 00 1D 5B 22 41 70 70 6C 65 22 2C 20   S.ÿ.........[.".A.p.p.l.e.".,..
+00000000: 00 64 02 06 00 00 04 00 00 00 45 6D 72 65 03 00   .d........Emre..
+00000010: 00 00 31 32 33 01 08 00 00 00 07 10 42 59 54 45   ..123.......BYTE
+00000020: 53 FF 1D 00 00 00 5B 22 41 70 70 6C 65 22 2C 20   S.Ã¿.........[.".A.p.p.l.e.".,..
 00000030: 22 42 61 6E 61 6E 61 22 2C 20 22 4F 72 61 6E 67   "Banana",."Orang
 00000040: 65 22 5D                                           e"]
 
 ```
 
-
-
-
```

### Comparing `PacketHandler-1.0.8/setup.py` & `PacketHandler-1.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='PacketHandler',
-    version='1.0.8',
-    description='Store data as packet. Serialize, Deserialize and Send, Recv, Encrypt, it.',
+    version='1.0.9',
+    description='Store data as packet. Send, Recv, Encrypt and Compress it. You will be able to manage **socket communication** easily and comprehensibly using this Python package.',
     long_description_content_type="text/markdown",
     long_description=README ,
     license='GPL',
     packages=["PacketHandler"],
     author='Emre Demircan',
     author_email='emrecpp1@gmail.com',
     keywords=['Packet', 'socket', 'Handler','PacketHandler', 'Packet Handler', 'send', 'recv','serialize','serialization','deserialize','deserialization','compress','encrypt'],
```

