# Comparing `tmp/orbit_component_base-1.0.51.tar.gz` & `tmp/orbit_component_base-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_base-1.0.51.tar", max compression
+gzip compressed data, was "orbit_component_base-1.0.9.tar", max compression
```

## Comparing `orbit_component_base-1.0.51.tar` & `orbit_component_base-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,28 @@
--rw-r--r--   0        0        0     1099 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/LICENSE.md
--rw-r--r--   0        0        0      307 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/README.md
--rw-r--r--   0        0        0      494 2024-05-15 15:03:18.928595 orbit_component_base-1.0.51/orbit_component_base/__init__.py
--rw-r--r--   0        0        0      206 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/orbit_component_base/cli/cli_base.py
--rw-r--r--   0        0        0     4646 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/orbit_component_base/cli/group_permissions.py
--rw-r--r--   0        0        0     3163 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/orbit_component_base/cli/permissions.py
--rw-r--r--   0        0        0     1691 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/orbit_component_base/cli/sessions.py
--rw-r--r--   0        0        0     2036 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/orbit_component_base/cli/users.py
--rw-r--r--   0        0        0     5263 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/orbit_component_base/plugin.py
--rw-r--r--   0        0        0     1963 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/orbit_component_base/schema/OrbitGroupPermissions.py
--rw-r--r--   0        0        0     1613 2024-05-10 20:37:52.492279 orbit_component_base-1.0.51/orbit_component_base/schema/OrbitPermissions.py
--rw-r--r--   0        0        0     1342 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/schema/OrbitSessions.py
--rw-r--r--   0        0        0     1413 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/schema/OrbitUsers.py
--rwxr-xr-x   0        0        0     5270 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/src/orbit_app.py
--rw-r--r--   0        0        0     8538 2024-05-13 15:21:15.533316 orbit_component_base-1.0.51/orbit_component_base/src/orbit_auth.py
--rw-r--r--   0        0        0     8515 2024-05-13 13:48:35.462230 orbit_component_base-1.0.51/orbit_component_base/src/orbit_config.py
--rw-r--r--   0        0        0     1264 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/src/orbit_database.py
--rw-r--r--   0        0        0     4302 2024-05-10 20:40:20.121347 orbit_component_base-1.0.51/orbit_component_base/src/orbit_decorators.py
--rw-r--r--   0        0        0      290 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/src/orbit_logger.py
--rw-r--r--   0        0        0      834 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/src/orbit_make_ssl.py
--rw-r--r--   0        0        0     9586 2024-05-10 20:40:20.121347 orbit_component_base-1.0.51/orbit_component_base/src/orbit_nql.py
--rw-r--r--   0        0        0     4578 2024-05-10 20:40:20.121347 orbit_component_base-1.0.51/orbit_component_base/src/orbit_nql_buffer.py
--rw-r--r--   0        0        0      895 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/src/orbit_nql_emitter.py
--rw-r--r--   0        0        0     4483 2024-05-10 20:40:20.121347 orbit_component_base-1.0.51/orbit_component_base/src/orbit_nql_session.py
--rw-r--r--   0        0        0     6977 2024-05-10 20:40:20.121347 orbit_component_base-1.0.51/orbit_component_base/src/orbit_orm.py
--rw-r--r--   0        0        0     3670 2024-05-10 20:40:20.121347 orbit_component_base-1.0.51/orbit_component_base/src/orbit_plugin.py
--rw-r--r--   0        0        0     1368 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/src/orbit_plugins.py
--rw-r--r--   0        0        0     3756 2024-05-15 15:03:18.928595 orbit_component_base-1.0.51/orbit_component_base/src/orbit_router.py
--rw-r--r--   0        0        0      629 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/src/orbit_shared.py
--rw-r--r--   0        0        0     6633 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/src/orbit_shells.py
--rw-r--r--   0        0        0       76 2024-05-10 20:37:52.496279 orbit_component_base-1.0.51/orbit_component_base/tests/test_main.py
--rw-r--r--   0        0        0       23 2024-05-19 20:28:58.406559 orbit_component_base-1.0.51/orbit_component_base/version.py
--rw-r--r--   0        0        0     1406 2024-05-19 20:28:58.402559 orbit_component_base-1.0.51/pyproject.toml
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 orbit_component_base-1.0.51/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/README.md
+-rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-07 22:18:42.405891 orbit_component_base-1.0.9/orbit_component_base/plugin.py
+-rw-r--r--   0        0        0     1290 2023-06-08 11:30:57.895776 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py
+-rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitUsers.py
+-rw-r--r--   0        0        0     1787 2023-06-08 11:31:11.007490 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitVersions.py
+-rwxr-xr-x   0        0        0     3603 2023-06-08 10:02:49.715966 orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py
+-rw-r--r--   0        0        0     6551 2023-06-08 12:34:02.238300 orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py
+-rw-r--r--   0        0        0     6878 2023-06-05 13:02:31.115557 orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py
+-rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py
+-rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py
+-rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_logger.py
+-rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py
+-rw-r--r--   0        0        0     8612 2023-06-07 11:18:34.376181 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py
+-rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py
+-rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py
+-rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py
+-rw-r--r--   0        0        0     6554 2023-06-07 23:22:03.266791 orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py
+-rw-r--r--   0        0        0     2983 2023-06-08 12:54:23.664990 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py
+-rw-r--r--   0        0        0     2148 2023-06-02 16:17:04.740333 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py
+-rw-r--r--   0        0        0     2323 2023-06-05 13:10:08.334760 orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py
+-rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py
+-rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_version.py
+-rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/tests/test_main.py
+-rw-r--r--   0        0        0       22 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/orbit_component_base/version.py
+-rw-r--r--   0        0        0     1394 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 orbit_component_base-1.0.9/PKG-INFO
```

### Comparing `orbit_component_base-1.0.51/LICENSE.md` & `orbit_component_base-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.51/orbit_component_base/schema/OrbitSessions.py` & `orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from orbit_component_base.src.orbit_orm import BaseTable, BaseCollection
 from orbit_database import SerialiserType, Doc
 from datetime import datetime
