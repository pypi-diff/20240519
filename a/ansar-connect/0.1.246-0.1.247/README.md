# Comparing `tmp/ansar_connect-0.1.246.tar.gz` & `tmp/ansar_connect-0.1.247.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.246.tar", last modified: Sat May 18 01:34:30 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.247.tar", last modified: Sun May 19 02:15:53 2024, max compression
```

## Comparing `ansar_connect-0.1.246.tar` & `ansar_connect-0.1.247.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.246/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.246/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-15 01:33:06.000000 ansar_connect-0.1.246/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-15 01:32:55.000000 ansar_connect-0.1.246/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.224791 ansar_connect-0.1.246/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.224791 ansar_connect-0.1.246/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.224791 ansar_connect-0.1.246/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.246/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.246/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.246/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.246/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-18 01:34:27.000000 ansar_connect-0.1.246/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.246/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.246/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.246/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10461 2024-05-10 15:14:29.000000 ansar_connect-0.1.246/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.246/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.246/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.246/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.246/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.246/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.246/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.246/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33894 2024-05-13 17:10:04.000000 ansar_connect-0.1.246/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.246/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    39110 2024-05-15 01:30:21.000000 ansar_connect-0.1.246/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.246/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.246/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.246/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.246/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-18 01:34:30.228791 ansar_connect-0.1.246/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-18 01:34:30.000000 ansar_connect-0.1.246/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 02:15:53.834678 ansar_connect-0.1.247/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.247/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-19 02:15:53.834678 ansar_connect-0.1.247/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.247/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-15 01:33:06.000000 ansar_connect-0.1.247/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-19 02:15:53.834678 ansar_connect-0.1.247/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-15 01:32:55.000000 ansar_connect-0.1.247/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 02:15:53.830677 ansar_connect-0.1.247/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 02:15:53.830677 ansar_connect-0.1.247/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 02:15:53.834678 ansar_connect-0.1.247/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.247/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.247/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.247/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.247/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 02:15:53.834678 ansar_connect-0.1.247/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-19 02:15:50.000000 ansar_connect-0.1.247/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.247/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88788 2024-05-18 21:19:19.000000 ansar_connect-0.1.247/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.247/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10461 2024-05-10 15:14:29.000000 ansar_connect-0.1.247/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.247/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15675 2024-05-19 00:14:47.000000 ansar_connect-0.1.247/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.247/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.247/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.247/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9680 2024-05-18 21:34:58.000000 ansar_connect-0.1.247/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.247/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33894 2024-05-13 17:10:04.000000 ansar_connect-0.1.247/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.247/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42061 2024-05-18 21:24:11.000000 ansar_connect-0.1.247/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.247/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.247/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.247/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.247/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 02:15:53.834678 ansar_connect-0.1.247/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-19 02:15:53.000000 ansar_connect-0.1.247/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-19 02:15:53.000000 ansar_connect-0.1.247/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-19 02:15:53.000000 ansar_connect-0.1.247/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-19 02:15:53.000000 ansar_connect-0.1.247/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-19 02:15:53.000000 ansar_connect-0.1.247/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-19 02:15:53.000000 ansar_connect-0.1.247/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.246/LICENSE` & `ansar_connect-0.1.247/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/PKG-INFO` & `ansar_connect-0.1.247/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.246
+Version: 0.1.247
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.246/README.md` & `ansar_connect-0.1.247/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/pyproject.toml` & `ansar_connect-0.1.247/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/setup.py` & `ansar_connect-0.1.247/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.247/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.247/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.247/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.247/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/__init__.py` & `ansar_connect-0.1.247/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: f998cfe99efc82b815305705e5b5d7644d129a40
-Version: 0.1.245 (2024-05-18@13:34:27+NZST)
+Commit: f7c5f46eb529957720427b34e0d97564257ac529
+Version: 0.1.246 (2024-05-19@14:15:50+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.246/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.247/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/directory.py` & `ansar_connect-0.1.247/src/ansar/connect/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -2764,18 +2764,59 @@
 ar.bind(PubSub, PUBSUB_DISPATCH)
 
 # The public interface to the directory service.
 #
 
 ### PS-pub-0 Start of publish
 def publish(self, requested_name, create_session=None, requested_scope=ScopeOfService.WAN):
+	"""
+	Establishes a pub-sub service presence under the specified name.
+
+	:param self: async entity
+	:type self: Point
+	:param requested_name: name this object will be known by
+	:type requested_name: str
+	:param create_session: object to create on successful connection
+	:type create_session: CreateFrame
+	:param requested_scope: highest level at which to expose name
+	:type requested_scope: enumeration
+	"""
 	self.send(PublishAsName(requested_name, create_session, requested_scope), pb.house)
 
 ### PS-sub-0 Start of subscribe
 def subscribe(self, requested_search, create_session=None, requested_scope=ScopeOfService.WAN):
+	"""
+	Establishes a pub-sub client search for the specified name.
+
+	:param self: async entity
+	:type self: Point
+	:param requested_search: name to search for (regular expression)
+	:type requested_search: str
+	:param create_session: object to create on successful connection
+	:type create_session: CreateFrame
+	:param requested_scope: highest level at which to search for name
+	:type requested_scope: enumeration
+	"""
 	self.send(SubscribeToName(requested_search, create_session, requested_scope), pb.house)
 
 def clear(self, session, value=None):
+	"""
+	Shutdown the specified messaging session, i.e. Available or Delivered, or all
+	sessions associated with async object.
+
+	:param self: async entity
+	:type self: function or Point-based class
+	:param session: session notification object
+	:type session: Available or Delivered
+	:param value: completion value for the session(s)
+	:type value: any
+	"""
 	self.send(Clear(session, value), session.agent_address)
 
 def retract(self):
+	"""
+	Cancel any previous publish/subscribe for the specified async object.
+
+	:param self: async entity
+	:type self: function or Point-based class
+	"""
 	self.send(Retract(self.address), pb.house)
```

### Comparing `ansar_connect-0.1.246/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.247/src/ansar/connect/directory_if.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,63 +47,150 @@
 # Build the local published/subscribed objects.
 #
 ScopeOfService = ar.Enumeration(PROCESS=1, GROUP=2, HOST=3, LAN=4, WAN=5)
 
 #
 #
 class Published(object):
+	"""Session notification, server presence established.
+
+	:param requested_name: name the server is known by
+	:type requested_name: str
+	:param requested_scope: highest level that name has been registered 
+	:type requested_scope: enumeration
+	:param listening_ipp: network presence created on behalf
+	:type listening_ipp: HostPort
+	:param published_at: moment of publication
+	:type published_at: datetime
+	"""
 	def __init__(self, requested_name=None, requested_scope=ScopeOfService.WAN, listening_ipp=None, published_at=None):
 		self.requested_name = requested_name
 		self.requested_scope = requested_scope
 		self.listening_ipp = listening_ipp or HostPort()
 		self.published_at = published_at
 
 class NotPublished(ar.Faulted):
+	"""Session notification, server presence not established.
+
+	:param requested_name: intended name of the server
+	:type requested_name: str
+	:param reason: short description
+	:type reason: str
+	"""
 	def __init__(self, requested_name=None, reason=None):
 		ar.Faulted.__init__(self, f'cannot publish "{requested_name}"', reason)
 		self.requested_name = requested_name
 		self.reason = reason
 
 class Subscribed(object):
+	"""Session notification, client search established.
+
+	:param requested_search: name the client is looking for (regular expression)
+	:type requested_search: str
+	:param requested_scope: highest level that search has been registered 
+	:type requested_scope: enumeration
+	:param subscribed_at: moment of subscription
+	:type subscribed_at: datetime
+	"""
 	def __init__(self, requested_search=None, requested_scope=ScopeOfService.WAN, subscribed_at=None):
 		self.requested_search = requested_search
 		self.requested_scope = requested_scope
 		self.subscribed_at = subscribed_at
 
 #
 #
 class Available(object):
+	"""Session notification, transport to server established.
+
+	:param matched_search: name the client was looking for (regular expression)
+	:type matched_search: str
+	:param matched_name: name the server is known by
+	:type matched_name: str
+	:param matched_scope: level at which match was made
+	:type matched_scope: enumeration
+	:param opened_at: start of messaging
+	:type opened_at: datetime
+	:param route_key: unique id for this session
+	:type route_key: str
+	:param agent_address: internal pub-sub controller
+	:type agent_address: async address
+	"""
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, opened_at=None, route_key=None, agent_address=None):
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.opened_at = opened_at
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotAvailable(ar.Faulted):
+	"""Session notification, transport to server not established.
+
+	:param matched_search: name the client was looking for (regular expression)
+	:type matched_search: str
+	:param matched_name: name the server is known by
+	:type matched_name: str
+	:param matched_scope: level at which match was made
+	:type matched_scope: enumeration
+	:param route_key: unique id for this session
+	:type route_key: str
+	:param reason: why the session could not proceed
+	:type reason: str
+	:param agent_address: internal pub-sub controller
+	:type agent_address: async address
+	"""
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, agent_address=None):
 		ar.Faulted.__init__(self, 'no subsciber peer', reason)
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.reason = reason
 		self.agent_address = agent_address
 
 class Delivered(object):
