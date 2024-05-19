# Comparing `tmp/pydglab_ws-0.1.0.tar.gz` & `tmp/pydglab_ws-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydglab_ws-0.1.0.tar", max compression
+gzip compressed data, was "pydglab_ws-1.0.0.tar", max compression
```

## Comparing `pydglab_ws-0.1.0.tar` & `pydglab_ws-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1535 2024-05-15 06:00:29.373034 pydglab_ws-0.1.0/LICENSE
--rw-r--r--   0        0        0     5811 2024-05-15 06:00:29.373034 pydglab_ws-0.1.0/README.md
--rw-r--r--   0        0        0      179 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/__init__.py
--rw-r--r--   0        0        0       82 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/client/__init__.py
--rw-r--r--   0        0        0     8466 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/client/base.py
--rw-r--r--   0        0        0      915 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/client/connect.py
--rw-r--r--   0        0        0     1542 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/client/local.py
--rw-r--r--   0        0        0     1557 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/client/ws.py
--rw-r--r--   0        0        0     3333 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/enums.py
--rw-r--r--   0        0        0      400 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/exceptions.py
--rw-r--r--   0        0        0     2304 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/models.py
--rw-r--r--   0        0        0       22 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/server/__init__.py
--rw-r--r--   0        0        0    11473 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/server/server.py
--rw-r--r--   0        0        0      930 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/typing.py
--rw-r--r--   0        0        0     3376 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pydglab_ws/utils.py
--rw-r--r--   0        0        0     1267 2024-05-15 06:00:29.377035 pydglab_ws-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6895 1970-01-01 00:00:00.000000 pydglab_ws-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1535 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6171 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/README.md
+-rw-r--r--   0        0        0      179 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/client/__init__.py
+-rw-r--r--   0        0        0     9795 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/client/base.py
+-rw-r--r--   0        0        0      923 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/client/connect.py
+-rw-r--r--   0        0        0     1552 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/client/local.py
+-rw-r--r--   0        0        0     1910 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/client/ws.py
+-rw-r--r--   0        0        0     3433 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/enums.py
+-rw-r--r--   0        0        0      724 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/exceptions.py
+-rw-r--r--   0        0        0     2813 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/models.py
+-rw-r--r--   0        0        0       22 2024-05-18 13:21:49.765006 pydglab_ws-1.0.0/pydglab_ws/server/__init__.py
+-rw-r--r--   0        0        0    17992 2024-05-18 13:21:49.769006 pydglab_ws-1.0.0/pydglab_ws/server/server.py
+-rw-r--r--   0        0        0      755 2024-05-18 13:21:49.769006 pydglab_ws-1.0.0/pydglab_ws/typing.py
+-rw-r--r--   0        0        0     4032 2024-05-18 13:21:49.769006 pydglab_ws-1.0.0/pydglab_ws/utils.py
+-rw-r--r--   0        0        0     1293 2024-05-18 13:21:49.769006 pydglab_ws-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 pydglab_ws-1.0.0/PKG-INFO
```

### Comparing `pydglab_ws-0.1.0/LICENSE` & `pydglab_ws-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydglab_ws-0.1.0/README.md` & `pydglab_ws-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 <h1 align="center">
   PyDGLab-WS
 </h1>
 
 <p align="center">
-  一个用于创建郊狼 DG-Lab App Socket 被控的客户端和服务端的 Python 库
+  一个用于创建郊狼 3.0 DG-Lab App Socket 控制终端和服务端的 Python 库
 </p>
 
 <p align="center">
   <a href="https://pydglab-ws.readthedocs.io">📖 完整文档</a>
 </p>
 
 <p align="center">
-  <a href="https://pypi.org/project/pydglab-ws" target="_blank">
-    <img src="https://img.shields.io/github/v/release/Ljzd-PRO/PyDGLab-WS?logo=python" alt="Version">
+  <a href="https://www.codefactor.io/repository/github/ljzd-pro/pydglab-ws">
+    <img src="https://www.codefactor.io/repository/github/ljzd-pro/pydglab-ws/badge" alt="CodeFactor" />
   </a>
 
-  <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/Ljzd-PRO/PyDGLab-WS" alt="BSD 3-Clause"/>
+  <a href="https://codecov.io/gh/Ljzd-PRO/PyDGLab-WS" target="_blank">
+      <img src="https://codecov.io/gh/Ljzd-PRO/PyDGLab-WS/branch/master/graph/badge.svg?token=VTr0LB1yWF" alt="codecov"/>
+  </a>
+
+  <a href="https://github.com/Ljzd-PRO/PyDGLab-WS/actions/workflows/codecov.yml" target="_blank">
+    <img alt="Test Result" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/PyDGLab-WS/codecov.yml">
+  </a>
+
+  <a href='https://pydglab-ws.readthedocs.io/'>
+    <img src='https://readthedocs.org/projects/pydglab-ws/badge/?version=latest' alt='Documentation Status' />
   </a>
 
   <a href="https://github.com/Ljzd-PRO/PyDGLab-WS/activity">
     <img src="https://img.shields.io/github/last-commit/Ljzd-PRO/PyDGLab-WS/master" alt="Last Commit"/>
   </a>
 
