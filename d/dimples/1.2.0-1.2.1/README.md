# Comparing `tmp/dimples-1.2.0.tar.gz` & `tmp/dimples-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-1.2.0.tar", last modified: Fri May 17 17:33:06 2024, max compression
+gzip compressed data, was "dist/dimples-1.2.1.tar", last modified: Sun May 19 17:29:35 2024, max compression
```

## Comparing `dimples-1.2.0.tar` & `dimples-1.2.1.tar`

### file list

```diff
@@ -1,164 +1,165 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-17 17:33:06.000000 dimples-1.2.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-1.2.0/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-1.2.0/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-1.2.0/dimples/client/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10946 2024-05-07 03:48:04.000000 dimples-1.2.0/dimples/client/archivist.py
--rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-1.2.0/dimples/client/checkpoint.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-1.2.0/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1952 2024-05-07 03:28:52.000000 dimples-1.2.0/dimples/client/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-1.2.0/dimples/client/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     9096 2024-05-07 16:12:33.000000 dimples-1.2.0/dimples/client/cpu/group.py
--rw-r--r--   0 moky       (501) staff       (20)     2173 2024-05-07 03:32:12.000000 dimples-1.2.0/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     5937 2024-05-07 03:34:38.000000 dimples-1.2.0/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3998 2024-05-07 03:35:17.000000 dimples-1.2.0/dimples/client/cpu/grp_join.py
--rw-r--r--   0 moky       (501) staff       (20)     4177 2024-05-07 03:35:53.000000 dimples-1.2.0/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     4388 2024-05-07 03:36:21.000000 dimples-1.2.0/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     5711 2024-05-07 03:36:56.000000 dimples-1.2.0/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     4086 2024-05-07 03:37:19.000000 dimples-1.2.0/dimples/client/cpu/grp_resign.py
--rw-r--r--   0 moky       (501) staff       (20)     5184 2024-05-07 03:50:13.000000 dimples-1.2.0/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     6404 2024-05-06 19:03:39.000000 dimples-1.2.0/dimples/client/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     9059 2024-05-07 03:49:36.000000 dimples-1.2.0/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-1.2.0/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7030 2024-05-09 20:14:55.000000 dimples-1.2.0/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     9334 2024-05-17 15:29:08.000000 dimples-1.2.0/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-1.2.0/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     9296 2024-05-07 03:57:08.000000 dimples-1.2.0/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6077 2024-05-07 04:00:01.000000 dimples-1.2.0/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5497 2024-05-17 16:36:59.000000 dimples-1.2.0/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-1.2.0/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-1.2.0/dimples/common/anonymous.py
--rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-1.2.0/dimples/common/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     7930 2024-05-06 18:08:29.000000 dimples-1.2.0/dimples/common/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/common/compat/
--rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-1.2.0/dimples/common/compat/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-1.2.0/dimples/common/compat/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-1.2.0/dimples/common/compat/compatible.py
--rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-1.2.0/dimples/common/compat/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-1.2.0/dimples/common/compat/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-1.2.0/dimples/common/compat/network.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-1.2.0/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7648 2024-05-06 18:49:56.000000 dimples-1.2.0/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2735 2024-05-06 18:36:11.000000 dimples-1.2.0/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     8062 2024-05-17 16:09:01.000000 dimples-1.2.0/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8591 2024-05-07 18:41:02.000000 dimples-1.2.0/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     9209 2024-05-07 18:48:04.000000 dimples-1.2.0/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     8616 2024-05-06 18:15:14.000000 dimples-1.2.0/dimples/common/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     2999 2024-05-07 18:46:08.000000 dimples-1.2.0/dimples/common/processer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-1.2.0/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-1.2.0/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-1.2.0/dimples/common/protocol/block.py
--rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-1.2.0/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-1.2.0/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-1.2.0/dimples/common/protocol/mute.py
--rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-1.2.0/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     6346 2024-05-06 18:17:07.000000 dimples-1.2.0/dimples/common/register.py
--rw-r--r--   0 moky       (501) staff       (20)     4591 2024-05-07 18:47:41.000000 dimples-1.2.0/dimples/common/session.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4508 2024-05-14 15:03:49.000000 dimples-1.2.0/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6276 2024-05-17 15:29:08.000000 dimples-1.2.0/dimples/conn/flexible.py
--rw-r--r--   0 moky       (501) staff       (20)    10956 2024-05-14 15:09:23.000000 dimples-1.2.0/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)    12264 2024-05-15 19:21:42.000000 dimples-1.2.0/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10810 2024-05-14 15:15:47.000000 dimples-1.2.0/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8002 2024-05-14 15:15:53.000000 dimples-1.2.0/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1916 2024-05-14 15:15:34.000000 dimples-1.2.0/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-1.2.0/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8992 2024-05-14 15:42:00.000000 dimples-1.2.0/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     6452 2024-05-16 07:26:50.000000 dimples-1.2.0/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-1.2.0/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     4407 2024-05-16 07:24:50.000000 dimples-1.2.0/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     7926 2024-05-17 15:29:08.000000 dimples-1.2.0/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-1.2.0/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8179 2024-05-06 18:51:03.000000 dimples-1.2.0/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-1.2.0/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4692 2024-05-14 14:54:42.000000 dimples-1.2.0/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     6360 2024-05-06 18:30:09.000000 dimples-1.2.0/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     5247 2024-05-06 18:21:39.000000 dimples-1.2.0/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     6045 2024-05-06 18:50:27.000000 dimples-1.2.0/dimples/database/dos/group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     2789 2024-05-06 18:39:54.000000 dimples-1.2.0/dimples/database/dos/group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     3101 2024-05-06 18:24:21.000000 dimples-1.2.0/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2646 2024-05-06 18:24:29.000000 dimples-1.2.0/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5553 2024-05-06 18:24:46.000000 dimples-1.2.0/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8045 2024-05-06 18:26:43.000000 dimples-1.2.0/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     2941 2024-05-06 18:27:02.000000 dimples-1.2.0/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3760 2024-05-06 18:51:40.000000 dimples-1.2.0/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4436 2024-05-06 18:53:13.000000 dimples-1.2.0/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     3132 2024-05-06 18:27:39.000000 dimples-1.2.0/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     4147 2024-05-06 18:30:39.000000 dimples-1.2.0/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     6567 2024-05-06 18:31:50.000000 dimples-1.2.0/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     5809 2024-05-06 18:50:47.000000 dimples-1.2.0/dimples/database/t_group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     4295 2024-05-06 18:41:59.000000 dimples-1.2.0/dimples/database/t_group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     4246 2024-05-06 18:41:59.000000 dimples-1.2.0/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     4405 2024-05-06 18:39:12.000000 dimples-1.2.0/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3756 2024-05-06 18:41:59.000000 dimples-1.2.0/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5909 2024-05-06 18:42:32.000000 dimples-1.2.0/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6845 2024-05-06 18:44:20.000000 dimples-1.2.0/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     3578 2024-05-06 18:45:26.000000 dimples-1.2.0/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-1.2.0/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    16117 2024-05-17 16:38:00.000000 dimples-1.2.0/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     6161 2024-05-15 16:34:13.000000 dimples-1.2.0/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2854 2024-05-17 16:40:17.000000 dimples-1.2.0/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/group/
--rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-1.2.0/dimples/group/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6217 2024-05-06 18:55:34.000000 dimples-1.2.0/dimples/group/admin.py
--rw-r--r--   0 moky       (501) staff       (20)     7191 2024-05-06 19:06:23.000000 dimples-1.2.0/dimples/group/builder.py
--rw-r--r--   0 moky       (501) staff       (20)     7337 2024-05-06 19:05:04.000000 dimples-1.2.0/dimples/group/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)    12302 2024-05-06 19:12:10.000000 dimples-1.2.0/dimples/group/emitter.py
--rw-r--r--   0 moky       (501) staff       (20)     5351 2024-05-16 07:07:02.000000 dimples-1.2.0/dimples/group/helper.py
--rw-r--r--   0 moky       (501) staff       (20)    16535 2024-05-06 19:16:50.000000 dimples-1.2.0/dimples/group/manager.py
--rw-r--r--   0 moky       (501) staff       (20)     5084 2024-05-06 19:10:38.000000 dimples-1.2.0/dimples/group/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2024-04-25 15:20:32.000000 dimples-1.2.0/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10595 2024-05-10 10:25:00.000000 dimples-1.2.0/dimples/register/base.py
--rw-r--r--   0 moky       (501) staff       (20)     8248 2024-05-10 10:25:44.000000 dimples-1.2.0/dimples/register/ext.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3901 2024-05-14 14:54:42.000000 dimples-1.2.0/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     4151 2024-05-07 17:52:52.000000 dimples-1.2.0/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-1.2.0/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7502 2024-05-07 17:25:09.000000 dimples-1.2.0/dimples/server/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-1.2.0/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2729 2024-05-07 04:03:19.000000 dimples-1.2.0/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4857 2024-05-07 04:03:27.000000 dimples-1.2.0/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4035 2024-05-07 04:22:27.000000 dimples-1.2.0/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4234 2024-05-07 04:22:59.000000 dimples-1.2.0/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3539 2024-05-07 04:23:05.000000 dimples-1.2.0/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    17809 2024-05-17 16:24:28.000000 dimples-1.2.0/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     4574 2024-05-07 17:29:24.000000 dimples-1.2.0/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6584 2024-05-07 04:15:23.000000 dimples-1.2.0/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)    14023 2024-05-07 18:39:52.000000 dimples-1.2.0/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5587 2024-05-17 16:32:27.000000 dimples-1.2.0/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     9537 2024-05-17 16:43:59.000000 dimples-1.2.0/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-1.2.0/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-1.2.0/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-1.2.0/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3112 2024-05-17 16:55:26.000000 dimples-1.2.0/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7523 2024-05-15 16:32:16.000000 dimples-1.2.0/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3755 2024-05-09 16:42:05.000000 dimples-1.2.0/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     4722 2024-05-17 15:32:17.000000 dimples-1.2.0/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6250 2024-05-17 15:44:13.000000 dimples-1.2.0/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-1.2.0/dimples/utils/config.py
--rw-r--r--   0 moky       (501) staff       (20)     7057 2024-05-14 14:54:42.000000 dimples-1.2.0/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-1.2.0/dimples/utils/log.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3980 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      104 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-17 17:33:06.000000 dimples-1.2.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1671 2024-05-17 16:46:53.000000 dimples-1.2.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-19 17:29:35.000000 dimples-1.2.1/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-1.2.1/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-1.2.1/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-1.2.1/dimples/client/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10946 2024-05-07 03:48:04.000000 dimples-1.2.1/dimples/client/archivist.py
+-rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-1.2.1/dimples/client/checkpoint.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-1.2.1/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1952 2024-05-07 03:28:52.000000 dimples-1.2.1/dimples/client/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-1.2.1/dimples/client/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     9096 2024-05-07 16:12:33.000000 dimples-1.2.1/dimples/client/cpu/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     2173 2024-05-07 03:32:12.000000 dimples-1.2.1/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     5937 2024-05-07 03:34:38.000000 dimples-1.2.1/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3998 2024-05-07 03:35:17.000000 dimples-1.2.1/dimples/client/cpu/grp_join.py
+-rw-r--r--   0 moky       (501) staff       (20)     4177 2024-05-07 03:35:53.000000 dimples-1.2.1/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     4388 2024-05-07 03:36:21.000000 dimples-1.2.1/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     5711 2024-05-07 03:36:56.000000 dimples-1.2.1/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     4086 2024-05-07 03:37:19.000000 dimples-1.2.1/dimples/client/cpu/grp_resign.py
+-rw-r--r--   0 moky       (501) staff       (20)     5184 2024-05-07 03:50:13.000000 dimples-1.2.1/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     6404 2024-05-06 19:03:39.000000 dimples-1.2.1/dimples/client/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     9059 2024-05-07 03:49:36.000000 dimples-1.2.1/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-1.2.1/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7057 2024-05-18 16:49:56.000000 dimples-1.2.1/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     9354 2024-05-18 18:17:35.000000 dimples-1.2.1/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-1.2.1/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     9296 2024-05-07 03:57:08.000000 dimples-1.2.1/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6077 2024-05-07 04:00:01.000000 dimples-1.2.1/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5497 2024-05-17 16:36:59.000000 dimples-1.2.1/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-1.2.1/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-1.2.1/dimples/common/anonymous.py
+-rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-1.2.1/dimples/common/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     7930 2024-05-06 18:08:29.000000 dimples-1.2.1/dimples/common/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/common/compat/
+-rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-1.2.1/dimples/common/compat/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-1.2.1/dimples/common/compat/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-1.2.1/dimples/common/compat/compatible.py
+-rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-1.2.1/dimples/common/compat/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-1.2.1/dimples/common/compat/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-1.2.1/dimples/common/compat/network.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-1.2.1/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7648 2024-05-06 18:49:56.000000 dimples-1.2.1/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2735 2024-05-06 18:36:11.000000 dimples-1.2.1/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     8062 2024-05-17 16:09:01.000000 dimples-1.2.1/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8591 2024-05-07 18:41:02.000000 dimples-1.2.1/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     9209 2024-05-07 18:48:04.000000 dimples-1.2.1/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     8616 2024-05-06 18:15:14.000000 dimples-1.2.1/dimples/common/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     2999 2024-05-07 18:46:08.000000 dimples-1.2.1/dimples/common/processer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-1.2.1/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-1.2.1/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-1.2.1/dimples/common/protocol/block.py
+-rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-1.2.1/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-1.2.1/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-1.2.1/dimples/common/protocol/mute.py
+-rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-1.2.1/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     6346 2024-05-06 18:17:07.000000 dimples-1.2.1/dimples/common/register.py
+-rw-r--r--   0 moky       (501) staff       (20)     4591 2024-05-07 18:47:41.000000 dimples-1.2.1/dimples/common/session.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4508 2024-05-14 15:03:49.000000 dimples-1.2.1/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6292 2024-05-18 18:17:47.000000 dimples-1.2.1/dimples/conn/flexible.py
+-rw-r--r--   0 moky       (501) staff       (20)    10956 2024-05-14 15:09:23.000000 dimples-1.2.1/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12304 2024-05-18 18:17:24.000000 dimples-1.2.1/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10810 2024-05-14 15:15:47.000000 dimples-1.2.1/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8002 2024-05-14 15:15:53.000000 dimples-1.2.1/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1916 2024-05-14 15:15:34.000000 dimples-1.2.1/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-1.2.1/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8992 2024-05-14 15:42:00.000000 dimples-1.2.1/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     6452 2024-05-16 07:26:50.000000 dimples-1.2.1/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-1.2.1/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     4407 2024-05-16 07:24:50.000000 dimples-1.2.1/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     7950 2024-05-18 18:16:57.000000 dimples-1.2.1/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-1.2.1/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8179 2024-05-06 18:51:03.000000 dimples-1.2.1/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-1.2.1/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4692 2024-05-14 14:54:42.000000 dimples-1.2.1/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     6360 2024-05-06 18:30:09.000000 dimples-1.2.1/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     5247 2024-05-06 18:21:39.000000 dimples-1.2.1/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     6045 2024-05-06 18:50:27.000000 dimples-1.2.1/dimples/database/dos/group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     2789 2024-05-06 18:39:54.000000 dimples-1.2.1/dimples/database/dos/group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     3101 2024-05-06 18:24:21.000000 dimples-1.2.1/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2646 2024-05-06 18:24:29.000000 dimples-1.2.1/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5553 2024-05-06 18:24:46.000000 dimples-1.2.1/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8045 2024-05-06 18:26:43.000000 dimples-1.2.1/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     2941 2024-05-06 18:27:02.000000 dimples-1.2.1/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3760 2024-05-06 18:51:40.000000 dimples-1.2.1/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4436 2024-05-06 18:53:13.000000 dimples-1.2.1/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     3132 2024-05-06 18:27:39.000000 dimples-1.2.1/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     4147 2024-05-06 18:30:39.000000 dimples-1.2.1/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     6567 2024-05-06 18:31:50.000000 dimples-1.2.1/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5809 2024-05-06 18:50:47.000000 dimples-1.2.1/dimples/database/t_group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     4295 2024-05-06 18:41:59.000000 dimples-1.2.1/dimples/database/t_group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     4246 2024-05-06 18:41:59.000000 dimples-1.2.1/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     4405 2024-05-06 18:39:12.000000 dimples-1.2.1/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3756 2024-05-06 18:41:59.000000 dimples-1.2.1/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5909 2024-05-06 18:42:32.000000 dimples-1.2.1/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6845 2024-05-06 18:44:20.000000 dimples-1.2.1/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     3578 2024-05-06 18:45:26.000000 dimples-1.2.1/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-1.2.1/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    16117 2024-05-17 16:38:00.000000 dimples-1.2.1/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     6161 2024-05-15 16:34:13.000000 dimples-1.2.1/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2854 2024-05-17 16:40:17.000000 dimples-1.2.1/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/group/
+-rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-1.2.1/dimples/group/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6217 2024-05-06 18:55:34.000000 dimples-1.2.1/dimples/group/admin.py
+-rw-r--r--   0 moky       (501) staff       (20)     7191 2024-05-06 19:06:23.000000 dimples-1.2.1/dimples/group/builder.py
+-rw-r--r--   0 moky       (501) staff       (20)     7337 2024-05-06 19:05:04.000000 dimples-1.2.1/dimples/group/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12302 2024-05-06 19:12:10.000000 dimples-1.2.1/dimples/group/emitter.py
+-rw-r--r--   0 moky       (501) staff       (20)     5351 2024-05-16 07:07:02.000000 dimples-1.2.1/dimples/group/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)    16535 2024-05-06 19:16:50.000000 dimples-1.2.1/dimples/group/manager.py
+-rw-r--r--   0 moky       (501) staff       (20)     5084 2024-05-06 19:10:38.000000 dimples-1.2.1/dimples/group/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2024-04-25 15:20:32.000000 dimples-1.2.1/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10595 2024-05-10 10:25:00.000000 dimples-1.2.1/dimples/register/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     8248 2024-05-10 10:25:44.000000 dimples-1.2.1/dimples/register/ext.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3901 2024-05-14 14:54:42.000000 dimples-1.2.1/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     4151 2024-05-07 17:52:52.000000 dimples-1.2.1/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-1.2.1/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7502 2024-05-07 17:25:09.000000 dimples-1.2.1/dimples/server/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-1.2.1/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2729 2024-05-07 04:03:19.000000 dimples-1.2.1/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4857 2024-05-07 04:03:27.000000 dimples-1.2.1/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4035 2024-05-07 04:22:27.000000 dimples-1.2.1/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4234 2024-05-07 04:22:59.000000 dimples-1.2.1/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3539 2024-05-07 04:23:05.000000 dimples-1.2.1/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    17805 2024-05-18 18:14:51.000000 dimples-1.2.1/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     4574 2024-05-07 17:29:24.000000 dimples-1.2.1/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6676 2024-05-19 05:13:31.000000 dimples-1.2.1/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)    14023 2024-05-07 18:39:52.000000 dimples-1.2.1/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5583 2024-05-18 18:15:46.000000 dimples-1.2.1/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     9533 2024-05-18 18:16:43.000000 dimples-1.2.1/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-1.2.1/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-1.2.1/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-1.2.1/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3112 2024-05-17 16:55:26.000000 dimples-1.2.1/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7523 2024-05-15 16:32:16.000000 dimples-1.2.1/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3755 2024-05-09 16:42:05.000000 dimples-1.2.1/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     4756 2024-05-18 18:30:49.000000 dimples-1.2.1/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6250 2024-05-18 18:31:54.000000 dimples-1.2.1/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-1.2.1/dimples/utils/config.py
+-rw-r--r--   0 moky       (501) staff       (20)     7057 2024-05-14 14:54:42.000000 dimples-1.2.1/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-1.2.1/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)      479 2024-05-18 18:57:33.000000 dimples-1.2.1/dimples/utils/runner.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     4004 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      104 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2024-05-19 17:29:35.000000 dimples-1.2.1/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-19 17:29:35.000000 dimples-1.2.1/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1671 2024-05-18 18:33:06.000000 dimples-1.2.1/setup.py
```

### Comparing `dimples-1.2.0/PKG-INFO` & `dimples-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 1.2.0
+Version: 1.2.1
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-1.2.0/README.md` & `dimples-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/__init__.py` & `dimples-1.2.1/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/__init__.py` & `dimples-1.2.1/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/archivist.py` & `dimples-1.2.1/dimples/client/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/checkpoint.py` & `dimples-1.2.1/dimples/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/__init__.py` & `dimples-1.2.1/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/commands.py` & `dimples-1.2.1/dimples/client/cpu/commands.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/creator.py` & `dimples-1.2.1/dimples/client/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/group.py` & `dimples-1.2.1/dimples/client/cpu/group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/grp_expel.py` & `dimples-1.2.1/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/grp_invite.py` & `dimples-1.2.1/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/grp_join.py` & `dimples-1.2.1/dimples/client/cpu/grp_join.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/grp_query.py` & `dimples-1.2.1/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/grp_quit.py` & `dimples-1.2.1/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/grp_reset.py` & `dimples-1.2.1/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/grp_resign.py` & `dimples-1.2.1/dimples/client/cpu/grp_resign.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/cpu/handshake.py` & `dimples-1.2.1/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/facebook.py` & `dimples-1.2.1/dimples/client/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/messenger.py` & `dimples-1.2.1/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/network/__init__.py` & `dimples-1.2.1/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/network/session.py` & `dimples-1.2.1/dimples/client/network/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         await super().start()
         # 2. start state machine
         fsm = self.fsm
         assert fsm.delegate is not None, 'FSM delegate not set: %s' % self
         await fsm.start()
         # 3. start an async task for this session
         self.__daemon.start()