+	"""Session notification, transport to client established.
+
+	:param matched_search: name the client was looking for (regular expression)
+	:type matched_search: str
+	:param matched_name: name the server is known by
+	:type matched_name: str
+	:param matched_scope: level at which match was made
+	:type matched_scope: enumeration
+	:param opened_at: start of messaging
+	:type opened_at: datetime
+	:param route_key: unique id for this session
+	:type route_key: str
+	:param agent_address: internal pub-sub controller
+	:type agent_address: async address
+	"""
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, opened_at=None, route_key=None, agent_address=None):
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.opened_at = opened_at
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotDelivered(ar.Faulted):
+	"""Session notification, transport to client not established.
+
+	:param matched_search: name the client was looking for (regular expression)
+	:type matched_search: str
+	:param matched_name: name the server is known by
+	:type matched_name: str
+	:param matched_scope: level at which match was made
+	:type matched_scope: enumeration
+	:param route_key: unique id for this session
+	:type route_key: str
+	:param reason: why the session could not proceed
+	:type reason: str
+	:param agent_address: internal pub-sub controller
+	:type agent_address: async address
+	"""
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, agent_address=None):
 		ar.Faulted.__init__(self, 'no publisher peer', reason)
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.reason = reason
@@ -111,24 +198,52 @@
 
 class Clear(object):
 	def __init__(self, session=None, value=None):
 		self.session = session
 		self.value = value
 
 class Cleared(object):
