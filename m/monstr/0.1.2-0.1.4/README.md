# Comparing `tmp/monstr-0.1.2.tar.gz` & `tmp/monstr-0.1.4.tar.gz`

## Comparing `monstr-0.1.2.tar` & `monstr-0.1.4.tar`

### file list

```diff
@@ -1,63 +1,86 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 monstr-0.1.2/requirements.txt
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 monstr-0.1.2/setup.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/basic_usage.py
--rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/create_test_environment.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/keys.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/persist_test.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/post_text.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/print_text_notes.py
--rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/query.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/republish.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/simple_bot.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 monstr-0.1.2/examples/view_profile.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/__init__.py
--rw-r--r--   0        0        0     9117 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/encrypt.py
--rw-r--r--   0        0        0    11714 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/entities.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/exception.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/inbox.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/signing.py
--rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/channels/__init__.py
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/channels/channel.py
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/channels/event_handlers.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/channels/persist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/client/__init__.py
--rw-r--r--   0        0        0    41383 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/client/client.py
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/client/event_handlers.py
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/client/messaging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/data/__init__.py
--rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/data/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/db/__init__.py
--rw-r--r--   0        0        0    15720 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/db/db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/__init__.py
--rw-r--r--   0        0        0    18381 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/event.py
--rw-r--r--   0        0        0    18270 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/event_handlers.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/expire.py
--rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/persist.py
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/persist_memory.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/persist_postgres.py
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/persist_sqlite.py
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/event/persist_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/ident/__init__.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/ident/alias.py
--rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/ident/event_handlers.py
--rw-r--r--   0        0        0    30307 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/ident/persist.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/ident/persist_test.py
--rw-r--r--   0        0        0    27579 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/ident/profile.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/relay/__init__.py
--rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/relay/accept_handlers.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/relay/exceptions.py
--rw-r--r--   0        0        0    27356 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/relay/relay.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/relay/relay_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/settings/__init__.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/settings/handler.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/settings/persist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/spam_handlers/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 monstr-0.1.2/src/monstr/spam_handlers/spam_handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 monstr-0.1.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 monstr-0.1.2/LICENSE
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monstr-0.1.2/README.md
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 monstr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 monstr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 monstr-0.1.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/backup.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/create_test_environment.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/entities.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/giftwrap_chat.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/keys.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/nip44_post.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/nip4_post.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/note_listen.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/note_listen_auth.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/note_post.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/post_auth.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/post_pow.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/post_signer.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/post_text.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/print_text_notes.py
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/query.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/republish.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/run_relay.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/run_relay_auth.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/run_relay_auth_sub.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/run_relay_mem_store.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/simple_bot.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/single_query.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 monstr-0.1.4/examples/view_profile.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/__init__.py
+-rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/encrypt.py
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/entities.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/exception.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/giftwrap.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/inbox.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/signing.py
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/channels/__init__.py
+-rw-r--r--   0        0        0     7060 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/channels/channel.py
+-rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/channels/event_handlers.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/channels/persist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/client/__init__.py
+-rw-r--r--   0        0        0    47903 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/client/client.py
+-rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/client/event_handlers.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/client/messaging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/data/__init__.py
+-rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/data/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/db/__init__.py
+-rw-r--r--   0        0        0    15723 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/db/db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/__init__.py
+-rw-r--r--   0        0        0    20402 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/event.py
+-rw-r--r--   0        0        0    18258 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/event_handlers.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/expire.py
+-rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/persist.py
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/persist_memory.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/persist_postgres.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/persist_sqlite.py
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/event/persist_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/ident/__init__.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/ident/alias.py
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/ident/event_handlers.py
+-rw-r--r--   0        0        0    30307 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/ident/persist.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/ident/persist_test.py
+-rw-r--r--   0        0        0    27579 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/ident/profile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/relay/__init__.py
+-rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/relay/accept_handlers.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/relay/exceptions.py
+-rw-r--r--   0        0        0    28631 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/relay/relay.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/settings/__init__.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/settings/handler.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/settings/persist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/spam_handlers/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 monstr-0.1.4/src/monstr/spam_handlers/spam_handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/nip13.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/nip19.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/nip4.py
+-rw-r--r--   0        0        0    11387 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/nip44.py
+-rw-r--r--   0        0        0    37630 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/nip44.vectors.json
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/nip59.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/persist_test.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/relay_test.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/scratch.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 monstr-0.1.4/tests/test_texts.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 monstr-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 monstr-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 monstr-0.1.4/README.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 monstr-0.1.4/PKG-INFO
```

### Comparing `monstr-0.1.2/examples/create_test_environment.py` & `monstr-0.1.4/examples/create_test_environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,32 +12,36 @@
 from monstr.client.client import Client
 from monstr.event.event import Event
 from monstr.ident.profile import ContactList
 from monstr.util import util_funcs
 from aiohttp import web
 from pathlib import Path
 
+COPY_RELAY = 'wss://nos.lol'
+OUR_RELAY_URL = 'localhost'
+OUR_RELAY_PORT = 8080
 WORK_DIR = f'{Path.home()}/.nostrpy/'
 DB = f'{WORK_DIR}test_env.db'
 
 
-async def run_relay():
+async def run_relay(at_host, at_port):
 
     r = Relay(store=ARelaySQLiteEventStore(DB),
               max_sub=10)
     # add some extra http methods to the relay so we can browse the data a little
     extra_routes = [
         web.get('/e', event_route(r)),
         web.get('/req', filter_route(r)),
         web.get('/view_profile', view_profile_route(r))
     ]
 
-    # await r.start_background(port=8888, routes=extra_routes)
-    await r.start(port=8888, routes=extra_routes, block=False)
-
+    await r.start(host=at_host,
+                  port=at_port,
+                  routes=extra_routes,
+                  block=False)
     return r
 
 
 async def populate_relay(pub_ks, dest_url: str, src_url):
     print('populating relay with data from pub_ks %s from relay: %s to %s' % (pub_ks,
                                                                               src_url,
                                                                               dest_url))
@@ -101,21 +105,18 @@
         for c_text in [c_evt for c_evt in evts if c_evt.kind == Event.KIND_TEXT_NOTE]:
             dest_client.publish(c_text)
 
         while (datetime.now() - last_msg).seconds < 5:
             print('waiting...')
             await asyncio.sleep(0.1)
 
-async def run(**kargs):
-    relay: Relay = await run_relay()
-
-    import_relay = 'wss://nostr-pub.wellorder.net'
-    if 'import_relay' in kargs:
-        import_relay = kargs['import_relay']
 
+async def run(import_relay, relay_host, relay_port, **kargs):
+    relay: Relay = await run_relay(at_host=relay_host,
+                                   at_port=relay_port)
 
     import_tasks = []
 
     # import these pub keys
     if 'import_keys' in kargs:
         print('importing: %s' % kargs['import_keys'])
 
@@ -188,16 +189,16 @@
                       on_notice=my_notice) as c:
         c.publish(n_evt)
         await asyncio.sleep(1)
 
 
 if __name__ == "__main__":
     logging.getLogger().setLevel(logging.DEBUG)
-    # import_relay = 'wss://nostr-pub.wellorder.net'
-    import_relay = 'wss://nos.lol'
     util_funcs.create_sqlite_store(DB)
 