+        # await self.run()
 
     # Override
     async def stop(self):
         # 1. mark this session to stopped
         await super().stop()
         # 2. stop state machine
         await self.fsm.stop()
```

### Comparing `dimples-1.2.0/dimples/client/network/state.py` & `dimples-1.2.1/dimples/client/network/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,16 @@
     def status(self) -> DockerStatus:
         docker = self.docker
         if docker is not None:
             return docker.status
         else:
             session = self.session
             gate = session.gate
-            task = Runner.async_run(coroutine=gate.fetch_docker([], remote=session.remote_address, local=None))
+            coro = gate.fetch_docker([], remote=session.remote_address, local=None)
+            task = Runner.async_task(coro=coro)
             task.add_done_callback(self._fetch_docker_callback)
         # waiting for callback
         return DockerStatus.ERROR
 
     def _fetch_docker_callback(self, t: asyncio.Task):
         self.docker = t.result()
```

### Comparing `dimples-1.2.0/dimples/client/network/transition.py` & `dimples-1.2.1/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/packer.py` & `dimples-1.2.1/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/processor.py` & `dimples-1.2.1/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/client/terminal.py` & `dimples-1.2.1/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/__init__.py` & `dimples-1.2.1/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/anonymous.py` & `dimples-1.2.1/dimples/common/anonymous.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/ans.py` & `dimples-1.2.1/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/archivist.py` & `dimples-1.2.1/dimples/common/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/compat/__init__.py` & `dimples-1.2.1/dimples/common/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/compat/btc.py` & `dimples-1.2.1/dimples/common/compat/btc.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/compat/compatible.py` & `dimples-1.2.1/dimples/common/compat/compatible.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/compat/entity.py` & `dimples-1.2.1/dimples/common/compat/entity.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/compat/meta.py` & `dimples-1.2.1/dimples/common/compat/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/compat/network.py` & `dimples-1.2.1/dimples/common/compat/network.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/dbi/__init__.py` & `dimples-1.2.1/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/dbi/account.py` & `dimples-1.2.1/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/dbi/message.py` & `dimples-1.2.1/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/dbi/session.py` & `dimples-1.2.1/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/facebook.py` & `dimples-1.2.1/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/messenger.py` & `dimples-1.2.1/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/packer.py` & `dimples-1.2.1/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/processer.py` & `dimples-1.2.1/dimples/common/processer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/protocol/__init__.py` & `dimples-1.2.1/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/protocol/ans.py` & `dimples-1.2.1/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/protocol/block.py` & `dimples-1.2.1/dimples/common/protocol/block.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/protocol/handshake.py` & `dimples-1.2.1/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/protocol/login.py` & `dimples-1.2.1/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/protocol/mute.py` & `dimples-1.2.1/dimples/common/protocol/mute.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/protocol/report.py` & `dimples-1.2.1/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/register.py` & `dimples-1.2.1/dimples/common/register.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/common/session.py` & `dimples-1.2.1/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/__init__.py` & `dimples-1.2.1/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/flexible.py` & `dimples-1.2.1/dimples/conn/flexible.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         elif MarsStreamDocker.check(data=data):
             docker = MarsStreamDocker(remote=self.remote_address, local=self.local_address)
         else:
             print('[FlexibleDocker] unsupported data format: %s' % data)
             return None
         # OK
         docker.delegate = self.delegate