-from loguru import logger as log
 
 
 class SessionsTable (BaseTable):
+
     norm_table_name = 'sessions'
     norm_auditing = True
     norm_codec = SerialiserType.UJSON
     norm_ensure = [
         {'index_name': 'by_when'   , 'duplicates': True , 'func': '{when:14.6f}'},
-        {'index_name': 'by_sid'    , 'duplicates': False, 'func': '{sid}'},
+        {'index_name': 'by_sid'    , 'duplicates': False, 'func': '{sid}', 'force': True},
         {'index_name': 'by_ns'     , 'duplicates': True,  'func': '{ns}'},
     ]
 
     def from_sid (self, sid, transaction=None):
         self.set(self.norm_tb.seek_one('by_sid', Doc({'sid': sid}), txn=transaction))
         return self
 
     @property
     def when (self):
         return datetime.utcfromtimestamp(self._when).strftime('%Y-%m-%d %H:%M:%S')
 
 
 class SessionsCollection (BaseCollection):
+
     table_class = SessionsTable
     table_strip = ['address', 'sid', 'user_id']
-    table_methods = ['get_ids']
-    
+
     def flush (self, nsp):
         limit = Doc({'ns': nsp})
         for result in self.filter(index_name='by_ns', lower=limit, upper=limit):
             result.doc.delete()
         return self
 
     def disconnect (self):
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_app.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
-from multiprocessing import freeze_support, set_start_method
 from aiohttp import web
 from aiohttp.web_runner import GracefulExit
 from argparse import ArgumentParser
-from asyncio import sleep, create_task
+from asyncio import sleep
+from loguru import logger as log
+from multiprocessing import freeze_support, set_start_method
 from socketio import AsyncServer
 from ssl import create_default_context, Purpose
-from asyncinotify import Inotify, Mask
-import os
-import sys
-from loguru import logger as log
+from sys import argv, exit
 #
 # These can be overridden
 #
 from orbit_component_base.src.orbit_router import OrbitRouter
 from orbit_component_base.src.orbit_config import OrbitConfig
 from orbit_component_base.src.orbit_database import OrbitDatabase
 from orbit_component_base.src.orbit_logger import OrbitLogger
@@ -41,80 +39,49 @@
         'cors_allowed_origins': '*'
     }
 
     def __init__ (self, app=None):
         if app:
             self.APPLICATION = app
         self._router = None
-        self._plugins = []
 
     async def startup (self, app=None):
-        log.debug(f'Orbit Application {self.APPLICATION} Starting up')
         if world.conf.sio_debug:
             self.SERVER_PARAMS['logger'] = self.LOGGER()
-        if world.conf.engineio_debug:
-            self.SERVER_PARAMS['engineio_logger'] = True
         sio = world.sio = AsyncServer(**self.SERVER_PARAMS)
         odb = self.MAINDB().open()
         
         for plugin in Plugins('Plugin'):
             plugin = plugin.Plugin(odb=odb).open().register(sio)
             sio.attach(app, socketio_path=plugin.ns)
             self._router.add_namespace(plugin.NAMESPACE)
-            self._plugins.append(plugin)
-        for plugin in Plugins('Tasks'):
-            await plugin.Tasks().open(odb, world.args).process()
-        if world.args.dev:
-            log.debug('Starting file watched, will auto-restart on changes ...')
-            create_task(self.watch_files())
-        
-    async def watch_files (self):
-        try:
-            with Inotify() as inotify:
-                base = os.environ.get('PYENV_VIRTUAL_ENV') + f'/lib/python{sys.version_info.major}.{sys.version_info.minor}/site-packages'
-                inotify.add_watch(base, Mask.MODIFY | Mask.CREATE | Mask.DELETE | Mask.MOVE)
-                for path, _, _ in os.walk(base):
-                    name = path.split('/')[-1]
-                    if name.startswith('orbit_'):
-                        inotify.add_watch(path, Mask.MODIFY | Mask.CREATE | Mask.DELETE | Mask.MOVE)
-                async for event in inotify:
-                    log.warning('<< Detected a filesystem change, waiting for 3s >>')
-                    await sleep(3)
-                    log.warning('<< Initiating a program restart >>')
-                    os.execv(sys.executable, ['python'] + sys.argv)
-        except Exception as e:
-            log.exception(e)
 
     async def shutdown(self, app=None):
-        count = 0
-        for socket in world.sio.manager.server.eio.sockets.values():
-            await socket.close()
-            count += 1
-        log.debug(f'Shutdown complete, closed {count} websocket connections')
-        await log.complete()
+        await sleep(1)
         raise GracefulExit()
 
     def run (self):
         set_start_method('spawn')
         freeze_support()
+       
+        world.conf = self.CONFIG(self.APPLICATION).open()       
 
-        parser = ArgumentParser()        
+        parser = ArgumentParser()
         for plugin in Plugins('Args'):
             plugin.Args(parser=parser).setup()
-        world.args = parser.parse_args()
-        world.conf = self.CONFIG(self.APPLICATION).open()
-               
+        world.args = parser.parse_args()        
+
         if not world.args.run:
-            odb = self.MAINDB().open(auditing=False)
+            odb = self.MAINDB().open()
             for plugin in Plugins('Plugin'):
                 plugin = plugin.Plugin(odb=odb).open(nql=False)
             for plugin in Plugins('Args'):
                 plugin.Args(parser=parser).open(odb, world.args).process()
             print('Please add "run" if you wish to launch the application')
-            sys.exit(0)
+            exit()
   
         self._router = router = self.ROUTER()
         app = router.application()
         app.on_startup.append(self.startup)
         app.on_shutdown.append(self.shutdown)
         try:
             if world.conf.secure:
@@ -131,8 +98,10 @@
                 web.run_app(
                     app,
                     host=world.conf.host,
                     port=world.conf.port)                   
         except Exception as e:
             log.exception(e)
         finally:
+            print()
+            log.info('Shutdown')
             raise GracefulExit()
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_auth.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from base64 import b64decode, b64encode
 from random import choice
 from orbit_database import Doc
 from datetime import datetime
 from orbit_component_base.schema.OrbitUsers import UsersCollection, UsersTable
 from orbit_component_base.schema.OrbitSessions import SessionsTable
 from orbit_component_base.src.orbit_shared import world
-from aiohttp import ClientSession, TCPConnector
-import ssl
 
 
 class OrbitAuth:
 
     CHARACTERS = '23456789ABCDEFGHJKLMNPQRSTUVWXYZ'
     CODE_SIZE = 8
     EXPIRY_TIME = 3600
@@ -34,15 +32,15 @@
 
     def activate_user(self, user):
         user.update({'active': True, 'code': None}).save()
         return {'ok': True, 'validate': False}
 
     def activate_session (self, user_id, auth, session):
         SessionsTable().from_doc(Doc({
-            # 'user_id'   : user_id,
+            'user_id'   : user_id,
             'when'      : datetime.now().timestamp(),
             'vendor'    : auth.get('vendor', 'unknown'),
             'platform'  : auth.get('platform', 'unknown'),
             'language'  : auth.get('language', 'unknown'),
             'address'   : session['address'],
             'host_id'   : session['host_id'],
             'sid'       : self._sid,
@@ -90,56 +88,20 @@
             host_id = auth.get('host_id')
             secret = auth.get('secret')
             if host_id != session['host_id']:
                 return {'ok': False, 'error': f'No such hostId: {host_id}'}
             cipher = PKCS1_OAEP.new(self._keyPair, SHA256)
             user_id = cipher.decrypt(b64decode(secret)).decode()
             user = UsersTable().from_key(host_id)
-            
-            if world.conf.authentication == 'cryptoloop':
-                meta = auth.get('metadata')
-                context = ssl._create_unverified_context()
-                conn = TCPConnector(ssl=context)
-                async with ClientSession(connector=conn) as web:
-                    url = meta.get("url")
-                    log.success(f'URL={url}')
-                    async with web.post(f'{url}', data=meta) as resp:
-                        if resp.status == 200:
-                            log.success(f'Validated new user [{host_id}]')
-                            uuid = meta.get('uuid')
-                            if user.isValid:
-                                if not user._uuids:
-                                    user._uuids = []
-                                if uuid not in user._uuids:
-                                    user.update({'uuids': user._uuids + [uuid]}).save()
-                            else:
-                                UsersTable().from_doc(Doc({
-                                    'user_id': user_id,
-                                    'active': True,
-                                    'code': None,
-                                    'uuids': [uuid] if uuid else [],
-                                    'tries': 0,
-                                }, oid=host_id)).append()
-
-                            session['activated'] = True
-                            session['perm'] = user._perm
-                            await save_session(self._sid, session)    
-                            self.activate_session(user._user_id, auth, session)
-                            return {'ok': True, 'validate': False}
-                        else:
-                            log.error(f'VALIDATE ERROR : {resp.status}')
-                log.error("DROP THRU")
-                return {'ok': True, 'validate': True}
-
             if user.isValid:
                 if user._user_id == user_id:
                     if user._active or world.conf.authentication == 'autoenroll':
                         session['activated'] = True
                         session['perm'] = user._perm
-                        # log.debug(f'Save: {self._sid} / {self._ns} => {session}')
+                        log.debug(f'Save: {self._sid} / {self._ns} => {session}')
                         try:
                             await save_session(self._sid, session)
                             self.activate_session(user._user_id, auth, session)
                         except Exception as e:
                             log.error(e)
                             
                         return {'ok': True, 'validate': False}
@@ -157,30 +119,30 @@
                     'user_id': user_id,
                     'active': activate,
                     'code': None if activate else self.generate_auth_code(),
                     'tries': 0,
                 }, oid=host_id)).append()
                 self.activate_session(user._user_id, auth, session)
                 return {'ok': True, 'validate': not activate}
+
         except Exception as e:
             log.exception(e)
             return {'ok': False, 'error': str(e)}
 
     async def hello(self, auth, get_session, save_session):
         session = await get_session(self._sid)
         try:
             text = f'-----BEGIN RSA PUBLIC KEY-----\n{auth["pubKey"]}\n-----END RSA PUBLIC KEY-----'
             session['pubkey'] = RSA.importKey(text)
             session['host_id'] = auth['hostId']
-            # log.warning("<< SAVE SESSION >>")
             await save_session(self._sid, session)
-            # log.warning(f'HELLO PROTOCOL: sid={self._sid} addr={session["address"]} hostId={auth["hostId"]}')
+            log.warning(f'HELLO PROTOCOL: sid={self._sid} addr={session["address"]} hostId={auth["hostId"]}')
             cipher = PKCS1_OAEP.new(session['pubkey'], SHA256)
             return {
                 'ok': True,
                 'pubKey': b"".join(self._keyPair.public_key().export_key().split(b'\n')[1:-1]),
                 'pemKey': self._keyPair.public_key().export_key(),
                 'secret': b64encode(cipher.encrypt('THESECRET'.encode('ascii'))).decode('ascii'),
             }
         except Exception as e:
             log.exception(e)