+	"""Session notification, shutdown of transport by local end.
+
+	:param matched_search: name the client was looking for (regular expression)
+	:type matched_search: str
+	:param matched_name: name the server is known by
+	:type matched_name: str
+	:param matched_scope: level at which match was made
+	:type matched_scope: enumeration
+	:param route_key: unique id for this session
+	:type route_key: str
+	:param reason: why the session could not proceed
+	:type reason: str
+	:param value: result of session
+	:type value: any
+	"""
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, value=None):
 		ar.Faulted.__init__(self, 'peer cleared', reason)
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.reason = reason
 		self.value = value
 
 class Dropped(ar.Faulted):
+	"""Session notification, shutdown of transport by remote end.
+
+	:param matched_search: name the client was looking for (regular expression)
+	:type matched_search: str
+	:param matched_name: name the server is known by
+	:type matched_name: str
+	:param matched_scope: level at which match was made
+	:type matched_scope: enumeration
+	:param route_key: unique id for this session
+	:type route_key: str
+	:param reason: why the session could not proceed
+	:type reason: str
+	"""
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None):
 		ar.Faulted.__init__(self, 'peer dropped', reason)
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.reason = reason
```

### Comparing `ansar_connect-0.1.246/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.247/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/group_if.py` & `ansar_connect-0.1.247/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/grouping.py` & `ansar_connect-0.1.247/src/ansar/connect/grouping.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,26 +37,51 @@
 	'GroupUpdate',
 	'AddressGroup',
 	'GroupObject',
 ]
 
 # The specification.
 class GroupTable(object):
+	"""Table of objects that create runtime objects, e.g. manage multiple connections.
+
+	:param member_frame: list of named CreateFrames
+	:type member_frame: dict
+	"""
 	def __init__(self, **member_frame):
 		if 'member_frame' in member_frame or 'create' in member_frame or 'update' in member_frame:
 			raise ValueError('names of members would hide GroupTable methods')
 		self.member_frame = member_frame
 
 	def create(self, owner, get_ready=None, session=None, resident_code=False, until_stopped=False):