-        Runner.async_run(coroutine=docker.set_connection(conn=self.connection))
+        coro = docker.set_connection(conn=self.connection)
+        Runner.async_task(coro=coro)
         self.__docker = docker
         return docker
 
     # Override
     async def set_connection(self, conn: Optional[Connection]):
         await super().set_connection(conn=conn)
         docker = self.__docker
```

### Comparing `dimples-1.2.0/dimples/conn/gate.py` & `dimples-1.2.1/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/gatekeeper.py` & `dimples-1.2.1/dimples/conn/gatekeeper.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,24 +178,26 @@
 
     # noinspection PyMethodMayBeStatic
     def _create_hub(self, delegate: ConnectionDelegate, address: Tuple[str, int], sock: Optional[socket.socket]) -> Hub:
         if sock is None:
             # client
             assert address is not None, 'remote address empty'
             hub = StreamClientHub(delegate=delegate)
-            Runner.async_run(coroutine=_client_connect(hub=hub, address=address))
+            coro = _client_connect(hub=hub, address=address)
+            Runner.async_task(coro=coro)
             self.info(msg='client hub created: %s' % str(address))
         else:
             # server
             sock.setblocking(False)
             # sock.settimeout(0.5)
             if address is None:
                 address = get_remote_address(sock=sock)
             channel = StreamChannel(remote=address, local=get_local_address(sock=sock))
