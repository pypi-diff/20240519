# Comparing `tmp/altmindpy-0.0.1a0.tar.gz` & `tmp/altmindpy-0.0.2.tar.gz`

## Comparing `altmindpy-0.0.1a0.tar` & `altmindpy-0.0.2.tar`

### file list

```diff
@@ -1,82 +1,84 @@
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/__init__.py
--rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_base_client.py
--rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_constants.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_qs.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_resource.py
--rw-r--r--   0        0        0    28381 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_response.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_streaming.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_types.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_utils/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/lib/.keep
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/__init__.py
--rw-r--r--   0        0        0    19806 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/assistants.py
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/login.py
--rw-r--r--   0        0        0    14139 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/runs.py
--rw-r--r--   0        0        0    17475 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/threads.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/experimental/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/experimental/experimental.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/experimental/stream.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/messages/__init__.py
--rw-r--r--   0        0        0    19898 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/messages/messages.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/messages/thread.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/users/__init__.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/users/me.py
--rw-r--r--   0        0        0    22517 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/resources/users/users.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/assistant.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/assistant_create_params.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/assistant_delete.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/assistant_list_params.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/assistant_update_params.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/assistants_response.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/login_access_token_params.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/message.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/message_create_params.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/message_delete.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/message_list_params.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/message_update_params.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/run.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/run_list_params.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/run_update_params.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/runs_response.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/thread.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/thread_create_params.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/thread_delete.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/thread_list_params.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/thread_update_params.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/threads_response.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/token.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/user_create_params.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/user_list_params.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/user_open_params.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/user_update_params.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/experimental/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/experimental/stream_retrieve_params.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/messages/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/messages/thread_list_params.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/shared/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/shared/messages_response.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/shared/response_message.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/shared/user.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/users/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/users/me_password_params.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/users/me_update_params.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/src/altmind/types/users/users.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/.gitignore
--rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 altmindpy-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/__init__.py
+-rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_base_client.py
+-rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_constants.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_qs.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_resource.py
+-rw-r--r--   0        0        0    28381 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_response.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_streaming.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_types.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_utils/__init__.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/lib/.keep
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/__init__.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/assistants.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/experimental.py
+-rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/login.py
+-rw-r--r--   0        0        0    19508 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/runs.py
+-rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/threads.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/messages/__init__.py
+-rw-r--r--   0        0        0    20011 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/messages/messages.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/messages/thread.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/users/__init__.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/users/open.py
+-rw-r--r--   0        0        0    20279 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/users/users.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/users/me/__init__.py
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/users/me/me.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/resources/users/me/password.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/assistant_create_params.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/assistant_delete.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/assistant_list_params.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/assistant_response.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/assistant_update_params.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/assistants_response.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/experimental_stream_params.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/login_access_token_params.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/message_create_params.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/message_delete.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/message_list_params.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/message_response.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/message_update_params.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/run_create_params.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/run_list_params.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/run_response.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/run_update_params.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/runs_response.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/thread_create_params.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/thread_delete.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/thread_list_params.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/thread_response.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/thread_update_params.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/threads_response.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/token.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/user_create_params.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/user_list_params.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/user_update_params.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/users_out.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/messages/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/messages/thread_list_params.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/shared/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/shared/messages_response.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/shared/response_message.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/shared/user_out.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/users/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/users/me_update_params.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/users/open_create_params.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/users/me/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 altmindpy-0.0.2/src/altmind/types/users/me/password_update_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 altmindpy-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 altmindpy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 altmindpy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 altmindpy-0.0.2/PKG-INFO
```

### Comparing `altmindpy-0.0.1a0/src/altmind/__init__.py` & `altmindpy-0.0.2/src/altmind/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_base_client.py` & `altmindpy-0.0.2/src/altmind/_base_client.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_client.py` & `altmindpy-0.0.2/src/altmind/_client.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_compat.py` & `altmindpy-0.0.2/src/altmind/_compat.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_exceptions.py` & `altmindpy-0.0.2/src/altmind/_exceptions.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_files.py` & `altmindpy-0.0.2/src/altmind/_files.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_models.py` & `altmindpy-0.0.2/src/altmind/_models.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_qs.py` & `altmindpy-0.0.2/src/altmind/_qs.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_resource.py` & `altmindpy-0.0.2/src/altmind/_resource.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_response.py` & `altmindpy-0.0.2/src/altmind/_response.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_streaming.py` & `altmindpy-0.0.2/src/altmind/_streaming.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_types.py` & `altmindpy-0.0.2/src/altmind/_types.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_utils/__init__.py` & `altmindpy-0.0.2/src/altmind/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_utils/_logs.py` & `altmindpy-0.0.2/src/altmind/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_utils/_proxy.py` & `altmindpy-0.0.2/src/altmind/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_utils/_sync.py` & `altmindpy-0.0.2/src/altmind/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_utils/_transform.py` & `altmindpy-0.0.2/src/altmind/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_utils/_typing.py` & `altmindpy-0.0.2/src/altmind/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/_utils/_utils.py` & `altmindpy-0.0.2/src/altmind/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/__init__.py` & `altmindpy-0.0.2/src/altmind/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/assistants.py` & `altmindpy-0.0.2/src/altmind/resources/assistants.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
-from ..types.assistant import Assistant
 from ..types.assistant_delete import AssistantDelete
+from ..types.assistant_response import AssistantResponse
 from ..types.assistants_response import AssistantsResponse
 
 __all__ = ["AssistantsResource", "AsyncAssistantsResource"]
 
 
 class AssistantsResource(SyncAPIResource):
     @cached_property
@@ -49,15 +49,15 @@
         name: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> AssistantResponse:
         """
         Create new assistant.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -77,28 +77,28 @@
                     "name": name,
                 },
                 assistant_create_params.AssistantCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=AssistantResponse,
         )
 
     def retrieve(
         self,
         assistant_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> AssistantResponse:
         """
         Retrieve assistant by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -110,15 +110,15 @@
         if not assistant_id:
             raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
         return self._get(
             f"/api/v1/assistants/{assistant_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=AssistantResponse,
         )
 
     def update(
         self,
         assistant_id: str,
         *,
         model: str,
@@ -128,15 +128,15 @@
         name: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> AssistantResponse:
         """
         Update assistant by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -158,15 +158,15 @@
                     "name": name,
                 },
                 assistant_update_params.AssistantUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=AssistantResponse,
         )
 
     def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
         offset: int | NotGiven = NOT_GIVEN,
@@ -260,15 +260,15 @@
         name: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> AssistantResponse:
         """
         Create new assistant.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -288,28 +288,28 @@
                     "name": name,
                 },
                 assistant_create_params.AssistantCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=AssistantResponse,
         )
 
     async def retrieve(
         self,
         assistant_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> AssistantResponse:
         """
         Retrieve assistant by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -321,15 +321,15 @@
         if not assistant_id:
             raise ValueError(f"Expected a non-empty value for `assistant_id` but received {assistant_id!r}")
         return await self._get(
             f"/api/v1/assistants/{assistant_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=AssistantResponse,
         )
 
     async def update(
         self,
         assistant_id: str,
         *,
         model: str,
@@ -339,15 +339,15 @@
         name: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Assistant:
+    ) -> AssistantResponse:
         """
         Update assistant by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -369,15 +369,15 @@
                     "name": name,
                 },
                 assistant_update_params.AssistantUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Assistant,
+            cast_to=AssistantResponse,
         )
 
     async def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
         offset: int | NotGiven = NOT_GIVEN,
```

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/login.py` & `altmindpy-0.0.2/src/altmind/resources/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from ..types.token import Token
 from .._base_client import (
     make_request_options,
 )
-from ..types.shared.user import User
+from ..types.shared.user_out import UserOut
 
 __all__ = ["LoginResource", "AsyncLoginResource"]
 
 
 class LoginResource(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> LoginResourceWithRawResponse:
@@ -90,22 +90,22 @@
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> UserOut:
         """Test access token"""
         return self._post(
             "/api/v1/login/test-token",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=UserOut,
         )
 
 
 class AsyncLoginResource(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncLoginResourceWithRawResponse:
         return AsyncLoginResourceWithRawResponse(self)
@@ -166,22 +166,22 @@
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> UserOut:
         """Test access token"""
         return await self._post(
             "/api/v1/login/test-token",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=UserOut,
         )
 
 
 class LoginResourceWithRawResponse:
     def __init__(self, login: LoginResource) -> None:
         self._login = login
```

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/runs.py` & `altmindpy-0.0.2/src/altmind/resources/threads.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,405 +1,500 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
+from typing import Optional
+
 import httpx
 
-from ..types import run_list_params, run_update_params
+from ..types import thread_list_params, thread_create_params, thread_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
-from ..types.run import Run
 from .._base_client import (
     make_request_options,
 )
-from ..types.runs_response import RunsResponse
+from ..types.thread_delete import ThreadDelete
+from ..types.thread_response import ThreadResponse
+from ..types.threads_response import ThreadsResponse
 