+		"""Create a child instance of `AddressGroup`. Return the address of the new object.
+
+		:param owner: async object to receive GroupUpdate messages
+		:type owner: Point
+		:param get_ready: time limit on achieving the ready state, or None
+		:type get_ready: float
+		:param session: object to be created at Ready state, or None
+		:type session: CreateFrame
+		:param resident_code: facilitate a series of sessions
+		:type resident_code: bool
+		:param until_stopped: a flag passed to AddressGroup
+		:type until_stopped: bool
+		:rtype: an ansar address
+		"""
 		for k in self.member_frame.keys():
 			setattr(self, k, None)	# Fill with blanks.
 		a = owner.create(AddressGroup, self.member_frame, session=session, resident_code=resident_code, get_ready=get_ready, until_stopped=until_stopped)
 		return a
 
 	def update(self, message):
+		"""Process a GroupUpdate message from the AddressGroup object.
+
+		:param message: acquire a new address or lose an existing address
+		:type message: GroupUpdate
+		:rtype: None
+		"""
 		if message.key in self.member_frame:
 			setattr(self, message.key, message.address)
 
 # Runtime image.
 class GroupUpdate(object):
 	def __init__(self, key=None, address=None):
 		self.key = key
@@ -87,14 +112,27 @@
 class CLEARING: pass
 class RUNNING: pass
 
 LATCH_ID = 1
 SESSION_ID = 2
 
 class AddressGroup(ar.Point, ar.StateMachine):
+	"""Manage a collection of objects that are acquiring addresses, e.g. network connections.
+
+	:param table: table of named CreateFrames
+	:type table: dict
+	:param session: object to be created at ready state, or None
+	:type session: CreateFrame
+	:param resident_code: facilitate a series of sessions
+	:type resident_code: bool
+	:param get_ready: time limit on achieving the ready state, or None
+	:type get_ready: float
+	:param until_stopped: override the completion value with the session completion
+	:type until_stopped: bool
+	"""
 	def __init__(self, table, session=None, resident_code=False, get_ready=None, until_stopped=False):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.table = table						# Rows of CreateFrames.
 		self.session = session					# The object to be created or null.
 		self.resident_code = resident_code		# Is this an endless series of sessions.
 		self.get_ready = get_ready				# Limit the setup time.
```

### Comparing `ansar_connect-0.1.246/src/ansar/connect/moving.py` & `ansar_connect-0.1.247/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/networking.py` & `ansar_connect-0.1.247/src/ansar/connect/networking.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,25 @@
 class CLOSING: pass
 class ACCEPTING: pass
 class READY: pass
 
 #
 #
 class ConnectToAddress(ar.Point, ar.StateMachine):
+	"""Maintain a connection to an IP address and port, perform retries.
+
+	:param ipp: IP address and port to connect to
+	:type ipp: HostPort
+	:param keep_connected: restart retry sequence after successful connect
+	:type keep_connected: bool
+	:param session: object to be created on connection, or None
+	:type session: CreateFrame
+	:param group_address: where to forward session messages, or None
+	:type group_address: async address
+	"""
 	def __init__(self, ipp, keep_connected=True, session=None, group_address=None):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.ipp = ipp
 		self.keep_connected = keep_connected
 		self.session = session
 		self.group_address = group_address
@@ -218,14 +229,23 @@
 ar.bind(ConnectToAddress, CONNECT_TO_ADDRESS_DISPATCH)
 
 #
 #
 LISTEN_RETRY = ar.RetryIntervals(first_steps=[], regular_steps=4.0, randomized=0.25)
 
 class ListenAtAddress(ar.Point, ar.StateMachine):
+	"""Maintain a network presence at an IP address and port.
+
+	:param ipp: IP address and port to listen at
+	:type ipp: HostPort
+	:param session: object to be created on accept, or None
+	:type session: CreateFrame
+	:param group_address: where to forward session messages, or None
+	:type group_address: async address
+	"""
 	def __init__(self, ipp, session=None, group_address=None):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.ipp = ipp
 		self.session = session
 		self.group_address = group_address
 
@@ -374,14 +394,27 @@
 }
 
 ar.bind(ListenAtAddress, LISTEN_AT_ADDRESS_DISPATCH)
 
 #
 # Subscribe/Publish
 class SubscribeToListing(ar.Point, ar.StateMachine):
