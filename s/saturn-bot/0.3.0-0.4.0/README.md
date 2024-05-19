# Comparing `tmp/saturn_bot-0.3.0.tar.gz` & `tmp/saturn_bot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn_bot-0.3.0.tar", max compression
+gzip compressed data, was "saturn_bot-0.4.0.tar", max compression
```

## Comparing `saturn_bot-0.3.0.tar` & `saturn_bot-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    16726 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/LICENSE
--rw-r--r--   0        0        0       70 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/README.md
--rw-r--r--   0        0        0     1471 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      370 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/__init__.py
--rw-r--r--   0        0        0      201 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/plugin/__init__.py
--rw-r--r--   0        0        0     1814 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/plugin/grpc_controller_pb2.py
--rw-r--r--   0        0        0      471 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/plugin/grpc_controller_pb2.pyi
--rw-r--r--   0        0        0     2934 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/plugin/grpc_controller_pb2_grpc.py
--rw-r--r--   0        0        0      201 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/protocol/__init__.py
--rw-r--r--   0        0        0      201 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/protocol/v1/__init__.py
--rw-r--r--   0        0        0     6174 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/protocol/v1/saturnbot_pb2.py
--rw-r--r--   0        0        0     4463 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/protocol/v1/saturnbot_pb2.pyi
--rw-r--r--   0        0        0    11868 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/protocol/v1/saturnbot_pb2_grpc.py
--rw-r--r--   0        0        0     5904 2024-04-28 16:53:23.336546 saturn_bot-0.3.0/saturn_bot/sdk.py
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 saturn_bot-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    16726 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/LICENSE
+-rw-r--r--   0        0        0       70 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/README.md
+-rw-r--r--   0        0        0     1471 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      322 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/__init__.py
+-rw-r--r--   0        0        0      201 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/plugin/__init__.py
+-rw-r--r--   0        0        0     1814 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/plugin/grpc_controller_pb2.py
+-rw-r--r--   0        0        0      471 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/plugin/grpc_controller_pb2.pyi
+-rw-r--r--   0        0        0     2934 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/plugin/grpc_controller_pb2_grpc.py
+-rw-r--r--   0        0        0      201 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/protocol/__init__.py
+-rw-r--r--   0        0        0      201 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/protocol/v1/__init__.py
+-rw-r--r--   0        0        0     9222 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/protocol/v1/saturnbot_pb2.py
+-rw-r--r--   0        0        0     7207 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/protocol/v1/saturnbot_pb2.pyi
+-rw-r--r--   0        0        0    11868 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/protocol/v1/saturnbot_pb2_grpc.py
+-rw-r--r--   0        0        0     7406 2024-05-19 14:57:33.502406 saturn_bot-0.4.0/saturn_bot/sdk.py
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 saturn_bot-0.4.0/PKG-INFO
```

### Comparing `saturn_bot-0.3.0/LICENSE` & `saturn_bot-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saturn_bot-0.3.0/pyproject.toml` & `saturn_bot-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [[tool.mypy.overrides]]
 module = "grpc_health.*"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "saturn-bot"