-            Runner.async_run(coroutine=channel.set_socket(sock=sock))
+            coro = channel.set_socket(sock=sock)
+            Runner.async_task(coro=coro)
             hub = StreamServerHub(delegate=delegate)
             hub.put_channel(channel=channel)
         return hub
 
     @property
     def remote_address(self) -> Tuple[str, int]:
         return self.__remote
```

### Comparing `dimples-1.2.0/dimples/conn/mars.py` & `dimples-1.2.1/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/mtp.py` & `dimples-1.2.1/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/protocol/__init__.py` & `dimples-1.2.1/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/protocol/mars.py` & `dimples-1.2.1/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/protocol/ws.py` & `dimples-1.2.1/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/queue.py` & `dimples-1.2.1/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/seeker.py` & `dimples-1.2.1/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/session.py` & `dimples-1.2.1/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/conn/ws.py` & `dimples-1.2.1/dimples/conn/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,16 @@
             # join the data to the memory cache
             data = self.__chunks + data
             self.__chunks = b''
             # parse handshake
             res = WebSocket.handshake(stream=data)
             if res is not None:
                 ship = WSDeparture(package=res, payload=b'')
-                Runner.async_run(coroutine=self.send_ship(ship=ship))
+                coro = self.send_ship(ship=ship)
+                Runner.async_task(coro=coro)
                 self.__handshaking = False
             elif len(data) < self.MAX_PACK_LENGTH:
                 # waiting for more data
                 self.__chunks = data + self.__chunks
             return []
         # normal state
         ships = []