-__all__ = ["RunsResource", "AsyncRunsResource"]
+__all__ = ["ThreadsResource", "AsyncThreadsResource"]
 
 
-class RunsResource(SyncAPIResource):
+class ThreadsResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> RunsResourceWithRawResponse:
-        return RunsResourceWithRawResponse(self)
+    def with_raw_response(self) -> ThreadsResourceWithRawResponse:
+        return ThreadsResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> RunsResourceWithStreamingResponse:
-        return RunsResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> ThreadsResourceWithStreamingResponse:
+        return ThreadsResourceWithStreamingResponse(self)
 
     def create(
         self,
-        run_id: str,
         *,
+        thread_metadata: object | NotGiven = NOT_GIVEN,
+        title: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
+    ) -> ThreadResponse:
         """
-        Delete run by ID.
+        Create new thread.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return self._post(
-            f"/api/v1/runs/{run_id}",
+            "/api/v1/threads/",
+            body=maybe_transform(
+                {
+                    "thread_metadata": thread_metadata,
+                    "title": title,
+                },
+                thread_create_params.ThreadCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Run,
+            cast_to=ThreadResponse,
         )
 
     def retrieve(
         self,
-        run_id: str,
+        thread_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
+    ) -> ThreadResponse:
         """
-        Retrieve run by ID.
+        Retrieve thread by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return self._get(
-            f"/api/v1/runs/{run_id}",
+            f"/api/v1/threads/{thread_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Run,
+            cast_to=ThreadResponse,
         )
 
     def update(
         self,
-        run_id: str,
+        thread_id: int,
         *,
-        run_metadata: object | NotGiven = NOT_GIVEN,
+        thread_metadata: object | NotGiven = NOT_GIVEN,
+        title: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
+    ) -> ThreadResponse:
         """
-        Update run metadata by ID.
+        Update thread by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return self._patch(
-            f"/api/v1/runs/{run_id}",
-            body=maybe_transform({"run_metadata": run_metadata}, run_update_params.RunUpdateParams),
+            f"/api/v1/threads/{thread_id}",
+            body=maybe_transform(
+                {
+                    "thread_metadata": thread_metadata,
+                    "title": title,
+                },
+                thread_update_params.ThreadUpdateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Run,
+            cast_to=ThreadResponse,
         )
 
     def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
         offset: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> RunsResponse:
+    ) -> ThreadsResponse:
         """
-        Retrieve runs.
+        Retrieve threads.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
-            "/api/v1/runs/",
+            "/api/v1/threads/",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "limit": limit,
                         "offset": offset,
                     },
-                    run_list_params.RunListParams,
+                    thread_list_params.ThreadListParams,
                 ),
             ),
-            cast_to=RunsResponse,
+            cast_to=ThreadsResponse,
         )
 