+	"""Maintain a connection to a published name.
+
+	:param listing: the name of interest (not a regular expression)
+	:type listing: str
+	:param scope: highest level to look for a match
+	:type scope: enumeration
+	:param keep_connected: allow for multiple sessions
+	:type keep_connected: bool
+	:param session: object to be created on connection, or None
+	:type session: CreateFrame
+	:param group_address: where to forward session messages, or None
+	:type group_address: async address
+	"""
 	def __init__(self, listing, scope=ScopeOfService.WAN, keep_connected=True, session=None, group_address=None):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.listing = listing
 		self.scope = scope
 		self.keep_connected = keep_connected
 		self.session = session
@@ -531,14 +564,23 @@
 }
 
 ar.bind(SubscribeToListing, SUBSCRIBE_TO_LISTING_DISPATCH)
 
 #
 #
 class PublishAListing(ar.Point, ar.StateMachine):
+	"""Maintain a network presence at a name.
+
+	:param listing: the name this object will be known by
+	:type listing: str
+	:param session: object to be created on delivery, or None
+	:type session: CreateFrame
+	:param group_address: where to forward session messages, or None
+	:type group_address: async address
+	"""
 	def __init__(self, listing, scope=ScopeOfService.WAN, session=None, group_address=None):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.listing = listing
 		self.scope = scope
 		self.session = session
 		self.group_address = group_address
@@ -666,14 +708,25 @@
 }
 
 ar.bind(PublishAListing, PUBLISH_A_LISTING_DISPATCH)
 
 #
 #
 class SubscribeToSearch(ar.Point, ar.StateMachine):
+	"""Maintain connections with multiple published names.
+
+	:param listing: the names to search for (regular expression)
+	:type listing: str
+	:param scope: highest level to look for a match
+	:type scope: enumeration
+	:param session: object to be created on connection, or None
+	:type session: CreateFrame
+	:param group_address: where to forward session messages, or None
+	:type group_address: async address
+	"""
 	def __init__(self, search, scope=ScopeOfService.WAN, session=None, group_address=None):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.search = search
 		self.scope = scope
 		self.session = session
 		self.group_address = group_address
```

### Comparing `ansar_connect-0.1.246/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.247/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/node.py` & `ansar_connect-0.1.247/src/ansar/connect/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -258,15 +258,40 @@
 #
 #
 def create_node(object_type, *fixed_value,
 	factory_settings=None, factory_input=None, factory_variables=None,
 	parameter_passing=node_passing, parameter_table=None,
 	upgrade=None, logs=ar.log_to_nowhere,
 	scope=ScopeOfService.PROCESS, **key_value):
+	"""Creates an async pub-sub process shim around a "main" async object. Returns nothing.
 
+	:param object_type: the type of an async object to be instantiated
+	:type object_type: a function or a Point-based class
+	:param fixed_value: position args to forward to the object
+	:type fixed_value: tuple
+	:param factory_settings: persistent values
+	:type factory_settings: instance of a registered class
+	:param factory_input: per-invocation values
+	:type factory_input: instance of a registered class
+	:param factory_variables: host environment values
+	:type factory_variables: instance of a registered class
+	:param parameter_passing: method for parsing sys.argv[]
+	:type parameter_passing: a function
+	:param parameter_table: table of sub-commands and their association functions
+	:type parameter_table: dict
+	:param upgrade: function that accepts old versions of settings/input and produces the current version
+	:type upgrade: function
+	:param logs: a callable object expecting to receive log objects
+	:type logs: function or class with __call__ method
+	:param scope: level of the internal directory object
+	:type scope: enumeration
+	:param key_value: named args to forward to the object
+	:type key_value: dict
+	:rtype: None
+	"""
 	node_settings.node_scope = scope
 
 	ar.create_object(object_type, *fixed_value,
 		factory_settings=factory_settings, factory_input=factory_input, factory_variables=factory_variables,
 		parameter_passing=parameter_passing, parameter_table=parameter_table,
 		start_vector=node_vector,
 		upgrade=upgrade, logs=logs, properties=NodeProperties, **key_value)
```

### Comparing `ansar_connect-0.1.246/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.247/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/procedure.py` & `ansar_connect-0.1.247/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/product.py` & `ansar_connect-0.1.247/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/socketry.py` & `ansar_connect-0.1.247/src/ansar/connect/socketry.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,21 @@
 ]
 
 #
 #
 LOCAL_HOST = '127.0.0.1'
 
 class HostPort(object):