```

### Comparing `dimples-1.2.0/dimples/database/__init__.py` & `dimples-1.2.1/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/account.py` & `dimples-1.2.1/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/__init__.py` & `dimples-1.2.1/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/base.py` & `dimples-1.2.1/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/document.py` & `dimples-1.2.1/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/group.py` & `dimples-1.2.1/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/group_history.py` & `dimples-1.2.1/dimples/database/dos/group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/group_keys.py` & `dimples-1.2.1/dimples/database/dos/group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/login.py` & `dimples-1.2.1/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/meta.py` & `dimples-1.2.1/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/private.py` & `dimples-1.2.1/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/station.py` & `dimples-1.2.1/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/dos/user.py` & `dimples-1.2.1/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/message.py` & `dimples-1.2.1/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/session.py` & `dimples-1.2.1/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_cipherkey.py` & `dimples-1.2.1/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_document.py` & `dimples-1.2.1/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_group.py` & `dimples-1.2.1/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_group_history.py` & `dimples-1.2.1/dimples/database/t_group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_group_keys.py` & `dimples-1.2.1/dimples/database/t_group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_login.py` & `dimples-1.2.1/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_message.py` & `dimples-1.2.1/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_meta.py` & `dimples-1.2.1/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_private.py` & `dimples-1.2.1/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_station.py` & `dimples-1.2.1/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/database/t_user.py` & `dimples-1.2.1/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/edge/__init__.py` & `dimples-1.2.1/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/edge/octopus.py` & `dimples-1.2.1/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/edge/shared.py` & `dimples-1.2.1/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/edge/start.py` & `dimples-1.2.1/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/group/__init__.py` & `dimples-1.2.1/dimples/group/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/group/admin.py` & `dimples-1.2.1/dimples/group/admin.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/group/builder.py` & `dimples-1.2.1/dimples/group/builder.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/group/delegate.py` & `dimples-1.2.1/dimples/group/delegate.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/group/emitter.py` & `dimples-1.2.1/dimples/group/emitter.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/group/helper.py` & `dimples-1.2.1/dimples/group/helper.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/group/manager.py` & `dimples-1.2.1/dimples/group/manager.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/group/packer.py` & `dimples-1.2.1/dimples/group/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/register/__init__.py` & `dimples-1.2.1/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/register/base.py` & `dimples-1.2.1/dimples/register/base.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/register/ext.py` & `dimples-1.2.1/dimples/register/ext.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/register/run.py` & `dimples-1.2.1/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/register/shared.py` & `dimples-1.2.1/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/__init__.py` & `dimples-1.2.1/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/archivist.py` & `dimples-1.2.1/dimples/server/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/cpu/__init__.py` & `dimples-1.2.1/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/cpu/ans.py` & `dimples-1.2.1/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/cpu/document.py` & `dimples-1.2.1/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/cpu/handshake.py` & `dimples-1.2.1/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/cpu/login.py` & `dimples-1.2.1/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/cpu/report.py` & `dimples-1.2.1/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/dispatcher.py` & `dimples-1.2.1/dimples/server/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     def roamer(self):  # -> Roamer
         runner = self.__roamer
         if runner is None:
             db = self.mdb
             assert db is not None, 'dispatcher not initialized'
             runner = Roamer(database=db)
             self.__roamer = runner