+    def delete(
+        self,
+        thread_id: int,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> ThreadDelete:
+        """
+        Delete thread.
+
+        Args:
+          extra_headers: Send extra headers
 
-class AsyncRunsResource(AsyncAPIResource):
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        return self._delete(
+            f"/api/v1/threads/{thread_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=ThreadDelete,
+        )
+
+
+class AsyncThreadsResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncRunsResourceWithRawResponse:
-        return AsyncRunsResourceWithRawResponse(self)
+    def with_raw_response(self) -> AsyncThreadsResourceWithRawResponse:
+        return AsyncThreadsResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncRunsResourceWithStreamingResponse:
-        return AsyncRunsResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncThreadsResourceWithStreamingResponse:
+        return AsyncThreadsResourceWithStreamingResponse(self)
 
     async def create(
         self,
-        run_id: str,
         *,
+        thread_metadata: object | NotGiven = NOT_GIVEN,
+        title: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
+    ) -> ThreadResponse:
         """
-        Delete run by ID.
+        Create new thread.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return await self._post(
-            f"/api/v1/runs/{run_id}",
+            "/api/v1/threads/",
+            body=await async_maybe_transform(
+                {
+                    "thread_metadata": thread_metadata,
+                    "title": title,
+                },
+                thread_create_params.ThreadCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Run,
+            cast_to=ThreadResponse,
         )
 
     async def retrieve(
         self,
-        run_id: str,
+        thread_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
+    ) -> ThreadResponse:
         """
-        Retrieve run by ID.
+        Retrieve thread by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return await self._get(
-            f"/api/v1/runs/{run_id}",
+            f"/api/v1/threads/{thread_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Run,
+            cast_to=ThreadResponse,
         )
 
     async def update(
         self,
-        run_id: str,
+        thread_id: int,
         *,
-        run_metadata: object | NotGiven = NOT_GIVEN,
+        thread_metadata: object | NotGiven = NOT_GIVEN,
+        title: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Run:
+    ) -> ThreadResponse:
         """
-        Update run metadata by ID.
+        Update thread by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        if not run_id:
-            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return await self._patch(
-            f"/api/v1/runs/{run_id}",
-            body=await async_maybe_transform({"run_metadata": run_metadata}, run_update_params.RunUpdateParams),
+            f"/api/v1/threads/{thread_id}",
+            body=await async_maybe_transform(
+                {
+                    "thread_metadata": thread_metadata,
+                    "title": title,
+                },
+                thread_update_params.ThreadUpdateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Run,
+            cast_to=ThreadResponse,
         )
 
     async def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
         offset: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> RunsResponse:
+    ) -> ThreadsResponse:
         """
-        Retrieve runs.
+        Retrieve threads.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
-            "/api/v1/runs/",
+            "/api/v1/threads/",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "limit": limit,
                         "offset": offset,
                     },
-                    run_list_params.RunListParams,
+                    thread_list_params.ThreadListParams,
                 ),
             ),
-            cast_to=RunsResponse,
+            cast_to=ThreadsResponse,
         )
 
+    async def delete(
+        self,
+        thread_id: int,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> ThreadDelete:
+        """
+        Delete thread.
+
+        Args:
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
+        return await self._delete(
+            f"/api/v1/threads/{thread_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=ThreadDelete,
+        )
 
-class RunsResourceWithRawResponse:
-    def __init__(self, runs: RunsResource) -> None:
-        self._runs = runs
+
+class ThreadsResourceWithRawResponse:
+    def __init__(self, threads: ThreadsResource) -> None:
+        self._threads = threads
 
         self.create = to_raw_response_wrapper(
-            runs.create,
+            threads.create,
         )
         self.retrieve = to_raw_response_wrapper(
-            runs.retrieve,
+            threads.retrieve,
         )
         self.update = to_raw_response_wrapper(
-            runs.update,
+            threads.update,
         )
         self.list = to_raw_response_wrapper(
-            runs.list,
+            threads.list,
+        )
+        self.delete = to_raw_response_wrapper(
+            threads.delete,
         )
 
 
-class AsyncRunsResourceWithRawResponse:
-    def __init__(self, runs: AsyncRunsResource) -> None:
-        self._runs = runs
+class AsyncThreadsResourceWithRawResponse:
+    def __init__(self, threads: AsyncThreadsResource) -> None:
+        self._threads = threads
 
         self.create = async_to_raw_response_wrapper(
-            runs.create,
+            threads.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
-            runs.retrieve,
+            threads.retrieve,
         )
         self.update = async_to_raw_response_wrapper(
-            runs.update,
+            threads.update,
         )
         self.list = async_to_raw_response_wrapper(
-            runs.list,
+            threads.list,
+        )
+        self.delete = async_to_raw_response_wrapper(
+            threads.delete,
         )
 
 
-class RunsResourceWithStreamingResponse:
-    def __init__(self, runs: RunsResource) -> None:
-        self._runs = runs
+class ThreadsResourceWithStreamingResponse:
+    def __init__(self, threads: ThreadsResource) -> None:
+        self._threads = threads
 
         self.create = to_streamed_response_wrapper(
-            runs.create,
+            threads.create,
         )
         self.retrieve = to_streamed_response_wrapper(
-            runs.retrieve,
+            threads.retrieve,
         )
         self.update = to_streamed_response_wrapper(
-            runs.update,
+            threads.update,
         )
         self.list = to_streamed_response_wrapper(
-            runs.list,
+            threads.list,
+        )
+        self.delete = to_streamed_response_wrapper(
+            threads.delete,
         )
 
 
-class AsyncRunsResourceWithStreamingResponse:
-    def __init__(self, runs: AsyncRunsResource) -> None:
-        self._runs = runs
+class AsyncThreadsResourceWithStreamingResponse:
+    def __init__(self, threads: AsyncThreadsResource) -> None:
+        self._threads = threads
 
         self.create = async_to_streamed_response_wrapper(
-            runs.create,
+            threads.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
-            runs.retrieve,
+            threads.retrieve,
         )
         self.update = async_to_streamed_response_wrapper(
-            runs.update,
+            threads.update,
         )
         self.list = async_to_streamed_response_wrapper(
-            runs.list,
+            threads.list,
+        )
+        self.delete = async_to_streamed_response_wrapper(
+            threads.delete,
         )
```

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/threads.py` & `altmindpy-0.0.2/src/altmind/resources/messages/messages.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,500 +1,549 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Iterable, Optional
+from typing_extensions import Literal
 
 import httpx
 
-from ..types import thread_list_params, thread_create_params, thread_update_params
-from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from .._utils import (
+from .thread import (
+    ThreadResource,
+    AsyncThreadResource,
+    ThreadResourceWithRawResponse,
+    AsyncThreadResourceWithRawResponse,
+    ThreadResourceWithStreamingResponse,
+    AsyncThreadResourceWithStreamingResponse,
+)
+from ...types import message_list_params, message_create_params, message_update_params
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import (
     maybe_transform,
     async_maybe_transform,
 )
-from .._compat import cached_property
-from .._resource import SyncAPIResource, AsyncAPIResource
-from .._response import (
+from ..._compat import cached_property
+from ..._resource import SyncAPIResource, AsyncAPIResource
+from ..._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
-from .._base_client import (
+from ..._base_client import (
     make_request_options,
 )
-from ..types.thread import Thread
-from ..types.thread_delete import ThreadDelete
-from ..types.threads_response import ThreadsResponse
+from ...types.message_delete import MessageDelete
+from ...types.message_response import MessageResponse
+from ...types.shared.messages_response import MessagesResponse
+
+__all__ = ["MessagesResource", "AsyncMessagesResource"]
 
-__all__ = ["ThreadsResource", "AsyncThreadsResource"]
 
+class MessagesResource(SyncAPIResource):
+    @cached_property
+    def thread(self) -> ThreadResource:
+        return ThreadResource(self._client)
 
-class ThreadsResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> ThreadsResourceWithRawResponse:
-        return ThreadsResourceWithRawResponse(self)
+    def with_raw_response(self) -> MessagesResourceWithRawResponse:
+        return MessagesResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> ThreadsResourceWithStreamingResponse:
-        return ThreadsResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> MessagesResourceWithStreamingResponse:
+        return MessagesResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
-        thread_metadata: object | NotGiven = NOT_GIVEN,
-        title: Optional[str] | NotGiven = NOT_GIVEN,
+        content: Iterable[message_create_params.Content],
+        message_metadata: object | NotGiven = NOT_GIVEN,
+        original_role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
+        role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
+        thread_id: Optional[int] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Thread:
+    ) -> MessageResponse:
         """
-        Create new thread.
+        Create new message.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._post(
-            "/api/v1/threads/",
+            "/api/v1/messages/",
             body=maybe_transform(
                 {
-                    "thread_metadata": thread_metadata,
-                    "title": title,
+                    "content": content,
+                    "message_metadata": message_metadata,
+                    "original_role": original_role,
+                    "role": role,
+                    "thread_id": thread_id,
                 },
-                thread_create_params.ThreadCreateParams,
+                message_create_params.MessageCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Thread,
+            cast_to=MessageResponse,
         )
 
     def retrieve(
         self,
-        thread_id: int,
+        message_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Thread:
+    ) -> MessageResponse:
         """
-        Retrieve thread by ID.
+        Retrieve message by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
-            f"/api/v1/threads/{thread_id}",
+            f"/api/v1/messages/{message_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Thread,
+            cast_to=MessageResponse,
         )
 
     def update(
         self,
-        thread_id: int,
+        message_id: int,
         *,
-        thread_metadata: object | NotGiven = NOT_GIVEN,
-        title: Optional[str] | NotGiven = NOT_GIVEN,
+        content: Optional[Iterable[message_update_params.Content]] | NotGiven = NOT_GIVEN,
+        message_metadata: object | NotGiven = NOT_GIVEN,
+        role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Thread:
+    ) -> MessageResponse:
         """
-        Update thread by ID.
+        Update message by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._patch(
-            f"/api/v1/threads/{thread_id}",
+            f"/api/v1/messages/{message_id}",
             body=maybe_transform(
                 {
-                    "thread_metadata": thread_metadata,
-                    "title": title,
+                    "content": content,
+                    "message_metadata": message_metadata,
+                    "role": role,
                 },
-                thread_update_params.ThreadUpdateParams,
+                message_update_params.MessageUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Thread,
+            cast_to=MessageResponse,
         )
 
     def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
         offset: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ThreadsResponse:
+    ) -> MessagesResponse:
         """
-        Retrieve threads.
+        Retrieve messages.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
-            "/api/v1/threads/",
+            "/api/v1/messages/",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "limit": limit,
                         "offset": offset,
                     },
-                    thread_list_params.ThreadListParams,
+                    message_list_params.MessageListParams,
                 ),
             ),
-            cast_to=ThreadsResponse,
+            cast_to=MessagesResponse,
         )
 
     def delete(
         self,
-        thread_id: int,
+        message_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ThreadDelete:
+    ) -> MessageDelete:
         """
-        Delete thread.
+        Delete message by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._delete(
-            f"/api/v1/threads/{thread_id}",
+            f"/api/v1/messages/{message_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=ThreadDelete,
+            cast_to=MessageDelete,
         )
 
 
-class AsyncThreadsResource(AsyncAPIResource):
+class AsyncMessagesResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncThreadsResourceWithRawResponse:
-        return AsyncThreadsResourceWithRawResponse(self)
+    def thread(self) -> AsyncThreadResource:
+        return AsyncThreadResource(self._client)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncThreadsResourceWithStreamingResponse:
-        return AsyncThreadsResourceWithStreamingResponse(self)
+    def with_raw_response(self) -> AsyncMessagesResourceWithRawResponse:
+        return AsyncMessagesResourceWithRawResponse(self)
+
+    @cached_property
+    def with_streaming_response(self) -> AsyncMessagesResourceWithStreamingResponse:
+        return AsyncMessagesResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
-        thread_metadata: object | NotGiven = NOT_GIVEN,
-        title: Optional[str] | NotGiven = NOT_GIVEN,
+        content: Iterable[message_create_params.Content],
+        message_metadata: object | NotGiven = NOT_GIVEN,
+        original_role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
+        role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
+        thread_id: Optional[int] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Thread:
+    ) -> MessageResponse:
         """
-        Create new thread.
+        Create new message.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
-            "/api/v1/threads/",
+            "/api/v1/messages/",
             body=await async_maybe_transform(
                 {
-                    "thread_metadata": thread_metadata,
-                    "title": title,
+                    "content": content,
+                    "message_metadata": message_metadata,
+                    "original_role": original_role,
+                    "role": role,
+                    "thread_id": thread_id,
                 },
-                thread_create_params.ThreadCreateParams,
+                message_create_params.MessageCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Thread,
+            cast_to=MessageResponse,
         )
 
     async def retrieve(
         self,
-        thread_id: int,
+        message_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Thread:
+    ) -> MessageResponse:
         """
-        Retrieve thread by ID.
+        Retrieve message by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
-            f"/api/v1/threads/{thread_id}",
+            f"/api/v1/messages/{message_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Thread,
+            cast_to=MessageResponse,
         )
 
     async def update(
         self,
-        thread_id: int,
+        message_id: int,
         *,
-        thread_metadata: object | NotGiven = NOT_GIVEN,
-        title: Optional[str] | NotGiven = NOT_GIVEN,
+        content: Optional[Iterable[message_update_params.Content]] | NotGiven = NOT_GIVEN,
+        message_metadata: object | NotGiven = NOT_GIVEN,
+        role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Thread:
+    ) -> MessageResponse:
         """
-        Update thread by ID.
+        Update message by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._patch(
-            f"/api/v1/threads/{thread_id}",
+            f"/api/v1/messages/{message_id}",
             body=await async_maybe_transform(
                 {
-                    "thread_metadata": thread_metadata,
-                    "title": title,
+                    "content": content,
+                    "message_metadata": message_metadata,
+                    "role": role,
                 },
-                thread_update_params.ThreadUpdateParams,
+                message_update_params.MessageUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Thread,
+            cast_to=MessageResponse,
         )
 
     async def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
         offset: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ThreadsResponse:
+    ) -> MessagesResponse:
         """
-        Retrieve threads.
+        Retrieve messages.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
-            "/api/v1/threads/",
+            "/api/v1/messages/",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "limit": limit,
                         "offset": offset,
                     },
-                    thread_list_params.ThreadListParams,
+                    message_list_params.MessageListParams,
                 ),
             ),
-            cast_to=ThreadsResponse,
+            cast_to=MessagesResponse,
         )
 
     async def delete(
         self,
-        thread_id: int,
+        message_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ThreadDelete:
+    ) -> MessageDelete:
         """
-        Delete thread.
+        Delete message by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._delete(
-            f"/api/v1/threads/{thread_id}",
+            f"/api/v1/messages/{message_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=ThreadDelete,
+            cast_to=MessageDelete,
         )
 
 
-class ThreadsResourceWithRawResponse:
-    def __init__(self, threads: ThreadsResource) -> None:
-        self._threads = threads
+class MessagesResourceWithRawResponse:
+    def __init__(self, messages: MessagesResource) -> None:
+        self._messages = messages
 
         self.create = to_raw_response_wrapper(
-            threads.create,
+            messages.create,
         )
         self.retrieve = to_raw_response_wrapper(
-            threads.retrieve,
+            messages.retrieve,
         )
         self.update = to_raw_response_wrapper(
-            threads.update,
+            messages.update,
         )
         self.list = to_raw_response_wrapper(
-            threads.list,
+            messages.list,
         )
         self.delete = to_raw_response_wrapper(
-            threads.delete,
+            messages.delete,
         )
 
+    @cached_property
+    def thread(self) -> ThreadResourceWithRawResponse:
+        return ThreadResourceWithRawResponse(self._messages.thread)
+
 
-class AsyncThreadsResourceWithRawResponse:
-    def __init__(self, threads: AsyncThreadsResource) -> None:
-        self._threads = threads
+class AsyncMessagesResourceWithRawResponse:
+    def __init__(self, messages: AsyncMessagesResource) -> None:
+        self._messages = messages
 
         self.create = async_to_raw_response_wrapper(
-            threads.create,
+            messages.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
-            threads.retrieve,
+            messages.retrieve,
         )
         self.update = async_to_raw_response_wrapper(
-            threads.update,
+            messages.update,
         )
         self.list = async_to_raw_response_wrapper(
-            threads.list,
+            messages.list,
         )
         self.delete = async_to_raw_response_wrapper(
-            threads.delete,
+            messages.delete,
         )
 
+    @cached_property
+    def thread(self) -> AsyncThreadResourceWithRawResponse:
+        return AsyncThreadResourceWithRawResponse(self._messages.thread)
+
 
-class ThreadsResourceWithStreamingResponse:
-    def __init__(self, threads: ThreadsResource) -> None:
-        self._threads = threads
+class MessagesResourceWithStreamingResponse:
+    def __init__(self, messages: MessagesResource) -> None:
+        self._messages = messages
 
         self.create = to_streamed_response_wrapper(
-            threads.create,
+            messages.create,
         )
         self.retrieve = to_streamed_response_wrapper(
-            threads.retrieve,
+            messages.retrieve,
         )
         self.update = to_streamed_response_wrapper(
-            threads.update,
+            messages.update,
         )
         self.list = to_streamed_response_wrapper(
-            threads.list,
+            messages.list,
         )
         self.delete = to_streamed_response_wrapper(
-            threads.delete,
+            messages.delete,
         )
 
+    @cached_property
+    def thread(self) -> ThreadResourceWithStreamingResponse:
+        return ThreadResourceWithStreamingResponse(self._messages.thread)
+
 
-class AsyncThreadsResourceWithStreamingResponse:
-    def __init__(self, threads: AsyncThreadsResource) -> None:
-        self._threads = threads
+class AsyncMessagesResourceWithStreamingResponse:
+    def __init__(self, messages: AsyncMessagesResource) -> None:
+        self._messages = messages
 
         self.create = async_to_streamed_response_wrapper(
-            threads.create,
+            messages.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
-            threads.retrieve,
+            messages.retrieve,
         )
         self.update = async_to_streamed_response_wrapper(
-            threads.update,
+            messages.update,
         )
         self.list = async_to_streamed_response_wrapper(
-            threads.list,
+            messages.list,
         )
         self.delete = async_to_streamed_response_wrapper(
-            threads.delete,
+            messages.delete,
         )
+
+    @cached_property
+    def thread(self) -> AsyncThreadResourceWithStreamingResponse:
+        return AsyncThreadResourceWithStreamingResponse(self._messages.thread)
```

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/messages/__init__.py` & `altmindpy-0.0.2/src/altmind/resources/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/messages/messages.py` & `altmindpy-0.0.2/src/altmind/resources/users/users.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Iterable, Optional
-from typing_extensions import Literal
+from typing import Optional
 
 import httpx
 
-from .thread import (
-    ThreadResource,
-    AsyncThreadResource,
-    ThreadResourceWithRawResponse,
-    AsyncThreadResourceWithRawResponse,
-    ThreadResourceWithStreamingResponse,
-    AsyncThreadResourceWithStreamingResponse,
+from .me import (
+    MeResource,
+    AsyncMeResource,
+    MeResourceWithRawResponse,
+    AsyncMeResourceWithRawResponse,
+    MeResourceWithStreamingResponse,
+    AsyncMeResourceWithStreamingResponse,
 )
-from ...types import message_list_params, message_create_params, message_update_params
+from .open import (
+    OpenResource,
+    AsyncOpenResource,
+    OpenResourceWithRawResponse,
+    AsyncOpenResourceWithRawResponse,
+    OpenResourceWithStreamingResponse,
+    AsyncOpenResourceWithStreamingResponse,
+)
+from .me.me import MeResource, AsyncMeResource
+from ...types import user_list_params, user_create_params, user_update_params
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
@@ -28,522 +36,554 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from ..._base_client import (
     make_request_options,
 )
-from ...types.message import Message
-from ...types.message_delete import MessageDelete
-from ...types.shared.messages_response import MessagesResponse
+from ...types.users_out import UsersOut
+from ...types.shared.user_out import UserOut
+from ...types.shared.response_message import ResponseMessage
+
+__all__ = ["UsersResource", "AsyncUsersResource"]
 
-__all__ = ["MessagesResource", "AsyncMessagesResource"]
 
+class UsersResource(SyncAPIResource):
+    @cached_property
+    def me(self) -> MeResource:
+        return MeResource(self._client)
 
-class MessagesResource(SyncAPIResource):
     @cached_property
-    def thread(self) -> ThreadResource:
-        return ThreadResource(self._client)
+    def open(self) -> OpenResource:
+        return OpenResource(self._client)
 
     @cached_property
-    def with_raw_response(self) -> MessagesResourceWithRawResponse:
-        return MessagesResourceWithRawResponse(self)
+    def with_raw_response(self) -> UsersResourceWithRawResponse:
+        return UsersResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> MessagesResourceWithStreamingResponse:
-        return MessagesResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> UsersResourceWithStreamingResponse:
+        return UsersResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
-        content: Iterable[message_create_params.Content],
-        message_metadata: object | NotGiven = NOT_GIVEN,
-        original_role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
-        role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
-        thread_id: Optional[int] | NotGiven = NOT_GIVEN,
+        email: str,
+        password: str,
+        full_name: Optional[str] | NotGiven = NOT_GIVEN,
+        is_active: bool | NotGiven = NOT_GIVEN,
+        is_superuser: bool | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> UserOut:
         """
-        Create new message.
+        Create new user.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._post(
-            "/api/v1/messages/",
+            "/api/v1/users/",
             body=maybe_transform(
                 {
-                    "content": content,
-                    "message_metadata": message_metadata,
-                    "original_role": original_role,
-                    "role": role,
-                    "thread_id": thread_id,
+                    "email": email,
+                    "password": password,
+                    "full_name": full_name,
+                    "is_active": is_active,
+                    "is_superuser": is_superuser,
                 },
-                message_create_params.MessageCreateParams,
+                user_create_params.UserCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=UserOut,
         )
 
     def retrieve(
         self,
-        message_id: int,
+        user_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> UserOut:
         """
-        Retrieve message by ID.
+        Get a specific user by id.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
-            f"/api/v1/messages/{message_id}",
+            f"/api/v1/users/{user_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=UserOut,
         )
 
     def update(
         self,
-        message_id: int,
+        user_id: int,
         *,
-        content: Optional[Iterable[message_update_params.Content]] | NotGiven = NOT_GIVEN,
-        message_metadata: object | NotGiven = NOT_GIVEN,
-        role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
+        email: Optional[str] | NotGiven = NOT_GIVEN,
+        full_name: Optional[str] | NotGiven = NOT_GIVEN,
+        is_active: bool | NotGiven = NOT_GIVEN,
+        is_superuser: bool | NotGiven = NOT_GIVEN,
+        password: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> UserOut:
         """
-        Update message by ID.
+        Update a user.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._patch(
-            f"/api/v1/messages/{message_id}",
+            f"/api/v1/users/{user_id}",
             body=maybe_transform(
                 {
-                    "content": content,
-                    "message_metadata": message_metadata,
-                    "role": role,
+                    "email": email,
+                    "full_name": full_name,
+                    "is_active": is_active,
+                    "is_superuser": is_superuser,
+                    "password": password,
                 },
-                message_update_params.MessageUpdateParams,
+                user_update_params.UserUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=UserOut,
         )
 
     def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
-        offset: int | NotGiven = NOT_GIVEN,
+        skip: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> MessagesResponse:
+    ) -> UsersOut:
         """
-        Retrieve messages.
+        Retrieve users.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
-            "/api/v1/messages/",
+            "/api/v1/users/",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "limit": limit,
-                        "offset": offset,
+                        "skip": skip,
                     },
-                    message_list_params.MessageListParams,
+                    user_list_params.UserListParams,
                 ),
             ),