+	"""Combination of an IP address or name, and a port number.
+
+	:param host: IP address or name
+	:type host: str
+	:param port: network port
+	:type port: int
+	"""
 	def __init__(self, host=None, port=None):
 		self.host = host
 		self.port = port
 	
 	def __str__(self):
 		return f'{self.host}:{self.port}'
 
@@ -123,14 +130,23 @@
         self.block = block
 
 ar.bind(Blob, object_schema={'block': ar.Block()})
 
 #
 #
 class CreateFrame(object):
+	"""Capture values needed for async object creation.
+
+	:param object_type: type to be created
+	:type object_type: function or Point-based class
+	:param args: positional parameters
+	:type args: tuple
+	:param kw: named parameters
+	:type kw: dict
+	"""
 	def __init__(self, object_type, *args, **kw):
 		self.object_type = object_type
 		self.args = args
 		self.kw = kw
 
 # Control messages sent to the sockets thread
 # via the control channel.
@@ -150,44 +166,102 @@
 
 class StopListening(object):
 	def __init__(self, listening_ipp=None):
 		self.listening_ipp = listening_ipp or HostPort()
 
 # Update messages from sockets thread to app.
 class Listening(object):
+	"""Session notification, server presence established.
+
+	:param requested_ipp: IP and port to listen at
+	:type requested_ipp: HostPort
+	:param listening_ipp: established IP and port
+	:type listening_ipp: HostPort
+	:param encrypted: is the client encrypting
+	:type encrypted: bool
+	"""
 	def __init__(self, requested_ipp=None, listening_ipp=None, encrypted=False):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.listening_ipp = listening_ipp or HostPort()
 		self.encrypted = encrypted
 
 class Accepted(object):
+	"""Session notification, transport to client established.
+
+	:param requested_ipp: IP and port listening at
+	:type requested_ipp: HostPort
+	:param accepted_ipp: local IP and port
+	:type accepted_ipp: HostPort
+	:param remote_address: address of SocketProxy
+	:type remote_address: async address
+	:param opened_at: moment of acceptance
+	:type opened_at: datetime
+	"""
 	def __init__(self, listening_ipp=None, accepted_ipp=None, remote_address=None, opened_at=None):
 		self.listening_ipp = listening_ipp or HostPort()
 		self.accepted_ipp = accepted_ipp or HostPort()
 		self.remote_address = remote_address
 		self.opened_at = opened_at
 
 class Connected(object):
+	"""Session notification, transport to server established.
+
+	:param requested_ipp: IP and port to connect to
+	:type requested_ipp: HostPort
+	:param connected_ipp: local IP and port
+	:type connected_ipp: HostPort
+	:param remote_address: address of SocketProxy
+	:type remote_address: async address
+	:param opened_at: moment of connection
+	:type opened_at: datetime
+	"""
 	def __init__(self, requested_ipp=None, connected_ipp=None, remote_address=None, opened_at=None):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.connected_ipp = connected_ipp or HostPort()
 		self.remote_address = remote_address
 		self.opened_at = opened_at
 
 class NotListening(ar.Faulted):
+	"""Session notification, server not established.
+
+	:param requested_ipp: IP and port to listen at
+	:type requested_ipp: HostPort
+	:param error_code: platform error number
+	:type error_code: int
+	:param error_text: platform error message
+	:type error_text: str
+	"""
 	def __init__(self, requested_ipp=None, error_code=0, error_text=None):
 		ar.Faulted.__init__(self, f'cannot listen at "{requested_ipp}"', error_text, exit_code=error_code)
 		self.requested_ipp = requested_ipp or HostPort()
 
 class NotAccepted(ar.Faulted):
+	"""Session notification, transport to client not established.
+
+	:param listening_ipp: IP and port listening at
+	:type listening_ipp: HostPort
+	:param error_code: platform error number
+	:type error_code: int
+	:param error_text: platform error message
+	:type error_text: str
+	"""
 	def __init__(self, listening_ipp=None, error_code=0, error_text=None):
 		ar.Faulted.__init__(self, f'cannot accept at "{listening_ipp}"', error_text, exit_code=error_code)
 		self.listening_ipp = listening_ipp or HostPort()
 
 class NotConnected(ar.Faulted):