-            return {'ok': False, 'error': str(e)}
+            return {'ok': False, 'error': str(e)}
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_config.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,35 +2,19 @@
 
 from configparser import ConfigParser
 from pathlib import Path
 from datetime import datetime
 from loguru import logger as log
 from orbit_component_base.src.orbit_shared import world
 from platform import system
-from cryptography.fernet import Fernet, InvalidToken
-
-
-class Section:
-
-    def __init__ (self, name):
-        self._name = name
-
-    def __getattr__(self, key):
-        try:
-            return super().__getattr__(key)
-        except AttributeError:
-            return None
 
 
 class OrbitConfig:
 
     BASE_authentication = 'autoenroll'
-    BASE_name = 'localhost'
-    BASE_network_host = '127.0.0.1'
-    BASE_network_port = '8445'
 
     @property
     def path (self):            return Path(self._conf.get('BASE', 'path')).expanduser()
 
     @property
     def code (self):            return Path(self._conf.get('BASE', 'code')).expanduser()
 
@@ -58,19 +42,15 @@
     @property
     def engineio_debug (self):  return self._conf.getboolean('NETWORK', 'engineio_debug')
 
     @property
     def vite_port (self):       return self._conf.getint('DEV', 'vite_port')
 
     @property
-    def debug (self):           return self._conf.getboolean('DEV', 'debug')
-
-    @property
-    def make_keys (self):       
-        return self._conf.get('DEV' if world.args.dev else 'BASE', 'make_keys')
+    def make_keys (self):       return self._conf.get('TOOLS', 'make_keys')
 
     @property
     def database (self):        return self.mkpath('DATA', 'database')
 
     @property
     def tmp (self):             return self.mkpath('DATA', 'tmp')
 
@@ -82,17 +62,14 @@
 
     @property
     def logs (self):             return self.mkpath('DATA', 'logs')
 
     @property
     def writemap (self):        return self._conf.get('DATA', 'writemap')
 
-    @property
-    def token (self):           return self._conf.get('ENCRYPTION', 'token').encode()
-
     def __init__ (self, application):
         self._appl = application
         self._path = Path('~/.local/' + application).expanduser()
         self._file = (self._path / 'config.ini').expanduser()
         self._conf = None
         self._changed = False
 
@@ -126,69 +103,46 @@
         if not value:
             return None
         if value[0] in './~':
             p = Path(self._conf.get(section, option)).expanduser()
         else:
             p = path / self._conf.get(section, option)
         try:
-            if not world.args or not world.args.dev:
-                p.mkdir(parents=True, exist_ok=True)
+            p.mkdir(parents=True, exist_ok=True)
         except FileExistsError:
             pass
         return p
 
     def open (self):
         self._path.mkdir(parents=True, exist_ok=True)
         self._conf = ConfigParser()
         self._conf.read(self._file.as_posix())
-        #
-        #   V2, generate read-only object
-        #
-        for section in self._conf.sections ():
-            local_section = Section (section)
-            for key in self._conf[section]:
-                setattr (local_section, key, self._conf[section][key])
-            setattr (self, section, local_section)
-        #
-        #
-        #
-        for section in ['BASE', 'NETWORK', 'TOOLS', 'DATA', 'SSL', 'DEV', 'ENCRYPTION']:
+        for section in ['BASE', 'NETWORK', 'TOOLS', 'DATA', 'SSL', 'DEV']:
             if section not in self._conf.sections():
                 self._conf.add_section(section)
                 self._changed = True
-                
-        if system() == 'Darwin':
-            code_path = f'/Applications/{self._appl}.app/Contents/Resources/'
-        else:
-            if world.args and world.args.dev:
-                code_path = f'~/{self._appl}/server'
-            else:
-                code_path = f'/opt/{self._appl}'
-
+        code_path = f'/Applications/{self._appl}.app/Contents/Resources/' if system() == 'Darwin' else f'/opt/{self._appl}'
         self._option('BASE', 'path', f'~/.local/{self._appl}', 'base location for this application')
         self._option('BASE', 'code', code_path, "where the application's code is located")
         self._option('BASE', 'authentication', self.BASE_authentication, 'the default type of authentication (autoenroll/secure)')
-        self._option('BASE', 'make_keys', f'{code_path}/scripts/make_keys.sh', 'the folder we store our make_keys script in')        
-        self._option('SSL', 'name', self.BASE_name, 'the host name (CN) for our SSL certificate')
+        self._option('SSL', 'name', 'localhost', 'the host name (CN) for our SSL certificate')
         self._option('SSL', 'ssl', 'ssl', 'the folder to store SSL files in')
         self._option('SSL', 'secure', 'true', 'whether to use SSL or not')
-        self._option('NETWORK', 'host', self.BASE_network_host, 'the host to expose the server on, use "0.0.0.0" for a local network')
-        self._option('NETWORK', 'port', self.BASE_network_port, "the port to expose the server on")
+        self._option('NETWORK', 'host', '127.0.0.1', 'the host to expose the server on, use "0.0.0.0" for a local network')
+        self._option('NETWORK', 'port', '8445', "the port to expose the server on")
         self._option('DEV', 'vite_port', '5173', 'the port to run "vite" on')