-version = "0.3.0"
+version = "0.4.0"
 description = "Synchronize and refactor repositories with ease."
 authors = ["Markus Meyer <hydrantanderwand@gmail.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/wndhydrnt/saturn-bot-protocol"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `saturn_bot-0.3.0/saturn_bot/plugin/grpc_controller_pb2.py` & `saturn_bot-0.4.0/saturn_bot/plugin/grpc_controller_pb2.py`

 * *Files identical despite different names*

### Comparing `saturn_bot-0.3.0/saturn_bot/plugin/grpc_controller_pb2_grpc.py` & `saturn_bot-0.4.0/saturn_bot/plugin/grpc_controller_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `saturn_bot-0.3.0/saturn_bot/protocol/v1/saturnbot_pb2.py` & `saturn_bot-0.4.0/saturn_bot/protocol/v1/saturnbot_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,50 +14,72 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&saturn_bot/protocol/v1/saturnbot.proto\x12\x0bprotocol.v1\"[\n\x15\x45xecuteActionsRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12.\n\x07\x63ontext\x18\x02 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\"=\n\x16\x45xecuteActionsResponse\x12\x19\n\x05\x65rror\x18\x01 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error\"G\n\x15\x45xecuteFiltersRequest\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\"S\n\x16\x45xecuteFiltersResponse\x12\x14\n\x05match\x18\x01 \x01(\x08R\x05match\x12\x19\n\x05\x65rror\x18\x02 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error\"\x90\x01\n\x10GetPluginRequest\x12\x41\n\x06\x63onfig\x18\x01 \x03(\x0b\x32).protocol.v1.GetPluginRequest.ConfigEntryR\x06\x63onfig\x1a\x39\n\x0b\x43onfigEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"h\n\x11GetPluginResponse\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1a\n\x08priority\x18\x02 \x01(\x05R\x08priority\x12\x19\n\x05\x65rror\x18\x03 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error\"B\n\x07\x43ontext\x12\x37\n\nrepository\x18\x01 \x01(\x0b\x32\x17.protocol.v1.RepositoryR\nrepository\"\x8c\x01\n\nRepository\x12\x1b\n\tfull_name\x18\x01 \x01(\tR\x08\x66ullName\x12$\n\x0e\x63lone_url_http\x18\x02 \x01(\tR\x0c\x63loneUrlHttp\x12\"\n\rclone_url_ssh\x18\x03 \x01(\tR\x0b\x63loneUrlSsh\x12\x17\n\x07web_url\x18\x04 \x01(\tR\x06webUrl\"C\n\x11OnPrClosedRequest\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\"9\n\x12OnPrClosedResponse\x12\x19\n\x05\x65rror\x18\x01 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error\"D\n\x12OnPrCreatedRequest\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\":\n\x13OnPrCreatedResponse\x12\x19\n\x05\x65rror\x18\x01 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error\"C\n\x11OnPrMergedRequest\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\"9\n\x12OnPrMergedResponse\x12\x19\n\x05\x65rror\x18\x01 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error2\x8d\x04\n\rPluginService\x12[\n\x0e\x45xecuteActions\x12\".protocol.v1.ExecuteActionsRequest\x1a#.protocol.v1.ExecuteActionsResponse\"\x00\x12[\n\x0e\x45xecuteFilters\x12\".protocol.v1.ExecuteFiltersRequest\x1a#.protocol.v1.ExecuteFiltersResponse\"\x00\x12L\n\tGetPlugin\x12\x1d.protocol.v1.GetPluginRequest\x1a\x1e.protocol.v1.GetPluginResponse\"\x00\x12O\n\nOnPrClosed\x12\x1e.protocol.v1.OnPrClosedRequest\x1a\x1f.protocol.v1.OnPrClosedResponse\"\x00\x12R\n\x0bOnPrCreated\x12\x1f.protocol.v1.OnPrCreatedRequest\x1a .protocol.v1.OnPrCreatedResponse\"\x00\x12O\n\nOnPrMerged\x12\x1e.protocol.v1.OnPrMergedRequest\x1a\x1f.protocol.v1.OnPrMergedResponse\"\x00\x42n\n\x0f\x63om.protocol.v1B\x0eSaturnbotProtoP\x01\xa2\x02\x03PXX\xaa\x02\x0bProtocol.V1\xca\x02\x0bProtocol\\V1\xe2\x02\x17Protocol\\V1\\GPBMetadata\xea\x02\x0cProtocol::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&saturn_bot/protocol/v1/saturnbot.proto\x12\x0bprotocol.v1\"[\n\x15\x45xecuteActionsRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12.\n\x07\x63ontext\x18\x02 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\"\xef\x02\n\x16\x45xecuteActionsResponse\x12\x19\n\x05\x65rror\x18\x01 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x12Z\n\rtemplate_vars\x18\x02 \x03(\x0b\x32\x35.protocol.v1.ExecuteActionsResponse.TemplateVarsEntryR\x0ctemplateVars\x12T\n\x0bplugin_data\x18\x03 \x03(\x0b\x32\x33.protocol.v1.ExecuteActionsResponse.PluginDataEntryR\npluginData\x1a?\n\x11TemplateVarsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a=\n\x0fPluginDataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x08\n\x06_error\"G\n\x15\x45xecuteFiltersRequest\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\"\x85\x03\n\x16\x45xecuteFiltersResponse\x12\x14\n\x05match\x18\x01 \x01(\x08R\x05match\x12\x19\n\x05\x65rror\x18\x02 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x12Z\n\rtemplate_vars\x18\x03 \x03(\x0b\x32\x35.protocol.v1.ExecuteFiltersResponse.TemplateVarsEntryR\x0ctemplateVars\x12T\n\x0bplugin_data\x18\x04 \x03(\x0b\x32\x33.protocol.v1.ExecuteFiltersResponse.PluginDataEntryR\npluginData\x1a?\n\x11TemplateVarsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a=\n\x0fPluginDataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x08\n\x06_error\"\x90\x01\n\x10GetPluginRequest\x12\x41\n\x06\x63onfig\x18\x01 \x03(\x0b\x32).protocol.v1.GetPluginRequest.ConfigEntryR\x06\x63onfig\x1a\x39\n\x0b\x43onfigEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"h\n\x11GetPluginResponse\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1a\n\x08priority\x18\x02 \x01(\x05R\x08priority\x12\x19\n\x05\x65rror\x18\x03 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error\"\x9b\x02\n\x07\x43ontext\x12\x37\n\nrepository\x18\x01 \x01(\x0b\x32\x17.protocol.v1.RepositoryR\nrepository\x12@\n\x0cpull_request\x18\x02 \x01(\x0b\x32\x18.protocol.v1.PullRequestH\x00R\x0bpullRequest\x88\x01\x01\x12\x45\n\x0bplugin_data\x18\x03 \x03(\x0b\x32$.protocol.v1.Context.PluginDataEntryR\npluginData\x1a=\n\x0fPluginDataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x0f\n\r_pull_request\">\n\x0bPullRequest\x12\x16\n\x06number\x18\x01 \x01(\x03R\x06number\x12\x17\n\x07web_url\x18\x02 \x01(\tR\x06webUrl\"\x8c\x01\n\nRepository\x12\x1b\n\tfull_name\x18\x01 \x01(\tR\x08\x66ullName\x12$\n\x0e\x63lone_url_http\x18\x02 \x01(\tR\x0c\x63loneUrlHttp\x12\"\n\rclone_url_ssh\x18\x03 \x01(\tR\x0b\x63loneUrlSsh\x12\x17\n\x07web_url\x18\x04 \x01(\tR\x06webUrl\"C\n\x11OnPrClosedRequest\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\"9\n\x12OnPrClosedResponse\x12\x19\n\x05\x65rror\x18\x01 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error\"D\n\x12OnPrCreatedRequest\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\":\n\x13OnPrCreatedResponse\x12\x19\n\x05\x65rror\x18\x01 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error\"C\n\x11OnPrMergedRequest\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x14.protocol.v1.ContextR\x07\x63ontext\"9\n\x12OnPrMergedResponse\x12\x19\n\x05\x65rror\x18\x01 \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error2\x8d\x04\n\rPluginService\x12[\n\x0e\x45xecuteActions\x12\".protocol.v1.ExecuteActionsRequest\x1a#.protocol.v1.ExecuteActionsResponse\"\x00\x12[\n\x0e\x45xecuteFilters\x12\".protocol.v1.ExecuteFiltersRequest\x1a#.protocol.v1.ExecuteFiltersResponse\"\x00\x12L\n\tGetPlugin\x12\x1d.protocol.v1.GetPluginRequest\x1a\x1e.protocol.v1.GetPluginResponse\"\x00\x12O\n\nOnPrClosed\x12\x1e.protocol.v1.OnPrClosedRequest\x1a\x1f.protocol.v1.OnPrClosedResponse\"\x00\x12R\n\x0bOnPrCreated\x12\x1f.protocol.v1.OnPrCreatedRequest\x1a .protocol.v1.OnPrCreatedResponse\"\x00\x12O\n\nOnPrMerged\x12\x1e.protocol.v1.OnPrMergedRequest\x1a\x1f.protocol.v1.OnPrMergedResponse\"\x00\x42n\n\x0f\x63om.protocol.v1B\x0eSaturnbotProtoP\x01\xa2\x02\x03PXX\xaa\x02\x0bProtocol.V1\xca\x02\x0bProtocol\\V1\xe2\x02\x17Protocol\\V1\\GPBMetadata\xea\x02\x0cProtocol::V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'saturn_bot.protocol.v1.saturnbot_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\017com.protocol.v1B\016SaturnbotProtoP\001\242\002\003PXX\252\002\013Protocol.V1\312\002\013Protocol\\V1\342\002\027Protocol\\V1\\GPBMetadata\352\002\014Protocol::V1'
+  _globals['_EXECUTEACTIONSRESPONSE_TEMPLATEVARSENTRY']._options = None
+  _globals['_EXECUTEACTIONSRESPONSE_TEMPLATEVARSENTRY']._serialized_options = b'8\001'
+  _globals['_EXECUTEACTIONSRESPONSE_PLUGINDATAENTRY']._options = None
+  _globals['_EXECUTEACTIONSRESPONSE_PLUGINDATAENTRY']._serialized_options = b'8\001'
+  _globals['_EXECUTEFILTERSRESPONSE_TEMPLATEVARSENTRY']._options = None
+  _globals['_EXECUTEFILTERSRESPONSE_TEMPLATEVARSENTRY']._serialized_options = b'8\001'
+  _globals['_EXECUTEFILTERSRESPONSE_PLUGINDATAENTRY']._options = None
+  _globals['_EXECUTEFILTERSRESPONSE_PLUGINDATAENTRY']._serialized_options = b'8\001'
   _globals['_GETPLUGINREQUEST_CONFIGENTRY']._options = None
   _globals['_GETPLUGINREQUEST_CONFIGENTRY']._serialized_options = b'8\001'
+  _globals['_CONTEXT_PLUGINDATAENTRY']._options = None
+  _globals['_CONTEXT_PLUGINDATAENTRY']._serialized_options = b'8\001'
   _globals['_EXECUTEACTIONSREQUEST']._serialized_start=55
   _globals['_EXECUTEACTIONSREQUEST']._serialized_end=146
-  _globals['_EXECUTEACTIONSRESPONSE']._serialized_start=148
-  _globals['_EXECUTEACTIONSRESPONSE']._serialized_end=209
-  _globals['_EXECUTEFILTERSREQUEST']._serialized_start=211
-  _globals['_EXECUTEFILTERSREQUEST']._serialized_end=282
-  _globals['_EXECUTEFILTERSRESPONSE']._serialized_start=284
-  _globals['_EXECUTEFILTERSRESPONSE']._serialized_end=367
-  _globals['_GETPLUGINREQUEST']._serialized_start=370
-  _globals['_GETPLUGINREQUEST']._serialized_end=514
-  _globals['_GETPLUGINREQUEST_CONFIGENTRY']._serialized_start=457
-  _globals['_GETPLUGINREQUEST_CONFIGENTRY']._serialized_end=514
-  _globals['_GETPLUGINRESPONSE']._serialized_start=516
-  _globals['_GETPLUGINRESPONSE']._serialized_end=620
-  _globals['_CONTEXT']._serialized_start=622
-  _globals['_CONTEXT']._serialized_end=688
-  _globals['_REPOSITORY']._serialized_start=691
-  _globals['_REPOSITORY']._serialized_end=831
-  _globals['_ONPRCLOSEDREQUEST']._serialized_start=833
-  _globals['_ONPRCLOSEDREQUEST']._serialized_end=900
-  _globals['_ONPRCLOSEDRESPONSE']._serialized_start=902
-  _globals['_ONPRCLOSEDRESPONSE']._serialized_end=959
-  _globals['_ONPRCREATEDREQUEST']._serialized_start=961
-  _globals['_ONPRCREATEDREQUEST']._serialized_end=1029
-  _globals['_ONPRCREATEDRESPONSE']._serialized_start=1031
-  _globals['_ONPRCREATEDRESPONSE']._serialized_end=1089
-  _globals['_ONPRMERGEDREQUEST']._serialized_start=1091
-  _globals['_ONPRMERGEDREQUEST']._serialized_end=1158
-  _globals['_ONPRMERGEDRESPONSE']._serialized_start=1160
-  _globals['_ONPRMERGEDRESPONSE']._serialized_end=1217
-  _globals['_PLUGINSERVICE']._serialized_start=1220
-  _globals['_PLUGINSERVICE']._serialized_end=1745
+  _globals['_EXECUTEACTIONSRESPONSE']._serialized_start=149
+  _globals['_EXECUTEACTIONSRESPONSE']._serialized_end=516
+  _globals['_EXECUTEACTIONSRESPONSE_TEMPLATEVARSENTRY']._serialized_start=380
+  _globals['_EXECUTEACTIONSRESPONSE_TEMPLATEVARSENTRY']._serialized_end=443
+  _globals['_EXECUTEACTIONSRESPONSE_PLUGINDATAENTRY']._serialized_start=445
+  _globals['_EXECUTEACTIONSRESPONSE_PLUGINDATAENTRY']._serialized_end=506
+  _globals['_EXECUTEFILTERSREQUEST']._serialized_start=518
+  _globals['_EXECUTEFILTERSREQUEST']._serialized_end=589
+  _globals['_EXECUTEFILTERSRESPONSE']._serialized_start=592
+  _globals['_EXECUTEFILTERSRESPONSE']._serialized_end=981
+  _globals['_EXECUTEFILTERSRESPONSE_TEMPLATEVARSENTRY']._serialized_start=380
+  _globals['_EXECUTEFILTERSRESPONSE_TEMPLATEVARSENTRY']._serialized_end=443
+  _globals['_EXECUTEFILTERSRESPONSE_PLUGINDATAENTRY']._serialized_start=445
+  _globals['_EXECUTEFILTERSRESPONSE_PLUGINDATAENTRY']._serialized_end=506
+  _globals['_GETPLUGINREQUEST']._serialized_start=984
+  _globals['_GETPLUGINREQUEST']._serialized_end=1128
+  _globals['_GETPLUGINREQUEST_CONFIGENTRY']._serialized_start=1071
+  _globals['_GETPLUGINREQUEST_CONFIGENTRY']._serialized_end=1128
+  _globals['_GETPLUGINRESPONSE']._serialized_start=1130
+  _globals['_GETPLUGINRESPONSE']._serialized_end=1234
+  _globals['_CONTEXT']._serialized_start=1237
+  _globals['_CONTEXT']._serialized_end=1520
+  _globals['_CONTEXT_PLUGINDATAENTRY']._serialized_start=445
+  _globals['_CONTEXT_PLUGINDATAENTRY']._serialized_end=506
+  _globals['_PULLREQUEST']._serialized_start=1522
+  _globals['_PULLREQUEST']._serialized_end=1584
+  _globals['_REPOSITORY']._serialized_start=1587
+  _globals['_REPOSITORY']._serialized_end=1727
+  _globals['_ONPRCLOSEDREQUEST']._serialized_start=1729
+  _globals['_ONPRCLOSEDREQUEST']._serialized_end=1796
+  _globals['_ONPRCLOSEDRESPONSE']._serialized_start=1798
+  _globals['_ONPRCLOSEDRESPONSE']._serialized_end=1855
+  _globals['_ONPRCREATEDREQUEST']._serialized_start=1857
+  _globals['_ONPRCREATEDREQUEST']._serialized_end=1925
+  _globals['_ONPRCREATEDRESPONSE']._serialized_start=1927
+  _globals['_ONPRCREATEDRESPONSE']._serialized_end=1985
+  _globals['_ONPRMERGEDREQUEST']._serialized_start=1987
+  _globals['_ONPRMERGEDREQUEST']._serialized_end=2054
+  _globals['_ONPRMERGEDRESPONSE']._serialized_start=2056
+  _globals['_ONPRMERGEDRESPONSE']._serialized_end=2113
+  _globals['_PLUGINSERVICE']._serialized_start=2116
+  _globals['_PLUGINSERVICE']._serialized_end=2641
 # @@protoc_insertion_point(module_scope)
```

### Comparing `saturn_bot-0.3.0/saturn_bot/protocol/v1/saturnbot_pb2.pyi` & `saturn_bot-0.4.0/saturn_bot/protocol/v1/saturnbot_pb2.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -14,32 +14,68 @@
     PATH_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     path: str
     context: Context
     def __init__(self, path: _Optional[str] = ..., context: _Optional[_Union[Context, _Mapping]] = ...) -> None: ...
 
 class ExecuteActionsResponse(_message.Message):
-    __slots__ = ("error",)
+    __slots__ = ("error", "template_vars", "plugin_data")
+    class TemplateVarsEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    class PluginDataEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     ERROR_FIELD_NUMBER: _ClassVar[int]
+    TEMPLATE_VARS_FIELD_NUMBER: _ClassVar[int]
+    PLUGIN_DATA_FIELD_NUMBER: _ClassVar[int]
     error: str
-    def __init__(self, error: _Optional[str] = ...) -> None: ...
+    template_vars: _containers.ScalarMap[str, str]
+    plugin_data: _containers.ScalarMap[str, str]
+    def __init__(self, error: _Optional[str] = ..., template_vars: _Optional[_Mapping[str, str]] = ..., plugin_data: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class ExecuteFiltersRequest(_message.Message):
     __slots__ = ("context",)
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     context: Context
     def __init__(self, context: _Optional[_Union[Context, _Mapping]] = ...) -> None: ...
 
 class ExecuteFiltersResponse(_message.Message):
-    __slots__ = ("match", "error")
+    __slots__ = ("match", "error", "template_vars", "plugin_data")
+    class TemplateVarsEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    class PluginDataEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     MATCH_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
+    TEMPLATE_VARS_FIELD_NUMBER: _ClassVar[int]
+    PLUGIN_DATA_FIELD_NUMBER: _ClassVar[int]
     match: bool
     error: str
-    def __init__(self, match: bool = ..., error: _Optional[str] = ...) -> None: ...
+    template_vars: _containers.ScalarMap[str, str]
+    plugin_data: _containers.ScalarMap[str, str]
+    def __init__(self, match: bool = ..., error: _Optional[str] = ..., template_vars: _Optional[_Mapping[str, str]] = ..., plugin_data: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class GetPluginRequest(_message.Message):
     __slots__ = ("config",)
     class ConfigEntry(_message.Message):
         __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
@@ -57,18 +93,37 @@
     ERROR_FIELD_NUMBER: _ClassVar[int]
     name: str
     priority: int
     error: str
     def __init__(self, name: _Optional[str] = ..., priority: _Optional[int] = ..., error: _Optional[str] = ...) -> None: ...
 
 class Context(_message.Message):
-    __slots__ = ("repository",)
+    __slots__ = ("repository", "pull_request", "plugin_data")
+    class PluginDataEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     REPOSITORY_FIELD_NUMBER: _ClassVar[int]
+    PULL_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    PLUGIN_DATA_FIELD_NUMBER: _ClassVar[int]
     repository: Repository
-    def __init__(self, repository: _Optional[_Union[Repository, _Mapping]] = ...) -> None: ...
+    pull_request: PullRequest
+    plugin_data: _containers.ScalarMap[str, str]
+    def __init__(self, repository: _Optional[_Union[Repository, _Mapping]] = ..., pull_request: _Optional[_Union[PullRequest, _Mapping]] = ..., plugin_data: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class PullRequest(_message.Message):
+    __slots__ = ("number", "web_url")
+    NUMBER_FIELD_NUMBER: _ClassVar[int]
+    WEB_URL_FIELD_NUMBER: _ClassVar[int]
+    number: int
+    web_url: str
+    def __init__(self, number: _Optional[int] = ..., web_url: _Optional[str] = ...) -> None: ...
 
 class Repository(_message.Message):
     __slots__ = ("full_name", "clone_url_http", "clone_url_ssh", "web_url")
     FULL_NAME_FIELD_NUMBER: _ClassVar[int]
     CLONE_URL_HTTP_FIELD_NUMBER: _ClassVar[int]
     CLONE_URL_SSH_FIELD_NUMBER: _ClassVar[int]
     WEB_URL_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `saturn_bot-0.3.0/saturn_bot/protocol/v1/saturnbot_pb2_grpc.py` & `saturn_bot-0.4.0/saturn_bot/protocol/v1/saturnbot_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `saturn_bot-0.3.0/saturn_bot/sdk.py` & `saturn_bot-0.4.0/saturn_bot/sdk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import contextlib
+import dataclasses
 import errno
 import os
 import random
 import socket
 import sys
 import time
 from concurrent import futures
-from typing import Iterator, Mapping
+from typing import Iterator, Mapping, MutableMapping
 
 import grpc
 from grpc_health.v1 import health_pb2, health_pb2_grpc
 from grpc_health.v1.health import HealthServicer
 
-from saturn_bot import Context
 from saturn_bot.plugin import grpc_controller_pb2_grpc
 from saturn_bot.protocol.v1 import saturnbot_pb2, saturnbot_pb2_grpc
 
 BIND_IP: str = "127.0.0.1"
 
 
+@dataclasses.dataclass
+class Context:
+    plugin_data: MutableMapping[str, str]
+    pull_request: saturnbot_pb2.PullRequest
+    repository: saturnbot_pb2.Repository
+    template_vars: MutableMapping[str, str]
+
+
 class Plugin:
     name: str
     priority: int = 0
 
     def init(self, config: Mapping[str, str]) -> None:
         pass
 
@@ -59,30 +67,49 @@
 class PluginService(saturnbot_pb2_grpc.PluginServiceServicer):
     def __init__(self, p: Plugin):
         self._plugin = p
 
     def ExecuteActions(
         self, request: saturnbot_pb2.ExecuteActionsRequest, context
     ) -> saturnbot_pb2.ExecuteActionsResponse:
+        ctx = Context(
+            pull_request=request.context.pull_request,
+            repository=request.context.repository,
+            template_vars={},
+            plugin_data=request.context.plugin_data,
+        )
         try:
             with in_checkout_dir(request.path):
-                self._plugin.apply(ctx=request.context)
+                self._plugin.apply(ctx=ctx)
         except Exception as e:
             return saturnbot_pb2.ExecuteActionsResponse(
                 error=f"failed to execute actions: {e}"
             )
 
-        return saturnbot_pb2.ExecuteActionsResponse(error=None)
+        return saturnbot_pb2.ExecuteActionsResponse(
+            error=None, plugin_data=ctx.plugin_data, template_vars=ctx.template_vars
+        )
 
     def ExecuteFilters(
         self, request: saturnbot_pb2.ExecuteFiltersRequest, context
     ) -> saturnbot_pb2.ExecuteFiltersResponse:
+        ctx = Context(
+            pull_request=request.context.pull_request,
+            repository=request.context.repository,
+            template_vars={},
+            plugin_data=request.context.plugin_data,
+        )
         try:
-            result = self._plugin.filter(ctx=request.context)
-            return saturnbot_pb2.ExecuteFiltersResponse(match=result, error=None)
+            result = self._plugin.filter(ctx=ctx)
+            return saturnbot_pb2.ExecuteFiltersResponse(
+                match=result,
+                error=None,
+                plugin_data=ctx.plugin_data,
+                template_vars=ctx.template_vars,
+            )
         except Exception as e:
             return saturnbot_pb2.ExecuteFiltersResponse(
                 match=False,
                 error=f"failed to execute filters: {e}",
             )
 
     def GetPlugin(
@@ -97,38 +124,56 @@
             return saturnbot_pb2.GetPluginResponse(
                 error=f"plugin '{self._plugin.name}' failed during initialization: {e}"
             )
 
     def OnPrClosed(
         self, request: saturnbot_pb2.OnPrClosedRequest, context
     ) -> saturnbot_pb2.OnPrClosedResponse:
+        ctx = Context(
+            pull_request=request.context.pull_request,
+            repository=request.context.repository,
+            template_vars={},
+            plugin_data=request.context.plugin_data,
+        )
         try:
-            self._plugin.on_pr_closed(request.context)
+            self._plugin.on_pr_closed(ctx=ctx)
             return saturnbot_pb2.OnPrClosedResponse(error=None)
         except Exception as e:
             return saturnbot_pb2.OnPrClosedResponse(
                 error=f"failed to execute OnPrClosed event: {e}"
             )
 
     def OnPrCreated(
         self, request: saturnbot_pb2.OnPrCreatedRequest, context
     ) -> saturnbot_pb2.OnPrCreatedResponse:
+        ctx = Context(
+            pull_request=request.context.pull_request,
+            repository=request.context.repository,
+            template_vars={},
+            plugin_data=request.context.plugin_data,
+        )
         try:
-            self._plugin.on_pr_created(request.context)
+            self._plugin.on_pr_created(ctx=ctx)
             return saturnbot_pb2.OnPrCreatedResponse(error=None)
         except Exception as e:
             return saturnbot_pb2.OnPrCreatedResponse(
                 error=f"failed to execute OnPrCreated event: {e}"
             )
 
     def OnPrMerged(
         self, request: saturnbot_pb2.OnPrMergedRequest, context
     ) -> saturnbot_pb2.OnPrMergedResponse:
+        ctx = Context(
+            pull_request=request.context.pull_request,
+            repository=request.context.repository,
+            template_vars={},
+            plugin_data=request.context.plugin_data,
+        )
         try:
-            self._plugin.on_pr_merged(request.context)
+            self._plugin.on_pr_merged(ctx=ctx)
             return saturnbot_pb2.OnPrMergedResponse(error=None)
         except Exception as e:
             return saturnbot_pb2.OnPrMergedResponse(
                 error=f"failed to execute OnPrMerged event: {e}"
             )
```

### Comparing `saturn_bot-0.3.0/PKG-INFO` & `saturn_bot-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saturn-bot
-Version: 0.3.0
+Version: 0.4.0
 Summary: Synchronize and refactor repositories with ease.
 Home-page: https://github.com/wndhydrnt/saturn-bot-protocol
 License: MPL-2.0
 Author: Markus Meyer
 Author-email: hydrantanderwand@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