-            cast_to=MessagesResponse,
+            cast_to=UsersOut,
         )
 
     def delete(
         self,
-        message_id: int,
+        user_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> MessageDelete:
+    ) -> ResponseMessage:
         """
-        Delete message by ID.
+        Delete a user.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._delete(
-            f"/api/v1/messages/{message_id}",
+            f"/api/v1/users/{user_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=MessageDelete,
+            cast_to=ResponseMessage,
         )
 
 
-class AsyncMessagesResource(AsyncAPIResource):
+class AsyncUsersResource(AsyncAPIResource):
     @cached_property
-    def thread(self) -> AsyncThreadResource:
-        return AsyncThreadResource(self._client)
+    def me(self) -> AsyncMeResource:
+        return AsyncMeResource(self._client)
 
     @cached_property
-    def with_raw_response(self) -> AsyncMessagesResourceWithRawResponse:
-        return AsyncMessagesResourceWithRawResponse(self)
+    def open(self) -> AsyncOpenResource:
+        return AsyncOpenResource(self._client)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncMessagesResourceWithStreamingResponse:
-        return AsyncMessagesResourceWithStreamingResponse(self)
+    def with_raw_response(self) -> AsyncUsersResourceWithRawResponse:
+        return AsyncUsersResourceWithRawResponse(self)
+
+    @cached_property
+    def with_streaming_response(self) -> AsyncUsersResourceWithStreamingResponse:
+        return AsyncUsersResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
-        content: Iterable[message_create_params.Content],
-        message_metadata: object | NotGiven = NOT_GIVEN,
-        original_role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
-        role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
-        thread_id: Optional[int] | NotGiven = NOT_GIVEN,
+        email: str,
+        password: str,
+        full_name: Optional[str] | NotGiven = NOT_GIVEN,
+        is_active: bool | NotGiven = NOT_GIVEN,
+        is_superuser: bool | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> UserOut:
         """