-        self._option('DEV', 'debug', 'false', 'whether debugging is enabled or not')
-        self._option('DEV', 'make_keys', 'scripts/make_keys.sh', 'the folder we store our make_keys script in')
         self._option('NETWORK', 'sio_debug', 'false', 'SIO debugging')
         self._option('NETWORK', 'engineio_debug', 'false', 'AIO debugging')
         self._option('DATA', 'database', 'orbit_database', 'the path name of the folder to store data in')
         self._option('DATA', 'tmp', 'tmp', 'the path name of a temporary folder')
         self._option('DATA', 'templates', 'templates', 'the path name of the folder to store templates in')
         self._option('DATA', 'web', 'web', 'the path name of the folder to store web assets for in production mode')
         self._option('DATA', 'logs', 'logs', 'the path name of the folder to store logs in')
         self._option('DATA', 'writemap', 'true', 'whether to use WRITEMAP on the database')
-        self._option('ENCRYPTION', 'token', Fernet.generate_key().decode(), 'a default field encryption key for the database [back this up!]')
+        self._option('TOOLS', 'make_keys', 'scripts/make_keys.sh', 'the folder we store our make_keys script in')
         if self._changed:
             with open(self._file.as_posix(), 'w') as configfile:
                 self._conf.set('DEFAULT', 'updated', datetime.now().isoformat())
                 self._conf.write(configfile)
         self.setup_logging()                
         return self
 
@@ -203,8 +157,7 @@
     print("Port           =", conf.port)
     print("sio_debug      =", conf.sio_debug)
     print("engineio_debug =", conf.engineio_debug)
     print("make_keys      =", conf.make_keys)
     print("database       =", conf.database)
     print("templates      =", conf.templates)
     print("web            =", conf.web)
-    print("token          =", conf.token)
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_database.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     PATH = 'default'
     FILE = None
     MAX_DATABASE_SIZE = 64
     COLLECTIONS = []
     CONFIG = {
         'map_size': 1024 * 1024 * 1024 * 64,
         'reindex': False,
+        'auditing': True,
         'writemap': True
     }
 
     @property
     def real_path (self):
         return self._floc
     
     def __init__ (self):
         self._path = self.PATH
         self._file = self.FILE
         self._config = self.CONFIG
         self._floc = None
        
-    def open(self, auditing=True):
-        self.CONFIG['auditing'] = auditing
+    def open(self):
         if self._path == 'default':
             path = world.conf.database
         elif path and self._file:
             path = Path(self._path) / self._file
         else:
             raise Exception(f'bad database specification: {self._path} / {self._file}')
         if not path.exists():
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_make_ssl.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_nql.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from loguru import logger as log
 from orbit_database import Doc, AuditEntry
 from orbit_component_base.src.orbit_nql_session import Session
 from orbit_component_base.src.orbit_nql_buffer import InputBuffer, OutputBuffer
 from orbit_component_base.src.orbit_nql_emitter import OrbitEmitter
 from orbit_component_base.src.orbit_shared import world
 
-DEBUG = False
-
 
 class NQL:
 
     def __init__(self, emit, ns):
         self._emit = emit
         self._ns = ns
         self._methods = {}
@@ -27,34 +25,25 @@
         return self
 
     def register(self, method_name, method):
         if not method:
             log.error(f'[programming error] unable to find routine "{method_name}" to publish')
         else:
             self._methods[method_name] = method
-            if DEBUG:
-                log.success(f'Register: {method_name} for {self._ns}')
+            log.success(f'Register: {method_name} for {self._ns}')
 
-    def connect(self, sid, session):
-        if DEBUG:
-            log.error(f'Connect: {sid} => {self._ns}')
-        self._sessions[sid] = Session(session)
+    def connect(self, sid):
+        self._sessions[sid] = Session()
         self._sessions[sid].clear()
-        
-        # log.success(f'[connect] {self._sessions.keys()}')
 
     def disconnect(self, sid):
         if sid in self._sessions:
             del self._sessions[sid]
-        if DEBUG:
-            log.success(f'[disconnect] {self._sessions.keys()}')
 
     def call(self, sid, params):
-        if DEBUG:
-            log.success(f'[call] {self._sessions.keys()}')
         session = self._sessions[sid]
         model_name = params.get('model')
         label_name = params.get('label')
         if not model_name:
             return {'ok': False, 'error': f'no model for "{params}"'}
         if not label_name:
             return {'ok': False, 'error': f'no label for "{params}"'}
@@ -126,25 +115,24 @@
                     # 'dref': dref
                 }
             else:
                 if 'ids' in result:
                     # result['dref'] = dref
                     # session.invalid_list[model_name] |= set(old_set) - set(result['ids'])
                     return result
-                # log.debug("#3")
+                log.debug("#3")
                 return {
                     'ok': True,
                     'ids': [],
                     'data': [],
                     # 'dref': dref
                 }
 
     def drop(self, sid, params):
-        if DEBUG:
-            log.warning(f"DROP: {params}")
+        # log.warning(f"DROP: {params}")
         session = self._sessions[sid]
         model_name = params.get('model')
         label_name = params.get('label')
         if not model_name:
             return {'ok': False, 'error': f'no model for "{params}"'}
         if not label_name:
             return {'ok': False, 'error': f'no label for "{params}"'}
@@ -166,73 +154,62 @@
         try:
             for doc in docs:
                 await self._emitter.emit(doc)
         except Exception as e:
             log.exception(e)
 
     async def update(self, model, docs):
-        # log.error('#1')
         if docs:
-            # log.error('#2')
             await self._input_buffer.enqueue(model, docs)
         
     async def update_next (self, model, docs):
-        # log.warning(f'Mode={model} Docs={docs}')
         try:
             for sid, session in dict(self._sessions).items():
                 if model not in session.cache_ids:
-                    # log.warning(f'[{model} not cached]')
                     continue
                 for doc in docs:
                     if doc._e != AuditEntry.DELETE.value:
                         session.cache_data[model].discard(doc._o if isinstance(doc, Doc) else doc)
                 for label in dict(session.cache_ids[model]):
-                    # for doc in docs:
-                        # log.critical(f'Model={model} Label={label} Docs={doc.doc}')
                     params = dict(session.cache_params[model][label])
                     old_set = set(session.cache_ids[model].get(label, []))
                     count = params.get('count', 20)
                     if len(old_set) > count:
                         params['count'] = len(old_set)
                     if params.get('next'):
                         del params['next']
                     try:
                         cls, fn = self._methods.get(params.get('method'))
                     except TypeError:
                         fn = self._methods.get(params.get('method'))
                         cls = None
                     if not fn:
-                        log.critical("[SKIP]")
                         continue
                     try:
                         if cls:
+                            # log.warning(f"Calling # 1: {sid} {params}")
                             result = fn(cls, session, params)
-                            # log.warning(f"Calling # 1: {sid} {params} => {result}")
                         else:
-                            # log.warning(f"Calling # 2: {fn} {params}")
+                            log.warning(f"Calling # 2: {fn} {params}")
                             result = fn(session, params)
                     except Exception as e:
                         log.error(e)
                         return
-                    response = {'sid': sid}
                     if isinstance(result, tuple):
                         ids, data = result
                     else:
                         ids = result.get('ids')
                         data = result.get('data')
-                        response['meta'] = result.get('meta', {})
+                    response = {'sid': sid}
                     if set(ids) != old_set:
                         response['ids'] = ids
                     if data:
                         response['data'] = data
-                    # if 'ids' in response or 'data' in response:
-                    # log.error(f'out> {sid} {model} {label} {response}')
-                    await self._output_buffer.enqueue(sid, model, label, response)
-                    # else:
-                    #     log.error(f'out> {sid} no output :: {response}')
+                    if 'ids' in response or 'data' in response:
+                        await self._output_buffer.enqueue(sid, model, label, response)
                 dref = session.verify(model)
                 if dref:
                     # log.error(f'Sending invalidate: {sid} => {model} => {dref}')
                     await self._output_buffer.enqueue(sid, model, '_invalidate', dref)
         except Exception as e:
             log.exception(e)
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_nql_buffer.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,72 +9,50 @@
     default_interval = 1.0
 
     def __init__(self, emitter):
         self._emitter = emitter
         self._flashpoints = {}
 
     async def run (self, model, flashpoint, delay=0):
-        # log.success(f"RUN> {delay}")
         await async_sleep(delay)
-        #
         output = []
-        #
-        #   Isolate meta and insert into output
-        #
-        for label in flashpoint.get('meta', {}):
-            response = {
-                'sid': flashpoint['sid'],
-                'meta': flashpoint['meta'][label]
-            }
-            output.append((f'{model}_{label}', response))
-        #
-        #   Add data items
-        #
         for label in flashpoint.get('data'):
             response = {}
             if isinstance(flashpoint['data'][label], list):
                 response['data'] = flashpoint['data'][label]
             else:
                 response['data'] = [v for v in flashpoint['data'][label].values()]
+                
             if response['data']:
                 response['sid'] = flashpoint['sid']
                 flashpoint['data'].update({label: {}})
                 output.append(((f'{model}_{label}', response)))
-        #
-        #   Reset trigger and flush output
-        #
+        
         flashpoint['trigger'] = False
         for entry in output:
             await self._emitter.emit(entry)
+        
                 
     async def enqueue (self, sid, model, label, response):
-        # log.warning(f'ENQ> sid={sid} model={model} label={label} response={response}')
         try:
             if 'ids' in response:
-                # log.warning(f'ENQ> emit={model}_{label}')
                 await self._emitter.emit((f'{model}_{label}', response))
                 return
             key = f'{sid}_{model}'
             if key not in self._flashpoints:
                 self._flashpoints[key] = {'time': 0, 'trigger': None, 'sid': sid, 'data': {}}
             flashpoint = self._flashpoints[key]
             if label not in flashpoint['data']:
                 flashpoint['data'][label] = {}
             
             if isinstance(response, dict):
-                # log.warning("#1")
-                for item in response.get('data', []):
+                for item in response['data']:
                     flashpoint['data'][label][item['_id']] = item
-                if 'meta' in response:
-                    # log.warning("#2")
-                    flashpoint['meta'] = {label: response['meta']}
             else:
                 flashpoint['data'][label] = response
-
-            # log.warning(f'Flashpoint: {flashpoint}')
                 
             if flashpoint['trigger']:
                 return
             flush = flashpoint['time']
             delay = 0 if time() > flush else flush - time()
             if not delay:
                 flashpoint['time'] = time() + self.default_interval
@@ -98,23 +76,17 @@
         docs = flashpoint.get('docs', [])
         # log.success(f'FLUSH: {model} => {len(docs)}')
         flashpoint.update({'docs': [], 'trigger': False})
         await self._next(model, docs)
 
     async def enqueue (self, model, docs):
         # log.debug(f'incoming: {model} => {len(docs)}')
-        # log.info(f'ENQ> model={model}')
         if model not in self._flashpoints:
             self._flashpoints[model] = {'time': 0, 'trigger': False, 'docs': []}
         flashpoint = self._flashpoints[model]