-            # Runner.async_run(coroutine=runner.start())
+            # Runner.async_task(coro=runner.start())
             Runner.thread_run(runner=runner)
         return runner
 
     def add_roaming(self, user: ID, station: ID) -> bool:
         """ Add roaming user with station """
         roamer = self.roamer
         return roamer.add_roaming(user=user, station=station)
```

### Comparing `dimples-1.2.0/dimples/server/messenger.py` & `dimples-1.2.1/dimples/server/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/packer.py` & `dimples-1.2.1/dimples/server/packer.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,24 +139,26 @@
         return False
 
 
 class MuteFilter(Logging):
     """ Filter for Push Notification service """
 
     async def is_muted(self, msg: ReliableMessage) -> bool:
+        if msg.get_bool(key='muted', default=False):
+            return True
         sender = msg.sender
         receiver = msg.receiver
         group = msg.group
         self.debug(msg='checking mute-list for: %s -> %s (group: %s)' % (sender, receiver, group))
         if sender.type == EntityType.STATION or receiver.type == EntityType.STATION:
             # mute all messages for stations
             return True
         elif sender.type == EntityType.BOT:
             # mute group message from bot
-            return group is not None or receiver.is_group
+            return receiver.is_group or group is not None or 'GF' in msg
         elif receiver.type == EntityType.BOT:
             # mute all messages to bots
             return True
         # TODO: check mute-list
 
 
 @Singleton