-  <a href="https://codecov.io/gh/Ljzd-PRO/PyDGLab-WS" target="_blank">
-      <img src="https://codecov.io/gh/Ljzd-PRO/PyDGLab-WS/branch/master/graph/badge.svg?token=VTr0LB1yWF" alt="codecov"/>
+  <a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/Ljzd-PRO/PyDGLab-WS" alt="BSD 3-Clause"/>
   </a>
 
-  <a href='https://pydglab-ws.readthedocs.io/'>
-    <img src='https://readthedocs.org/projects/pydglab-ws/badge/?version=latest' alt='Documentation Status' />
+  <a href="https://pypi.org/project/pydglab-ws" target="_blank">
+    <img src="https://img.shields.io/github/v/release/Ljzd-PRO/PyDGLab-WS?logo=python" alt="Version">
   </a>
 </p>
 
-> [!Warning]
-> 目前项目还在开发中，API 可能发生较多变更
-
 ## 💡 特性
 
 - 通过该库可开发 Python 程序，接入 DG-Lab App
 - 完全使用 asyncio 异步，并发执行各项操作
 - 可部署第三方终端与 Socket 服务一体的服务端，降低部署复杂度和延迟
-- 使用异步生成器、迭代器等，结合语言特性
+- 使用异步生成器、上下文管理器等，结合语言特性
 - 通过 Pydantic, 枚举 管理消息结构和常量，便于开发
 
 ### 🔧 DG-Lab App 的 Socket 被控功能支持的操作
 
 - 获取 A, B 通道强度 以及 通道强度上限 的数据更新
 - 对 A, B 通道强度进行操作，支持增加、减少、设定到指定值
 - 向 App 发送持续一段时间的波形操作数据
@@ -67,22 +72,24 @@
 
 ### 📡 搭建服务端
 
 ```python3
 import asyncio
 from pydglab_ws.server import DGLabWSServer
 
+
 async def main():
     async with DGLabWSServer("0.0.0.0", 5678, 60) as server:
         while True:
-            print(f"已连接的 WebSocket 客户端（终端/App）：{list(server.ws_client_ids)}")
+            print(f"已连接的 WebSocket 客户端（终端/App）：{list(server.uuid_to_ws.keys())}")
             print(f"已连接的本地终端：{list(server.local_client_ids)}")
             print(f"关系绑定：{server.client_id_to_target_id}")
             await asyncio.sleep(5)
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 更多演示请查看 [`examples/server.py`](examples/server.py)
 
 ### 🕹️ 搭建客户端 / 第三方终端
@@ -90,18 +97,20 @@
 当进入 `DGLabWSServer` 的异步生成器时，从 WebSocket 服务端获取 `clientId` 的操作会 **自动完成**
 
 ```python3
 import asyncio
 from websockets import ConnectionClosedOK
 from pydglab_ws import DGLabWSConnect
 
+
 def print_qrcode(_: str):
     """输出二维码到终端界面"""
     ...
 
+
 async def main():
     try:
         async with DGLabWSConnect("ws://192.168.1.161:5678") as client:
             # 获取二维码
             url = client.get_qrcode()
             print("请用 DG-Lab App 扫描二维码以连接")
             print_qrcode(url)
@@ -112,14 +121,15 @@
 
             # 从 App 接收数据更新，并进行远控操作
             async for data in client.data_generator():
                 print(f"收取到数据：{data}")
     except ConnectionClosedOK:
         print("Socket 服务端断开连接")
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 更多演示请查看 [`examples/ws_client.py`](examples/ws_client.py)
 
 ### 🕹️ 搭建与第三方终端一体的 WebSocket 服务端
@@ -131,18 +141,20 @@
 > 因此在该段代码中，终端相关的逻辑与上面的独立的 WebSocket 终端的实现基本相同。 \
 > 这种方式，省去了终端连接 WebSocket 服务端的环节，终端与 WebSocket 服务端一体，**网络延迟更低，部署更方便**。
 
 ```python3
 import asyncio
 from pydglab_ws import DGLabWSServer
 
+
 def print_qrcode(_: str):
     """输出二维码到终端界面"""
     ...
 
+
 async def main():
     async with DGLabWSServer("0.0.0.0", 5678, 60) as server:
         client = server.new_local_client()
 
         url = client.get_qrcode("ws://192.168.1.161:5678")
         print("请用 DG-Lab App 扫描二维码以连接")
         print_qrcode(url)
@@ -151,14 +163,15 @@
         await client.bind()
         print(f"已与 App {client.target_id} 成功绑定")
 
         # 从 App 接收数据更新，并进行远控操作
         async for data in client.data_generator():
             print(f"收取到数据：{data}")
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
 
 更多演示请查看 [`examples/local_client_with_server.py`](examples/server_with_local_client.py)
```