-    asyncio.run(run(import_relay=import_relay,
+    asyncio.run(run(import_relay=COPY_RELAY,
+                    relay_host=OUR_RELAY_URL,
+                    relay_port=OUR_RELAY_PORT,
                     import_keys=['5c4bf3e548683d61fb72be5f48c2dff0cf51901b9dd98ee8db178efe522e325f'],
                     import_follows=['5c4bf3e548683d61fb72be5f48c2dff0cf51901b9dd98ee8db178efe522e325f']))
     # asyncio.run(relay_basic())
     # asyncio.run(post_basic())
```

### Comparing `monstr-0.1.2/examples/keys.py` & `monstr-0.1.4/examples/keys.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/examples/persist_test.py` & `monstr-0.1.4/tests/persist_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import logging
-import asyncio
-from datetime import datetime, timedelta
-from pathlib import Path
-from monstr.util import util_funcs
-from monstr.client.client import Client
-from monstr.event.event import Event
-from monstr.event.event_handlers import StoreEventHandler
-from monstr.event.persist import RelaySQLiteEventStore, ARelaySQLiteEventStore, SQLEventStore, AEventStoreInterface
-from monstr.encrypt import Keys
-
-# working directory it'll be created it it doesn't exist
-WORK_DIR = '%s/.nostrpy/' % Path.home()
-# and db we'll use
-DB_FILE = WORK_DIR+'persist_test.db'
-
-
-async def test_publish():
-    k = Keys()
-    last_msg = datetime.now()
-
-    def my_ok(the_client: Client, event_id, success, msg):
-        nonlocal last_msg
-        last_msg = datetime.now()
-
-    async with Client('ws://localhost:8888', on_ok=my_ok) as c:
-        for i in range(0, 1000):
-            n_evt = Event(kind=1,
-                          content='this is event %s for %s ' % (i,
-                                                                k.private_key_hex()),
-                          pub_key=k.public_key_hex())
-            n_evt.sign(k.private_key_hex())
-            c.publish(n_evt)
-
-        while (datetime.now() - last_msg).seconds < 2:
-            await asyncio.sleep(0.1)
-
-async def test_events():
-    my_persist = StoreEventHandler(ARelaySQLiteEventStore(DB_FILE))
-    # my_persist = StoreEventHandler(SQLEventStore(SQLiteDatabase(DB_FILE)))
-    async with Client('ws://localhost:8888') as c:
-        evts = await c.query(
-            filters={
-                'kinds': [Event.KIND_TEXT_NOTE],
-                'limit': 100
-            },
-            do_event=my_persist.do_event
-        )
-        for c_evt in evts:
-            print(c_evt)
-        await my_persist.wait_tasks()
-
-async def test_delete():
-    store = ARelaySQLiteEventStore(DB_FILE)
-    # no need to sign as we're just doing through store
-    delete_event = Event(
-        kind=Event.KIND_DELETE,
-        tags=[
-            ['e', '06a443c4e9428908504cd23c3c84861378fb21cd4f0936dc1639d01fa38d35f5'],
-            ['e', '898c0b8c40974bf10860afbd103e275d6183709cc813104c0fe97c591cc92c89']
-        ]
-    )
-    if isinstance(store, AEventStoreInterface):
-        await store.do_delete(delete_event)
-    else:
-        store.do_delete(delete_event)
-
-
-async def test_query():
-    store = ARelaySQLiteEventStore(DB_FILE)
-    filter = {
-        'authors': ['00000000827ffaa94bfea288c3dfce4422c794fbb96625b6b31e9049f729d700']
-    }
-
-    if isinstance(store, AEventStoreInterface):
-        evts = await store.get_filter(filter)
-    else:
-        evts = store.get_filter(filter)
-
-    print(len(evts))
-
-if __name__ == "__main__":
-    logging.getLogger().setLevel(logging.DEBUG)
-    util_funcs.create_sqlite_store(DB_FILE)
-    asyncio.run(test_events())
-    # asyncio.run(test_events())
-    # asyncio.run(test_delete())
-    # asyncio.run(test_query())
+# import logging
+# import asyncio
+# from datetime import datetime, timedelta
+# from pathlib import Path
+# from monstr.util import util_funcs
+# from monstr.client.client import Client
+# from monstr.event.event import Event
+# from monstr.event.event_handlers import StoreEventHandler
+# from monstr.event.persist import RelaySQLiteEventStore, ARelaySQLiteEventStore, SQLEventStore, AEventStoreInterface
+# from monstr.encrypt import Keys
+#
+# # working directory it'll be created it it doesn't exist
+# WORK_DIR = '%s/.nostrpy/' % Path.home()
+# # and db we'll use
+# DB_FILE = WORK_DIR+'persist_test.db'
+#
+#
+# async def test_publish():
+#     k = Keys()
+#     last_msg = datetime.now()
+#
+#     def my_ok(the_client: Client, event_id, success, msg):
+#         nonlocal last_msg
+#         last_msg = datetime.now()
+#
+#     async with Client('ws://localhost:8888', on_ok=my_ok) as c:
+#         for i in range(0, 1000):
+#             n_evt = Event(kind=1,
+#                           content='this is event %s for %s ' % (i,
+#                                                                 k.private_key_hex()),
+#                           pub_key=k.public_key_hex())
+#             n_evt.sign(k.private_key_hex())
+#             c.publish(n_evt)
+#
+#         while (datetime.now() - last_msg).seconds < 2:
+#             await asyncio.sleep(0.1)
+#
+# async def test_events():
+#     my_persist = StoreEventHandler(ARelaySQLiteEventStore(DB_FILE))
+#     # my_persist = StoreEventHandler(SQLEventStore(SQLiteDatabase(DB_FILE)))
+#     async with Client('ws://localhost:8888') as c:
+#         evts = await c.query(
+#             filters={
+#                 'kinds': [Event.KIND_TEXT_NOTE],
+#                 'limit': 100
+#             },
+#             do_event=my_persist.do_event
+#         )
+#         for c_evt in evts:
+#             print(c_evt)
+#         await my_persist.wait_tasks()
+#
+# async def test_delete():
+#     store = ARelaySQLiteEventStore(DB_FILE)
+#     # no need to sign as we're just doing through store
+#     delete_event = Event(
+#         kind=Event.KIND_DELETE,
+#         tags=[
+#             ['e', '06a443c4e9428908504cd23c3c84861378fb21cd4f0936dc1639d01fa38d35f5'],
+#             ['e', '898c0b8c40974bf10860afbd103e275d6183709cc813104c0fe97c591cc92c89']
+#         ]
+#     )
+#     if isinstance(store, AEventStoreInterface):
+#         await store.do_delete(delete_event)
+#     else:
+#         store.do_delete(delete_event)
+#
+#
+# async def test_query():
+#     store = ARelaySQLiteEventStore(DB_FILE)
+#     filter = {
+#         'authors': ['00000000827ffaa94bfea288c3dfce4422c794fbb96625b6b31e9049f729d700']
+#     }
+#
+#     if isinstance(store, AEventStoreInterface):
+#         evts = await store.get_filter(filter)
+#     else:
+#         evts = store.get_filter(filter)
+#
+#     print(len(evts))
+#
+# if __name__ == "__main__":
+#     logging.getLogger().setLevel(logging.DEBUG)
+#     util_funcs.create_sqlite_store(DB_FILE)
+#     asyncio.run(test_events())
+#     # asyncio.run(test_events())
+#     # asyncio.run(test_delete())
+#     # asyncio.run(test_query())
```

### Comparing `monstr-0.1.2/examples/post_text.py` & `monstr-0.1.4/examples/post_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import argparse
 from monstr.encrypt import Keys
 from monstr.client.client import ClientPool, Client
 from monstr.event.event import Event
 from monstr.util import ConfigError
 
 # default relay
-RELAY = 'ws://localhost:8888'
+RELAY = 'ws://localhost:8080'
 # default from user
 FROM_USER = None
 # default to user
 TO_USER = None
 
 
 def get_args():
@@ -86,25 +86,23 @@
     relay = args.relay.split(',')
     as_user: Keys = args.as_user
     to_user: Keys = args.to_user
 
     print('type exit to quit')
     msg_n = ''
 
-
     def on_auth(the_client: Client, challenge: str):
-        the_client.auth(as_user, challenge)
+        asyncio.create_task(the_client.auth(as_user, challenge))
 
     client = ClientPool(clients=relay,
                         on_auth=on_auth)
 
     asyncio.create_task(client.run())
 
 
-
     # exit cleanly on ctrl c
     def sigint_handler(signal, frame):
         print('stopping...')
         client.end()
         sys.exit(0)
 
     signal.signal(signal.SIGINT, sigint_handler)
@@ -125,13 +123,13 @@
             client.publish(n_event)
 
     print('stopping...')
     client.end()
 
 
 if __name__ == "__main__":
-    logging.getLogger().setLevel(logging.ERROR)
+    logging.getLogger().setLevel(logging.DEBUG)
     try:
         print(asyncio.run(prompt_post(get_args())))
     except ConfigError as ce:
         print(ce)
```

### Comparing `monstr-0.1.2/examples/print_text_notes.py` & `monstr-0.1.4/examples/print_text_notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from monstr.client.client import Client
 from monstr.client.event_handlers import EventHandler, LastEventHandler
 from monstr.event.event import Event
 from monstr.util import util_funcs
 from monstr.encrypt import Keys
 
 
-async def get_notes(for_key, relay='ws://localhost:8888/'):
+async def get_notes(for_key, relay='ws://localhost:8080/'):
     print('getting text(1) kind notes for key: %s from %s' % (for_key,
                                                               relay))
 
     # track last since so that if we reconnect we don't ask for everything again
     last_since = LastEventHandler()
     sub_id = None
```

### Comparing `monstr-0.1.2/examples/query.py` & `monstr-0.1.4/examples/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from monstr.event.event import Event
 from monstr.util import ConfigError
 from monstr.encrypt import Keys
 from monstr.ident.alias import ProfileFileAlias
 
 # defaults
 # working directory it'll be created it it doesn't exist
-WORK_DIR = '%s/.nostrpy/' % Path.home()
+WORK_DIR = f'{Path.home()}/.nostrpy/'
 #  relay to query
-DEFAULT_RELAY = 'ws://localhost:8888'
+DEFAULT_RELAY = 'ws://localhost:8080'
 # max time we'll wait for the query to complete
 DEFAULT_TIMEOUT = 10
 # limit on number of returned results
 DEFAULT_LIMIT = 100
 # kinds to return
 DEFAULT_KINDS = None
```

### Comparing `monstr-0.1.2/examples/simple_bot.py` & `monstr-0.1.4/examples/simple_bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import asyncio
 from datetime import datetime
 from monstr.client.client import Client, ClientPool
 from monstr.client.event_handlers import EventHandler,DeduplicateAcceptor
 from monstr.event.event import Event
-from monstr.encrypt import Keys
+from monstr.encrypt import Keys, NIP4Encrypt
 from monstr.util import util_funcs
 
 # default relay if not otherwise given
 # DEFAULT_RELAY = 'wss://nostr-pub.wellorder.net,wss://nos.lol'
-DEFAULT_RELAY = 'ws://localhost:8888'
+DEFAULT_RELAY = 'ws://localhost:8080'
 # DEFAULT_RELAY = 'wss://nos.lol'
 # bot account priv_k - to remove hardcode
 USE_KEY = 'nsec1fnyygyh57chwf7zhw3mwmrltc2hatfwn0hldtl4z5axv4netkjlsy0u220'
 
 
 def get_args():
     return {
@@ -24,16 +24,22 @@
 
 class BotEventHandler(EventHandler):
 
     def __init__(self, as_user: Keys, clients: ClientPool):
         self._as_user = as_user
         self._clients = clients
 
+        # to encrypt replies if nip4
+        self._nip4_enc = NIP4Encrypt(self._as_user)
+
         # track count times we replied to each p_pub_k
         self._replied = {}
+
+        # TODO - we should if check the events is for us in do_event or use an acceptor to do the same
+        # currently we're just relying on the filter being currect (and the relay ofcourse...)
         super().__init__(event_acceptors=[DeduplicateAcceptor()])
 
     def _make_reply_tags(self, src_evt: Event) -> []:
         """
             minimal tagging just that we're replying to sec_evt and tag in the creater pk so they see our reply
         """
         return [
@@ -58,34 +64,27 @@
             kind=evt.kind,
             content=response_text,
             tags=self._make_reply_tags(evt),
             pub_key=self._as_user.public_key_hex()
         )
 
         if response_event.kind == Event.KIND_ENCRYPT:
-            response_event.content = response_event.encrypt_content(priv_key=self._as_user.private_key_hex(),
-                                                                    pub_key=evt.pub_key)
+            response_event = self._nip4_enc.encrypt_event(response_event,
+                                                          to_pub_k=evt.pub_key)
 
         response_event.sign(self._as_user.private_key_hex())
-        self._clients.publish(response_event)
-        if self._store:
-            # store the txt decrypted?
-            if evt.kind == Event.KIND_ENCRYPT:
-                evt.content = prompt_text
-                response_event.content = response_text
 
-            asyncio.create_task(self._store.put(prompt_evt=evt,
-                                                reply_evt=response_event))
+        self._clients.publish(response_event)
 
     def get_response_text(self, the_event):
         # possible parse this text also before passing onm
         prompt_text = the_event.content
         if the_event.kind == Event.KIND_ENCRYPT:
-            prompt_text = the_event.decrypted_content(priv_key=self._as_user.private_key_hex(),
-                                                      pub_key=the_event.pub_key)
+            prompt_text = self._nip4_enc.decrypt(payload=prompt_text,
+                                                 for_pub_k=the_event.pub_key)
 
         # do whatever to get the response
         pk = the_event.pub_key
         reply_n = self._replied[pk] = self._replied.get(pk, 0)+1
         reply_name = util_funcs.str_tails(pk)
 
         response_text = f'hey {reply_name} this is reply {reply_n} to you'
@@ -117,16 +116,15 @@
                                  '#p': [as_user.public_key_hex()],
                                  'since': util_funcs.date_as_ticks(datetime.now())
                              })
     # add the on_connect
     my_clients.set_on_connect(on_connect)
 
     # start the clients
-    print('monitoring for events from or to account %s on relays %s' % (as_user.public_key_hex(),
-                                                                        relays))
+    print(f'monitoring for events from or to account {as_user.public_key_bech32()} on relays {relays}')
     await my_clients.run()
 
 
 if __name__ == "__main__":
     logging.getLogger().setLevel(logging.DEBUG)
     asyncio.run(main(get_args()))
```

### Comparing `monstr-0.1.2/examples/view_profile.py` & `monstr-0.1.4/examples/view_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,26 +49,28 @@
             pub_k = request.query['pub_k']
 
         if pub_k == '':
             raise ServerError('pub_k param is required')
 
         k = Keys.get_key(pub_k)
         if k is None:
-            raise ServerError('%s - doesn\'t look like a nonstr key' % pub_k)
+            raise ServerError(f'{pub_k} - doesn\'t look like a nonstr key')
 
+        pub_k = k.public_key_hex()
         ret = {
             'pub_k': pub_k,
             'error': 'not found'
         }
-        p = await self._my_peh.get_profile(pub_k)
+
+        p = await self._my_peh.aget_profile(pub_k)
         if p:
             ret = p.as_dict()
         return web.json_response(ret)
 
-    async def start(self, host='localhost', port=8080):
+    async def start(self, host='localhost', port=8081):
         logging.debug('started web server at %s port=%s' % (host, port))
         await self._runner.setup()
         site = web.TCPSite(self._runner,
                            host=host,
                            port=port)
         await site.start()
 
@@ -95,13 +97,13 @@
         await meta_server.start()
         while run:
             await asyncio.sleep(0.1)
 
 if __name__ == "__main__":
     logging.getLogger().setLevel(logging.DEBUG)
     # relays = ['wss://nostr-pub.wellorder.net']
-    relays= ['ws://localhost:8888']
+    relays= ['ws://localhost:8080']
     args = sys.argv[1:]
     if args:
         relays = args[0].split(',')
 
     asyncio.run(start_server(relays))
```

### Comparing `monstr-0.1.2/src/monstr/inbox.py` & `monstr-0.1.4/src/monstr/inbox.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import hashlib
 import json
-from monstr.encrypt import SharedEncrypt, Keys
+from monstr.encrypt import Keys
 from monstr.signing import SignerInterface
 from monstr.event.event import Event
 from monstr.util import util_funcs
 
 
 class Inbox:
 
@@ -12,14 +12,15 @@
         an inbox is a standard account that is used for wrapping other messages in so that only those that
         have the priv_k to the inbox can see.
         It can be watched via looking for messages with the same pub_k and kind (default kind4)
         When using encrypted messages over the inbox they can only be encrypted if you know the shared key,
         so you need to know which pubkeys you might expect messages from.
         The shared key is added to the wrapping event as shared tag
 
+        TODO - support use of NIP44 for the encryption
 
     """
 
     @staticmethod
     async def generate_share_key(for_sign: SignerInterface, to_pub_k: str) -> str:
         # TODO: the shared key is sha256(echd_key) of for_sign to to_key
         #  this is the same as the how clust did it - maybe though we should add
@@ -85,24 +86,23 @@
         shared_key = None
         if from_sign and to_k:
             shared_key = await self.generate_share_key(for_sign=from_sign,
                                                        to_pub_k=to_k)
             tags.append(['shared', shared_key])
 
         evt = Event(kind=self.kind,
-                    content=json.dumps(evt.event_data()),
+                    content=json.dumps(evt.data()),
                     pub_key=await self.pub_key,
                     tags=tags)
 
         if shared_key:
-            evt.content = await from_sign.encrypt_text(plain_text=evt.content,
+            evt.content = await from_sign.nip4_encrypt(plain_text=evt.content,
                                                        to_pub_k=to_k)
-            # evt = await from_sign.encrypt_event(evt, to_pub_k=to_k)
         else:
-            evt.content = await self._signer.encrypt_text(plain_text=evt.content,
+            evt.content = await self._signer.nip4_encrypt(plain_text=evt.content,
                                                           to_pub_k=await self.pub_key)
 
         await self._signer.sign_event(evt)
 
         return evt
 
     async def unwrap_event(self, evt: Event, user_sign: SignerInterface):
@@ -116,22 +116,22 @@
             # if us we'll try and unwrap, otherwise we'll just ret None - not for us?...
             share_map = {}
 
             if user_pub_k in self._share_maps:
                 share_map = self._share_maps[user_pub_k]
             if shared in share_map:
                 try:
-                    content = await user_sign.decrypt_text(encrypt_text=evt.content,
+                    content = await user_sign.nip4_decrypt(payload=evt.content,
                                                            for_pub_k=share_map[shared])
 
-                    ret = Event.from_JSON(json.loads(content))
+                    ret = Event.load(content)
                 except Exception as e:
                     pass
         # we'll just treat it as standard
         else:
             try:
-                content = await self._signer.decrypt_text(encrypt_text=evt.content,
+                content = await self._signer.nip4_decrypt(payload=evt.content,
                                                           for_pub_k=await self.pub_key)
-                ret = Event.from_JSON(json.loads(content))
+                ret = Event.load(content)
             except Exception as e:
                 pass
         return ret
```

### Comparing `monstr-0.1.2/src/monstr/util.py` & `monstr-0.1.4/src/monstr/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,23 +35,25 @@
             ret = [arr[i:i + chunk_size] for i in range(0, len(arr), chunk_size)]
         else:
             ret = [arr]
 
         return ret
 
     @staticmethod
-    def str_tails(the_str, taillen=4):
+    def str_tails(the_str, taillen=4, spacer='...'):
         # returns str start...end chars for taillen
         ret = '?...?'
 
         if the_str:
             if len(the_str) < (taillen*2)+3:
                 ret = the_str
             else:
-                ret = '%s...%s' % (the_str[:taillen], the_str[len(the_str)-taillen:])
+                ret = (f'{the_str[:taillen]}'
+                       f'{spacer}'
+                       f'{the_str[len(the_str)-taillen:]}')
         return ret
 
     @staticmethod
     def create_work_dir(top_dir, sub_dir=None):
         def fix_path_str(the_str):
             return the_str.replace(os.path.sep + os.path.sep, os.path.sep)
 
@@ -80,14 +82,17 @@
             if not the_sub_dir.is_dir():
                 try:
                     os.makedirs(the_sub_dir)
                 except PermissionError as pe:
                     print('error trying to create work sub director %s - %s' % (the_sub_dir, pe))
                     sys.exit(os.EX_CANTCREAT)
 
+
+
+
     @staticmethod
     def create_sqlite_store(db_file):
         from monstr.event.persist_sqlite import RelaySQLiteEventStore
         from monstr.ident.persist import SQLiteProfileStore
         from monstr.channels.persist import SQLiteSQLChannelStore
         from monstr.settings.persist import SQLiteSettingsStore
         my_events = RelaySQLiteEventStore(db_file)
```

### Comparing `monstr-0.1.2/src/monstr/channels/channel.py` & `monstr-0.1.4/src/monstr/channels/channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    pass
-
-import logging
-from datetime import datetime
-import json
-from json import JSONDecodeError
-from monstr.util import util_funcs
-from monstr.event.event import Event
-
-
-class Channel:
-
-    @staticmethod
-    def from_event(evt: Event):
-        """
-        TODO: add option to verify sig/eror if invalid?
-        creates an event object from json - at the moment this must be a full event, has id and has been signed,
-        may add option for presigned event in future
-        :param evt_json: json to create the event, as you'd recieve from subscription
-        :return:
-        """
-        return Channel(event_id=evt.id,
-                       create_pub_k=evt.pub_key,
-                       attrs=evt.content,
-                       created_at=util_funcs.date_as_ticks(evt.created_at))
-
-    @staticmethod
-    def get_msg_channel_id(evt: Event):
-        """
-        for given channel message event returns the channel id that that msg is in
-        :param evt:
-        :return:
-        """
-        ret = None
-        if evt.kind == Event.KIND_CHANNEL_MESSAGE:
-            e_tags = evt.e_tags
-            if e_tags:
-                ret = e_tags[0]
-        return ret
-
-    def __init__(self, event_id: str, create_pub_k: str, attrs=None,
-                 created_at: int = None, updated_at: int = None,
-                 last_post: Event = None):
-        self._event_id = event_id
-        self._create_pub_k = create_pub_k
-        self._attrs = {}
-        if attrs is not None:
-            if isinstance(attrs, dict):
-                self._attrs = attrs
-            # if is str rep e.g. directly from event turn it to {}
-            elif isinstance(attrs, str):
-                try:
-                    self._attrs = json.loads(attrs)
-                except JSONDecodeError as e:
-                    print(attrs)
-                    logging.debug(e)
-
-        self._created_at = created_at
-        if self._created_at is None:
-            self._created_at = util_funcs.date_as_ticks(datetime.now())
-
-        self._updated_at = self._created_at
-        if updated_at is not None:
-            self._updated_at = updated_at
-
-        self._last_post = last_post
-
-    def as_dict(self):
-        last_post = None
-        if self._last_post:
-            last_post = self._last_post.event_data()
-
-        return {
-            'id': self.event_id,
-            'create_pub_k': self.create_pub_k,
-            'name': self.name,
-            'about': self.about,
-            'picture': self.picture,
-            'last_post': last_post
-        }
-
-    @property
-    def name(self):
-        ret = self.get_attr('name')
-        if ret is None:
-            ret = '?unknown?'
-        return ret
-
-    @property
-    def picture(self):
-        return self.get_attr('picture')
-
-    @property
-    def about(self):
-        return self.get_attr('about')
-
-    @property
-    def event_id(self):
-        return self._event_id
-
-    @property
-    def create_pub_k(self):
-        return self._create_pub_k
-
-    @property
-    def created_at(self):
-        return self._created_at
-
-    @property
-    def updated_at(self):
-        return self._updated_at
-
-    @property
-    def attrs(self):
-        return self._attrs
-
-    @attrs.setter
-    def attrs(self, attrs) -> dict:
-        self._attrs = attrs
-
-    def get_attr(self, name):
-        # returns vale for named atr, None if it isn't defined
-        ret = None
-        if name in self._attrs:
-            ret = self._attrs[name]
-        return ret
-
-    def set_attr(self, name, value):
-        self._attrs[name] = value
-
-    @property
-    def last_post(self) -> Event:
-        return self._last_post
-
-    @last_post.setter
-    def last_post(self, evt: Event):
-        self._last_post = evt
-
-    def do_post(self, evt: Event):
-        # as last_post except it'll only update _last_post if the given evt is actually newer
-        if self._last_post is None or evt.created_at_ticks > self.last_post.created_at_ticks:
-            self._last_post = evt
-
-    def __str__(self):
-        return '%s[%s]' % (self.name[0:15].ljust(18), self.event_id)
-
-    def __lt__(self, other):
-        ret = False
-        if self.name and other.name:
-            ret = self.name.lower() < other.name.lower()
-        elif self.name and other.name is None:
-            ret = True
-        return ret
-
-
-class ChannelList:
-
-    def __init__(self, channels: [Channel]):
-        self._channels = channels
-        self._lookup = {}
-        c_c: Channel
-        for c_c in self._channels:
-            self._lookup[c_c.event_id] = c_c
-
-        self._lock = BoundedSemaphore()
-
-    def matches(self, m_str, max_match=None, search_about=False):
-        self.sort()
-        if m_str.replace(' ', '') == '':
-            ret = self._channels
-            if max_match:
-                ret = ret[:max_match]
-            return ret
-
-        # simple text text lookup against name/pubkey
-        ret = []
-        # we're going to ignore case
-        m_str = m_str.lower()
-        c_c: Channel
-
-        for c_c in self._channels:
-            # pubkey should be lowercase but name we convert
-            if m_str in c_c.event_id or \
-                    c_c.name and m_str in c_c.name.lower() \
-                    or search_about and c_c.about is not None and m_str in c_c.about:
-                ret.append(c_c)
-
-            # found enough matches
-            if max_match and len(ret) >= max_match:
-                break
-        return ret
-
-    def put(self, c:Channel):
-        ret = False
-        if c.event_id not in self._lookup:
-            self._channels.append(c)
-            self._lookup[c.event_id] = c
-            ret = True
-        else:
-            o_c = self._lookup[c.event_id]
-            if c.updated_at > o_c.updated_at:
-                self._channels = [c_c for c_c in self._channels if c_c.event_id != c.event_id]
-                self._lookup[c.event_id] = c
-                ret = True
-        return ret
-
-    def channel(self, channel_id):
-        ret = None
-        if channel_id in self._lookup:
-            ret = self._lookup[channel_id]
-        return ret
-
-    @property
-    def channels(self):
-        return self._channels
-
-    def sort(self):
-        def keyFunc(c: Channel):
-            ret = 0
-            if c.last_post:
-                ret = c.last_post.created_at_ticks
-            return ret
-
-        with self._lock:
-            self._channels.sort(key=keyFunc,
-                                reverse=True)
-
-    def __len__(self):
-        return len(self._channels)
-
-    def __getitem__(self, item):
-        return self._channels[item]
+# from __future__ import annotations
+# from typing import TYPE_CHECKING
+# if TYPE_CHECKING:
+#     pass
+#
+# import logging
+# from datetime import datetime
+# import json
+# from json import JSONDecodeError
+# from monstr.util import util_funcs
+# from monstr.event.event import Event
+#
+#
+# class Channel:
+#
+#     @staticmethod
+#     def from_event(evt: Event):
+#         """
+#         TODO: add option to verify sig/eror if invalid?
+#         creates an event object from json - at the moment this must be a full event, has id and has been signed,
+#         may add option for presigned event in future
+#         :param evt_json: json to create the event, as you'd recieve from subscription
+#         :return:
+#         """
+#         return Channel(event_id=evt.id,
+#                        create_pub_k=evt.pub_key,
+#                        attrs=evt.content,
+#                        created_at=util_funcs.date_as_ticks(evt.created_at))
+#
+#     @staticmethod
+#     def get_msg_channel_id(evt: Event):
+#         """
+#         for given channel message event returns the channel id that that msg is in
+#         :param evt:
+#         :return:
+#         """
+#         ret = None
+#         if evt.kind == Event.KIND_CHANNEL_MESSAGE:
+#             e_tags = evt.e_tags
+#             if e_tags:
+#                 ret = e_tags[0]
+#         return ret
+#
+#     def __init__(self, event_id: str, create_pub_k: str, attrs=None,
+#                  created_at: int = None, updated_at: int = None,
+#                  last_post: Event = None):
+#         self._event_id = event_id
+#         self._create_pub_k = create_pub_k
+#         self._attrs = {}
+#         if attrs is not None:
+#             if isinstance(attrs, dict):
+#                 self._attrs = attrs
+#             # if is str rep e.g. directly from event turn it to {}
+#             elif isinstance(attrs, str):
+#                 try:
+#                     self._attrs = json.loads(attrs)
+#                 except JSONDecodeError as e:
+#                     print(attrs)
+#                     logging.debug(e)
+#
+#         self._created_at = created_at
+#         if self._created_at is None:
+#             self._created_at = util_funcs.date_as_ticks(datetime.now())
+#
+#         self._updated_at = self._created_at
+#         if updated_at is not None:
+#             self._updated_at = updated_at
+#
+#         self._last_post = last_post
+#
+#     def as_dict(self):
+#         last_post = None
+#         if self._last_post:
+#             last_post = self._last_post.data()
+#
+#         return {
+#             'id': self.event_id,
+#             'create_pub_k': self.create_pub_k,
+#             'name': self.name,
+#             'about': self.about,
+#             'picture': self.picture,
+#             'last_post': last_post
+#         }
+#
+#     @property
+#     def name(self):
+#         ret = self.get_attr('name')
+#         if ret is None:
+#             ret = '?unknown?'
+#         return ret
+#
+#     @property
+#     def picture(self):
+#         return self.get_attr('picture')
+#
+#     @property
+#     def about(self):
+#         return self.get_attr('about')
+#
+#     @property
+#     def event_id(self):
+#         return self._event_id
+#
+#     @property
+#     def create_pub_k(self):
+#         return self._create_pub_k
+#
+#     @property
+#     def created_at(self):
+#         return self._created_at
+#
+#     @property
+#     def updated_at(self):
+#         return self._updated_at
+#
+#     @property
+#     def attrs(self):
+#         return self._attrs
+#
+#     @attrs.setter
+#     def attrs(self, attrs) -> dict:
+#         self._attrs = attrs
+#
+#     def get_attr(self, name):
+#         # returns vale for named atr, None if it isn't defined
+#         ret = None
+#         if name in self._attrs:
+#             ret = self._attrs[name]
+#         return ret
+#
+#     def set_attr(self, name, value):
+#         self._attrs[name] = value
+#
+#     @property
+#     def last_post(self) -> Event:
+#         return self._last_post
+#
+#     @last_post.setter
+#     def last_post(self, evt: Event):
+#         self._last_post = evt
+#
+#     def do_post(self, evt: Event):
+#         # as last_post except it'll only update _last_post if the given evt is actually newer
+#         if self._last_post is None or evt.created_at_ticks > self.last_post.created_at_ticks:
+#             self._last_post = evt
+#
+#     def __str__(self):
+#         return '%s[%s]' % (self.name[0:15].ljust(18), self.event_id)
+#
+#     def __lt__(self, other):
+#         ret = False
+#         if self.name and other.name:
+#             ret = self.name.lower() < other.name.lower()
+#         elif self.name and other.name is None:
+#             ret = True
+#         return ret
+#
+#
+# class ChannelList:
+#
+#     def __init__(self, channels: [Channel]):
+#         self._channels = channels
+#         self._lookup = {}
+#         c_c: Channel
+#         for c_c in self._channels:
+#             self._lookup[c_c.event_id] = c_c
+#
+#         self._lock = BoundedSemaphore()
+#
+#     def matches(self, m_str, max_match=None, search_about=False):
+#         self.sort()
+#         if m_str.replace(' ', '') == '':
+#             ret = self._channels
+#             if max_match:
+#                 ret = ret[:max_match]
+#             return ret
+#
+#         # simple text text lookup against name/pubkey
+#         ret = []
+#         # we're going to ignore case
+#         m_str = m_str.lower()
+#         c_c: Channel
+#
+#         for c_c in self._channels:
+#             # pubkey should be lowercase but name we convert
+#             if m_str in c_c.event_id or \
+#                     c_c.name and m_str in c_c.name.lower() \
+#                     or search_about and c_c.about is not None and m_str in c_c.about:
+#                 ret.append(c_c)
+#
+#             # found enough matches
+#             if max_match and len(ret) >= max_match:
+#                 break
+#         return ret
+#
+#     def put(self, c:Channel):
+#         ret = False
+#         if c.event_id not in self._lookup:
+#             self._channels.append(c)
+#             self._lookup[c.event_id] = c
+#             ret = True
+#         else:
+#             o_c = self._lookup[c.event_id]
+#             if c.updated_at > o_c.updated_at:
+#                 self._channels = [c_c for c_c in self._channels if c_c.event_id != c.event_id]
+#                 self._lookup[c.event_id] = c
+#                 ret = True
+#         return ret
+#
+#     def channel(self, channel_id):
+#         ret = None
+#         if channel_id in self._lookup:
+#             ret = self._lookup[channel_id]
+#         return ret
+#
+#     @property
+#     def channels(self):
+#         return self._channels
+#
+#     def sort(self):
+#         def keyFunc(c: Channel):
+#             ret = 0
+#             if c.last_post:
+#                 ret = c.last_post.created_at_ticks
+#             return ret
+#
+#         with self._lock:
+#             self._channels.sort(key=keyFunc,
+#                                 reverse=True)
+#
+#     def __len__(self):
+#         return len(self._channels)
+#
+#     def __getitem__(self, item):
+#         return self._channels[item]
```

### Comparing `monstr-0.1.2/src/monstr/channels/event_handlers.py` & `monstr-0.1.4/src/monstr/channels/event_handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,223 +1,225 @@
-from __future__ import annotations
-import time
-from monstr.event.event import Event
-from monstr.channels.persist import ChannelStoreInterface, Channel, ChannelList
-from monstr.util import util_funcs
-from monstr.client.client import Client
-import logging
-
-
-class ChannelEventHandler:
-    """
-        similar to the profile event handler but for channels
-    """
-
-    @staticmethod
-    def import_channel_info(channel_handler: ChannelEventHandler, events: [Event]):
-        # just incase , make sure sorted newest first else last posts will be incorrect
-        evts = Event.sort(events, inplace=False)
-
-        last_posts = {}
-        for_keys = set([])
-
-        for c_evt in evts:
-            k = Channel.get_msg_channel_id(c_evt)
-            # important uses .channels.channel as this won't attempt ot fetch missing
-            if k and k not in for_keys and channel_handler.channels.channel(k) is None:
-                for_keys.add(k)
-                last_posts[k] = c_evt
-
-        # chunk same reason as profiles
-        for k_chunk in util_funcs.chunk(list(for_keys), 250):
-            channels = channel_handler.get_channels(k_chunk, create_missing=True)
-            c_chn: Channel
-            # now update the last post we the msg that triggered us to create the channel
-            for c_chn in channels:
-                c_chn.do_post(last_posts[c_chn.event_id])
-
-    def __init__(self,
-                 channel_store: ChannelStoreInterface,
-                 on_channel_update=None,
-                 max_insert_batch=500):
-
-        self._store = channel_store
-        self._channels = self._store.select()
-        self._on_channel_update = on_channel_update
-        self._max_insert_batch = max_insert_batch
-
-    def do_event(self, sub_id, evt: Event, relay):
-        if not hasattr(evt, '__iter__'):
-            evt = [evt]
-
-        def get_store_func(the_chunk, for_func):
-            def the_func():
-                for_func(the_chunk)
-            return the_func
-
-        channel_creates = self._get_filtered_creates(evt)
-        for c_chunk in util_funcs.chunk(channel_creates, self._max_insert_batch):
-            util_funcs.retry_db_func(get_store_func(c_chunk, self._do_creates))
-            time.sleep(0.1)
-
-        channel_posts = self._get_filtered_posts(evt)
-        for c_chunk in util_funcs.chunk(channel_posts, self._max_insert_batch):
-            util_funcs.retry_db_func(get_store_func(c_chunk, self._do_posts))
-            time.sleep(0.1)
-
-        if channel_posts:
-            self.channels.sort()
-
-    def _get_filtered_creates(self, evts: [Event]) -> [Event]:
-        # split events
-        c_evt: Event
-        ret = [Channel.from_event(c_evt) for c_evt in evts if c_evt.kind == Event.KIND_CHANNEL_CREATE]
-
-        # maybe change but for now cut any non named channels, also skip if we already have this channel id
-        c_c: Channel
-        ret = [c_c for c_c in ret
-               if c_c.name and not self._channels.channel(c_c.event_id)]
-
-        return ret
-
-    def _get_filtered_posts(self, evts: [Event]) -> [Event]:
-        # split events
-        c_evt: Event
-        ret = [c_evt for c_evt in evts if c_evt.kind == Event.KIND_CHANNEL_MESSAGE]
-
-        # we only keep those for which we know the channel
-        ret = [c_evt for c_evt in ret
-               if self.channels.channel(Channel.get_msg_channel_id(c_evt))]
-
-        return ret
-
-    def _do_posts(self, posts: [Event]):
-        c_evt: Event
-        c: Channel
-        for c_evt in posts:
-            c = self.channels.channel(Channel.get_msg_channel_id(c_evt))
-            # updates if c_evt is newer than whatever we already have
-            c.do_post(c_evt)
-
-    def _do_creates(self, channels: [Channel]):
-        c_evt: Event
-        c_c: Channel
-        c_e: Channel
-
-        self._store.put(channels)
-
-        # update local cache
-        updates = []
-        for c_c in channels:
-            o_e = self._channels.channel(c_c.event_id)
-            if self._channels.put(c_c):
-                updates.append([c_c, o_e])
-
-        # fire update if any, probably change to send as batch too
-        if self._on_channel_update:
-            for i, c_update in enumerate(updates):
-                try:
-                    self._on_channel_update(c_update[0], c_update[1])
-                except Exception as e:
-                    logging.debug('ChannelEventHandler:_do_creates>_on_channel_update error: %s, channel: %s ' % (e,
-                                                                                                                  c_c.event_id))
-
-    @property
-    def channels(self) -> ChannelList:
-        return self._channels
-
-    @property
-    def store(self) -> ChannelStoreInterface:
-        return self._store
-
-    def set_on_update(self, on_update):
-        self._on_update = on_update
-
-    def get_id(self, channel_id) -> Channel:
-        return self._channels.channel(channel_id)
-
-    def get_channels(self, channel_ids: [str], create_missing=True) -> ChannelList:
-        if isinstance(channel_ids, str):
-            channel_ids = [channel_ids]
-
-        channels = []
-        for k in channel_ids:
-            c = self.channels.channel(k)
-            if c:
-                channels.append(c)
-            elif create_missing:
-                # TODO check k is valid?
-                channels.append(Channel(event_id=k))
-
-        return ChannelList(channels)
-
-    def matches(self, m_str='', max_match=None):
-        return self._channels.matches(m_str=m_str,
-                                      max_match=max_match,
-                                      search_about=False)
-
-
-class NetworkedChannelEventHandler(ChannelEventHandler):
-
-    def __init__(self,
-                 channel_store: ChannelStoreInterface,
-                 client: Client,
-                 on_channel_update=None,
-                 max_insert_batch=500):
-
-        self._client = client
-        super().__init__(channel_store=channel_store,
-                         on_channel_update=on_channel_update,
-                         max_insert_batch=max_insert_batch)
-
-    def fetch_channel_creates(self, keys):
-        if isinstance(keys, str):
-            keys = keys.split(',')
-
-        evts = self._client.query({
-            'kinds': [Event.KIND_CHANNEL_CREATE],
-            'ids': keys
-        })
-        ret = []
-        c_evt: Event
-        if evts:
-            # return chanels we found
-            ret = [Channel.from_event(c_evt) for c_evt in evts]
-            # Greenlet(util_funcs.get_background_task(self._do_creates, ret)).start_later(0)
-
-        return ret
-
-    def get_id(self, channel_id) -> Channel:
-        ret = super().get_id(channel_id)
-        if ret is None:
-            fetched = self.fetch_channel_creates(channel_id)
-            if fetched:
-                ret = fetched[0]
-
-        return ret
-
-    def get_channels(self, channel_ids: [str], create_missing=True) -> ChannelList:
-        if isinstance(channel_ids, str):
-            channel_ids = [channel_ids]
-        ret = super().get_channels(channel_ids, create_missing=False)
-        to_fetch = [k for k in channel_ids if ret.channel(k) is None]
-
-        ret = ret.channels
-
-        if to_fetch:
-            to_fetch.sort()
-            ret = ret + self.fetch_channel_creates(','.join(to_fetch))
-
-        c: Channel
-        if len(ret) != len(channel_ids) and create_missing:
-            got = set([c.event_id for c in ret])
-            for k in channel_ids:
-                if k not in got:
-                    empty_channel = Channel(event_id=k,
-                                            # sub the same as we have no idea what the pub_k is
-                                            create_pub_k='')
-                    ret.append(empty_channel)
-                    # so we won't continually be trying to fetch
-                    # on seeing a meta event it'll get updated anyhow
-                    self.channels.put(empty_channel)
-
-        return ChannelList(ret)
+# from __future__ import annotations
+# import time
+# from monstr.event.event import Event
+# from monstr.channels.persist import ChannelStoreInterface, Channel, ChannelList
+# from monstr.util import util_funcs
+# from monstr.client.client import Client
+# import logging
+#
+#
+# class ChannelEventHandler:
+#     """
+#         similar to the profile event handler but for channels
+#     """
+#
+#     @staticmethod
+#     def import_channel_info(channel_handler: ChannelEventHandler, events: [Event]):
+#         # just incase , make sure sorted newest first else last posts will be incorrect
+#         evts = Event.sort(events, inplace=False)
+#
+#         last_posts = {}
+#         for_keys = set([])
+#
+#         for c_evt in evts:
+#             k = Channel.get_msg_channel_id(c_evt)
+#             # important uses .channels.channel as this won't attempt ot fetch missing
+#             if k and k not in for_keys and channel_handler.channels.channel(k) is None:
+#                 for_keys.add(k)
+#                 last_posts[k] = c_evt
+#
+#         # chunk same reason as profiles
+#         for k_chunk in util_funcs.chunk(list(for_keys), 250):
+#             channels = channel_handler.get_channels(k_chunk, create_missing=True)
+#             c_chn: Channel
+#             # now update the last post we the msg that triggered us to create the channel
+#             for c_chn in channels:
+#                 c_chn.do_post(last_posts[c_chn.event_id])
+#
+#     def __init__(self,
+#                  channel_store: ChannelStoreInterface,
+#                  on_channel_update=None,
+#                  max_insert_batch=500):
+#
+#         self._store = channel_store
+#         self._channels = self._store.select()
+#         self._on_channel_update = on_channel_update
+#         self._max_insert_batch = max_insert_batch
+#
+#     def do_event(self, sub_id, evt: Event, relay):
+#         if not hasattr(evt, '__iter__'):
+#             evt = [evt]
+#
+#         def get_store_func(the_chunk, for_func):
+#             def the_func():
+#                 for_func(the_chunk)
+#             return the_func
+#
+#         channel_creates = self._get_filtered_creates(evt)
+#         for c_chunk in util_funcs.chunk(channel_creates, self._max_insert_batch):
+#             util_funcs.retry_db_func(get_store_func(c_chunk, self._do_creates))
+#             time.sleep(0.1)
+#
+#         channel_posts = self._get_filtered_posts(evt)
+#         for c_chunk in util_funcs.chunk(channel_posts, self._max_insert_batch):
+#             util_funcs.retry_db_func(get_store_func(c_chunk, self._do_posts))
+#             time.sleep(0.1)
+#
+#         if channel_posts:
+#             self.channels.sort()
+#
+#     def _get_filtered_creates(self, evts: [Event]) -> [Event]:
+#         # split events
+#         c_evt: Event
+#         ret = [Channel.from_event(c_evt) for c_evt in evts if c_evt.kind == Event.KIND_CHANNEL_CREATE]
+#
+#         # maybe change but for now cut any non named channels, also skip if we already have this channel id
+#         c_c: Channel
+#         ret = [c_c for c_c in ret
+#                if c_c.name and not self._channels.channel(c_c.event_id)]
+#
+#         return ret
+#
+#     def _get_filtered_posts(self, evts: [Event]) -> [Event]:
+#         # split events
+#         c_evt: Event
+#         ret = [c_evt for c_evt in evts if c_evt.kind == Event.KIND_CHANNEL_MESSAGE]
+#
+#         # we only keep those for which we know the channel
+#         ret = [c_evt for c_evt in ret
+#                if self.channels.channel(Channel.get_msg_channel_id(c_evt))]
+#
+#         return ret
+#
+#     def _do_posts(self, posts: [Event]):
+#         c_evt: Event
+#         c: Channel
+#         for c_evt in posts:
+#             c = self.channels.channel(Channel.get_msg_channel_id(c_evt))
+#             # updates if c_evt is newer than whatever we already have
+#             c.do_post(c_evt)
+#
+#     def _do_creates(self, channels: [Channel]):
+#         c_evt: Event
+#         c_c: Channel
+#         c_e: Channel
+#
+#         self._store.put(channels)
+#
+#         # update local cache
+#         updates = []
+#         for c_c in channels:
+#             o_e = self._channels.channel(c_c.event_id)
+#             if self._channels.put(c_c):
+#                 updates.append([c_c, o_e])
+#
+#         # fire update if any, probably change to send as batch too
+#         if self._on_channel_update:
+#             for i, c_update in enumerate(updates):
+#                 try:
+#                     self._on_channel_update(c_update[0], c_update[1])
+#                 except Exception as e:
+#                     logging.debug('ChannelEventHandler:_do_creates>_on_channel_update error: %s, channel: %s ' % (e,
+#                                                                                                                   c_c.event_id))
+#
+#     @property
+#     def channels(self) -> ChannelList:
+#         return self._channels
+#
+#     @property
+#     def store(self) -> ChannelStoreInterface:
+#         return self._store
+#
+#     def set_on_update(self, on_update):
+#         self._on_update = on_update
+#
+#     def get_id(self, channel_id) -> Channel:
+#         return self._channels.channel(channel_id)
+#
+#     def get_channels(self, channel_ids: [str], create_missing=True) -> ChannelList:
+#         if isinstance(channel_ids, str):
+#             channel_ids = [channel_ids]
+#
+#         channels = []
+#         for k in channel_ids:
+#             c = self.channels.channel(k)
+#             if c:
+#                 channels.append(c)
+#             elif create_missing:
+#                 # TODO check k is valid?
+#                 channels.append(Channel(event_id=k))
+#
+#         return ChannelList(channels)
+#
+#     def matches(self, m_str='', max_match=None):
+#         return self._channels.matches(m_str=m_str,
+#                                       max_match=max_match,
+#                                       search_about=False)
+#
+#
+# class NetworkedChannelEventHandler(ChannelEventHandler):
+#
+#     def __init__(self,
+#                  channel_store: ChannelStoreInterface,
+#                  client: Client,
+#                  on_channel_update=None,
+#                  max_insert_batch=500):
+#
+#         self._client = client
+#         super().__init__(channel_store=channel_store,
+#                          on_channel_update=on_channel_update,
+#                          max_insert_batch=max_insert_batch)
+#
+#     def fetch_channel_creates(self, keys):
+#         if isinstance(keys, str):
+#             keys = keys.split(',')
+#
+#         evts = self._client.query({
+#             'kinds': [Event.KIND_CHANNEL_CREATE],
+#             'ids': keys
+#         })
+#         ret = []
+#         c_evt: Event
+#         if evts:
+#             # return chanels we found
+#             ret = [Channel.from_event(c_evt) for c_evt in evts]
+#             # Greenlet(util_funcs.get_background_task(self._do_creates, ret)).start_later(0)
+#
+#         return ret
+#
+#     def get_id(self, channel_id) -> Channel:
+#         ret = super().get_id(channel_id)
+#         if ret is None:
+#             fetched = self.fetch_channel_creates(channel_id)
+#             if fetched:
+#                 ret = fetched[0]
+#
+#         return ret
+#
+#     def get_channels(self, channel_ids: [str], create_missing=True) -> ChannelList:
+#         if isinstance(channel_ids, str):
+#             channel_ids = [channel_ids]
+#         ret = super().get_channels(channel_ids, create_missing=False)
+#         to_fetch = [k for k in channel_ids if ret.channel(k) is None]
+#
+#         ret = ret.channels
+#
+#         if to_fetch:
+#             to_fetch.sort()
+#             ret = ret + self.fetch_channel_creates(','.join(to_fetch))
+#
+#         c: Channel
+#         if len(ret) != len(channel_ids) and create_missing:
+#             got = set([c.event_id for c in ret])
+#             for k in channel_ids:
+#                 if k not in got:
+#                     empty_channel = Channel(event_id=k,
+#                                             # sub the same as we have no idea what the pub_k is
+#                                             create_pub_k='')
+#                     ret.append(empty_channel)
+#                     # so we won't continually be trying to fetch
+#                     # on seeing a meta event it'll get updated anyhow
+#                     self.channels.put(empty_channel)
+#
+#         return ChannelList(ret)
+#
+#
```

### Comparing `monstr-0.1.2/src/monstr/channels/persist.py` & `monstr-0.1.4/src/monstr/channels/persist.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from monstr.event.persist import ClientEventStoreInterface
-
-import json
-from abc import ABC, abstractmethod
-from monstr.channels.channel import Channel, ChannelList
-from monstr.db.db import SQLiteDatabase, QueryFromFilter
-from monstr.data.data import DataSet
-from monstr.event.event import Event
-
-
-class ChannelStoreInterface(ABC):
-
-    @abstractmethod
-    def put(self, c: Channel):
-        """
-        :param c:
-        :return:
-        """
-
-    @abstractmethod
-    def select(self, filter={}) -> ChannelList:
-        """
-        :param filter:
-        :return:
-        """
-
-    @abstractmethod
-    def channels_for_keys(self, keys: [str]):
-        """
-        :param keys:
-        :return:
-        """
-
-
-    def import_from_events(self,
-                           event_store: ClientEventStoreInterface,
-                           evts: [Event] = None,
-                           since=None):
-        """
-        :param evts:
-        :param event_store:
-        :param since:
-        :return:
-        """
-
-        # if no events given then events since from events_store
-        if evts is None:
-            evt_filter = {
-                'kinds': [Event.KIND_CHANNEL_CREATE]
-            }
-            if since is not None:
-                evt_filter['since'] = since
-                evts = event_store.get_filter(evt_filter)
-
-        c: Channel
-        for c_evt in evts:
-            c = Channel.from_event(c_evt)
-            # if they're not named we won't import at least not for now
-            if c.name is not None:
-                self.put(c)
-
-
-class SQLiteSQLChannelStore(ChannelStoreInterface):
-
-    def __init__(self, db_file):
-        self._db_file = db_file
-        self._db = SQLiteDatabase(self._db_file)
-
-    def _prepare_put(self, c: Channel, batch=None):
-        if batch is None:
-            batch = []
-
-        sql = """
-            insert or replace into 
-                channels (event_id, attrs, name, picture, about, create_pub_k, created_at, updated_at) 
-                        values(?,?,?,?,?,?,?,?)
-            on conflict(event_id)
-            do update set 
-                attrs = excluded.attrs,
-                name = excluded.name,
-                picture = excluded.picture,
-                about = excluded.about,
-                updated_at = excluded.updated_at
-            where excluded.updated_at > updated_at
-        """
-        args = [
-            c.event_id,
-            json.dumps(c.attrs),
-            c.name, c.picture, c.about, c.create_pub_k,
-            c.created_at,
-            c.updated_at
-        ]
-
-        batch.append({
-            'sql': sql,
-            'args': args
-        })
-
-        return batch
-
-    def put(self, c: Channel):
-        batch = []
-        if not hasattr(c, '__iter__'):
-            c = [c]
-
-        for c_c in c:
-            self._prepare_put(c_c, batch)
-
-        return self._db.execute_batch(batch)
-
-    def select(self, limit=None, until=None) -> DataSet:
-        my_sql ="""
-			select 
-				c.event_id as c_id,
-                c.create_pub_k as c_create_pub_k,
-                c.attrs as c_attrs,
-                c.created_at as c_created_at,
-                c.updated_at as c_updated_at,
-                last_post_pub_k,
-                last_post_text,
-                last_post_time
-			from channels c
-			left outer join 
-			(select 
-                c_id,
-                c_create_pub_k,
-                c_attrs,
-                c_created_at,
-                c_updated_at,
-                last_post_pub_k,
-                last_post_text,
-                last_post_time
-                from (
-                select 
-                c.event_id as c_id,
-                c.create_pub_k as c_create_pub_k,
-                c.attrs as c_attrs,
-                c.created_at as c_created_at,
-                c.updated_at as c_updated_at,
-                e.content as last_post_text,
-                e.pubkey as last_post_pub_k,
-                e.created_at as last_post_time,
-                row_number() over (PARTITION by et.value order by e.created_at desc) as rn
-                from channels c
-                inner join event_tags et on et.type='e' and et.value=c.event_id
-                inner join events e on et.id = e.id
-                where e.kind=42
-                ) as channels
-                where channels.rn=1) as with_posts on c.event_id = c_id
-        """
-        args = []
-
-        if until:
-            my_sql = my_sql + 'and last_post_time < %s' % self._db.placeholder
-            args.append(until)
-
-        my_sql = my_sql + ' order by last_post_time desc'
-
-        if limit:
-            my_sql = my_sql + ' limit %s' % self._db.placeholder
-            args.append(limit)
-
-        channels = self._db.select_sql(sql=my_sql, args=args)
-
-        ret = []
-        new_c: Channel
-        for c_c in channels:
-            new_c = Channel(event_id=c_c['c_id'],
-                            create_pub_k=c_c['c_create_pub_k'],
-                            attrs=c_c['c_attrs'],
-                            created_at=c_c['c_created_at'],
-                            updated_at=c_c['c_updated_at'])
-
-            if c_c['last_post_pub_k']:
-                new_c.last_post = Event(
-                    kind=Event.KIND_CHANNEL_MESSAGE,
-                    content=c_c['last_post_text'],
-                    pub_key=c_c['last_post_pub_k'],
-                    created_at=c_c['last_post_time']
-                )
-
-            ret.append(new_c)
-        return ChannelList(ret)
-
-
-    def channels_for_keys(self, keys: [str]):
-        my_q = QueryFromFilter("""
-            select distinct et.value 
-            from events e
-            inner join event_tags et on et.id = e.id
-            inner join channels c on et.value = c.event_id
-        """,
-                               filter=[
-                                   {
-                                       'kind': 42
-                                   },
-                                   'and',
-                                   {
-                                       'pubkey': keys
-                                   }
-                               ],
-                               placeholder='?').get_query()
-        return self._db.select_sql(sql=my_q['sql'],
-                                   args=my_q['args']).data_arr('value')
-
-    def create(self):
-        self._db.execute_batch([
-            {
-                'sql': """
-                    create table channels(
-                        event_id text,
-                        attrs text,
-                        name text,
-                        picture text,
-                        about text,
-                        create_pub_k text,
-                        created_at int,
-                        updated_at int,
-                        UNIQUE(event_id) ON CONFLICT IGNORE
-                    )
-            """
-            }
-        ])
-
-    def destroy(self):
-        self._db.execute_batch([
-            {
-                'sql': 'drop table channels'
-            }
-        ])
+# from __future__ import annotations
+# from typing import TYPE_CHECKING
+# if TYPE_CHECKING:
+#     from monstr.event.persist import ClientEventStoreInterface
+#
+# import json
+# from abc import ABC, abstractmethod
+# from monstr.channels.channel import Channel, ChannelList
+# from monstr.db.db import SQLiteDatabase, QueryFromFilter
+# from monstr.data.data import DataSet
+# from monstr.event.event import Event
+#
+#
+# class ChannelStoreInterface(ABC):
+#
+#     @abstractmethod
+#     def put(self, c: Channel):
+#         """
+#         :param c:
+#         :return:
+#         """
+#
+#     @abstractmethod
+#     def select(self, filter={}) -> ChannelList:
+#         """
+#         :param filter:
+#         :return:
+#         """
+#
+#     @abstractmethod
+#     def channels_for_keys(self, keys: [str]):
+#         """
+#         :param keys:
+#         :return:
+#         """
+#
+#
+#     def import_from_events(self,
+#                            event_store: ClientEventStoreInterface,
+#                            evts: [Event] = None,
+#                            since=None):
+#         """
+#         :param evts:
+#         :param event_store:
+#         :param since:
+#         :return:
+#         """
+#
+#         # if no events given then events since from events_store
+#         if evts is None:
+#             evt_filter = {
+#                 'kinds': [Event.KIND_CHANNEL_CREATE]
+#             }
+#             if since is not None:
+#                 evt_filter['since'] = since
+#                 evts = event_store.get_filter(evt_filter)
+#
+#         c: Channel
+#         for c_evt in evts:
+#             c = Channel.from_event(c_evt)
+#             # if they're not named we won't import at least not for now
+#             if c.name is not None:
+#                 self.put(c)
+#
+#
+# class SQLiteSQLChannelStore(ChannelStoreInterface):
+#
+#     def __init__(self, db_file):
+#         self._db_file = db_file
+#         self._db = SQLiteDatabase(self._db_file)
+#
+#     def _prepare_put(self, c: Channel, batch=None):
+#         if batch is None:
+#             batch = []
+#
+#         sql = """
+#             insert or replace into
+#                 channels (event_id, attrs, name, picture, about, create_pub_k, created_at, updated_at)
+#                         values(?,?,?,?,?,?,?,?)
+#             on conflict(event_id)
+#             do update set
+#                 attrs = excluded.attrs,
+#                 name = excluded.name,
+#                 picture = excluded.picture,
+#                 about = excluded.about,
+#                 updated_at = excluded.updated_at
+#             where excluded.updated_at > updated_at
+#         """
+#         args = [
+#             c.event_id,
+#             json.dumps(c.attrs),
+#             c.name, c.picture, c.about, c.create_pub_k,
+#             c.created_at,
+#             c.updated_at
+#         ]
+#
+#         batch.append({
+#             'sql': sql,
+#             'args': args
+#         })
+#
+#         return batch
+#
+#     def put(self, c: Channel):
+#         batch = []
+#         if not hasattr(c, '__iter__'):
+#             c = [c]
+#
+#         for c_c in c:
+#             self._prepare_put(c_c, batch)
+#
+#         return self._db.execute_batch(batch)
+#
+#     def select(self, limit=None, until=None) -> DataSet:
+#         my_sql ="""
+# 			select
+# 				c.event_id as c_id,
+#                 c.create_pub_k as c_create_pub_k,
+#                 c.attrs as c_attrs,
+#                 c.created_at as c_created_at,
+#                 c.updated_at as c_updated_at,
+#                 last_post_pub_k,
+#                 last_post_text,
+#                 last_post_time
+# 			from channels c
+# 			left outer join
+# 			(select
+#                 c_id,
+#                 c_create_pub_k,
+#                 c_attrs,
+#                 c_created_at,
+#                 c_updated_at,
+#                 last_post_pub_k,
+#                 last_post_text,
+#                 last_post_time
+#                 from (
+#                 select
+#                 c.event_id as c_id,
+#                 c.create_pub_k as c_create_pub_k,
+#                 c.attrs as c_attrs,
+#                 c.created_at as c_created_at,
+#                 c.updated_at as c_updated_at,
+#                 e.content as last_post_text,
+#                 e.pubkey as last_post_pub_k,
+#                 e.created_at as last_post_time,
+#                 row_number() over (PARTITION by et.value order by e.created_at desc) as rn
+#                 from channels c
+#                 inner join event_tags et on et.type='e' and et.value=c.event_id
+#                 inner join events e on et.id = e.id
+#                 where e.kind=42
+#                 ) as channels
+#                 where channels.rn=1) as with_posts on c.event_id = c_id
+#         """
+#         args = []
+#
+#         if until:
+#             my_sql = my_sql + 'and last_post_time < %s' % self._db.placeholder
+#             args.append(until)
+#
+#         my_sql = my_sql + ' order by last_post_time desc'
+#
+#         if limit:
+#             my_sql = my_sql + ' limit %s' % self._db.placeholder
+#             args.append(limit)
+#
+#         channels = self._db.select_sql(sql=my_sql, args=args)
+#
+#         ret = []
+#         new_c: Channel
+#         for c_c in channels:
+#             new_c = Channel(event_id=c_c['c_id'],
+#                             create_pub_k=c_c['c_create_pub_k'],
+#                             attrs=c_c['c_attrs'],
+#                             created_at=c_c['c_created_at'],
+#                             updated_at=c_c['c_updated_at'])
+#
+#             if c_c['last_post_pub_k']:
+#                 new_c.last_post = Event(
+#                     kind=Event.KIND_CHANNEL_MESSAGE,
+#                     content=c_c['last_post_text'],
+#                     pub_key=c_c['last_post_pub_k'],
+#                     created_at=c_c['last_post_time']
+#                 )
+#
+#             ret.append(new_c)
+#         return ChannelList(ret)
+#
+#
+#     def channels_for_keys(self, keys: [str]):
+#         my_q = QueryFromFilter("""
+#             select distinct et.value
+#             from events e
+#             inner join event_tags et on et.id = e.id
+#             inner join channels c on et.value = c.event_id
+#         """,
+#                                filter=[
+#                                    {
+#                                        'kind': 42
+#                                    },
+#                                    'and',
+#                                    {
+#                                        'pubkey': keys
+#                                    }
+#                                ],
+#                                placeholder='?').get_query()
+#         return self._db.select_sql(sql=my_q['sql'],
+#                                    args=my_q['args']).data_arr('value')
+#
+#     def create(self):
+#         self._db.execute_batch([
+#             {
+#                 'sql': """
+#                     create table channels(
+#                         event_id text,
+#                         attrs text,
+#                         name text,
+#                         picture text,
+#                         about text,
+#                         create_pub_k text,
+#                         created_at int,
+#                         updated_at int,
+#                         UNIQUE(event_id) ON CONFLICT IGNORE
+#                     )
+#             """
+#             }
+#         ])
+#
+#     def destroy(self):
+#         self._db.execute_batch([
+#             {
+#                 'sql': 'drop table channels'
+#             }
+#         ])
```

### Comparing `monstr-0.1.2/src/monstr/client/client.py` & `monstr-0.1.4/src/monstr/client/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """
     web socket netork stuff for our monstr client
 
     TODO: change timers to check the actual time that has passed
 
 """
 from __future__ import annotations
-from typing import Callable
+
+import copy
+# from typing import Callable
 import logging
 import aiohttp
 try:
     from aiohttp_socks import SocksConnector
 except:
     pass
 import asyncio
 import json
+from typing import Callable
 from json import JSONDecodeError
-from datetime import datetime, timedelta
+from datetime import datetime
 from monstr.util import util_funcs
 from monstr.event.event import Event
+from monstr.signing import SignerInterface, BasicKeySigner
 from monstr.encrypt import Keys
-from monstr.signing import SignerInterface
 
 
 class QueryTimeoutException(Exception):
     pass
 
 
 class QueryLostConnectionException(Exception):
@@ -266,26 +269,35 @@
             logging.debug(
                 'Client::_on_message event for subscription with no handler registered subscription : %s\n event: %s' % (
                     sub_id, message))
             return
 
         if self.have_sub(sub_id):
             the_sub = self._subs[sub_id]
+            the_evt = Event.load(message[2])
+            # bad json??
+            if the_evt is None:
+                return
             # still receiving stored events
             if the_sub['is_eose'] is False:
-                the_sub['events'].append(Event.from_JSON(message[2]))
+                the_sub['events'].append(the_evt)
                 the_sub['last_event'] = datetime.now()
 
             # receiving adhoc events
             else:
                 try:
-                    the_evt = Event.from_JSON(message[2])
                     for c_handler in the_sub['handlers']:
                         try:
-                            c_handler.do_event(self, sub_id, the_evt)
+
+                            if callable(c_handler):
+                                c_handler(self, sub_id, the_evt)
+                            # should be a class with do_event defined (e.g. extends client.event_handlers.EventHandler)
+                            else:
+                                c_handler.do_event(self, sub_id, the_evt)
+
                         except Exception as e:
                             logging.debug(f'Client::_do_events in handler {c_handler} - {e}')
 
                 except Exception as e:
                     logging.debug(f'Client::_do_events error {e}')
 
     def _do_eose(self, sub_id):
@@ -343,55 +355,68 @@
 
     @property
     def running(self) -> bool:
         return self._run
 
     def publish(self, evt: Event):
         if self._write:
-            logging.debug('Client::publish - %s', evt.event_data())
+            logging.debug('Client::publish - %s', evt.data())
             self._publish_q.put_nowait(
                 json.dumps([
-                    'EVENT', evt.event_data()
+                    'EVENT', evt.data()
                 ])
             )
 
-    async def auth(self, signer: SignerInterface, challenge: str):
+    async def auth(self, signer: SignerInterface | Keys, challenge: str):
+        # better to use signer but if we just got keys we'll turn into a BasicKeySigner
+        if isinstance(signer, Keys):
+            signer = BasicKeySigner(signer)
+
         auth_event = Event(kind=Event.KIND_AUTH,
                            tags=[
                                ['relay', self.url],
                                ['challenge', challenge]
                            ],
                            pub_key=await signer.get_public_key())
 
         await signer.sign_event(auth_event)
 
         self._publish_q.put_nowait(
             json.dumps([
-                'AUTH', auth_event.event_data()
+                'AUTH', auth_event.data()
             ])
         )
 
-    async def query(self, filters: object = [],
-                    do_event: object = None,
+    async def query(self,
+                    filters: object = None,
+                    do_event: callable = None,
                     timeout=None,
                     wait_connect=False,
                     **kargs) -> [Event]:
         """
         do simple one off queries to a given relay
         :param timeout:
         :rtype: object
         :param filters:
         :param do_event:
+        :param wait_connect:
         :return:
         """
         is_done = False
         ret = None
         total_time = 0
 
 
+        # fix up filters
+        if filters is None:
+            filters = []
+        elif isinstance(filters, dict):
+            filters = [filters]
+
+        # use default timeout for client
         if timeout is None:
             timeout = self._query_timeout
 
         def my_done(the_client: Client, sub_id: str, events: [Event]):
             nonlocal is_done
             nonlocal ret
             ret = events
@@ -423,14 +448,90 @@
 
             await asyncio.sleep(sleep_time)
             total_time += sleep_time
 
         cleanup()
         return ret
 
+    async def query_until(self,
+                          until_date: datetime | int,
+                          filters: object = None,
+                          do_event: callable = None,
+                          timeout=None,
+                          wait_connect=False,
+                          **kargs) -> [Event]:
+        """
+            query as above except that it'll scan back until until_date
+            it's possible that it might also be useful to scan forward but to keep thing simple backward only
+            (if you supply a since in the query it'll be back from that point)
+        """
+
+        # fix filters
+        if filters is None:
+            filters = []
+        elif isinstance(filters, dict):
+            filters = [filters]
+
+        # because we're going to mod
+        filters = copy.deepcopy(filters)
+
+        # make sure until_date is int
+        if isinstance(until_date, datetime):
+            until_date = util_funcs.date_as_ticks(until_date)
+
+        ret = []
+        done = False
+        old_event = None
+
+        while done is False:
+            c_evts = await self.query(filters)
+
+            # run out of events
+            if not c_evts:
+                done = True
+            else:
+                # events should be ordered from relay but just incase....
+                c_evts.sort()
+
+                # cut any events upto and including anylast old event if we had one
+                if old_event:
+                    for back_seek in range(0, len(c_evts)):
+                        # the cut off event - last oldest should be the newest in this set
+                        if c_evts[back_seek].id == old_event.id:
+                            # cut any events before we reach the id of last event
+                            c_evts = c_evts[back_seek + 1:]
+                            break
+
+                # if no events then we're done
+                if not c_evts:
+                    done = True
+                else:
+                    # set an oldest event for next query
+                    old_event = c_evts[len(c_evts) - 1]
+                    oldest_date = old_event.created_at_ticks
+
+                    # if oldest date is lest then until date then we'll query again
+                    if oldest_date < until_date:
+                        # all dates are valid to ret
+                        ret = ret + c_evts
+                        # mod each filter in base query to have an until date
+                        for c_f in filters:
+                            c_f['until'] = oldest_date
+
+                    # oldest date us after until, append only event before until date
+                    else:
+                        done = True
+                        for c_evt in c_evts:
+                            if c_evt.created_at_ticks < until_date:
+                                ret.append(c_evt)
+                            else:
+                                break
+
+        return ret
+
     def subscribe(self, sub_id=None, handlers=None, filters={}, eose_func=None):
         """
         :param sub_id: if none a rndish 4digit hex sub_id will be given
         :param handler: single or [] of handlers that'll get called for events on sub
         :param filters: filter to be sent to relay for matching events were interested in
         see https://github.com/fiatjaf/nostr/blob/master/nips/01.md
         :return: sub_id
@@ -443,15 +544,15 @@
             sub_id = util_funcs.get_rnd_hex_str(4)
         the_req.append(sub_id)
         if isinstance(filters, dict):
             filters = [filters]
         the_req = the_req + filters
 
         the_req = json.dumps(the_req)
-        logging.debug('Client::subscribe - %s', the_req)
+        logging.debug(f'Client::subscribe - {the_req}')
 
         # make sure handler is list
         if handlers is None:
             handlers = []
         # added ClientPool else we end up itering over Clients and thinking they're handlers!
         elif not hasattr(handlers, '__iter__') or isinstance(handlers, ClientPool):
             handlers = [handlers]
@@ -948,20 +1049,23 @@
             c_client.unsubscribe(sub_id)
 
         del self._handlers[sub_id]
 
     def have_sub(self, sub_id: str):
         return sub_id in self._handlers
 
-    async def query(self, filters=[],
-                    do_event=None,
-                    wait_connect=False,
-                    emulate_single=True,
-                    timeout=None,
-                    on_complete=None):
+    async def _query(self,
+                     filters: [] = None,
+                     do_event: callable = None,
+                     wait_connect: bool = False,
+                     emulate_single: bool = True,
+                     timeout: int = None,
+                     on_complete: callable = None,
+                     until_date: int = None
+                     ):
         """
         similar to the query func, if you don't supply a ret_func we try and act in the same way as a single
         client would but wait for all clients to return and merge results into a single result with duplicate
         events removed
         probably better to supply a ret func though in which case it'll be called with the client and that clients
         results as they come in
 
@@ -977,27 +1081,41 @@
         c_client: Client
         client_wait = 0
         ret = {}
 
         async def get_q(the_client: Client):
             nonlocal client_wait
             try:
-                ret[the_client.url] = await the_client.query(filters,
-                                                             do_event=do_event,
-                                                             wait_connect=wait_connect,
-                                                             timeout=timeout)
+                # no until date, only one query will be done and what we get might not be everything
+                # as the relay most likely applies limits event if we don't request
+                if until_date is None:
+                    ret[the_client.url] = await the_client.query(filters,
+                                                                 do_event=do_event,
+                                                                 wait_connect=wait_connect,
+                                                                 timeout=timeout)
+
+                # with an until date, we'll try and get all event suntil until date
+                # this most likely will be made of multiple fetches
+                else:
+                    ret[the_client.url] = await the_client.query_until(until_date=until_date,
+                                                                       filters=filters,
+                                                                       do_event=do_event,
+                                                                       wait_connect=wait_connect,
+                                                                       timeout=timeout)
+
                 # ret_func(the_client, the_client.query(filters, wait_connect=False))
             except QueryTimeoutException as toe:
-                logging.debug('ClientPool::query timout - %s ' % toe)
+                logging.debug(f'ClientPool::query timout - {toe}')
             except Exception as e:
-                logging.debug('ClientPool::query exception - %s' % e)
+                logging.debug(f'ClientPool::query exception - {e}')
             client_wait -= 1
 
+            # callback that the fetch has completed
             if client_wait == 0 and on_complete:
-                on_complete()
+                on_complete(Event.merge(*ret.values()))
 
         c_client: Client
         query_tasks = []
 
         for c_client in self.clients:
             if c_client.read:
                 client_wait += 1
@@ -1006,16 +1124,53 @@
         while client_wait > 0:
             await asyncio.sleep(0.1)
             if ret and not emulate_single:
                 break
 
         return Event.merge(*ret.values())
 
+    def query(self,
+              filters: [] = None,
+              do_event: callable = None,
+              wait_connect: bool = False,
+              emulate_single: bool = True,
+              timeout: int = None,
+              on_complete: callable = None):
+
+        return self._query(filters=filters,
+                           do_event=do_event,
+                           wait_connect=wait_connect,
+                           emulate_single=emulate_single,
+                           timeout=timeout,
+                           on_complete=on_complete)
+
+    def query_until(self,
+                    until_date: datetime | int,
+                    filters: [] = None,
+                    do_event: callable = None,
+                    wait_connect: bool = False,
+                    emulate_single: bool = True,
+                    timeout: int = None,
+                    on_complete: callable = None):
+        """
+            query with backscan till until date, note if you set emulate_single False
+            then you'll probably want to supply an on_compete function
+        """
+
+        return self._query(until_date=until_date,
+                           filters=filters,
+                           do_event=do_event,
+                           wait_connect=wait_connect,
+                           emulate_single=emulate_single,
+                           timeout=timeout,
+                           on_complete=on_complete)
+
+
     def publish(self, evt: Event):
-        logging.debug('ClientPool::publish - %s', evt.event_data())
+        logging.debug(f'ClientPool::publish - {evt.data()}')
         c_client: Client
 
         for c_client in self:
             # c_client = self._clients[c_client]
             if c_client.write:
                 try:
                     c_client.publish(evt)
@@ -1083,15 +1238,19 @@
 
         # only do anything if relay read is True
         if self._clients[client.url]['client'].read:
             # note no de-duplication is done here, you might see the same event from mutiple relays
             if sub_id in self._handlers:
                 for c_handler in self._handlers[sub_id]:
                     try:
-                        c_handler.do_event(client, sub_id, evt)
+                        if callable(c_handler):
+                            c_handler(client, sub_id, evt)
+                        # should be a class with do_event defined (e.g. extends client.event_handlers.EventHandler)
+                        else:
+                            c_handler.do_event(client, sub_id, evt)
                     except Exception as e:
                         logging.debug('ClientPool::do_event, problem in handler - %s' % e)
 
             else:
                 # supose this might happen if unsubscribe then evt comes in...
                 logging.debug(
                     'ClientPool::do_event event for subscription with no handler registered subscription : %s\n event: %s' % (
```

### Comparing `monstr-0.1.2/src/monstr/client/event_handlers.py` & `monstr-0.1.4/src/monstr/client/event_handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from datetime import datetime
 from monstr.ident.profile import ProfileList, Profile, Contact, ContactList
 from abc import ABC, abstractmethod
 import base64
 import logging
 import json
 from collections import OrderedDict
-from threading import BoundedSemaphore
-from monstr.encrypt import SharedEncrypt
+from monstr.encrypt import NIP4Encrypt
 from monstr.util import util_funcs
 from monstr.event.event import Event
 
 
 class EventAccepter(ABC):
 
     @abstractmethod
@@ -133,16 +132,18 @@
         if self._max and msg_len > self._max:
             ret = False
         return ret
 
 
 class EventHandler(ABC):
 
-    def __init__(self, event_acceptors: [EventAccepter] = []):
-        if not hasattr(event_acceptors, '__iter__'):
+    def __init__(self, event_acceptors: [EventAccepter] = None):
+        if event_acceptors is None:
+            event_acceptors = []
+        elif not hasattr(event_acceptors, '__iter__'):
             event_acceptors = [event_acceptors]
         self._event_acceptors = event_acceptors
 
     def accept_event(self,
                      the_client: Client,
                      sub_id: str,
                      evt: Event) -> bool:
@@ -223,20 +224,23 @@
                                    util_funcs.str_tails(profile_name, 4),
                                    content))
 
 
 class LastEventHandler(EventHandler):
     """
         use to keep track of the last time we received events for a given relay
+        if event_acceptors is given then only accepted events are used to update the time
     """
-    def __init__(self):
+    def __init__(self, event_acceptors: [EventAccepter] = None):
+        super().__init__(event_acceptors=event_acceptors)
         self._url_time_map = {}
 
     def do_event(self, the_client: Client, sub_id, evt: Event):
-        self.set_now(the_client)
+        if self.accept_event(the_client, sub_id, evt):
+            self.set_now(the_client)
 
     def set_now(self, the_client):
         url = self._client_url(the_client)
         self._url_time_map[url] = datetime.now()
 
     @staticmethod
     def _client_url(the_client) -> str:
@@ -254,58 +258,41 @@
 
     def set_last_event_dt(self, the_client: Client, dt: datetime):
         self._url_time_map[self._client_url(the_client)] = dt
 
 
 class DecryptPrintEventHandler(PrintEventHandler):
     """
-        prints out decrypted messages we created or sent to us
-        NOTE: this is not the style that is compatiable with clust, that uses a public inbox
-        and encrypts the event as a package... want to add this too
+        Basic event printer for encrypted events
+        supports NIP4 events,
+        add support for NIP44
+        add support for signer interface for decrypting events -
+        events would have to be queued and printed
     """
-
     def __init__(self, priv_k, view_on=True):
         self._priv_k = priv_k
-        self._my_encrypt = SharedEncrypt(priv_k)
+        self._nip4_decrypt = NIP4Encrypt(key=priv_k)
         super(DecryptPrintEventHandler, self).__init__(view_on)
 
-    def _do_dycrypt(self, crypt_text, pub_key):
-        msg_split = crypt_text.split('?iv')
-        text = base64.b64decode(msg_split[0])
-        iv = base64.b64decode(msg_split[1])
-
-        return (self._my_encrypt.decrypt_message(encrypted_data=text,
-                                                 iv=iv,
-                                                 # note the ext is ignored anyway
-                                                 pub_key_hex='02' + pub_key))
-
     def do_event(self, the_client: Client, sub_id, evt: Event):
         if self._view_on is False:
             return
-        do_decrypt = False
-        to_key = evt['tags'][0][1]
-        print(to_key, self._my_encrypt.public_key_hex)
-        if evt['kind'] == Event.KIND_ENCRYPT:
-            # messages we created
-            if evt['pubkey'] == self._my_encrypt.public_key_hex[2:]:
-                pub_key = to_key
-                do_decrypt = True
-
-            # messages sent to us
-            elif to_key == self._my_encrypt.public_key_hex[2:]:
-                pub_key = evt['pubkey']
-                do_decrypt = True
-
-        content = evt['content']
-        if do_decrypt:
-            content = self._do_dycrypt(evt['content'], pub_key)
-
-        print('%s: %s - %s' % (util_funcs.ticks_as_date(evt['created_at']),
-                               evt['pubkey'],
-                               content))
+
+        out_event = evt
+        try:
+            out_event = self._nip4_decrypt.decrypt_event(evt)
+        except:
+            pass
+
+        self.print(the_client, sub_id, out_event)
+
+    def print(self, the_client: Client, sub_id, evt: Event):
+        print(f'{util_funcs.ticks_as_date(evt.created_at)}'
+              f'{util_funcs.str_tails(evt.pub_key)}'
+              f'{evt.content}')
 
 
 class FileEventHandler:
 
     def __init__(self, file_name, delete_exist=True):
         self._file_name = file_name
         if delete_exist:
@@ -316,44 +303,35 @@
         # appends to
         with open(self._file_name, "a") as f:
             evt['pubkey'] = evt['pubkey']
             f.writelines(json.dumps(evt) + '\n')
         logging.debug('FileEventHandler::do_event event appended to file %s' % self._file_name)
 
 
-# class EventTimeHandler:
-#
-#     def __init__(self, callback=None):
-#         self._callback = callback
-#
-#     def do_event(self, the_client: Client, sub_id, evt: Event):
-#         self._callback(evt['created_at'])
-
-
-class RepostEventHandler:
+class RepostEventHandler(EventHandler):
     """
     reposts events seen  on to given Client/ClientPool object
     event size number of event ids to keep to prevent duplicates being sent out
     NOTE though this is really just to prevent wasteful repost of events, relays
     shouldn't have a problem receiving duplicate ids
 
     to_client, TODO: define interface that both Client and ClientPool share and type hint with that
 
     """
-    def __init__(self, to_client, max_dedup=1000):
+    def __init__(self, to_client, max_dedup=1000, event_acceptors=None):
         self._to_client = to_client
         self._duplicates = OrderedDict()
         self._max_dedup = max_dedup
-        self._lock = BoundedSemaphore()
+        super().__init__(event_acceptors=event_acceptors)
 
     def do_event(self, the_client: Client, sub_id, evt: Event):
         do_send = False
-        with self._lock:
+        if self.accept_event(the_client, sub_id, evt):
             if evt.id not in self._duplicates:
                 do_send = True
                 self._duplicates[evt.id] = True
                 if len(self._duplicates) >= self._max_dedup:
                     self._duplicates.popitem(False)
 
         if do_send:
             self._to_client.publish(evt)
-            print('RepostEventHandler::sent event %s to %s' % (evt, self._to_client))
+            print(f'RepostEventHandler::sent event {evt.id} to {self._to_client}')
```

### Comparing `monstr-0.1.2/src/monstr/client/messaging.py` & `monstr-0.1.4/src/monstr/client/messaging.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import base64
 import logging
 # from gevent.lock import BoundedSemaphore
 from monstr.ident.profile import Profile
 from monstr.client.client import Client
 from monstr.event.event import Event
-from monstr.encrypt import SharedEncrypt
+from monstr.encrypt import NIP4Encrypt
 
 
 class MessageThreads:
     """
         keep a track of all 1-1 message for from_p
         if evt_store is given then
 
@@ -126,15 +126,15 @@
                     'msgs': []
                 }
             }
 
         if msg_evt.kind == Event.KIND_ENCRYPT:
             # we keep in memory unecrypted, probably we should decrypt at the point
             # we're outputing to screen
-            msg_copy = Event.create_from_JSON(msg_evt.event_data())
+            msg_copy = Event.load(msg_evt.data())
             try:
 
                 msg_copy.content = msg_evt.decrypted_content(self._from.private_key, to_id)
 
             except Exception as e:
                 msg_copy.content = '!!!unable to decrypt!!!'
         self._msg_threads[to_id][msg_evt.kind]['msgs'].append(msg_copy)
@@ -159,16 +159,16 @@
         :return:
         """
         the_content = text
 
         # # encrypt text as NIP4 if encrypted kind
         if kind == Event.KIND_ENCRYPT:
             # as decrypt add this as event method
-            my_enc = SharedEncrypt(self._from.private_key)
-            my_enc.derive_shared_key('02' + to_user.public_key)
+            my_enc = NIP4Encrypt(self._from.private_key)
+            my_enc.get_echd_key_hex(to_user.public_key)
             # crypt_message = my_enc.encrypt_message(b'a very simple message to test encrypt')
             crypt_message = my_enc.encrypt_message(bytes(text.encode('utf8')))
             enc_message = base64.b64encode(crypt_message['text'])
             iv_env = base64.b64encode(crypt_message['iv'])
             the_content = '%s?iv=%s' % (enc_message.decode(), iv_env.decode())
 
         n_event = Event(kind=kind,
```

### Comparing `monstr-0.1.2/src/monstr/data/data.py` & `monstr-0.1.4/src/monstr/data/data.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/db/db.py` & `monstr-0.1.4/src/monstr/db/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         #     finally:
         #         if c:
         #             c.close()
         #
         # if not catch_err and was_err:
         #     raise was_err
 
-        return ret
+        #return ret
 
     def execute_batch(self, batch):
         """
         :param batch: array of {
             'sql' : str,
             'args' : [] optional
         }
@@ -300,15 +300,15 @@
         #     finally:
         #         if c:
         #             c.close()
         #
         # if not catch_err and was_err:
         #     raise was_err
 
-        return ret
+        # return ret
 
     async def execute_batch(self, batch):
         """
         :param batch: array of {
             'sql' : str,
             'args' : [] optional
         }
```

### Comparing `monstr-0.1.2/src/monstr/event/event.py` & `monstr-0.1.4/src/monstr/event/event.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from datetime import datetime
-import base64
 import json
 import logging
 from json import JSONDecodeError
 import secp256k1
 import hashlib
+from copy import copy
 from monstr.util import util_funcs
-from monstr.encrypt import SharedEncrypt, Keys
 
 
 class EventTags:
     """
         split out so we can use event tags without have to create the whole event
     """
     def __init__(self, tags):
@@ -111,14 +110,20 @@
     KIND_CONTACT_LIST = 3
     KIND_ENCRYPT = 4
     KIND_DELETE = 5
     # NIP 25 reactions https://github.com/nostr-protocol/nips/blob/master/25.md
     KIND_REACTION = 7
     # NIP 58 badges https://github.com/nostr-protocol/nips/pull/229
     KIND_BADGE = 8
+
+    # NIP59 seal and gift wrap as defined in  https://github.com/nostr-protocol/nips/blob/master/59.md
+    KIND_SEAL = 13
+    KIND_RUMOUR = 14
+    KIND_GIFT_WRAP = 1059
+
     # NIP 28 events for group chat
     # https://github.com/nostr-protocol/nips/blob/af6893145f9a4a63be3d90beffbcfd4d90e872ae/28.md
     KIND_CHANNEL_CREATE = 40
     KIND_CHANNEL_META = 41
     KIND_CHANNEL_MESSAGE = 42
     KIND_CHANNEL_HIDE = 43
     KIND_CHANNEL_MUTE = 44
@@ -134,34 +139,87 @@
 
     # a raw bitcoin transaction
     KIND_BTC_TX = 28333
 
     # user status events https://github.com/nostr-protocol/nips/blob/master/38.md
     KIND_USER_STATUS = 30315
 
+    # @staticmethod
+    # def from_JSON(evt_json):
+    #     # TODO: remove!!!! change to using load in place
+    #     # this was never really from json anway it's from dict
+    #     return Event(
+    #         id=evt_json['id'],
+    #         sig=evt_json['sig'],
+    #         kind=evt_json['kind'],
+    #         content=evt_json['content'],
+    #         tags=evt_json['tags'],
+    #         pub_key=evt_json['pubkey'],
+    #         created_at=evt_json['created_at']
+    #     )
 
     @staticmethod
-    def from_JSON(evt_json):
+    def load(event_data: str | dict, validate=False) -> 'Event':
         """
-        TODO: add option to verify sig/eror if invalid?
-        creates an event object from json - at the moment this must be a full event, has id and has been signed,
-        may add option for presigned event in future
-        :param evt_json: json to create the event, as you'd recieve from subscription
-        :return:
+            return a Event object either from a dict or json str this replaces the old from_JSON method
+            that was actually just from a string...
+            if validate is set True will test the event sig, if it's not None will be returned
+
         """
-        return Event(
-            id=evt_json['id'],
-            sig=evt_json['sig'],
-            kind=evt_json['kind'],
-            content=evt_json['content'],
-            tags=evt_json['tags'],
-            pub_key=evt_json['pubkey'],
-            created_at=evt_json['created_at']
+        if isinstance(event_data, str):
+            try:
+                event_data = json.loads(event_data)
+            except Exception as e:
+                event_data = {}
+
+        id = None
+        if 'id' in event_data:
+            id = event_data['id']
+
+        sig = None
+        if 'sig' in event_data:
+            sig = event_data['sig']
+
+        kind = None
+        if 'kind' in event_data:
+            kind = event_data['kind']
+
+        content = None
+        if 'content' in  event_data:
+            content = event_data['content']
+
+        tags = None
+        if 'tags' in event_data:
+            tags = event_data['tags']
+
+        pub_key = None
+        if 'pubkey' in event_data:
+            pub_key = event_data['pubkey']
+
+        created_at = None
+        if 'created_at' in event_data:
+            created_at = event_data['created_at']
+
+        ret = Event(
+            id=id,
+            sig=sig,
+            kind=kind,
+            content=content,
+            tags=tags,
+            pub_key=pub_key,
+            created_at=created_at
         )
 
+        # None ret if validating and the evnt is not valid
+        if validate is True and ret.is_valid() is False:
+            ret = None
+
+        return ret
+
+
     @staticmethod
     def is_event_id(event_id: str):
         """
         basic check that given str is a monstr event id
         """
         ret = False
         if len(event_id) == 64:
@@ -198,15 +256,21 @@
 
     @staticmethod
     def sort(evts: [], reverse=True, inplace=False):
         """
         :param evts:    events to be sorted either {} or Event
         :param reverse: True is newest first which is default
         :param inplace: act on evts or create new []
-        :return:
+        :return: sorted events
+
+        NOTE - if you're only working with events and inplace is fine you can just use standard python sort
+        i.e
+            evts = [Events]
+            evts.sort()
+
         """
         # sort events newest to oldest
         def sort_func(evt: Event):
             if isinstance(evt, Event):
                 ret = evt.created_at_ticks
             else:
                 ret = evt['created_at']
@@ -245,32 +309,14 @@
                 since_lookup.add(c_evt.pub_key)
                 ret.append(c_evt)
             elif c_evt.kind == kind:
                 logging.debug('latest_events_only: ignore superceeded event %s' % c_evt)
 
         return ret
 
-    @staticmethod
-    def decrypt_nip4(evt: 'Event', keys: Keys, check_kind=True) -> 'Event':
-        """
-        returns a copy of evt but with the content decrtpted as NIP4
-        """
-
-        # make a copy
-        ret = Event.from_JSON(evt.event_data())
-        # now decrypt the content
-        pub_k = evt.pub_key
-        if pub_k == keys.public_key_hex():
-            pub_k = evt.p_tags[0]
-
-        ret.content = evt.decrypted_content(priv_key=keys.private_key_hex(),
-                                            pub_key=pub_k,
-                                            check_kind=check_kind)
-        return ret
-
     def __init__(self, id=None, sig=None, kind=None, content=None, tags=None, pub_key=None, created_at=None):
         self._id = id
         self._sig = sig
         self._kind = kind
         self._created_at = created_at
         # normally the case when creating a new event
         if created_at is None:
@@ -279,15 +325,19 @@
             self._created_at = util_funcs.date_as_ticks(self._created_at)
 
         # content forced to str
         self._content = str(content)
 
         self._pub_key = pub_key
 
-        self._tags = EventTags(tags)
+        if isinstance(tags, EventTags):
+            # TODO - change to copy instead of same obj?
+            self._tags = tags
+        else:
+            self._tags = EventTags(tags)
 
     def serialize(self):
         """
             see https://github.com/fiatjaf/nostr/blob/master/nips/01.md
         """
         if self._pub_key is None:
             raise Exception('Event::serialize can\'t be done unless pub key is set')
@@ -307,22 +357,27 @@
         """
             see https://github.com/fiatjaf/nostr/blob/master/nips/01.md
             pub key must be set to generate the id
         """
         evt_str = self.serialize()
         self._id = hashlib.sha256(evt_str.encode('utf-8')).hexdigest()
 
+    def _invalidate(self):
+        # should be called on any property set, as this will no longer be valid
+        self._id = None
+        self._sig = None
+
     def sign(self, priv_key):
         """
             see https://github.com/fiatjaf/nostr/blob/master/nips/01.md
             pub key must be set to generate the id
 
             if you were doing we an existing event for some reason you'd need to change the pub_key
             as else the sig we give won't be as expected
-
+            Eventually it might be move this into signer and always exepct use of signer...
         """
         self._get_id()
 
         # pk = secp256k1.PrivateKey(priv_key)
         pk = secp256k1.PrivateKey()
         pk.deserialize(priv_key)
 
@@ -341,15 +396,15 @@
         ret = pub_key.schnorr_verify(
             msg=bytes.fromhex(self._id),
             schnorr_sig=bytes.fromhex(self._sig),
             bip340tag='', raw=True)
 
         return ret
 
-    def event_data(self):
+    def data(self):
         return {
             'id': self._id,
             'pubkey': self._pub_key,
             'created_at': self._created_at,
             'kind': self._kind,
             'tags': self._tags.tags,
             'content': self._content,
@@ -446,16 +501,22 @@
         return 30000 <= self.kind < 40000
 
     @property
     def tags(self):
         return self._tags
 
     @tags.setter
-    def tags(self, tags) -> EventTags:
-        self._tags = EventTags(tags)
+    def tags(self, tags):
+        self._invalidate()
+        # already a EventTags obj
+        if isinstance(tags, EventTags):
+            self._tags = tags
+        # should be [[]]
+        else:
+            self._tags = EventTags(tags)
 
     def get_tags(self, tag_name):
         return self._tags.get_tags(tag_name)
 
     def get_tags_value(self, tag_name):
         return self._tags.get_tags_value(tag_name)
 
@@ -482,100 +543,114 @@
 
     @property
     def pub_key(self):
         return self._pub_key
 
     @pub_key.setter
     def pub_key(self, pub_key):
+        self._invalidate()
         self._pub_key = pub_key
 
     @property
     def id(self):
+        if self._id is None:
+            self._get_id()
         return self._id
 
     @property
     def short_id(self):
         # shorter version of id for display, note id doesn't until signing
         return util_funcs.str_tails(self.id, 4)
 
     @property
     def created_at(self) -> datetime:
         return util_funcs.ticks_as_date(self._created_at)
 
     @created_at.setter
     def created_at(self, dt):
+        self._invalidate()
         if dt is None or not isinstance(dt, (datetime, int)):
-            raise ValueError('Event::created_at: invalid value for created_at - %s' % dt)
+            raise ValueError(f'Event::created_at: invalid value for created_at - {dt}')
         elif isinstance(dt, datetime):
-            self._created_at = util_funcs.date_as_ticks(self._created_at)
+            self._created_at = util_funcs.date_as_ticks(dt)
         elif isinstance(dt, int):
             self._created_at = dt
 
     @property
     def created_at_ticks(self):
         return self._created_at
 
     @property
     def kind(self) -> int:
         return self._kind
 
+    @kind.setter
+    def kind(self, kind: int):
+        self._invalidate()
+        self._kind = kind
+
     @property
     def content(self) -> str:
         return self._content
 
-    def decrypted_content(self, priv_key, pub_key, check_kind=True):
-        """
-        dycrypts a NIP04 encoded event...
-        :param priv_key:
-        :return:
-        """
-        if check_kind and self.kind not in (Event.KIND_ENCRYPT, Event.KIND_REPUBLISH):
-            raise Exception('attempt to decrypt non encrypted event %s' % self.id)
-
-        my_enc = SharedEncrypt(priv_key)
-        msg_split = self.content.split('?iv')
-
-        try:
-            text = base64.b64decode(msg_split[0])
-            iv = base64.b64decode(msg_split[1])
-
-            if len(pub_key) == 64:
-                pub_key = '02' + pub_key
-
-            ret = my_enc.decrypt_message(text, iv, pub_key).decode('utf8')
-
-        except Exception as e:
-            raise Exception('unable to decrypt event %s using given priv_k' % priv_key)
-
-        return ret
-
-    # def encrypt_content(self, priv_key, pub_key):
-    #     my_enc = SharedEncrypt(priv_key)
-    #     if len(pub_key) == 64:
-    #         pub_key = '02' + pub_key
-    #
-    #     my_enc.derive_shared_key(pub_key)
-    #
-    #     crypt_message = my_enc.encrypt_message(bytes(self.content.encode('utf8')))
-    #     enc_message = base64.b64encode(crypt_message['text'])
-    #     iv_env = base64.b64encode(crypt_message['iv'])
-    #
-    #     return '%s?iv=%s' % (enc_message.decode(), iv_env.decode())
-
-    # FIXME:
-    #  setters should probably invalidate the id and sig as they'll need to be done again,
-    #  though only important if going to post
     @content.setter
     def content(self, content):
+        self._invalidate()
         self._content = content
 
     @property
     def sig(self):
         return self._sig
 
     def __str__(self):
         ret = super(Event, self).__str__()
-        # on signed events we can retrn something more useful
-        if self.id:
-            ret =  '%s@%s' % (self.id, self.created_at)
+        # hopefully id is set but it might not be if the event is being prepeped
+        # perhaps we should check pubkey here instead because if that exists we can gen the id
+        if self._id is not None:
+            ret = f'{self.id}@{self.created_at}'
+        return ret
+
+    def add_pow(self, target: int = 4):
+        if target < 4 or target > 64:
+            raise ValueError(f"target should be in range 4 to 64 got {target}")
+
+        val = 0
+        leading_z = 0
+        original_tags = self.tags.tags[:]
+        nonce_template = original_tags + [['nonce', '', f'{target}']]
+
+        while leading_z < target:
+            nonce_template[-1][1] = f'{val}'
+            self.tags = nonce_template
+
+            # Directly convert the hexadecimal id to an integer and calculate leading zeros
+            leading_z = (256 - int(self.id, 16).bit_length())
+            val += 1
+
+    @property
+    def pow(self):
+        # returns the events pow value - not necessarily targeted
+        return 256 - int(self.id, 16).bit_length()
+
+    def nip13_valid_pow(self, min_pow):
+        """
+            returns True if this event has valid targeted pow and that pow is >= min_pow
+            https://github.com/nostr-protocol/nips/blob/master/13.md
+            NOTE you also need to check if the event is valid!
+        """
+        ret = False
+        pow_value = self.pow
+        try:
+            nonce = self.get_tags('nonce')[0][1]
+            target_pow = int(nonce)
+            ret = pow_value >= target_pow >= min_pow
+        except Exception as e:
+            pass
+        return ret
+
+    def __lt__(self, other: 'Event'):
+        # added so we can support basic sorting, newest events will be first
+        ret = True
+        if self.created_at_ticks < other.created_at_ticks:
+            ret = False
         return ret
```

### Comparing `monstr-0.1.2/src/monstr/event/event_handlers.py` & `monstr-0.1.4/src/monstr/event/event_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 pub_k = '?no_pub_k?'
                 p_tags = EventTags(r_evt['tags']).p_tags
                 if p_tags:
                     pub_k = p_tags[0]
 
                 r_evt['react_event'] = Event(id=r_id,
                                              content='unable to find reacted to event',
-                                             pub_key=pub_k).event_data()
+                                             pub_key=pub_k).data()
 
             # add interpretation
             interpretation = EventHandler.reaction_lookup(r_evt['content'])
             r_evt['interpretation'] = interpretation
             if interpretation == 'like' and use_profile and use_profile.public_key == r_evt['pubkey']:
                 r_evt['react_event']['react_like'] = True
 
@@ -337,15 +337,15 @@
 
         ret = {}
         complete = False
 
         def _do_event(the_client: Client, sub_id: str, evts):
             nonlocal ret
             relay = the_client.url
-            ret[relay] = [c_evt.event_data() for c_evt in evts]
+            ret[relay] = [c_evt.data() for c_evt in evts]
             c_evt: Event
             self.do_event(sub_id, evts, relay)
             if self._on_fetch:
                 self._on_fetch(evts)
 
         def _complete():
             nonlocal complete
```

### Comparing `monstr-0.1.2/src/monstr/event/expire.py` & `monstr-0.1.4/src/monstr/event/expire.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/event/persist.py` & `monstr-0.1.4/src/monstr/event/persist.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/event/persist_memory.py` & `monstr-0.1.4/src/monstr/event/persist_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 for c_filter in filters:
                     if c_evt.test(c_filter):
                         ret.add(c_evt)
 
         def _updated_sort(evt_data):
             return evt_data['created_at']
 
-        ret = [c_evt.event_data() for c_evt in ret]
+        ret = [c_evt.data() for c_evt in ret]
         if self._sort_direction != SortDirection.natural:
             ret.sort(key=_updated_sort, reverse=self._sort_direction==SortDirection.newest_first)
 
         if limit is not None:
             ret = ret[:limit]
 
         return ret
```

### Comparing `monstr-0.1.2/src/monstr/event/persist_postgres.py` & `monstr-0.1.4/src/monstr/event/persist_postgres.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/event/persist_sqlite.py` & `monstr-0.1.4/src/monstr/event/persist_sqlite.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/event/persist_test.py` & `monstr-0.1.4/src/monstr/event/persist_test.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/ident/alias.py` & `monstr-0.1.4/src/monstr/ident/alias.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/ident/event_handlers.py` & `monstr-0.1.4/src/monstr/ident/event_handlers.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/ident/persist.py` & `monstr-0.1.4/src/monstr/ident/persist.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/ident/persist_test.py` & `monstr-0.1.4/src/monstr/ident/persist_test.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/ident/profile.py` & `monstr-0.1.4/src/monstr/ident/profile.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/relay/accept_handlers.py` & `monstr-0.1.4/src/monstr/relay/accept_handlers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import json
+from abc import ABC, abstractmethod
 from datetime import datetime
 from aiohttp import http_websocket
 from monstr.relay.exceptions import NostrCommandException, NostrNoticeException, NostrNotAuthenticatedException
 from monstr.event.event import Event
 from monstr.util import util_funcs, NIPSupport
 
 
-
-class AcceptReqHandler:
+class AcceptReqHandler(ABC):
     """
         request handler for relay, a request handler just has to have
         accept_post(self, ws: WebSocket, evt: Event) method that throws
         NostrCommandException if we don't want to accept message
     """
     def __init__(self, descriptive_msg=True):
         self._desc_msg = descriptive_msg
@@ -18,14 +19,35 @@
     def raise_err(self, event: Event, message: str, success: bool = False):
         if self._desc_msg:
             raise NostrCommandException(event.id, success, message)
         else:
             raise NostrNoticeException('post not accepted')
 
     def accept_post(self, ws: http_websocket, evt: Event):
+        """
+            if this method isn't happy it should use raise_err otherwise the event will be accepted
+            so AcceptReqHandler() will accept anything
+        """
+        pass
+
+
+class SubscriptionFilter(ABC):
+    """
+        similar to AcceptRequestHandler but use when deciding if we'll send an event out
+        that has matched a filter
+        for example used to only restrict kind 4 DMs to only sender/reciever
+    """
+    def __init__(self):
+        pass
+
+    @abstractmethod
+    def send_event(self, ws: http_websocket, sub, evt: Event) -> bool:
+        """
+            this method should be implemented and return True or False if to send out this event
+        """
         pass
 
 
 class LengthAcceptReqHandler(AcceptReqHandler):
     """
     use to only accept messages of set lengths, most likely upto a max size
     """
@@ -173,10 +195,116 @@
                                message=f'restricted: user {evt.pub_key} authenticated but not allowed')
 
         # no authentication done at all yet?
         except AttributeError as ae:
             raise NostrNotAuthenticatedException(f'restricted: user {evt.pub_key} not yet authenticated')
 
 
-        return ret
+class POWAcceptor(AcceptReqHandler):
+    """
+        only accept posts with a min level of pow
+    """
+    def __init__(self,
+                 min_pow: int = 16,
+                 descriptive_msg=True):
+
+        self._min_pow = min_pow
+        super().__init__(descriptive_msg)
+
+    def accept_post(self, ws: http_websocket, evt: Event):
+        evt_pow = evt.pow
+        if evt_pow < self._min_pow:
+            self.raise_err(event=evt,
+                           success=False,
+                           message=f'blocked: event does not have enough pow {evt_pow} - required {self._min_pow}')
+
+
+class ORAcceptor(AcceptReqHandler, NIPSupport):
+    """
+        returns true if any of the given accept handlers don't error
+    """
+    def __init__(self,
+                 acceptors: [AcceptReqHandler],
+                 descriptive_msg=True):
+
+        if not isinstance(acceptors, list):
+            acceptors = [acceptors]
+        self._acceptors = acceptors
+
+
+        # extract nip support if any from acceptors
+        nips = set()
+        for c_accept in self._acceptors:
+            if isinstance(c_accept, NIPSupport):
+                nips.update(set(c_accept.supported_nips))
+
+        # currently only 22 and 42 this way so thats all we worry about
+        NIPSupport.__init__(
+            self,
+            nip22=22 in nips,
+            nip42=42 in nips
+        )
+        print(self.supported_nips)
+        super().__init__(descriptive_msg)
+
 
 
+    def accept_post(self, ws: http_websocket, evt: Event):
+        accept = False
+        last_exception = None
+        auth_exception = None
+
+        for c_accept in self._acceptors:
+            try:
+                c_accept.accept_post(ws, evt)
+                accept = True
+                break
+
+            except (NostrNoticeException,
+                    NostrCommandException) as e:
+                last_exception = e
+            except NostrNotAuthenticatedException as na:
+                auth_exception = na
+
+        # if no accepter passed we'll have to raise an error
+        if accept is False:
+            # auth takes priority so we can force an auth request
+            if auth_exception:
+                raise auth_exception
+            # otherwise raise the last exception
+            else:
+                raise last_exception
+
+
+class RestrictDM(SubscriptionFilter):
+
+    def __init__(self, kinds: [int] = None):
+        super().__init__()
+        if kinds is None:
+            self._kinds = {Event.KIND_ENCRYPT, Event.KIND_GIFT_WRAP}
+        else:
+            if isinstance(kinds, int):
+                kinds = [int]
+            self._kinds = set(kinds)
+
+    def send_event(self, ws: http_websocket, sub, evt: dict) -> bool:
+        ret = False
+        if evt['kind'] in self._kinds:
+            # as we've now got to look at it turn the dict to an event obj as it'll make things easier
+            evt = Event.load(evt)
+
+            ps = set(evt.p_tags)
+            ps.add(evt.pub_key)
+
+            # who is authed on this ws
+            authed = ws.authenticated_pub_ks
+
+            for c_p in ps:
+                if c_p in authed:
+                    ret = True
+                    break
+
+            # TODO: if we failed raise auth error so we can get them to auth??
+            # if ret is False:
+            #     raise NostrNotAuthenticatedException()
+
+        return ret
```

### Comparing `monstr-0.1.2/src/monstr/relay/exceptions.py` & `monstr-0.1.4/src/monstr/relay/exceptions.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/relay/relay.py` & `monstr-0.1.4/src/monstr/relay/relay.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from aiohttp import WSCloseCode
 from aiohttp import web, http_websocket
 import json
 from json import JSONDecodeError
 from monstr.event.event import Event
 from monstr.event.persist import RelayEventStoreInterface, ARelayEventStoreInterface
 from monstr.encrypt import Keys
-from monstr.relay.accept_handlers import AcceptReqHandler
+from monstr.relay.accept_handlers import AcceptReqHandler, SubscriptionFilter
 from monstr.relay.exceptions import NostrCommandException, NostrNoticeException, NostrNotAuthenticatedException
 from monstr.util import NIPSupport, util_funcs
 
 
 # from sqlite3 import IntegrityError
 # try:
 #     import psycopg2.errors as pg_errors
@@ -72,16 +72,17 @@
 
         TODO: write some test code for each NIP...
 
     """
     VALID_CMDS = ['EVENT', 'REQ', 'CLOSE', 'AUTH']
 
     def __init__(self,
-                 store: RelayEventStoreInterface = None,
-                 accept_req_handler=None,
+                 store: RelayEventStoreInterface | ARelayEventStoreInterface = None,
+                 accept_req_handler:[AcceptReqHandler] = None,
+                 sub_filter: [SubscriptionFilter] = None,
                  max_sub=10,
                  name: str = None,
                  description: str = None,
                  pubkey: str = None,
                  contact: str = None,
                  ack_events=True,
                  request_auth: bool = False,
@@ -117,14 +118,20 @@
         # send out auth request on connect also on auth exceptions from accept_req_handlers
         self._request_auth = request_auth
 
         # convert to array of only single class handed in
         if not hasattr(self._accept_req, '__iter__'):
             self._accept_req = [self._accept_req]
 
+        # sub filters are similar to accept filter accept they are applied before we send events that matched
+        # sub filters rather than before we accept and store event we recieve
+        self._sub_filters = sub_filter
+        if self._sub_filters is not None and not hasattr(self._sub_filters, '__iter__'):
+            self._sub_filters = [self._sub_filters]
+
         # this is the server that we run as, it's created after calling start()
         # default is localhost:8080
         self._server: web.Application = None
         self._runner: web.AppRunner = None
         self._host = None
         self._port = None
         self._end_point = None
@@ -144,19 +151,25 @@
             nips.add(20)
 
         # if any _accept_req check them and see if they mean we're supporting any additional nips
         for c_accept in self._accept_req:
             if isinstance(c_accept, NIPSupport):
                 nips.update(set(c_accept.supported_nips))
 
-        # maybe we should error our here, not request auth when we have acceptors that check auth means those acceptors
-        # will always fail!
+        # if request auth is false but we have requesters that are expecting nip42 then we'll bug out to be safe
         if not self._request_auth and 42 in nips:
-            logging.debug('Relay::__init__ request_auth is False but have acceptor that requires authentication!?')
-            nips.remove(42)
+            raise Exception('Relay::__init__ request_auth is False but have acceptor that requires authentication!?')
+
+        # if request auth set nip42 True even if if we don't have acceptors using it... basically this means
+        # we'll send auth requests and auth clients but it's a little pointless because we never actually use that
+        # authentication
+        if request_auth:
+            nips.add(42)
+
+
 
         # output nip info - only named so may not be all...
         logging.info(f'Relay::__init__ maxsub={self._max_sub}, '
                      f'Deletes(NIP9)={9 in nips}, '
                      f'Event treatment(NIP16)={16 in nips}, '
                      f'Commands(NIP20)={self._ack_events}, '
                      f'Parameterized Replaceable Events(NIP33)={33 in nips}, '
@@ -357,15 +370,15 @@
             await self._do_send(ws=ws,
                                 data=err)
 
     async def _do_event(self, req_json, ws):
         if len(req_json) <= 1:
             raise NostrNoticeException('EVENT command missing event data')
 
-        evt = Event.from_JSON(req_json[1])
+        evt = Event.load(req_json[1])
         # check event sig matches pub_key
         if not evt.is_valid():
             raise NostrCommandException(event_id=evt.id,
                                         success=False,
                                         message='invalid: signature validation failed')
 
         # check against any acceptors we've been handed
@@ -400,15 +413,15 @@
         """
         tasks = set()
         for socket_id in self._ws:
             for c_sub_id in self._ws[socket_id]['subs']:
                 the_sub = self._ws[socket_id]['subs'][c_sub_id]
                 # event passes sub filter
                 if evt.test(the_sub['filter']):
-                    n_task = asyncio.create_task(self._send_event(self._ws[socket_id]['ws'], c_sub_id, evt.event_data()))
+                    n_task = asyncio.create_task(self._send_event(self._ws[socket_id]['ws'], the_sub, evt.data()))
                     tasks.add(n_task)
                     n_task.add_done_callback(tasks.discard)
 
     async def _do_sub(self, req_json, ws):
         logging.info('subscription requested - %s' % req_json)
         # get sub_id and filter fro the json
         if len(req_json) <= 1:
@@ -429,15 +442,15 @@
         if sub_id in self._ws[socket_id]['subs']:
             raise NostrNoticeException('REQ command for sub_id that already exists - %s' % sub_id)
         # this sub would put us over max for this socket
         sub_count = len(self._ws[socket_id]['subs'])
         if sub_count >= self._max_sub:
             raise NostrNoticeException('REQ new sub_id %s not allowed, already at max subs=%s' % (sub_id, self._max_sub))
 
-        self._ws[socket_id]['subs'][sub_id] = {
+        the_sub = self._ws[socket_id]['subs'][sub_id] = {
             'id': sub_id,
             'filter': filter
         }
 
         logging.info('Relay::_do_sub subscription added %s (%s)' % (sub_id, filter))
 
         # get and send any stored events we have and send back
@@ -445,15 +458,15 @@
         if self._store:
             if isinstance(self._store, ARelayEventStoreInterface):
                 evts = await self._store.get_filter(filter)
             else:
                 evts = self._store.get_filter(filter)
 
         for c_evt in evts:
-            await self._send_event(ws, sub_id, c_evt)
+            await self._send_event(ws, the_sub, c_evt)
 
         await self._send_eose(ws, sub_id)
 
     async def _do_unsub(self, req_json, ws):
         logging.info('un-subscription requested')
         if len(req_json) <= 1:
             raise NostrCommandException('REQ command missing sub_id')
@@ -470,15 +483,15 @@
         # not actual exception but this will send notice back that sub_id has been closed, might be useful to client?
         raise NostrNoticeException('CLOSE command for sub_id %s - success' % sub_id)
 
     async def _do_auth(self, auth_json, ws):
         if len(auth_json) <= 1:
             raise NostrNoticeException('AUTH command missing event data')
 
-        evt = Event.from_JSON(auth_json[1])
+        evt = Event.load(auth_json[1])
         if not evt.is_valid():
             raise NostrNoticeException('Authentication failed: auth event signature validation failed')
 
         # for now we're only checking the challenge tag, probably we should check the relay also
         # though I don't think it helps any auth who shouldnt be able to
         challenge = evt.tags.get_tags_value('challenge')
         if not challenge or challenge[0] != ws.challenge:
@@ -490,21 +503,33 @@
 
     async def _do_send(self, ws: http_websocket, data):
         try:
             await ws.send_str(json.dumps(data))
         except Exception as e:
             logging.info(f'Relay::_do_send error: {e}')
 
-    async def _send_event(self, ws: http_websocket, sub_id, evt):
-        await self._do_send(ws=ws,
-                            data=[
-                                'EVENT',
-                                sub_id,
-                                evt
-                            ])
+    async def _send_event(self, ws: http_websocket, the_sub, evt):
+        send_event = True
+        if self._sub_filters is not None:
+            for c_filter in self._sub_filters:
+                try:
+                    send_event = c_filter.send_event(ws, the_sub, evt)
+                # except NostrNotAuthenticatedException as ne:
+                #     raise ne
+                except Exception as e:
+                    logging.debug(f'Relay::_send_event error in _sub_filters, event will not be sent error {e})')
+                    send_event = False
+
+        if send_event:
+            await self._do_send(ws=ws,
+                                data=[
+                                    'EVENT',
+                                    the_sub['id'],
+                                    evt
+                                ])
 
     async def _send_eose(self, ws: http_websocket, sub_id):
         """
         NIP15 send end of stored events notice
         https://github.com/nostr-protocol/nips/blob/master/15.md
         """
         await self._do_send(ws=ws,
@@ -615,15 +640,15 @@
             }
 
             if isinstance(r.store, ARelayEventStoreInterface):
                 evts = await r.store.get_filter(filter)
             else:
                 evts = r.store.get_filter(filter)
 
-            evts = Event.latest_events_only([Event.from_JSON(c_evt) for c_evt in evts],
+            evts = Event.latest_events_only([Event.load(c_evt) for c_evt in evts],
                                             kind=Event.KIND_META)
 
 
 
 
             if evts:
                 p_attrs = json.loads(evts[0].content)
```

### Comparing `monstr-0.1.2/src/monstr/relay/relay_test.py` & `monstr-0.1.4/tests/relay_test.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/settings/handler.py` & `monstr-0.1.4/src/monstr/settings/handler.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/settings/persist.py` & `monstr-0.1.4/src/monstr/settings/persist.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/src/monstr/spam_handlers/spam_handlers.py` & `monstr-0.1.4/src/monstr/spam_handlers/spam_handlers.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/LICENSE` & `monstr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `monstr-0.1.2/pyproject.toml` & `monstr-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "aioconsole>=0.6.0",
     "aiohttp>=3.8.4",
     "aiosqlite>=0.18.0",
     "bech32>=1.2.0",
     "cachetools>=5.3.0",
     "cryptography>=39.0.1",
     "secp256k1>=0.14.0",
+    "pycryptodome>=3.20.0"
 ]
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     "clean","dist",".venv",
 ]
 [tool.hatch.build.targets.wheel]
```