-        # if isinstance(docs, list):
-            # for doc in docs:
-                # log.info(f"Flash: {doc.doc}")
-        # else:
-            # log.info(f"Flash: {docs.doc}")
         flashpoint['docs'] += docs
         if flashpoint['trigger']:
             # log.warning('triggered')
             return
         flush = flashpoint['time']
         delay = 0 if time() > flush else flush - time()
         if not delay:
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_nql_emitter.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_nql_session.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from collections import defaultdict
 from loguru import logger as log
 from orbit_database import Doc
 
 
 class Session:
 
-    def __init__(self, session):
+    def __init__(self):
         self.clear()
-        self._session = session
 
     def has_context(self, params):
         return self.context_ids.get(params.get('model'), {}).get(params.get('label')) is not None
 
     def context(self, params):
         return self.context_ids.get(params.get('model'), {}).get(params.get('label'))
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_orm.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,19 +79,14 @@
     def clone(self):
         self.oid = None
         return self
 
     def lookup_by_key(self, index_name, doc, transaction=None):
         self.set(self.norm_tb.seek_one(index_name, doc, txn=transaction))
         return self
-    
-    def resolve_by_key(self, index_name, limit, transaction=None):
-        for result in self.norm_tb.filter(index_name, lower=limit, upper=limit, txn=transaction):
-            return self.set(result.doc)
-        return self
 
 
 class BaseCollection:
 
     _dbh = None
     _nql = None
     _api = {}
@@ -145,16 +140,14 @@
             for method in self.table_methods:
                 nql.register(f'api_{self.table_class.norm_table_name}_{method}' , (self.__class__, getattr(self.__class__, method)))
             self.table_class.norm_tb.watch(callback=self.callback)
             for fn in self._api.keys():
                 nql.register(fn, self._api[fn])
 
     async def callback(self, docs):
-        # for doc in docs:
-        #     log.success(f'Callback={doc.doc}')
         try:
             await self._nql.update(self.table_class.norm_table_name, docs)
         except Exception as e:
             log.exception(e)
        
     def filter(self, *args, **kwargs):
         try:
@@ -165,17 +158,14 @@
                 return []
         except Exception as e:
             log.exception(e)
 
     def records(self, transaction=None):
         return self.table_class.norm_tb.records()
 
-    def delete(self, keys, transaction=None):
-        return self.table_class.norm_tb.delete(keys, txn=transaction)
-
     def empty(self, transaction=None):
         if self.table_class.norm_tb is not None:
             return self.table_class.norm_tb.empty(txn=transaction)
         return None
 
     def drop(self, index_name, transaction=None):
         return self.table_class.norm_tb.drop(index_name, txn=transaction)
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_router.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,97 @@
-from aiohttp import web
-from orbit_component_base.src.orbit_shared import world
-from aiohttp import web, ClientSession, TCPConnector, client_exceptions
-from aiohttp.web_exceptions import HTTPNotFound
+import functools
 from loguru import logger as log
+from asyncio import sleep
+from time import time
+from os import times
 
-routes = web.RouteTableDef()
 
-
-class OrbitRouter:
-
-    def __init__(self, context=None, args=None):
-        self._context = context
-        self._args = args
-        self._namespaces = set([])
-
-    async def redirect(self, request):
+async def run_and_log(func, args, kwargs):
+    try:
+        tstart = time()
+        cstart = times()
         try:
-            if str(request.rel_url).startswith('/assets/'):
-                path = str(request.rel_url)[1:]
-                headers = {
-                    'Cache-Control': 'max-age=0, s-maxage=0',
-                    'Access-Control-Allow-Origin': '*'
-                }
-                origin = f"https://{world.conf.name}:{world.conf.vite_port}"
-                headers['Origin'] = origin
-                fullpath = world.conf.web / path
-                try:
-                    response =  web.FileResponse(fullpath.as_posix(), headers=headers)
-                    return response
-                except FileNotFoundError:
-                    log.error(f'File not found: {fullpath.as_posix()}')
-                    return ''
-                except Exception as e:
-                    log.error(e)
-                    return ''
-            if not world.conf.web or world.args.dev:
-                async with ClientSession(connector=TCPConnector(verify_ssl=False), skip_auto_headers=['accept-encoding']) as session:
-                    origin = f"https://{world.conf.name}:{world.conf.vite_port}"
-                    try:
-                        async with session.get(f'{origin}{request.rel_url}') as resp:
-                            headers = dict(resp.headers)
-                            headers['Origin'] = origin
-                            headers['Cache-Control'] = 'max-age=0, s-maxage=0'
-                            return web.Response(body=await resp.content.read(), status=resp.status, headers=headers)
-                    except FileNotFoundError:
-                        log.error(f'File not found2: {fullpath.as_posix()}')
-                        return ''
-                    except client_exceptions.ClientConnectorError as e:
-                        log.error(f'VITE server is down on: {origin}')
-                        return ''
-            else:
-                path = (request.path if request.path != '/' else 'index.html').strip('/')
-                headers = {'Cache-Control': 'max-age=0, s-maxage=0'}
-                fullpath = world.conf.web / path
-                return web.FileResponse(fullpath.as_posix(), headers=headers)
-        except FileNotFoundError:
-            log.error(f'File not found3: {fullpath.as_posix()}')
-            return ''
+            output = await func(*args, **kwargs)
         except Exception as e:
             log.exception(e)