### Comparing `pydglab_ws-0.1.0/pydglab_ws/client/base.py` & `pydglab_ws-1.0.0/pydglab_ws/client/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,24 +58,24 @@
     def not_bind(self) -> bool:
         """终端是否未完成与 App 的绑定"""
         return self._client_id is None or self.target_id is None
 
     @abstractmethod
     async def _recv(self) -> WebSocketMessage:
         """
-        收取来自 WebSocket 服务端的消息，并解析为 :class:`WebSocketMessage`
+        收取来自 WebSocket 服务端的消息，并解析为 [`WebSocketMessage`][pydglab_ws.models.WebSocketMessage]
         """
         ...
 
     @abstractmethod
     async def _send(self, message: WebSocketMessage):
         """
         向 WebSocket 服务端发送消息
 
-        :param message: 解析为 :class:`WebSocketMessage` 的消息
+        :param message: 解析为 [`WebSocketMessage`][pydglab_ws.models.WebSocketMessage] 的消息
         """
         ...
 
     def get_qrcode(self, uri: str) -> Optional[str]:
         """
         终端二维码，二维码图像需要自行生成
 
@@ -108,39 +108,44 @@
             target_id=self._target_id,
             message=msg
         )
         await self._send(message)
 
     @staticmethod
     def _handle_msg(message: WebSocketMessage) -> Optional[Union[StrengthData, FeedbackButton]]:
-        """处理类型为 ``msg`` 的消息"""
-        if message.message.startswith(MessageDataHead.STRENGTH.value):
-            return parse_strength_data(message.message)
-        elif message.message.startswith(MessageDataHead.FEEDBACK.value):
-            return parse_feedback_data(message.message)
-        else:
-            return None
+        """
+        处理类型为 ``msg`` 的消息
+
+        :raise InvalidStrengthData: [`InvalidStrengthData`][pydglab_ws.exceptions.InvalidStrengthData]
+        :raise InvalidFeedbackData: [`InvalidFeedbackData`][pydglab_ws.exceptions.InvalidFeedbackData]
+        """
+        if isinstance(message.message, str):
+            if message.message.startswith(MessageDataHead.STRENGTH.value):
+                return parse_strength_data(message.message)
+            elif message.message.startswith(MessageDataHead.FEEDBACK.value):
+                return parse_feedback_data(message.message)
+        return None
 
     @staticmethod
     def _handle_break(message: WebSocketMessage) -> Optional[Literal[RetCode.CLIENT_DISCONNECTED]]:
         """处理类型为 ``break`` 的消息"""
-        return RetCode(int(message.message)) if message.message.isdigit() else None
+        return message.message
 
     @staticmethod
     def _handle_heartbeat(message: WebSocketMessage) -> Optional[Literal[RetCode.SUCCESS]]:
         """处理类型为 ``heartbeat`` 的消息"""
-        return RetCode(int(message.message)) if message.message.isdigit() else None
+        return message.message
 
     async def register(self):
         """
         从 WebSocket 服务端中获取 ``client_id`` 并保存
         """
         while self.not_registered:
             message = await self._recv()
-            if message.type == MessageType.BIND and message.message == MessageDataHead.TARGET_ID.value:
+            if message.type == MessageType.BIND and message.message == MessageDataHead.TARGET_ID:
                 self._client_id = message.client_id
 
     async def ensure_bind(self):
         """确保终端已完成与 App 的绑定"""
         while True:
             if self.not_registered:
                 await self.register()
@@ -152,28 +157,31 @@
     async def bind(self) -> RetCode:
         """
         等待与 DG-Lab App 的关系绑定，并保存 ``target_id``
         :return: 响应码
         """
         while self.not_bind:
             message = await self._recv_owned()
-            if message.type == MessageType.BIND and message.message.isdigit():
-                ret_code = RetCode(int(message.message))
-                if ret_code == RetCode.SUCCESS:
+            if message.type == MessageType.BIND and isinstance(message.message, RetCode):
+                if message.message == RetCode.SUCCESS:
                     self._target_id = message.target_id
-                return ret_code
+                return message.message
 
     async def recv_data(self) -> Union[StrengthData, FeedbackButton, RetCode]:
         """
         获取 WebSocket 服务端的数据
 
         注意，获取到的是队列中最早的数据，可能不是最新的
 