```

### Comparing `dimples-1.2.0/dimples/server/processor.py` & `dimples-1.2.1/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/push.py` & `dimples-1.2.1/dimples/server/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 class PushCenter(Runner, Logging):
 
     def __init__(self):
         super().__init__(interval=Runner.INTERVAL_SLOW)
         self.__queue = MessageQueue()
         self.__keeper = BadgeKeeper()
         self.__service: Optional[PushService] = None
-        # Runner.async_run(coroutine=self.start())
+        # Runner.async_task(coro=self.start())
         Runner.thread_run(runner=self)
 
     @property
     def service(self) -> Optional[PushService]:
         return self.__service
 
     @service.setter
```

### Comparing `dimples-1.2.0/dimples/server/session.py` & `dimples-1.2.1/dimples/server/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,25 +91,25 @@
 
     # Override
     def set_identifier(self, identifier: ID) -> bool:
         old = self.identifier
         if super().set_identifier(identifier=identifier):
             session_change_id(session=self, new_id=identifier, old_id=old)
             # load cached message asynchronously
-            crt = load_cached_messages(session=self)
-            Runner.async_run(coroutine=crt)
+            coro = load_cached_messages(session=self)
+            Runner.async_task(coro=coro)
             return True
 
     # Override
     def set_active(self, active: bool, when: float = None) -> bool:
         if super().set_active(active=active, when=when):
             session_change_active(session=self, active=active)
             # load cached message asynchronously