-        return ''
-
-    @web.middleware
-    async def default_route(self, request, handler, *args):
+            return {'ok': False, 'error': str(e)}
+        tend = time()
+        cend = times()
+        real_time = (tend - tstart) * 1000
+        sys_time = (cend[0] - cstart[0]) * 1000
+        usr_time = (cend[1] - cstart[1]) * 1000
+        new_args = []
+        for arg in args:
+            if isinstance(arg, str):
+                if len(arg) > 20:
+                    arg = arg[:20] + '...'
+            elif isinstance(arg, bytes):
+                if len(arg) > 20:
+                    arg = arg[:20] + b'...'
+            new_args += [arg]
+        if len(new_args) > 2:
+            params = new_args[2]
+            if isinstance(params, dict):
+                log.log('RPC', f'{func.__name__} => {params.get("method")} :: real={real_time:.0f}ms, sys={sys_time:.0f}ms usr={usr_time:.0f}ms repeat@{1000/real_time:.0f}/sec')
+                return output
+        log.log('RPC', f'{func.__name__} :: real={real_time:.0f}ms, sys={sys_time:.0f}ms usr={usr_time:.0f}ms repeat@{1000/real_time:.0f}/sec') ## :: {new_args}')
+        return output
+    except Exception as e:
+        log.exception(e)
+
+
+def navGuard(func):
+    @functools.wraps(func)
+    async def wrapper(*args, **kwargs):
         try:
-            ns = request.path.strip('/').split('/')[0]
-            return await (handler(request) if ns in self._namespaces else self.redirect(request))
-        except HTTPNotFound:
-            if world.conf.debug:
-                log.debug (f'debug: 404 Not Found: {request.path}')
-            return web.Response(body='404 Not Found', status=404)
+            retrying = False
+            while True:
+                try:
+                    session = await args[0].get_session(args[1])
+                except KeyError:
+                    log.warning('<< disconnected dead session >>')
+                    return {'ok': False, 'error': 'Server was restarted'}
+                except Exception as e:
+                    log.exception(e)
+                    raise
+                if not session.get('activated', False):
+                    if not retrying:
+                        log.debug(f'<< waiting for authentication >> {args[1]}')
+                        retrying = True
+                    await sleep(0.1)
+                    continue
+                return await run_and_log(func, args, kwargs)
         except Exception as e:
             log.exception(e)
+    return wrapper
 
-    def application(self):
-        app = web.Application(client_max_size=1024*1024*1024, middlewares=[self.default_route])
-        if world.conf.debug:
-            log.debug(f'debug: Installing routes: {routes}')
-            for route in routes:
-                log.debug(f'debug: -> {route}')
-        app.add_routes(routes)
-        return app
-    
-    def add_namespace (self, nsp):
-        self._namespaces.add(nsp)
+
+def apiSentry(permissions):
+    def navGuard(func):
+        @functools.wraps(func)
+        async def wrapper(*args, **kwargs):
+            try:
+                retrying = False
+                while True:
+                    try:
+                        session = await args[0].get_session(args[1])
+                        if session.get('perm') not in permissions:
+                            error = f'insufficient permissions, wanted: {permissions}, got: {session.get("perm")}'
+                            log.error(error)
+                            return { 'ok': False, 'error': error }
+                    except KeyError:
+                        log.warning('<< disconnected dead session >>')
+                        return {'ok': False, 'error': 'Server was restarted'}
+                    except Exception as e:
+                        log.exception(e)
+                        raise
+                    if not session.get('activated', False):
+                        if not retrying:
+                            log.debug(f'<< waiting for authentication >> {args[1]}')
+                            retrying = True
+                        await sleep(0.1)
+                        continue
+                    return await run_and_log(func, args, kwargs)
+            except Exception as e:
+                log.exception(e)
+        return wrapper
+    return navGuard
```

### Comparing `orbit_component_base-1.0.51/orbit_component_base/src/orbit_shared.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.51/pyproject.toml` & `orbit_component_base-1.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-base"
-version = "1.0.51"
+version = "1.0.9"
 description = "Orbit Framework - base component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "orbit_component_base"}]
 include = ['README.md', 'LICENSE.md']
 keywords = ['orbit-framework', 'orbit-component', 'orbit-database']
@@ -23,23 +23,21 @@
 
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-component-base"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-component-base/-/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-socketio = "^5"
-orbit-database = "^1.0"
-loguru = "^0.7"
-ujson = "^5.7"
-pycryptodome = "^3.18"
-tqdm = "^4"
-aiohttp = "^3"
-rich = "^13"
-asyncinotify = "^4"
+python-socketio = "^5.8.0"
+orbit-database = "^0.99.91"
+loguru = "^0.7.0"
+ujson = "^5.7.0"
+pycryptodome = "^3.18.0"
+tqdm = "^4.65.0"
+aiohttp = "^3.8.4"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.3.1"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `orbit_component_base-1.0.51/PKG-INFO` & `orbit_component_base-1.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: orbit-component-base
-Version: 1.0.51
+Version: 1.0.9
 Summary: Orbit Framework - base component
 Home-page: https://gitlab.com/madpenguin/orbit-component-base
 License: MIT
 Keywords: orbit-framework,orbit-component,orbit-database
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: aiohttp (>=3,<4)
-Requires-Dist: asyncinotify (>=4,<5)
-Requires-Dist: loguru (>=0.7,<0.8)
-Requires-Dist: orbit-database (>=1.0,<2.0)
-Requires-Dist: pycryptodome (>=3.18,<4.0)
-Requires-Dist: python-socketio (>=5,<6)
-Requires-Dist: rich (>=13,<14)
-Requires-Dist: tqdm (>=4,<5)
-Requires-Dist: ujson (>=5.7,<6.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: orbit-database (>=0.99.91,<0.100.0)
+Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
+Requires-Dist: python-socketio (>=5.8.0,<6.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-component-base
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-component-base
 Description-Content-Type: text/markdown
 
 # Orbit Component :: Base : Server
 
 #### This is the base compoent for the orbit framework back-end. It's required for all other components and for the framework itself, assuming you want the framework to do something useful.
```