-        :return: 可能为 **强度数据** - :class:`StrengthData`、**App 反馈数据** - :class:`FeedbackButton` \
-            、**心跳** - ``RetCode.SUCCESS``、**App 断开连接** - ``RetCode.CLIENT_DISCONNECTED``
+        :return: 可能为 **强度数据** - [`StrengthData`][pydglab_ws.models.StrengthData]、 \
+            **App 反馈数据** - [`FeedbackButton`][pydglab_ws.enums.FeedbackButton] \
+            、**心跳** - [`RetCode.SUCCESS`][pydglab_ws.enums.RetCode]、 \
+            **App 断开连接** - [`RetCode.CLIENT_DISCONNECTED`][pydglab_ws.enums.RetCode]
+        :raise InvalidStrengthData: [`InvalidStrengthData`][pydglab_ws.exceptions.InvalidStrengthData]
+        :raise InvalidFeedbackData: [`InvalidFeedbackData`][pydglab_ws.exceptions.InvalidFeedbackData]
         """
         await self.ensure_bind()
         while True:
             message = await self._recv_owned()
             handler = self._message_type_to_handler.get(message.type)
             if handler and (result := handler(message)) is not None:
                 return result
@@ -185,19 +193,20 @@
         """
         强度数据异步生成器
 
         注意，是从队列中最早的数据开始获取，可能不是最新的
 
         示例：
         ```python3
-        async for data in client.data_generator():
+        async for data in client.data_generator(StrengthData, FeedbackButton):
             print(f"Got data from App: {data}")
         ```
         :param targets: 目标类型，只有为目标类型的数据会被返回，为空即默认值时则不进行限制
-        :return: 可能为 **强度数据** - :class:`StrengthData`、**App 反馈数据** - :class:`FeedbackButton` \
+        :return: 可能为 **强度数据** - [`StrengthData`][pydglab_ws.models.StrengthData]、 \
+            **App 反馈数据** - [`FeedbackButton`][pydglab_ws.enums.FeedbackButton] \
             、**心跳** - ``RetCode.SUCCESS``、**App 断开连接** - ``RetCode.CLIENT_DISCONNECTED``
         """
         while True:
             data = await self.recv_data()
             if not targets or type(data) in targets:
                 yield data
 
@@ -224,27 +233,33 @@
             self,
             channel: Channel,
             *pulses: PulseOperation
     ):
         """
         下发波形数据
 
+        - 每条波形数据代表了 100ms 的数据，所以若每次发送的数据有 10 条，那么就是 1s 的数据。 \
+          由于网络有一定延时，若要保证波形输出的连续性，建议波形数据的发送间隔略微小于波形数据的时间长度 (< 1s)
+        - 数组最大长度为 100,也就是最多放置 10s 的数据，另外 App 中的波形队列最大长度为 500，即为 50s 的数据， \
+          若后接收到的数据无法全部放入波形队列，多余的部分会丢弃。所以谨慎考虑您的数据长度和数据发送间隔
+
         :param channel: 通道选择
         :param pulses: 波形操作数据，最大长度为 100
         """
         await self.ensure_bind()
         await self._send_owned(
             MessageType.MSG,
             dump_add_pulses(channel, *pulses)
         )
 
     async def clear_pulses(self, channel: Channel):
         """
         清空波形队列
 
         :param channel: 通道选择
+        :raise InvalidPulseOperation: [`InvalidPulseOperation`][pydglab_ws.exceptions.InvalidPulseOperation]
         """
         await self.ensure_bind()
         await self._send_owned(
             MessageType.MSG,
             dump_clear_pulses(channel)
         )
```

### Comparing `pydglab_ws-0.1.0/pydglab_ws/client/connect.py` & `pydglab_ws-1.0.0/pydglab_ws/client/connect.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
     DG-Lab 终端的 WebSocket 连接管理器
 
     示例：
     ```python3
     async with DGLabWSConnect("ws://localhost:5678") as client:
         await client.bind()
-        await client.
+        print("成功绑定")
     ```
 
     :param uri: WebSocket 服务端 Uri
     :param kwargs: :class:`websockets.client.connect` 的其他参数
     """
 
     def __init__(self, uri: str, **kwargs):
```

### Comparing `pydglab_ws-0.1.0/pydglab_ws/client/local.py` & `pydglab_ws-1.0.0/pydglab_ws/client/local.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class DGLabLocalClient(DGLabClient):
     # noinspection SpellCheckingInspection
     """
         DG-Lab 终端，并不实际发送 WebSocket 消息，而是直接与本地服务端进行通信
 
-        本地服务端指同一线程下的 :class:`pydglab_ws.server.server.DGLabWSServer`
+        本地服务端指同一线程下的 [`DGLabWSServer`][pydglab_ws.server.server.DGLabWSServer]
 
         :param client_id: 终端 ID
         :param sender: 用于客户端发送消息的回调函数
         :param queue_setter: 回调函数，用于服务端设置客户端的消息队列
         :param max_queue: 消息队列最大长度
         """
```

### Comparing `pydglab_ws-0.1.0/pydglab_ws/client/ws.py` & `pydglab_ws-1.0.0/pydglab_ws/client/ws.py`

 * *Files 26% similar despite different names*

```diff
@@ -44,7 +44,17 @@
                 pass
             else:
                 host = f"[{host}]" if is_v6 else host
             socket = self._websocket.transport.get_extra_info("socket")
             secure = isinstance(socket, SSLSocket)
             uri = f"{'wss' if secure else 'ws'}://{host}:{port}"
         return super().get_qrcode(uri)