-            crt = load_cached_messages(session=self)
-            Runner.async_run(coroutine=crt)
+            coro = load_cached_messages(session=self)
+            Runner.async_task(coro=coro)
             return True
 
     #
     #   Docker Delegate
     #
 
     # Override
```

### Comparing `dimples-1.2.0/dimples/server/session_center.py` & `dimples-1.2.1/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/server/trace.py` & `dimples-1.2.1/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/station/__init__.py` & `dimples-1.2.1/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/station/handler.py` & `dimples-1.2.1/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/station/shared.py` & `dimples-1.2.1/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/station/start.py` & `dimples-1.2.1/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/utils/__init__.py` & `dimples-1.2.1/dimples/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,19 @@
 from dimsdk import DateTime
 from dimsdk import ReliableMessage
 from dimsdk import DocumentHelper
 
 from dimplugins.crypto.aes import random_bytes
 
 from startrek.skywalker import Singleton
-from startrek.skywalker import Runnable, Runner, Daemon
+from startrek.skywalker import Runnable, Daemon
 from startrek.fsm import Delegate as StateDelegate
 from startrek.net.socket import get_remote_address, get_local_address
 
+from .runner import PatchRunner as Runner
 from .log import Log, Logging
 from .dos import Path, File, TextFile, JSONFile
 from .cache import CachePool, CacheHolder, CacheManager
 
 from .config import Config
```

### Comparing `dimples-1.2.0/dimples/utils/cache.py` & `dimples-1.2.1/dimples/utils/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     ~~~~~~~~~~~~~~~
 
 """
 
 from typing import TypeVar, Generic, Optional, Dict, Set, Tuple
 
 from startrek.skywalker import Singleton
-from startrek.skywalker import Runner
 from dimsdk import DateTime
 
+from .runner import PatchRunner as Runner
 from .log import Logging
 
 
 K = TypeVar('K')
 V = TypeVar('V')
 
 
@@ -137,15 +137,15 @@
 @Singleton
 class CacheManager(Runner, Logging):
 
     def __init__(self):
         super().__init__(interval=2.0)
         self.__pools: Dict[str, CachePool] = {}  # name -> pool
         self.__next_time = DateTime.now()
-        # Runner.async_run(coroutine=self.start())
+        # Runner.async_task(coro=self.start())
         Runner.thread_run(runner=self)
 
     # Override
     async def setup(self):
         pass
 
     # Override
```

### Comparing `dimples-1.2.0/dimples/utils/config.py` & `dimples-1.2.1/dimples/utils/config.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/utils/dos.py` & `dimples-1.2.1/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples/utils/log.py` & `dimples-1.2.1/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-1.2.0/dimples.egg-info/PKG-INFO` & `dimples-1.2.1/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 1.2.0
+Version: 1.2.1
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-1.2.0/dimples.egg-info/SOURCES.txt` & `dimples-1.2.1/dimples.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -134,8 +134,9 @@
 dimples/station/handler.py
 dimples/station/shared.py
 dimples/station/start.py
 dimples/utils/__init__.py
 dimples/utils/cache.py
 dimples/utils/config.py
 dimples/utils/dos.py
-dimples/utils/log.py
+dimples/utils/log.py
+dimples/utils/runner.py
```

### Comparing `dimples-1.2.0/setup.py` & `dimples-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -54,12 +54,12 @@
         'dimplugins>=2.0.0',
 
         'dimsdk>=2.0.0',
         'dimp>=2.0.0',
         'dkd>=2.0.0',
         'mkm>=2.0.0',
 
-        'startrek>=2.1.0',
-        'tcp>=2.1.0',
-        'udp>=2.1.0',
+        'startrek>=2.1.1',
+        'tcp>=2.1.1',
+        'udp>=2.1.1',
     ]
 )
```