-        Create new message.
+        Create new user.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
-            "/api/v1/messages/",
+            "/api/v1/users/",
             body=await async_maybe_transform(
                 {
-                    "content": content,
-                    "message_metadata": message_metadata,
-                    "original_role": original_role,
-                    "role": role,
-                    "thread_id": thread_id,
+                    "email": email,
+                    "password": password,
+                    "full_name": full_name,
+                    "is_active": is_active,
+                    "is_superuser": is_superuser,
                 },
-                message_create_params.MessageCreateParams,
+                user_create_params.UserCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=UserOut,
         )
 
     async def retrieve(
         self,
-        message_id: int,
+        user_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> UserOut:
         """
-        Retrieve message by ID.
+        Get a specific user by id.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
-            f"/api/v1/messages/{message_id}",
+            f"/api/v1/users/{user_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=UserOut,
         )
 
     async def update(
         self,
-        message_id: int,
+        user_id: int,
         *,
-        content: Optional[Iterable[message_update_params.Content]] | NotGiven = NOT_GIVEN,
-        message_metadata: object | NotGiven = NOT_GIVEN,
-        role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
+        email: Optional[str] | NotGiven = NOT_GIVEN,
+        full_name: Optional[str] | NotGiven = NOT_GIVEN,
+        is_active: bool | NotGiven = NOT_GIVEN,
+        is_superuser: bool | NotGiven = NOT_GIVEN,
+        password: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Message:
+    ) -> UserOut:
         """
-        Update message by ID.
+        Update a user.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._patch(
-            f"/api/v1/messages/{message_id}",
+            f"/api/v1/users/{user_id}",
             body=await async_maybe_transform(
                 {
-                    "content": content,
-                    "message_metadata": message_metadata,
-                    "role": role,
+                    "email": email,
+                    "full_name": full_name,
+                    "is_active": is_active,
+                    "is_superuser": is_superuser,
+                    "password": password,
                 },
-                message_update_params.MessageUpdateParams,
+                user_update_params.UserUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=Message,
+            cast_to=UserOut,
         )
 
     async def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
-        offset: int | NotGiven = NOT_GIVEN,
+        skip: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> MessagesResponse:
+    ) -> UsersOut:
         """
-        Retrieve messages.
+        Retrieve users.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
-            "/api/v1/messages/",
+            "/api/v1/users/",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "limit": limit,
-                        "offset": offset,
+                        "skip": skip,
                     },
-                    message_list_params.MessageListParams,
+                    user_list_params.UserListParams,
                 ),
             ),
-            cast_to=MessagesResponse,
+            cast_to=UsersOut,
         )
 
     async def delete(
         self,
-        message_id: int,
+        user_id: int,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> MessageDelete:
+    ) -> ResponseMessage:
         """
-        Delete message by ID.
+        Delete a user.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._delete(
-            f"/api/v1/messages/{message_id}",
+            f"/api/v1/users/{user_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=MessageDelete,
+            cast_to=ResponseMessage,
         )
 
 
-class MessagesResourceWithRawResponse:
-    def __init__(self, messages: MessagesResource) -> None:
-        self._messages = messages
+class UsersResourceWithRawResponse:
+    def __init__(self, users: UsersResource) -> None:
+        self._users = users
 
         self.create = to_raw_response_wrapper(
-            messages.create,
+            users.create,
         )
         self.retrieve = to_raw_response_wrapper(
-            messages.retrieve,
+            users.retrieve,
         )
         self.update = to_raw_response_wrapper(
-            messages.update,
+            users.update,
         )
         self.list = to_raw_response_wrapper(
-            messages.list,
+            users.list,
         )
         self.delete = to_raw_response_wrapper(
-            messages.delete,
+            users.delete,
         )
 
     @cached_property
-    def thread(self) -> ThreadResourceWithRawResponse:
-        return ThreadResourceWithRawResponse(self._messages.thread)
+    def me(self) -> MeResourceWithRawResponse:
+        return MeResourceWithRawResponse(self._users.me)
+
+    @cached_property
+    def open(self) -> OpenResourceWithRawResponse:
+        return OpenResourceWithRawResponse(self._users.open)
 
 
-class AsyncMessagesResourceWithRawResponse:
-    def __init__(self, messages: AsyncMessagesResource) -> None:
-        self._messages = messages
+class AsyncUsersResourceWithRawResponse:
+    def __init__(self, users: AsyncUsersResource) -> None:
+        self._users = users
 
         self.create = async_to_raw_response_wrapper(
-            messages.create,
+            users.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
-            messages.retrieve,
+            users.retrieve,
         )
         self.update = async_to_raw_response_wrapper(
-            messages.update,
+            users.update,
         )
         self.list = async_to_raw_response_wrapper(
-            messages.list,
+            users.list,
         )
         self.delete = async_to_raw_response_wrapper(
-            messages.delete,
+            users.delete,
         )
 
     @cached_property
-    def thread(self) -> AsyncThreadResourceWithRawResponse:
-        return AsyncThreadResourceWithRawResponse(self._messages.thread)
+    def me(self) -> AsyncMeResourceWithRawResponse:
+        return AsyncMeResourceWithRawResponse(self._users.me)
+
+    @cached_property
+    def open(self) -> AsyncOpenResourceWithRawResponse:
+        return AsyncOpenResourceWithRawResponse(self._users.open)
 
 
-class MessagesResourceWithStreamingResponse:
-    def __init__(self, messages: MessagesResource) -> None:
-        self._messages = messages
+class UsersResourceWithStreamingResponse:
+    def __init__(self, users: UsersResource) -> None:
+        self._users = users
 
         self.create = to_streamed_response_wrapper(
-            messages.create,
+            users.create,
         )
         self.retrieve = to_streamed_response_wrapper(
-            messages.retrieve,
+            users.retrieve,
         )
         self.update = to_streamed_response_wrapper(
-            messages.update,
+            users.update,
         )
         self.list = to_streamed_response_wrapper(
-            messages.list,
+            users.list,
         )
         self.delete = to_streamed_response_wrapper(
-            messages.delete,
+            users.delete,
         )
 
     @cached_property
-    def thread(self) -> ThreadResourceWithStreamingResponse:
-        return ThreadResourceWithStreamingResponse(self._messages.thread)
+    def me(self) -> MeResourceWithStreamingResponse:
+        return MeResourceWithStreamingResponse(self._users.me)
+
+    @cached_property
+    def open(self) -> OpenResourceWithStreamingResponse:
+        return OpenResourceWithStreamingResponse(self._users.open)
 
 
-class AsyncMessagesResourceWithStreamingResponse:
-    def __init__(self, messages: AsyncMessagesResource) -> None:
-        self._messages = messages
+class AsyncUsersResourceWithStreamingResponse:
+    def __init__(self, users: AsyncUsersResource) -> None:
+        self._users = users
 
         self.create = async_to_streamed_response_wrapper(
-            messages.create,
+            users.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
-            messages.retrieve,
+            users.retrieve,
         )
         self.update = async_to_streamed_response_wrapper(
-            messages.update,
+            users.update,
         )
         self.list = async_to_streamed_response_wrapper(
-            messages.list,
+            users.list,
         )
         self.delete = async_to_streamed_response_wrapper(
-            messages.delete,
+            users.delete,
         )
 
     @cached_property
-    def thread(self) -> AsyncThreadResourceWithStreamingResponse:
-        return AsyncThreadResourceWithStreamingResponse(self._messages.thread)
+    def me(self) -> AsyncMeResourceWithStreamingResponse:
+        return AsyncMeResourceWithStreamingResponse(self._users.me)
+
+    @cached_property
+    def open(self) -> AsyncOpenResourceWithStreamingResponse:
+        return AsyncOpenResourceWithStreamingResponse(self._users.open)
```

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/messages/thread.py` & `altmindpy-0.0.2/src/altmind/resources/messages/thread.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/users/__init__.py` & `altmindpy-0.0.2/src/altmind/resources/users/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,22 @@
     MeResource,
     AsyncMeResource,
     MeResourceWithRawResponse,
     AsyncMeResourceWithRawResponse,
     MeResourceWithStreamingResponse,
     AsyncMeResourceWithStreamingResponse,
 )
+from .open import (
+    OpenResource,
+    AsyncOpenResource,
+    OpenResourceWithRawResponse,
+    AsyncOpenResourceWithRawResponse,
+    OpenResourceWithStreamingResponse,
+    AsyncOpenResourceWithStreamingResponse,
+)
 from .users import (
     UsersResource,
     AsyncUsersResource,
     UsersResourceWithRawResponse,
     AsyncUsersResourceWithRawResponse,
     UsersResourceWithStreamingResponse,
     AsyncUsersResourceWithStreamingResponse,
@@ -20,14 +28,20 @@
 __all__ = [
     "MeResource",
     "AsyncMeResource",
     "MeResourceWithRawResponse",
     "AsyncMeResourceWithRawResponse",
     "MeResourceWithStreamingResponse",
     "AsyncMeResourceWithStreamingResponse",
+    "OpenResource",
+    "AsyncOpenResource",
+    "OpenResourceWithRawResponse",
+    "AsyncOpenResourceWithRawResponse",
+    "OpenResourceWithStreamingResponse",
+    "AsyncOpenResourceWithStreamingResponse",
     "UsersResource",
     "AsyncUsersResource",
     "UsersResourceWithRawResponse",
     "AsyncUsersResourceWithRawResponse",
     "UsersResourceWithStreamingResponse",
     "AsyncUsersResourceWithStreamingResponse",
 ]
```

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/users/me.py` & `altmindpy-0.0.2/src/altmind/resources/users/me/me.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,39 +2,50 @@
 
 from __future__ import annotations
 
 from typing import Optional
 
 import httpx
 
-from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._utils import (
+from .password import (
+    PasswordResource,
+    AsyncPasswordResource,
+    PasswordResourceWithRawResponse,
+    AsyncPasswordResourceWithRawResponse,
+    PasswordResourceWithStreamingResponse,
+    AsyncPasswordResourceWithStreamingResponse,
+)
+from ...._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ...._utils import (
     maybe_transform,
     async_maybe_transform,
 )
-from ..._compat import cached_property
-from ..._resource import SyncAPIResource, AsyncAPIResource
-from ..._response import (
+from ...._compat import cached_property
+from ...._resource import SyncAPIResource, AsyncAPIResource
+from ...._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
-from ...types.users import me_update_params, me_password_params
-from ..._base_client import (
+from ....types.users import me_update_params
+from ...._base_client import (
     make_request_options,
 )
-from ...types.shared.user import User
-from ...types.shared.response_message import ResponseMessage
+from ....types.shared.user_out import UserOut
 
 __all__ = ["MeResource", "AsyncMeResource"]
 
 
 class MeResource(SyncAPIResource):
     @cached_property
+    def password(self) -> PasswordResource:
+        return PasswordResource(self._client)
+
+    @cached_property
     def with_raw_response(self) -> MeResourceWithRawResponse:
         return MeResourceWithRawResponse(self)
 
     @cached_property
     def with_streaming_response(self) -> MeResourceWithStreamingResponse:
         return MeResourceWithStreamingResponse(self)
 
@@ -43,36 +54,36 @@
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> UserOut:
         """Get current user."""
         return self._get(
             "/api/v1/users/me",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=UserOut,
         )
 
     def update(
         self,
         *,
         email: Optional[str] | NotGiven = NOT_GIVEN,
         full_name: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> UserOut:
         """
         Update own user.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -89,59 +100,24 @@
                     "full_name": full_name,
                 },
                 me_update_params.MeUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
-        )
-
-    def password(
-        self,
-        *,
-        current_password: str,
-        new_password: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ResponseMessage:
-        """
-        Update own password.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        return self._patch(
-            "/api/v1/users/me/password",
-            body=maybe_transform(
-                {
-                    "current_password": current_password,
-                    "new_password": new_password,
-                },
-                me_password_params.MePasswordParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=ResponseMessage,
+            cast_to=UserOut,
         )
 
 
 class AsyncMeResource(AsyncAPIResource):
     @cached_property
+    def password(self) -> AsyncPasswordResource:
+        return AsyncPasswordResource(self._client)
+
+    @cached_property
     def with_raw_response(self) -> AsyncMeResourceWithRawResponse:
         return AsyncMeResourceWithRawResponse(self)
 
     @cached_property
     def with_streaming_response(self) -> AsyncMeResourceWithStreamingResponse:
         return AsyncMeResourceWithStreamingResponse(self)
 
@@ -150,36 +126,36 @@
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> UserOut:
         """Get current user."""
         return await self._get(
             "/api/v1/users/me",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=UserOut,
         )
 
     async def update(
         self,
         *,
         email: Optional[str] | NotGiven = NOT_GIVEN,
         full_name: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> UserOut:
         """
         Update own user.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -196,108 +172,73 @@
                     "full_name": full_name,
                 },
                 me_update_params.MeUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
-        )
-
-    async def password(
-        self,
-        *,
-        current_password: str,
-        new_password: str,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ResponseMessage:
-        """
-        Update own password.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        return await self._patch(
-            "/api/v1/users/me/password",
-            body=await async_maybe_transform(
-                {
-                    "current_password": current_password,
-                    "new_password": new_password,
-                },
-                me_password_params.MePasswordParams,
-            ),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=ResponseMessage,
+            cast_to=UserOut,
         )
 
 
 class MeResourceWithRawResponse:
     def __init__(self, me: MeResource) -> None:
         self._me = me
 
         self.retrieve = to_raw_response_wrapper(
             me.retrieve,
         )
         self.update = to_raw_response_wrapper(
             me.update,
         )
-        self.password = to_raw_response_wrapper(
-            me.password,
-        )
+
+    @cached_property
+    def password(self) -> PasswordResourceWithRawResponse:
+        return PasswordResourceWithRawResponse(self._me.password)
 
 
 class AsyncMeResourceWithRawResponse:
     def __init__(self, me: AsyncMeResource) -> None:
         self._me = me
 
         self.retrieve = async_to_raw_response_wrapper(
             me.retrieve,
         )
         self.update = async_to_raw_response_wrapper(
             me.update,
         )
-        self.password = async_to_raw_response_wrapper(
-            me.password,
-        )
+
+    @cached_property
+    def password(self) -> AsyncPasswordResourceWithRawResponse:
+        return AsyncPasswordResourceWithRawResponse(self._me.password)
 
 
 class MeResourceWithStreamingResponse:
     def __init__(self, me: MeResource) -> None:
         self._me = me
 
         self.retrieve = to_streamed_response_wrapper(
             me.retrieve,
         )
         self.update = to_streamed_response_wrapper(
             me.update,
         )
-        self.password = to_streamed_response_wrapper(
-            me.password,
-        )
+
+    @cached_property
+    def password(self) -> PasswordResourceWithStreamingResponse:
+        return PasswordResourceWithStreamingResponse(self._me.password)
 
 
 class AsyncMeResourceWithStreamingResponse:
     def __init__(self, me: AsyncMeResource) -> None:
         self._me = me
 
         self.retrieve = async_to_streamed_response_wrapper(
             me.retrieve,
         )
         self.update = async_to_streamed_response_wrapper(
             me.update,
         )
-        self.password = async_to_streamed_response_wrapper(
-            me.password,
-        )
+
+    @cached_property
+    def password(self) -> AsyncPasswordResourceWithStreamingResponse:
+        return AsyncPasswordResourceWithStreamingResponse(self._me.password)
```

### Comparing `altmindpy-0.0.1a0/src/altmind/resources/users/users.py` & `altmindpy-0.0.2/src/altmind/resources/runs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,650 +1,540 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Optional
+from typing_extensions import Literal
 
 import httpx
 
-from .me import (
-    MeResource,
-    AsyncMeResource,
-    MeResourceWithRawResponse,
-    AsyncMeResourceWithRawResponse,
-    MeResourceWithStreamingResponse,
-    AsyncMeResourceWithStreamingResponse,
-)
-from ...types import user_list_params, user_open_params, user_create_params, user_update_params
-from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._utils import (
+from ..types import run_list_params, run_create_params, run_update_params
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
-from ..._compat import cached_property
-from ..._resource import SyncAPIResource, AsyncAPIResource
-from ..._response import (
+from .._compat import cached_property
+from .._resource import SyncAPIResource, AsyncAPIResource
+from .._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
-from ..._base_client import (
+from .._base_client import (
     make_request_options,
 )
-from ...types.shared.user import User
-from ...types.users.users import Users
-from ...types.shared.response_message import ResponseMessage
-
-__all__ = ["UsersResource", "AsyncUsersResource"]
+from ..types.run_response import RunResponse
+from ..types.runs_response import RunsResponse
 
+__all__ = ["RunsResource", "AsyncRunsResource"]
 
-class UsersResource(SyncAPIResource):
-    @cached_property
-    def me(self) -> MeResource:
-        return MeResource(self._client)
 
+class RunsResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> UsersResourceWithRawResponse:
-        return UsersResourceWithRawResponse(self)
+    def with_raw_response(self) -> RunsResourceWithRawResponse:
+        return RunsResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> UsersResourceWithStreamingResponse:
-        return UsersResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> RunsResourceWithStreamingResponse:
+        return RunsResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
-        email: str,
-        password: str,
-        full_name: Optional[str] | NotGiven = NOT_GIVEN,
-        is_active: bool | NotGiven = NOT_GIVEN,
-        is_superuser: bool | NotGiven = NOT_GIVEN,
+        assistant_id: Optional[int],
+        thread_id: Optional[int],
+        stream: bool | NotGiven = NOT_GIVEN,
+        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        model: Optional[str] | NotGiven = NOT_GIVEN,
+        run_metadata: object | NotGiven = NOT_GIVEN,
+        type: Literal["default", "analysis", "execution"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> object:
         """
-        Create new user.
+        Create new run.
 
         Args:
+          additional_instructions: Additional instructions for this run, appended to the assistant instructions
+
+          instructions: Override the assistant instructions for this run
+
+          model: Override the assistant model for this run
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._post(
-            "/api/v1/users/",
+            "/api/v1/runs/",
             body=maybe_transform(
                 {
-                    "email": email,
-                    "password": password,
-                    "full_name": full_name,
-                    "is_active": is_active,
-                    "is_superuser": is_superuser,
+                    "assistant_id": assistant_id,
+                    "thread_id": thread_id,
+                    "additional_instructions": additional_instructions,
+                    "instructions": instructions,
+                    "model": model,
+                    "run_metadata": run_metadata,
+                    "type": type,
                 },
-                user_create_params.UserCreateParams,
+                run_create_params.RunCreateParams,
             ),
             options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                query=maybe_transform({"stream": stream}, run_create_params.RunCreateParams),
             ),
-            cast_to=User,
+            cast_to=object,
         )
 
     def retrieve(
         self,
-        user_id: int,
+        run_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> RunResponse:
         """
-        Get a specific user by id.
+        Retrieve run by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return self._get(
-            f"/api/v1/users/{user_id}",
+            f"/api/v1/runs/{run_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=RunResponse,
         )
 
     def update(
         self,
-        user_id: int,
+        run_id: str,
         *,
-        email: Optional[str] | NotGiven = NOT_GIVEN,
-        full_name: Optional[str] | NotGiven = NOT_GIVEN,
-        is_active: bool | NotGiven = NOT_GIVEN,
-        is_superuser: bool | NotGiven = NOT_GIVEN,
-        password: Optional[str] | NotGiven = NOT_GIVEN,
+        run_metadata: object | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> RunResponse:
         """
-        Update a user.
+        Update run metadata by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return self._patch(
-            f"/api/v1/users/{user_id}",
-            body=maybe_transform(
-                {
-                    "email": email,
-                    "full_name": full_name,
-                    "is_active": is_active,
-                    "is_superuser": is_superuser,
-                    "password": password,
-                },
-                user_update_params.UserUpdateParams,
-            ),
+            f"/api/v1/runs/{run_id}",
+            body=maybe_transform({"run_metadata": run_metadata}, run_update_params.RunUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=RunResponse,
         )
 
     def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
-        skip: int | NotGiven = NOT_GIVEN,
+        offset: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Users:
+    ) -> RunsResponse:
         """
-        Retrieve users.
+        Retrieve runs.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get(
-            "/api/v1/users/",
+            "/api/v1/runs/",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "limit": limit,
-                        "skip": skip,
+                        "offset": offset,
                     },
-                    user_list_params.UserListParams,
+                    run_list_params.RunListParams,
                 ),
             ),
-            cast_to=Users,
+            cast_to=RunsResponse,
         )
 
     def delete(
         self,
-        user_id: int,
+        run_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ResponseMessage:
+    ) -> RunResponse:
         """
-        Delete a user.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        return self._delete(
-            f"/api/v1/users/{user_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=ResponseMessage,
-        )
-
-    def open(
-        self,
-        *,
-        email: str,
-        password: str,
-        full_name: Optional[str] | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
-        """
-        Create new user without the need to be logged in.
+        Delete run by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return self._post(
-            "/api/v1/users/open",
-            body=maybe_transform(
-                {
-                    "email": email,
-                    "password": password,
-                    "full_name": full_name,
-                },
-                user_open_params.UserOpenParams,
-            ),
+            f"/api/v1/runs/{run_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=RunResponse,
         )
 
 
-class AsyncUsersResource(AsyncAPIResource):
+class AsyncRunsResource(AsyncAPIResource):
     @cached_property
-    def me(self) -> AsyncMeResource:
-        return AsyncMeResource(self._client)
+    def with_raw_response(self) -> AsyncRunsResourceWithRawResponse:
+        return AsyncRunsResourceWithRawResponse(self)
 
     @cached_property
-    def with_raw_response(self) -> AsyncUsersResourceWithRawResponse:
-        return AsyncUsersResourceWithRawResponse(self)
-
-    @cached_property
-    def with_streaming_response(self) -> AsyncUsersResourceWithStreamingResponse:
-        return AsyncUsersResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncRunsResourceWithStreamingResponse:
+        return AsyncRunsResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
-        email: str,
-        password: str,
-        full_name: Optional[str] | NotGiven = NOT_GIVEN,
-        is_active: bool | NotGiven = NOT_GIVEN,
-        is_superuser: bool | NotGiven = NOT_GIVEN,
+        assistant_id: Optional[int],
+        thread_id: Optional[int],
+        stream: bool | NotGiven = NOT_GIVEN,
+        additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        instructions: Optional[str] | NotGiven = NOT_GIVEN,
+        model: Optional[str] | NotGiven = NOT_GIVEN,
+        run_metadata: object | NotGiven = NOT_GIVEN,
+        type: Literal["default", "analysis", "execution"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> object:
         """
-        Create new user.
+        Create new run.
 
         Args:
+          additional_instructions: Additional instructions for this run, appended to the assistant instructions
+
+          instructions: Override the assistant instructions for this run
+
+          model: Override the assistant model for this run
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
-            "/api/v1/users/",
+            "/api/v1/runs/",
             body=await async_maybe_transform(
                 {
-                    "email": email,
-                    "password": password,
-                    "full_name": full_name,
-                    "is_active": is_active,
-                    "is_superuser": is_superuser,
+                    "assistant_id": assistant_id,
+                    "thread_id": thread_id,
+                    "additional_instructions": additional_instructions,
+                    "instructions": instructions,
+                    "model": model,
+                    "run_metadata": run_metadata,
+                    "type": type,
                 },
-                user_create_params.UserCreateParams,
+                run_create_params.RunCreateParams,
             ),
             options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                query=await async_maybe_transform({"stream": stream}, run_create_params.RunCreateParams),
             ),
-            cast_to=User,
+            cast_to=object,
         )
 
     async def retrieve(
         self,
-        user_id: int,
+        run_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> RunResponse:
         """
-        Get a specific user by id.
+        Retrieve run by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return await self._get(
-            f"/api/v1/users/{user_id}",
+            f"/api/v1/runs/{run_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=RunResponse,
         )
 
     async def update(
         self,
-        user_id: int,
+        run_id: str,
         *,
-        email: Optional[str] | NotGiven = NOT_GIVEN,
-        full_name: Optional[str] | NotGiven = NOT_GIVEN,
-        is_active: bool | NotGiven = NOT_GIVEN,
-        is_superuser: bool | NotGiven = NOT_GIVEN,
-        password: Optional[str] | NotGiven = NOT_GIVEN,
+        run_metadata: object | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> RunResponse:
         """
-        Update a user.
+        Update run metadata by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return await self._patch(
-            f"/api/v1/users/{user_id}",
-            body=await async_maybe_transform(
-                {
-                    "email": email,
-                    "full_name": full_name,
-                    "is_active": is_active,
-                    "is_superuser": is_superuser,
-                    "password": password,
-                },
-                user_update_params.UserUpdateParams,
-            ),
+            f"/api/v1/runs/{run_id}",
+            body=await async_maybe_transform({"run_metadata": run_metadata}, run_update_params.RunUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=RunResponse,
         )
 
     async def list(
         self,
         *,
         limit: int | NotGiven = NOT_GIVEN,
-        skip: int | NotGiven = NOT_GIVEN,
+        offset: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Users:
+    ) -> RunsResponse:
         """
-        Retrieve users.
+        Retrieve runs.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._get(
-            "/api/v1/users/",
+            "/api/v1/runs/",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "limit": limit,
-                        "skip": skip,
+                        "offset": offset,
                     },
-                    user_list_params.UserListParams,
+                    run_list_params.RunListParams,
                 ),
             ),
-            cast_to=Users,
+            cast_to=RunsResponse,
         )
 
     async def delete(
         self,
-        user_id: int,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> ResponseMessage:
-        """
-        Delete a user.
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        return await self._delete(
-            f"/api/v1/users/{user_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=ResponseMessage,
-        )
-
-    async def open(
-        self,
+        run_id: str,
         *,
-        email: str,
-        password: str,
-        full_name: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> User:
+    ) -> RunResponse:
         """
-        Create new user without the need to be logged in.
+        Delete run by ID.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
+        if not run_id:
+            raise ValueError(f"Expected a non-empty value for `run_id` but received {run_id!r}")
         return await self._post(
-            "/api/v1/users/open",
-            body=await async_maybe_transform(
-                {
-                    "email": email,
-                    "password": password,
-                    "full_name": full_name,
-                },
-                user_open_params.UserOpenParams,
-            ),
+            f"/api/v1/runs/{run_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=User,
+            cast_to=RunResponse,
         )
 
 
-class UsersResourceWithRawResponse:
-    def __init__(self, users: UsersResource) -> None:
-        self._users = users
+class RunsResourceWithRawResponse:
+    def __init__(self, runs: RunsResource) -> None:
+        self._runs = runs
 
         self.create = to_raw_response_wrapper(
-            users.create,
+            runs.create,
         )
         self.retrieve = to_raw_response_wrapper(
-            users.retrieve,
+            runs.retrieve,
         )
         self.update = to_raw_response_wrapper(
-            users.update,
+            runs.update,
         )
         self.list = to_raw_response_wrapper(
-            users.list,
+            runs.list,
         )
         self.delete = to_raw_response_wrapper(
-            users.delete,
+            runs.delete,
         )
-        self.open = to_raw_response_wrapper(
-            users.open,
-        )
-
-    @cached_property
-    def me(self) -> MeResourceWithRawResponse:
-        return MeResourceWithRawResponse(self._users.me)
 
 
-class AsyncUsersResourceWithRawResponse:
-    def __init__(self, users: AsyncUsersResource) -> None:
-        self._users = users
+class AsyncRunsResourceWithRawResponse:
+    def __init__(self, runs: AsyncRunsResource) -> None:
+        self._runs = runs
 
         self.create = async_to_raw_response_wrapper(
-            users.create,
+            runs.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
-            users.retrieve,
+            runs.retrieve,
         )
         self.update = async_to_raw_response_wrapper(
-            users.update,
+            runs.update,
         )
         self.list = async_to_raw_response_wrapper(
-            users.list,
+            runs.list,
         )
         self.delete = async_to_raw_response_wrapper(
-            users.delete,
+            runs.delete,
         )
-        self.open = async_to_raw_response_wrapper(
-            users.open,
-        )
-
-    @cached_property
-    def me(self) -> AsyncMeResourceWithRawResponse:
-        return AsyncMeResourceWithRawResponse(self._users.me)
 
 
-class UsersResourceWithStreamingResponse:
-    def __init__(self, users: UsersResource) -> None:
-        self._users = users
+class RunsResourceWithStreamingResponse:
+    def __init__(self, runs: RunsResource) -> None:
+        self._runs = runs
 
         self.create = to_streamed_response_wrapper(
-            users.create,
+            runs.create,
         )
         self.retrieve = to_streamed_response_wrapper(
-            users.retrieve,
+            runs.retrieve,
         )
         self.update = to_streamed_response_wrapper(
-            users.update,
+            runs.update,
         )
         self.list = to_streamed_response_wrapper(
-            users.list,
+            runs.list,
         )
         self.delete = to_streamed_response_wrapper(
-            users.delete,
+            runs.delete,
         )
-        self.open = to_streamed_response_wrapper(
-            users.open,
-        )
-
-    @cached_property
-    def me(self) -> MeResourceWithStreamingResponse:
-        return MeResourceWithStreamingResponse(self._users.me)
 
 
-class AsyncUsersResourceWithStreamingResponse:
-    def __init__(self, users: AsyncUsersResource) -> None:
-        self._users = users
+class AsyncRunsResourceWithStreamingResponse:
+    def __init__(self, runs: AsyncRunsResource) -> None:
+        self._runs = runs
 
         self.create = async_to_streamed_response_wrapper(
-            users.create,
+            runs.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
-            users.retrieve,
+            runs.retrieve,
         )
         self.update = async_to_streamed_response_wrapper(
-            users.update,
+            runs.update,
         )
         self.list = async_to_streamed_response_wrapper(
-            users.list,
+            runs.list,
         )
         self.delete = async_to_streamed_response_wrapper(
-            users.delete,
+            runs.delete,
         )
-        self.open = async_to_streamed_response_wrapper(
-            users.open,
-        )
-
-    @cached_property
-    def me(self) -> AsyncMeResourceWithStreamingResponse:
-        return AsyncMeResourceWithStreamingResponse(self._users.me)
```

### Comparing `altmindpy-0.0.1a0/src/altmind/types/__init__.py` & `altmindpy-0.0.2/src/altmind/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from .run import Run as Run
 from .token import Token as Token
-from .users import Users as Users
-from .shared import User as User, ResponseMessage as ResponseMessage, MessagesResponse as MessagesResponse
-from .thread import Thread as Thread
-from .message import Message as Message
-from .assistant import Assistant as Assistant
+from .shared import UserOut as UserOut, ResponseMessage as ResponseMessage, MessagesResponse as MessagesResponse
+from .users_out import UsersOut as UsersOut
+from .run_response import RunResponse as RunResponse
 from .runs_response import RunsResponse as RunsResponse
 from .thread_delete import ThreadDelete as ThreadDelete
 from .message_delete import MessageDelete as MessageDelete
 from .run_list_params import RunListParams as RunListParams
+from .thread_response import ThreadResponse as ThreadResponse
 from .assistant_delete import AssistantDelete as AssistantDelete
+from .message_response import MessageResponse as MessageResponse
 from .threads_response import ThreadsResponse as ThreadsResponse
 from .user_list_params import UserListParams as UserListParams
-from .user_open_params import UserOpenParams as UserOpenParams
+from .run_create_params import RunCreateParams as RunCreateParams
 from .run_update_params import RunUpdateParams as RunUpdateParams
+from .assistant_response import AssistantResponse as AssistantResponse
 from .thread_list_params import ThreadListParams as ThreadListParams
 from .user_create_params import UserCreateParams as UserCreateParams
 from .user_update_params import UserUpdateParams as UserUpdateParams
 from .assistants_response import AssistantsResponse as AssistantsResponse
 from .message_list_params import MessageListParams as MessageListParams
 from .thread_create_params import ThreadCreateParams as ThreadCreateParams
 from .thread_update_params import ThreadUpdateParams as ThreadUpdateParams
 from .assistant_list_params import AssistantListParams as AssistantListParams
 from .message_create_params import MessageCreateParams as MessageCreateParams
 from .message_update_params import MessageUpdateParams as MessageUpdateParams
 from .assistant_create_params import AssistantCreateParams as AssistantCreateParams
 from .assistant_update_params import AssistantUpdateParams as AssistantUpdateParams
 from .login_access_token_params import LoginAccessTokenParams as LoginAccessTokenParams
+from .experimental_stream_params import ExperimentalStreamParams as ExperimentalStreamParams
```

### Comparing `altmindpy-0.0.1a0/src/altmind/types/message.py` & `altmindpy-0.0.2/src/altmind/types/message_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import List, Union, Optional
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = [
-    "Message",
+    "MessageResponse",
     "Content",
     "ContentTextContent",
     "ContentTextContentText",
     "ContentImageFileContent",
     "ContentImageFileContentImageFile",
 ]
 
@@ -34,15 +34,15 @@
 
     type: Optional[Literal["image_file"]] = None
 
 
 Content = Union[ContentTextContent, ContentImageFileContent]
 
 
-class Message(BaseModel):
+class MessageResponse(BaseModel):
     id: int
 
     content: List[Content]
 
     created_at: int
 
     original_role: Optional[Literal["user", "assistant", "system", "tool"]] = None
```

### Comparing `altmindpy-0.0.1a0/src/altmind/types/message_create_params.py` & `altmindpy-0.0.2/src/altmind/types/message_create_params.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/types/message_update_params.py` & `altmindpy-0.0.2/src/altmind/types/message_update_params.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/src/altmind/types/run.py` & `altmindpy-0.0.2/src/altmind/types/run_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import builtins
 from typing import Dict, Optional
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = ["Run"]
+__all__ = ["RunResponse"]
 
 
-class Run(BaseModel):
+class RunResponse(BaseModel):
     id: int
 
     additional_instructions: Optional[str] = None
 
     assistant_id: Optional[int] = None
 
     created_at: int
```

### Comparing `altmindpy-0.0.1a0/LICENSE` & `altmindpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.1a0/pyproject.toml` & `altmindpy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "altmindpy"
-version = "0.0.1-alpha"
+version = "0.0.2"
 description = "The official Python library for the altmind API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Altmind", email = "azzi.leonardo@gmail.com" },
 ]
 dependencies = [
```

### Comparing `altmindpy-0.0.1a0/PKG-INFO` & `altmindpy-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: altmindpy
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: The official Python library for the altmind API
 Project-URL: Homepage, https://github.com/AltermindLabs/altmind-python
 Project-URL: Repository, https://github.com/AltermindLabs/altmind-python
 Author-email: Altmind <azzi.leonardo@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -60,19 +60,19 @@
 ```python
 from altmind import Altmind
 
 client = Altmind(
     access_token="My Access Token",
 )
 
-token = client.login.access_token(
+user_out = client.users.create(
+    email="string",
     password="string",
-    username="string",
 )
-print(token.access_token)
+print(user_out.id)
 ```
 
 ## Async usage
 
 Simply import `AsyncAltmind` instead of `Altmind` and use `await` with each API call:
 
 ```python
@@ -81,19 +81,19 @@
 
 client = AsyncAltmind(
     access_token="My Access Token",
 )
 
 
 async def main() -> None:
-    token = await client.login.access_token(
+    user_out = await client.users.create(
+        email="string",
         password="string",
-        username="string",
     )
-    print(token.access_token)
+    print(user_out.id)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -120,17 +120,17 @@
 from altmind import Altmind
 
 client = Altmind(
     access_token="My Access Token",
 )
 
 try:
-    client.login.access_token(
+    client.users.create(
+        email="string",
         password="string",
-        username="string",
     )
 except altmind.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except altmind.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
 except altmind.APIStatusError as e:
@@ -167,17 +167,17 @@
 client = Altmind(
     # default is 2
     max_retries=0,
     access_token="My Access Token",
 )
 
 # Or, configure per-request:
-client.with_options(max_retries=5).login.access_token(
+client.with_options(max_retries=5).users.create(
+    email="string",
     password="string",
-    username="string",
 )
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
@@ -195,17 +195,17 @@
 # More granular control:
 client = Altmind(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
     access_token="My Access Token",
 )
 
 # Override per-request:
-client.with_options(timeout=5.0).login.access_token(
+client.with_options(timeout=5.0).users.create(
+    email="string",
     password="string",
-    username="string",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/AltermindLabs/altmind-python/tree/main/#retries).
 
@@ -239,38 +239,38 @@
 
 ```py
 from altmind import Altmind
 
 client = Altmind(
     access_token="My Access Token",
 )
-response = client.login.with_raw_response.access_token(
+response = client.users.with_raw_response.create(
+    email="string",
     password="string",
-    username="string",
 )
 print(response.headers.get('X-My-Header'))
 
-login = response.parse()  # get the object that `login.access_token()` would have returned
-print(login.access_token)
+user = response.parse()  # get the object that `users.create()` would have returned
+print(user.id)
 ```
 
 These methods return an [`APIResponse`](https://github.com/AltermindLabs/altmind-python/tree/main/src/altmind/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/AltermindLabs/altmind-python/tree/main/src/altmind/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
-with client.login.with_streaming_response.access_token(
+with client.users.with_streaming_response.create(
+    email="string",
     password="string",
-    username="string",
 ) as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
 ```
```