+
+    @property
+    def websocket(self) -> WebSocketClientProtocol:
+        """
+        终端的 WebSocket 连接对象
+
+        可用来获取连接延迟等信息，但不建议调用它的 recv, send 等方法，可能会影响
+        [`DGLabWSClient`][pydglab_ws.client.ws.DGLabWSClient] 的各项功能
+        """
+        return self._websocket
```

### Comparing `pydglab_ws-0.1.0/pydglab_ws/enums.py` & `pydglab_ws-1.0.0/pydglab_ws/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 此处定义了一些常量枚举
 """
+import enum
 from enum import Enum, IntEnum
 
 __all__ = (
     "MessageType",
     "RetCode",
     "MessageDataHead",
     "StrengthOperationType",
     "FeedbackButton",
     "Channel"
 )
 
 
-class MessageType(Enum):
+@enum.unique
+class MessageType(str, Enum):
     """
     WebSocket 消息类型
 
     :ivar HEARTBEAT: 心跳包数据
     :ivar BIND: ID 关系绑定
     :ivar MSG: 波形下发/强度变化/队列清空等数据指令
     :ivar BREAK: 连接断开
@@ -26,14 +28,15 @@
     HEARTBEAT = "heartbeat"
     BIND = "bind"
     MSG = "msg"
     BREAK = "break"
     ERROR = "error"
 
 
+@enum.unique
 class RetCode(IntEnum):
     """
     WebSocket 消息错误码枚举
 
     :ivar SUCCESS: 成功
     :ivar CLIENT_DISCONNECTED: 对方客户端已断开
     :ivar INVALID_CLIENT_ID: 二维码中没有有效的 ``clientId``
@@ -55,15 +58,16 @@
     INCOMPATIBLE_RELATIONSHIP = 402
     NON_JSON_CONTENT = 403
     RECIPIENT_NOT_FOUND = 404
     MESSAGE_TOO_LONG = 405
     SERVER_INTERNAL_ERROR = 500
 
 
-class MessageDataHead(Enum):
+@enum.unique
+class MessageDataHead(str, Enum):
     """
     WebSocket 消息数据开头部分
 
     :ivar TARGET_ID: Socket 通道与终端绑定
     :ivar DG_LAB: 关系绑定
     :ivar STRENGTH: 强度操作
     :ivar PULSE: 波形操作
@@ -75,14 +79,15 @@
     DG_LAB = "DGLAB"
     STRENGTH = "strength"
     PULSE = "pulse"
     CLEAR = "clear"
     FEEDBACK = "feedback"
 
 
+@enum.unique
 class StrengthOperationType(IntEnum):
     """
     强度变化模式
 
     :ivar DECREASE: 通道强度减少
     :ivar INCREASE: 通道强度增加
     :ivar SET_TO: 通道强度变化为指定数值
@@ -103,14 +108,15 @@
 #     """
 #     NONE = 0b00
 #     INCREASE = 0b01
 #     DECREASE = 0b10
 #     SET_TO = 0b11
 
 
+@enum.unique
 class FeedbackButton(IntEnum):
     """
     App 反馈按钮
 
     * A 通道 5 个按钮（从左至右）的角标为 0,1,2,3,4
     * B 通道 5 个按钮（从左至右）的角标为 5,6,7,8,9
     """
@@ -122,14 +128,15 @@
     B1 = 5
     B2 = 6
     B3 = 7
     B4 = 8
     B5 = 9
 
 
+@enum.unique
 class Channel(IntEnum):
     """
     通道
 
     :ivar A: A 通道
     :ivar B: B 通道
     """
```

### Comparing `pydglab_ws-0.1.0/pydglab_ws/models.py` & `pydglab_ws-1.0.0/pydglab_ws/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 此处定义了一些 Pydantic 模型，使用 Pydantic V2
 """
-from typing import Optional, Any
+from typing import Optional, Any, Union
 
 from pydantic import BaseModel, UUID4, ConfigDict, field_serializer, AliasGenerator, model_validator, \
     field_validator
 from pydantic.alias_generators import to_camel, to_snake
 
-from .enums import MessageType
+from .enums import MessageType, RetCode, MessageDataHead
 
 __all__ = ("WebSocketMessage", "StrengthData")
 
 
 # noinspection PyNestedDecorators
 class WebSocketMessage(BaseModel):
     """
@@ -29,15 +29,31 @@
             serialization_alias=to_camel
         )
     )
 
     type: MessageType
     client_id: Optional[UUID4] = None
     target_id: Optional[UUID4] = None
-    message: str
+    message: Union[str, RetCode, MessageDataHead]
+
+    @field_validator("message")
+    @classmethod
+    def _validate_message(cls, value: Any):
+        """
+        自动先行尝试解析 `message`
+        """
+        if isinstance(value, str):
+            try:
+                return RetCode(int(value))
+            except ValueError:
+                try:
+                    return MessageDataHead(value)
+                except ValueError:
+                    pass
+        return value
 
     @field_serializer("client_id", "target_id")
     def _serialize_id(self, value: Optional[UUID4]):
         """
         序列化时，当值为 ``None``，序列化成空字符串
         """
         return value or ""