+	"""Session notification, transport to server established.
+
+	:param requested_ipp: IP and port to connect to
+	:type requested_ipp: HostPort
+	:param error_code: platform error number
+	:type error_code: int
+	:param error_text: platform error message
+	:type error_text: str
+	"""
 	def __init__(self, requested_ipp=None, error_code=0, error_text=None):
 		ar.Faulted.__init__(self, f'cannot connect to "{requested_ipp}"', error_text, exit_code=error_code)
 		self.requested_ipp = requested_ipp or HostPort()
 
 CONTROL_SCHEMA = {
 	'requested_ipp': ar.UserDefined(HostPort),
 	'controller_address': ar.Address(),
@@ -215,25 +289,48 @@
 ar.bind(NotListening, object_schema=CONTROL_SCHEMA)
 ar.bind(NotAccepted, object_schema=CONTROL_SCHEMA)
 ar.bind(NotConnected, object_schema=CONTROL_SCHEMA)
 
 # Session termination messages. Handshake between app
 # and sockets thread to cleanly terminate a connection.
 class Close(object):
+	"""Session control, terminate the messaging transport.
+
+	:param value: completion value for the session
+	:type value: any
+	"""
 	def __init__(self, value=None):
 		self.value = value
 
 class Closed(ar.Faulted):
+	"""Session notification, local termination of the messaging transport.
+
+	:param value: completion value for the session
+	:type value: any
+	:param reason: short description
+	:type reason: str
+	:param opened_ipp: local IP address and port number
+	:type opened_ipp: HostPort
+	:param opened_at: moment of termination
+	:type opened_at: datetime
+	"""
 	def __init__(self, value=None, reason=None, opened_ipp=None, opened_at=None):
 		ar.Faulted.__init__(self, f'closed {opened_ipp}', reason)
 		self.value = value
 		self.opened_ipp = opened_ipp or HostPort()
 		self.opened_at = opened_at
 
 class Abandoned(ar.Faulted):
+	"""Session notification, remote termination of the messaging transport.
+
+	:param opened_ipp: local IP address and port number
+	:type opened_ipp: HostPort
+	:param opened_at: moment of termination
+	:type opened_at: datetime
+	"""
 	def __init__(self, opened_ipp=None, opened_at=None):
 		ar.Faulted.__init__(self, f'abandoned by {opened_ipp}')
 		self.opened_ipp = opened_ipp or HostPort()
 		self.opened_at = opened_at
 
 ENDING_SCHEMA = {
 	'value': ar.Any,
```

### Comparing `ansar_connect-0.1.246/src/ansar/connect/standard.py` & `ansar_connect-0.1.247/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/transporting.py` & `ansar_connect-0.1.247/src/ansar/connect/transporting.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,18 +41,44 @@
 	root.select(ar.Completed)
 
 ar.AddOn(create_sockets, stop_sockets)
 
 #
 #
 def connect(self, requested_ipp, session=None, encrypted=False):
+	"""
+	Initiates a network connection to the specified IP
+	address and port number.
+
+	:param self: async entity
+	:type self: Point
+	:param requested_ipp: host and port to connect to
+	:type requested_ipp: HostPort
+	:param session: object to create on successful connection
+	:type session: CreateFrame
+	:param encrypted: is the server encrypting
+	:type encrypted: bool
+	"""
 	ts.channel.send(ConnectStream(requested_ipp=requested_ipp, create_session=session, encrypted=encrypted), self.address)
 
 #
 #
 def listen(self, requested_ipp, session=None, encrypted=False):
+	"""
+	Establishes a network presence at the specified IP
+	address and port number.
+
+	:param self: async entity
+	:type self: Point
+	:param requested_ipp: host and port to listen at
+	:type requested_ipp: HostPort
+	:param session: object to create on successful connection
+	:type session: CreateFrame
+	:param encrypted: is the client encrypting
+	:type encrypted: bool
+	"""
 	ts.channel.send(ListenForStream(requested_ipp=requested_ipp, create_session=session, encrypted=encrypted), self.address)
 
 #
 #
 def stop_listen(self, requested_ipp):
 	ts.channel.send(StopListening(requested_ipp), self.address)
```

### Comparing `ansar_connect-0.1.246/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.247/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar/connect/wan.py` & `ansar_connect-0.1.247/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.246/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.247/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.246
+Version: 0.1.247
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.246/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.247/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