@@ -52,15 +68,15 @@
 
     @model_validator(mode="before")
     @classmethod
     def _field_to_pascal(cls, data: Any):
         """
         验证模型时，将所有的键名更改为蛇形命名法（下划线）
 
-        验证时不取别名的原因是，取别名会影响对象初始化参数名，而 AliasChoices 不知为何不起作用
+        验证时不取别名的原因是，取别名会影响对象初始化参数名，而 ``AliasChoices`` 不知为何不起作用
         """
         if isinstance(data, dict):
             for key in list(data.keys()):
                 data[to_snake(key)] = data.pop(key)
         return data
```

### Comparing `pydglab_ws-0.1.0/pydglab_ws/typing.py` & `pydglab_ws-1.0.0/pydglab_ws/typing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 """
 此处创建了一些自定义类型
 """
-from typing import NewType, Tuple
+from typing import Tuple
 
 __all__ = (
     "WaveformFrequency",
     "WaveformStrength",
     "WaveformFrequencyOperation",
     "WaveformStrengthOperation",
     "PulseOperation"
 )
 
-WaveformFrequency = NewType("WaveformFrequency", int)
-"""波形频率"""
-WaveformStrength = NewType("WaveformStrength", int)
-"""波形强度"""
-WaveformFrequencyOperation = NewType(
-    "WaveformFrequencyOperation",
-    Tuple[
-        WaveformFrequency, WaveformFrequency, WaveformFrequency, WaveformFrequency
-    ]
-)
-WaveformStrengthOperation = NewType(
-    "WaveformStrengthOperation",
-    Tuple[
-        WaveformStrength, WaveformStrength, WaveformStrength, WaveformStrength
-    ]
-)
-PulseOperation = NewType(
-    "PulseOperation",
-    Tuple[
-        WaveformFrequencyOperation,
-        WaveformStrengthOperation
-    ]
-)
-"""波形操作数据，类似 DG-Lab-V3 蓝牙协议中的波形数据"""
+WaveformFrequency = int
+"""波形频率，范围在 [10, 240]"""
+WaveformStrength = int
+"""波形强度，范围在 [0, 100]"""
+WaveformFrequencyOperation = Tuple[
+    WaveformFrequency, WaveformFrequency, WaveformFrequency, WaveformFrequency
+]
+"""波形频率操作数据"""
+WaveformStrengthOperation = Tuple[
+    WaveformStrength, WaveformStrength, WaveformStrength, WaveformStrength
+]
+"""波形强度操作数据"""
+PulseOperation = Tuple[
+    WaveformFrequencyOperation,
+    WaveformStrengthOperation
+]
+"""波形操作数据"""
```

### Comparing `pydglab_ws-0.1.0/pydglab_ws/utils.py` & `pydglab_ws-1.0.0/pydglab_ws/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 此处提供一些工具函数
 """
 import json
 
 from pydantic import UUID4
 
 from .enums import StrengthOperationType, Channel, MessageDataHead, FeedbackButton
-from .exceptions import InvalidStrengthData, InvalidFeedbackData
+from .exceptions import InvalidStrengthData, InvalidFeedbackData, InvalidPulseOperation
 from .models import StrengthData
 from .typing import PulseOperation
 
 __all__ = (
     "dump_pulse_operation",
     "dg_lab_client_qrcode",
     "dump_strength_operation",
@@ -22,15 +22,15 @@
 
 
 def parse_strength_data(data: str) -> StrengthData:
     """
     解析消息中的强度数据
 
     :param data: WebSocket 消息中的 ``message``
-    :raise InvalidStrengthData: :class:`InvalidStrengthData`
+    :raise InvalidStrengthData: [`InvalidStrengthData`][pydglab_ws.exceptions.InvalidStrengthData]
     """
     try:
         values = data.split("-")[1].split("+")
         return StrengthData(
             a=int(values[0]),
             b=int(values[1]),
             a_limit=int(values[2]),
@@ -41,15 +41,15 @@
 
 
 def parse_feedback_data(data: str) -> FeedbackButton:
     """
     解析消息中的 App 反馈数据
 
     :param data: WebSocket 消息中的 ``message``
-    :raise InvalidFeedbackData: :class:`InvalidFeedbackData`
+    :raise InvalidFeedbackData: [`InvalidFeedbackData`][pydglab_ws.exceptions.InvalidFeedbackData]
     """
     try:
         return FeedbackButton(int(data.split("-")[1]))
     except IndexError as e:
         raise InvalidFeedbackData(data) from e
 
 
@@ -80,44 +80,54 @@
 
 
 def dump_pulse_operation(pulse: PulseOperation) -> str:
     """
     生成波形操作的数据
 
     :param pulse: 波形操作数据
-    :return: 返回数据可作为 WebSocket 消息中的 ``message``
+    :return: 返回数据与蓝牙协议类似
+    :raise InvalidPulseOperation: [`InvalidPulseOperation`][pydglab_ws.exceptions.InvalidPulseOperation]
     """
-    pulse_bytes = bytes().join(
-        value.to_bytes() for operation in pulse for value in operation
-    )
-    return pulse_bytes.hex()
+    try:
+        pulse_bytes = bytes().join(
+            # int.to_bytes Python 3.11 才添加了 length, byteorder 的默认参数值
+            value.to_bytes(
+                length=1,
+                byteorder='big'
+            ) for operation in pulse for value in operation
+        )
+    except (TypeError, AttributeError, OverflowError) as e:
+        raise InvalidPulseOperation(pulse) from e
+    else:
+        return pulse_bytes.hex()
 
 
 def dump_add_pulses(
         channel: Channel,
         *pulses: PulseOperation
 ) -> str:
     """
     生成下放波形操作的数据
 
     :param channel: 通道选择
     :param pulses: 波形操作数据
     :return: 返回数据可作为 WebSocket 消息中的 ``message``
+    :raise InvalidPulseOperation: [`InvalidPulseOperation`][pydglab_ws.exceptions.InvalidPulseOperation]
     """
     dict_data = {
         f"{MessageDataHead.PULSE.value}-{channel.value}": [dump_pulse_operation(pulse) for pulse in pulses]
     }
     return json.dumps(dict_data)
 
 
-def dg_lab_client_qrcode(uri: str, client_id: UUID4):
+def dg_lab_client_qrcode(uri: str, client_id: UUID4) -> str:
     """
     生成终端二维码，二维码图像需要自行生成
 
     :param uri: WebSocket 服务端 URI，例如：``ws://107.47.91.92:4567``
             （注意末尾不能有 ``/``）
     :param client_id: 终端 ID
-    :return:
+    :return: 终端二维码内容，二维码图像需要自行生成
     """
     return (f"https://www.dungeon-lab.com/app-download.php"
             f"#DGLAB-SOCKET"
             f"#{uri}/{client_id}")
```

### Comparing `pydglab_ws-0.1.0/pyproject.toml` & `pydglab_ws-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydglab-ws"
-version = "0.1.0"
+version = "1.0.0"
 description = "一个通过 WebSocket 控制郊狼 DG-Lab 的 Python 库"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.asia>"]
 readme = "README.md"
 homepage = "https://pydglab-ws.readthedocs.io"
 repository = "https://github.com/Ljzd-PRO/PyDGLab-WS"
 documentation = "https://pydglab-ws.readthedocs.io"
 
@@ -30,14 +30,15 @@
 mike = "^2.1.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.0"
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
 pytest-order = "^1.2.1"
+pytest-timeout = "^2.3.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `pydglab_ws-0.1.0/PKG-INFO` & `pydglab_ws-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydglab-ws
-Version: 0.1.0
+Version: 1.0.0
 Summary: 一个通过 WebSocket 控制郊狼 DG-Lab 的 Python 库
 Home-page: https://pydglab-ws.readthedocs.io
 Keywords: dg-lab,dg-lab-v3,websocket,library,os-independent
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.asia
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,52 +24,57 @@
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   PyDGLab-WS
 </h1>
 
 <p align="center">
-  一个用于创建郊狼 DG-Lab App Socket 被控的客户端和服务端的 Python 库
+  一个用于创建郊狼 3.0 DG-Lab App Socket 控制终端和服务端的 Python 库
 </p>
 
 <p align="center">
   <a href="https://pydglab-ws.readthedocs.io">📖 完整文档</a>
 </p>
 
 <p align="center">
-  <a href="https://pypi.org/project/pydglab-ws" target="_blank">
-    <img src="https://img.shields.io/github/v/release/Ljzd-PRO/PyDGLab-WS?logo=python" alt="Version">
+  <a href="https://www.codefactor.io/repository/github/ljzd-pro/pydglab-ws">
+    <img src="https://www.codefactor.io/repository/github/ljzd-pro/pydglab-ws/badge" alt="CodeFactor" />
   </a>
 
-  <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/Ljzd-PRO/PyDGLab-WS" alt="BSD 3-Clause"/>
+  <a href="https://codecov.io/gh/Ljzd-PRO/PyDGLab-WS" target="_blank">
+      <img src="https://codecov.io/gh/Ljzd-PRO/PyDGLab-WS/branch/master/graph/badge.svg?token=VTr0LB1yWF" alt="codecov"/>
+  </a>
+
+  <a href="https://github.com/Ljzd-PRO/PyDGLab-WS/actions/workflows/codecov.yml" target="_blank">
+    <img alt="Test Result" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/PyDGLab-WS/codecov.yml">
+  </a>
+
+  <a href='https://pydglab-ws.readthedocs.io/'>
+    <img src='https://readthedocs.org/projects/pydglab-ws/badge/?version=latest' alt='Documentation Status' />
   </a>
 
   <a href="https://github.com/Ljzd-PRO/PyDGLab-WS/activity">
     <img src="https://img.shields.io/github/last-commit/Ljzd-PRO/PyDGLab-WS/master" alt="Last Commit"/>
   </a>
 
-  <a href="https://codecov.io/gh/Ljzd-PRO/PyDGLab-WS" target="_blank">
-      <img src="https://codecov.io/gh/Ljzd-PRO/PyDGLab-WS/branch/master/graph/badge.svg?token=VTr0LB1yWF" alt="codecov"/>
+  <a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/Ljzd-PRO/PyDGLab-WS" alt="BSD 3-Clause"/>
   </a>
 
-  <a href='https://pydglab-ws.readthedocs.io/'>
-    <img src='https://readthedocs.org/projects/pydglab-ws/badge/?version=latest' alt='Documentation Status' />
+  <a href="https://pypi.org/project/pydglab-ws" target="_blank">
+    <img src="https://img.shields.io/github/v/release/Ljzd-PRO/PyDGLab-WS?logo=python" alt="Version">
   </a>
 </p>
 
-> [!Warning]
-> 目前项目还在开发中，API 可能发生较多变更
-
 ## 💡 特性
 
 - 通过该库可开发 Python 程序，接入 DG-Lab App
 - 完全使用 asyncio 异步，并发执行各项操作
 - 可部署第三方终端与 Socket 服务一体的服务端，降低部署复杂度和延迟
-- 使用异步生成器、迭代器等，结合语言特性
+- 使用异步生成器、上下文管理器等，结合语言特性
 - 通过 Pydantic, 枚举 管理消息结构和常量，便于开发
 
 ### 🔧 DG-Lab App 的 Socket 被控功能支持的操作
 
 - 获取 A, B 通道强度 以及 通道强度上限 的数据更新
 - 对 A, B 通道强度进行操作，支持增加、减少、设定到指定值
 - 向 App 发送持续一段时间的波形操作数据
@@ -92,22 +97,24 @@
 
 ### 📡 搭建服务端
 
 ```python3
 import asyncio
 from pydglab_ws.server import DGLabWSServer
 
+
 async def main():
     async with DGLabWSServer("0.0.0.0", 5678, 60) as server:
         while True:
-            print(f"已连接的 WebSocket 客户端（终端/App）：{list(server.ws_client_ids)}")
+            print(f"已连接的 WebSocket 客户端（终端/App）：{list(server.uuid_to_ws.keys())}")
             print(f"已连接的本地终端：{list(server.local_client_ids)}")
             print(f"关系绑定：{server.client_id_to_target_id}")
             await asyncio.sleep(5)
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 更多演示请查看 [`examples/server.py`](examples/server.py)
 
 ### 🕹️ 搭建客户端 / 第三方终端
@@ -115,18 +122,20 @@
 当进入 `DGLabWSServer` 的异步生成器时，从 WebSocket 服务端获取 `clientId` 的操作会 **自动完成**
 
 ```python3
 import asyncio
 from websockets import ConnectionClosedOK
 from pydglab_ws import DGLabWSConnect
 
+
 def print_qrcode(_: str):
     """输出二维码到终端界面"""
     ...
 
+
 async def main():
     try:
         async with DGLabWSConnect("ws://192.168.1.161:5678") as client:
             # 获取二维码
             url = client.get_qrcode()
             print("请用 DG-Lab App 扫描二维码以连接")
             print_qrcode(url)
@@ -137,14 +146,15 @@
 
             # 从 App 接收数据更新，并进行远控操作
             async for data in client.data_generator():
                 print(f"收取到数据：{data}")
     except ConnectionClosedOK:
         print("Socket 服务端断开连接")
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 更多演示请查看 [`examples/ws_client.py`](examples/ws_client.py)
 
 ### 🕹️ 搭建与第三方终端一体的 WebSocket 服务端
@@ -156,18 +166,20 @@
 > 因此在该段代码中，终端相关的逻辑与上面的独立的 WebSocket 终端的实现基本相同。 \
 > 这种方式，省去了终端连接 WebSocket 服务端的环节，终端与 WebSocket 服务端一体，**网络延迟更低，部署更方便**。
 
 ```python3
 import asyncio
 from pydglab_ws import DGLabWSServer
 
+
 def print_qrcode(_: str):
     """输出二维码到终端界面"""
     ...
 
+
 async def main():
     async with DGLabWSServer("0.0.0.0", 5678, 60) as server:
         client = server.new_local_client()
 
         url = client.get_qrcode("ws://192.168.1.161:5678")
         print("请用 DG-Lab App 扫描二维码以连接")
         print_qrcode(url)
@@ -176,14 +188,15 @@
         await client.bind()
         print(f"已与 App {client.target_id} 成功绑定")
 
         # 从 App 接收数据更新，并进行远控操作
         async for data in client.data_generator():
             print(f"收取到数据：{data}")
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
 
 更多演示请查看 [`examples/local_client_with_server.py`](examples/server_with_local_client.py)
```

